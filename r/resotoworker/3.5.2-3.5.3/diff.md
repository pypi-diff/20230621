# Comparing `tmp/resotoworker-3.5.2.tar.gz` & `tmp/resotoworker-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.5.2.tar", last modified: Tue Jun 13 13:06:57 2023, max compression
+gzip compressed data, was "resotoworker-3.5.3.tar", last modified: Wed Jun 21 14:25:24 2023, max compression
```

## Comparing `resotoworker-3.5.2.tar` & `resotoworker-3.5.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.587864 resotoworker-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:07.000000 resotoworker-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-13 13:06:57.587864 resotoworker-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-13 13:03:07.000000 resotoworker-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 13:03:07.000000 resotoworker-3.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.583864 resotoworker-3.5.2/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.583864 resotoworker-3.5.2/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:20.000000 resotoworker-3.5.2/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:06:57.587864 resotoworker-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.583864 resotoworker-3.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.292047 resotoworker-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:21:54.000000 resotoworker-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-21 14:25:24.292047 resotoworker-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-21 14:21:54.000000 resotoworker-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 14:21:54.000000 resotoworker-3.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.288047 resotoworker-3.5.3/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.288047 resotoworker-3.5.3/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:22:56.000000 resotoworker-3.5.3/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:25:24.292047 resotoworker-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.292047 resotoworker-3.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_utils.py
```

### Comparing `resotoworker-3.5.2/PKG-INFO` & `resotoworker-3.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.2
+Version: 3.5.3
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.5.2/README.md` & `resotoworker-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/pyproject.toml` & `resotoworker-3.5.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "resotoworker"
-version = "3.5.2"
+version = "3.5.3"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.2",
+    "resotolib==3.5.3",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 resotoworker = "resotoworker.__main__:main"
```

### Comparing `resotoworker-3.5.2/resotoworker/__main__.py` & `resotoworker-3.5.3/resotoworker/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import threading
 import cherrypy  # type: ignore
 import time
 from functools import partial
 from queue import Queue
 from signal import SIGTERM
-from typing import List, Dict, Type, Optional, Any
+from typing import List, Dict, Type, Optional, Any, Callable
 
 import requests
 
 import resotolib.proc
 from resotolib.args import ArgumentParser
 from resotolib.baseplugin import BaseActionPlugin, BasePostCollectPlugin, BaseCollectorPlugin, PluginType
 from resotolib.config import Config
@@ -71,14 +71,17 @@
     plugin_loader = PluginLoader()
     plugin_loader.add_plugin_args(arg_parser)
 
     # At this point the CLI, all Plugins as well as the WebServer have
     # added their args to the arg parser
     arg_parser.parse_args()
 
+    # Register functions to detect system healthiness
+    health_conditions: Dict[str, Callable[[], bool]] = {}
+
     try:
         wait_for_resotocore(resotocore.http_uri)
     except TimeoutError as e:
         log.fatal(f"Failed to connect to resotocore: {e}")
         sys.exit(1)
 
     tls_data: Optional[TLSData] = None
@@ -89,14 +92,15 @@
         )
         tls_data.start()
     config = Config(
         ArgumentParser.args.subscriber_id,
         resotocore_uri=resotocore.http_uri,
         tls_data=tls_data,
     )
+    health_conditions["Config Listener"] = config.connected
 
     add_config(config, plugin_loader.all_collector_plugins())
     plugin_loader.add_plugin_config(config)
     config.load_config()
 
     write_files_to_home_dir(config.resotoworker.all_files_in_home_dir(), write_utf8_file)
 
@@ -126,15 +130,19 @@
     web_server_args = {}
     if tls_data and not Config.resotoworker.no_tls:
         web_server_args = {
             "ssl_cert": tls_data.cert_path,
             "ssl_key": tls_data.key_path,
         }
     web_server = WebServer(
-        WorkerWebApp(mountpoint=Config.resotoworker.web_path, plugin_loader=plugin_loader),
+        WorkerWebApp(
+            mountpoint=Config.resotoworker.web_path,
+            plugin_loader=plugin_loader,
+            health_conditions=health_conditions,
+        ),
         web_host=Config.resotoworker.web_host,
         web_port=Config.resotoworker.web_port,
         **web_server_args,
     )
     web_server.daemon = True
     web_server.start()
 
@@ -152,14 +160,15 @@
                 "wait_for_completion": True,
             },
         },
         message_processor=partial(core_actions_processor, config, plugin_loader, tls_data, collector),
         tls_data=tls_data,
         incoming_messages=core_messages,
     )
+    health_conditions["CoreActions"] = core_actions.connected
 
     # make tagging by collectors available out of the box
     collect_plugins: List[BaseCollectorPlugin] = plugin_loader.plugins(PluginType.COLLECTOR)  # type: ignore
     task_handler = [
         CoreTaskHandler(
             name="tag",
             info="already provided",
@@ -182,14 +191,15 @@
         identifier=f"{ArgumentParser.args.subscriber_id}-task-handler",
         resotocore_ws_uri=resotocore.ws_uri,
         task_handler=task_handler,
         tls_data=tls_data,
     )
     core_actions.start()
     core_tasks.start()
+    health_conditions["CoreTasks"] = core_tasks.connected
 
     for plugin_class in plugin_loader.plugins(PluginType.ACTION):
         assert issubclass(plugin_class, BaseActionPlugin)
         try:
             log.debug(f"Starting action plugin {plugin_class}")
             plugin = plugin_class(tls_data=tls_data)
             plugin.start()
```

### Comparing `resotoworker-3.5.2/resotoworker/cleanup.py` & `resotoworker-3.5.3/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/resotoworker/collect.py` & `resotoworker-3.5.3/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/resotoworker/config.py` & `resotoworker-3.5.3/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/resotoworker/pluginloader.py` & `resotoworker-3.5.3/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/resotoworker/resotocore.py` & `resotoworker-3.5.3/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/resotoworker/tag.py` & `resotoworker-3.5.3/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/resotoworker/utils.py` & `resotoworker-3.5.3/resotoworker/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from resotoworker.config import HomeDirectoryFile
 
 
 def write_utf8_file(path: Path, content: str) -> None:
     """Write a UTF-8 encoded file to disk"""
     try:
         path.parent.mkdir(parents=True, exist_ok=True)
-        with open(os.open(path, os.O_CREAT | os.O_WRONLY, 0o600), "wb") as f:
+        with open(os.open(path, os.O_CREAT | os.O_WRONLY | os.O_TRUNC, 0o600), "wb") as f:
             f.write(content.encode("utf-8"))
 
     except Exception as e:
         log.warning(f"Failed to write file {path}: {e}")
         return
```

### Comparing `resotoworker-3.5.2/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.5.3/resotoworker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.2
+Version: 3.5.3
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.5.2/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.5.3/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/test/test_args.py` & `resotoworker-3.5.3/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/test/test_collect.py` & `resotoworker-3.5.3/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/test/test_resotocore.py` & `resotoworker-3.5.3/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.2/test/test_utils.py` & `resotoworker-3.5.3/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from typing import Optional, List, Any
 
 
 def test_write_utf8_file() -> None:
     with TemporaryDirectory() as tmpdir:
         f = Path(tmpdir) / "foo" / "test.txt"
+        write_utf8_file(f, "extra long line that must be truncated first")
         write_utf8_file(f, "bar")
         assert f.read_text(encoding="utf-8") == "bar"
         assert f.stat().st_mode & 0o777 == 0o600
 
 
 class InMemoryFile:
     def __init__(self) -> None:
```

