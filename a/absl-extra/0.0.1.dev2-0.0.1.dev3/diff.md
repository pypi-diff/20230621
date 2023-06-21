# Comparing `tmp/absl_extra-0.0.1.dev2.tar.gz` & `tmp/absl_extra-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.1.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.1.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.1.dev2.tar` & `absl_extra-0.0.1.dev3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1578 2023-06-21 21:02:49.905090 absl_extra-0.0.1.dev2/Readme.md
--rw-r--r--   0        0        0       61 2023-06-21 21:02:49.905090 absl_extra-0.0.1.dev2/absl_extra/__init__.py
--rw-r--r--   0        0        0     1443 2023-06-21 21:02:49.905090 absl_extra-0.0.1.dev2/absl_extra/logging_utils.py
--rw-r--r--   0        0        0     2487 2023-06-21 21:02:49.905090 absl_extra-0.0.1.dev2/absl_extra/notifier.py
--rw-r--r--   0        0        0     3957 2023-06-21 21:02:49.905090 absl_extra-0.0.1.dev2/absl_extra/tasks.py
--rw-r--r--   0        0        0     4500 2023-06-21 21:02:49.905090 absl_extra-0.0.1.dev2/absl_extra/tf_utils.py
--rw-r--r--   0        0        0      880 2023-06-21 21:02:49.905090 absl_extra-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 absl_extra-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1578 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/Readme.md
+-rw-r--r--   0        0        0       61 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/__init__.py
+-rw-r--r--   0        0        0     1443 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/logging_utils.py
+-rw-r--r--   0        0        0     2487 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/notifier.py
+-rw-r--r--   0        0        0     3654 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/tasks.py
+-rw-r--r--   0        0        0     4474 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/tf_utils.py
+-rw-r--r--   0        0        0      880 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 absl_extra-0.0.1.dev3/PKG-INFO
```

### Comparing `absl_extra-0.0.1.dev2/Readme.md` & `absl_extra-0.0.1.dev3/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev2/absl_extra/logging_utils.py` & `absl_extra-0.0.1.dev3/absl_extra/logging_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev2/absl_extra/notifier.py` & `absl_extra-0.0.1.dev3/absl_extra/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev2/absl_extra/tasks.py` & `absl_extra-0.0.1.dev3/absl_extra/tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 import json
 from functools import wraps, partial
 from importlib import util
-from typing import Callable, NamedTuple, TypeVar, Mapping
+from typing import Callable, NamedTuple, TypeVar, Mapping, List
 
 from absl import app, flags, logging
 
 from absl_extra.notifier import BaseNotifier
 
 T = TypeVar("T", bound=Callable, covariant=True)
 FLAGS = flags.FLAGS
 
-flags.DEFINE_string("task", default="main", help="Name of task to run.")
-
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
 else:
     logging.warning("pymongo not installed.")
 
 if util.find_spec("ml_collections"):
     from ml_collections import config_flags
@@ -36,15 +34,21 @@
         self.name = name
         self.notifier = notifier
 
     def handle(self, exception: Exception) -> None:
         self.notifier.notify_job_failed(self.name, exception)
 
 
-_TASKS = {}
+class TaskT(NamedTuple):
+    fn: Callable
+    name: str | Callable[[], str]
+    init_callbacks: List[Callable[[...], None]] = []
+
+
+_TASK_STORE = None
 
 
 def register_task(
     fn: Callable[[str], None], name: str | Callable[[], str] = "main"
 ) -> None:
     """
 
@@ -53,30 +57,31 @@
     fn
     name
 
     Returns
     -------
 
     """
-    if isinstance(name, Callable):
-        name = name()
-    if name in _TASKS:
-        raise RuntimeError(f"Can't register 2 tasks with same name: {name}")
-    _TASKS[name] = fn
+    global _TASK_STORE
+    _TASK_STORE = TaskT(fn=fn, name=name)
 
 
-def hook_task(
-    task: Callable[[...], None],
+def pseudo_main(
+    task: TaskT,
     app_name: str,
-    task_name: str,
     notifier: BaseNotifier,
     config_file: str | None,
 ) -> Callable[[...], None]:
     @wraps(task)
     def wrapper(*, db=None):
+        if isinstance(task.name, Callable):
+            task_name = task.name()
+        else:
+            task_name = task.name
+
         logging.info("-" * 50)
         logging.info(
             f"Flags: {json.dumps(flags.FLAGS.flag_values_dict(), sort_keys=True, indent=4)}"
         )
         if util.find_spec("ml_collections") and config_file is not None:
             config = config_flags.DEFINE_config_file("config", default=config_file)
         else:
@@ -84,28 +89,23 @@
 
         if config is not None:
             config = config.value
             logging.info(
                 f"Config: {json.dumps(dict(config), sort_keys=True, indent=4)}"
             )
         logging.info("-" * 50)
-        if util.find_spec("tensorflow") is not None:
-            import tensorflow as tf
-
-            logging.info(f"TF decices -> {tf.config.list_logical_devices()}")
-
         notifier.notify_job_started(f"{app_name}.{task_name}")
 
         kwargs = {}
         if db is not None:
             kwargs["db"] = db
         if config is not None:
             kwargs["config"] = config
 
-        ret_val = task(**kwargs)
+        ret_val = task.fn(**kwargs)
         notifier.notify_job_finished(f"{app_name}.{task_name}")
         return ret_val
 
     return wrapper
 
 
 def run(
@@ -123,36 +123,28 @@
     config_file
     mongo_config
 
     Returns
     -------
 
     """
-
-    def pseudo_main(cmd, **kwargs) -> None:
-        TASKS[FLAGS.task](**kwargs)
-
     if notifier is None:
         notifier = BaseNotifier()
 
     if util.find_spec("pymongo") and mongo_config is not None:
         if isinstance(mongo_config, Mapping):
             mongo_config = MongoConfig(**mongo_config)
         db = MongoClient(mongo_config.uri).get_database(mongo_config.db_name)
         if mongo_config.collection is not None:
             db = db.get_collection(mongo_config.collection)
     else:
         db = None
 
     app.install_exception_handler(_ExceptionHandlerImpl(app_name, notifier))
-    global _TASKS
-    TASKS = {
-        k: hook_task(
-            task=v,
-            task_name=k,
-            notifier=notifier,
-            config_file=config_file,
-            app_name=app_name,
-        )
-        for k, v in _TASKS.items()
-    }
-    app.run(partial(pseudo_main, db=db))
+
+    task_fn = pseudo_main(
+        task=_TASK_STORE,
+        notifier=notifier,
+        config_file=config_file,
+        app_name=app_name,
+    )
+    app.run(partial(task_fn, db=db))
```

### Comparing `absl_extra-0.0.1.dev2/absl_extra/tf_utils.py` & `absl_extra-0.0.1.dev3/absl_extra/tf_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import (
     Callable,
     TypeVar,
     Protocol,
     ContextManager,
     runtime_checkable,
     Type,
-    Mapping,
 )
 from contextlib import contextmanager
 import tensorflow as tf
 import platform
 
 
 R = TypeVar("R")
@@ -40,19 +39,23 @@
         Function with the same signature as original one.
 
     """
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs) -> R:
         if linux_only and platform.system() != "linux":
+            logging.info(
+                "Not running on linux, and linux_only==True, ignoring GPU strategy check."
+            )
             return func(*args, **kwargs)
 
-        if len(tf.config.list_physical_devices("GPU")) == 0:
+        gpus = tf.config.list_physical_devices("GPU")
+        logging.info(f"Available GPUs -> {gpus}")
+        if len(gpus) == 0:
             raise RuntimeError("No GPU available.")
-
         return func(*args, **kwargs)
 
     return wrapper
 
 
 @runtime_checkable
 class StrategyLike(Protocol):
@@ -73,20 +76,14 @@
     """
     Used for testing locally scripts, which them must run on Colab TPUs. Allows to keep the same scripts,
     without changing strategy assignment.
     If running on linux, will try to create TPUStrategy. Otherwise, will return NoOpStrategy.
 
     Parameters
     ----------
-    cluster_resolver_kwargs:
-        Kwargs passed to TPUClusterResolver.
-    connector_kwargs:
-        Kwargs passed to experimental_connect_to_cluster.
-    strategy_kwargs:
-        Kwargs passed to TPUStrategy.
 
     Returns
     -------
 
     strategy: TPUStrategy on Linux, NoOpStrategy for other OS hosts.
```

### Comparing `absl_extra-0.0.1.dev2/pyproject.toml` & `absl_extra-0.0.1.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.1dev2"
+version = "0.0.1dev3"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.1.dev2/PKG-INFO` & `absl_extra-0.0.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

