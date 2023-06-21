# Comparing `tmp/machinable-4.3.1.tar.gz` & `tmp/machinable-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machinable-4.3.1.tar", max compression
+gzip compressed data, was "machinable-4.4.0.tar", max compression
```

## Comparing `machinable-4.3.1.tar` & `machinable-4.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      896 2023-06-07 18:23:36.935176 machinable-4.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2023-06-07 18:23:36.935176 machinable-4.3.1/LICENSE.txt
--rw-r--r--   0        0        0     1135 2023-06-07 18:23:36.935176 machinable-4.3.1/README.md
--rw-r--r--   0        0        0     2137 2023-06-07 18:23:36.939177 machinable-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     1385 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/__init__.py
--rw-r--r--   0        0        0     3137 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/cli.py
--rw-r--r--   0        0        0    37644 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/collection.py
--rw-r--r--   0        0        0    11517 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/component.py
--rw-r--r--   0        0        0     2933 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/config.py
--rw-r--r--   0        0        0    22346 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/element.py
--rw-r--r--   0        0        0      615 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/errors.py
--rw-r--r--   0        0        0     6562 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/execution.py
--rw-r--r--   0        0        0     1596 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/group.py
--rw-r--r--   0        0        0     7787 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/index.py
--rw-r--r--   0        0        0    13534 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/interface.py
--rw-r--r--   0        0        0     2480 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/mixin.py
--rw-r--r--   0        0        0    10929 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/project.py
--rw-r--r--   0        0        0       10 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/py.typed
--rw-r--r--   0        0        0      630 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/schedule.py
--rw-r--r--   0        0        0     1296 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/schema.py
--rw-r--r--   0        0        0     1002 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/settings.py
--rw-r--r--   0        0        0     1041 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/storage.py
--rw-r--r--   0        0        0      359 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/types.py
--rw-r--r--   0        0        0    16362 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/utils.py
--rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 machinable-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1245 2023-06-21 04:47:12.751073 machinable-4.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2023-06-21 04:47:12.751073 machinable-4.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1135 2023-06-21 04:47:12.751073 machinable-4.4.0/README.md
+-rw-r--r--   0        0        0     2137 2023-06-21 04:47:12.755073 machinable-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1356 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/__init__.py
+-rw-r--r--   0        0        0     3137 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/cli.py
+-rw-r--r--   0        0        0    37541 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/collection.py
+-rw-r--r--   0        0        0     8576 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/component.py
+-rw-r--r--   0        0        0     2933 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/config.py
+-rw-r--r--   0        0        0    22767 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/element.py
+-rw-r--r--   0        0        0      615 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/errors.py
+-rw-r--r--   0        0        0    14141 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/execution.py
+-rw-r--r--   0        0        0     1596 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/group.py
+-rw-r--r--   0        0        0     8877 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/index.py
+-rw-r--r--   0        0        0    13936 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/interface.py
+-rw-r--r--   0        0        0     2480 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/mixin.py
+-rw-r--r--   0        0        0    10835 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/project.py
+-rw-r--r--   0        0        0       10 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/py.typed
+-rw-r--r--   0        0        0      630 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/schedule.py
+-rw-r--r--   0        0        0     1349 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/schema.py
+-rw-r--r--   0        0        0      952 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/settings.py
+-rw-r--r--   0        0        0     1041 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/storage.py
+-rw-r--r--   0        0        0      359 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/types.py
+-rw-r--r--   0        0        0    16651 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/utils.py
+-rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 machinable-4.4.0/PKG-INFO
```

### Comparing `machinable-4.3.1/CHANGELOG.md` & `machinable-4.4.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 <!-- Please add changes under the Unreleased section that reads 'No current changes' otherwise -->
 
 # Unreleased
 
 No current changes
 
+# v4.4.0
+
+- Improved tracking of execution meta-data
+- Realiable `.execution` access to make None-checks obsolete
+- Adds `stream_output` to simplify live monitoring of execution logs
+- Allow predicate specification based on the element kind
+- Prevent index errors in multithreaded enviroments
+- Disables automatic gathering of project relationship
+
 # v4.3.1
 
 - Drops commandlib dependency
 - Fix Component.execution resolution for resource retrieval
 
 # v4.3.0
```

### Comparing `machinable-4.3.1/LICENSE.txt` & `machinable-4.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/README.md` & `machinable-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/pyproject.toml` & `machinable-4.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "machinable"
-version = "4.3.1"
+version = "4.4.0"
 description = "A modular configuration system for research projects"
 license = "MIT"
 authors = [
     "Frithjof Gressmann <hello@machinable.org>"
 ]
 maintainers = [
     "Frithjof Gressmann <hello@machinable.org>"
@@ -24,27 +24,27 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 flatten-dict = "^0.4"
 jsonlines = "^3.1"
 pydantic = "^1.10.8"
 arrow = "^1.2"
-importlib-metadata = {version = "^6.6", python = "<3.8"}
+importlib-metadata = {version = "^6.7", python = "<3.8"}
 omegaconf = "^2.3.0"
 dill = "^0.3.6"
 typing-extensions = {version = "^4.5.0", python = "<3.11"}
 
 
 [tool.poetry.dev-dependencies]
 isort = "^5.11.5"
 pyupgrade = "^3.3"
 black = "^23.3.0"
 pytest = "^7.3"
 pre-commit = "^2.21.0"
-editorconfig-checker = "^2.7.1"
+editorconfig-checker = "^2.7.2"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 all = [
   "numpy",
   "pandas",
 ]
```

### Comparing `machinable-4.3.1/src/machinable/__init__.py` & `machinable-4.4.0/src/machinable/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from machinable.storage import Storage
 from machinable.types import Optional, Union, VersionType
 
 
 def get(
     module: Union[str, Element, None] = None,
     version: VersionType = None,
-    predicate: Optional[str] = get_settings().default_predicate,
+    predicate: Optional[str] = "$",
     **kwargs,
 ) -> Interface:
     return Interface.get(module, version, predicate, **kwargs)
 
 
 def get_version() -> str:
     try:
```

### Comparing `machinable-4.3.1/src/machinable/cli.py` & `machinable-4.4.0/src/machinable/cli.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/src/machinable/collection.py` & `machinable-4.4.0/src/machinable/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import copy
 from functools import reduce
 from json import dumps
 from pprint import pprint
 
-from machinable.settings import get_settings
 from machinable.types import VersionType
 
 long = int
 unicode = str
 basestring = str
 
 
@@ -1380,15 +1379,15 @@
     def filter_by_module(self, module):
         return self.filter(lambda x: x.module == module)
 
     def filter_by_predicate(
         self,
         module: str,
         version: VersionType = None,
-        predicate: str = get_settings().default_predicate,
+        predicate: str = "$",
         **kwargs,
     ):
         from machinable import Element
 
         try:
             instance = Element.make(module, version, **kwargs)
         except ModuleNotFoundError:
@@ -1403,15 +1402,15 @@
 
         return self.filter(lambda x: x.matches(instance, predicate))
 
     def singleton(
         self,
         module: str,
         version: VersionType = None,
-        predicate: str = get_settings().default_predicate,
+        predicate: str = "$",
         **kwargs,
     ) -> Union[Any, "Component"]:
         from machinable import Element
 
         instance = Element.make(module, version, **kwargs)
 
         for candidate in self:
@@ -1441,22 +1440,22 @@
     def launch(self) -> "ComponentCollection":
         """Executes all components in the collection"""
         for component in self:
             component.launch()
 
         return self
 
+
+class ExecutionCollection(ElementCollection):
+    def __str__(self):
+        return f"Executions <{len(self.items)}>"
+
     def status(self, status="started"):
         """Filters the collection by a status attribute
 
         # Arguments
         status: String, status field: 'started', 'finished', 'alive'
         """
         try:
             return self.filter(lambda item: getattr(item, "is_" + status)())
         except AttributeError as _ex:
             raise ValueError(f"Invalid status field: {status}") from _ex
-
-
-class ExecutionCollection(ElementCollection):
-    def __str__(self):
-        return f"Executions <{len(self.items)}>"
```

### Comparing `machinable-4.3.1/src/machinable/component.py` & `machinable-4.4.0/src/machinable/component.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 from typing import TYPE_CHECKING, List, Optional, Union
 
+import os
 import random
 import sys
 import threading
 
-import arrow
 from machinable.settings import get_settings
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 from typing import Dict
 
 from machinable import errors, schema
 from machinable.collection import ComponentCollection, ExecutionCollection
 from machinable.element import _CONNECTIONS as connected_elements
-from machinable.element import Element, get_dump, get_lineage
+from machinable.element import get_dump, get_lineage
+from machinable.index import Index
 from machinable.interface import Interface, belongs_to, belongs_to_many
 from machinable.project import Project
 from machinable.storage import Storage
-from machinable.types import DatetimeType, TimestampType, VersionType
-from machinable.utils import generate_seed, load_file, save_file
+from machinable.types import VersionType
+from machinable.utils import generate_seed
 
 if TYPE_CHECKING:
     from machinable.execution import Execution
 
 
 class Component(Interface):
     kind = "Component"
@@ -52,102 +48,134 @@
             module=self.__model__.module,
             config=self.__model__.config,
             version=self.__model__.version,
             seed=seed,
             lineage=get_lineage(self),
         )
         self.__model__._dump = get_dump(self)
+        self._current_execution_context = None
+
+    @property
+    def current_execution_context(self) -> "Execution":
+        if self._current_execution_context is None:
+            from machinable.execution import Execution
+
+            self._current_execution_context = Execution.get()
+        return self._current_execution_context
 
     @belongs_to_many(key="execution_history")
     def executions() -> ExecutionCollection:
         from machinable.execution import Execution
 
         return Execution
 
-    @belongs_to(key="execution_history", cached=False)
-    def execution() -> "Execution":
+    @property
+    def execution(self) -> "Execution":
         from machinable.execution import Execution
 
-        return Execution
+        related = None
+        if self.is_mounted():
+            # if mounted, search for related, most recent execution
+            related = Index.get().find_related(
+                relation="Execution.Component.execution_history",
+                uuid=self.uuid,
+                inverse=True,
+            )
 
-    @property
-    def seed(self) -> int:
-        return self.__model__.seed
+            if related is not None and len(related) > 0:
+                related = Interface.find(
+                    sorted(related, key=lambda x: x.timestamp, reverse=True)[
+                        0
+                    ].uuid
+                )
+            else:
+                related = None
 
-    @property
-    def nickname(self) -> str:
-        return self.__model__.nickname
+        # use context if no related execution was found
+        if related is None:
+            if Execution.is_connected():
+                related = Execution.get()
+            else:
+                related = self.current_execution_context
+
+        related.of(self)
+
+        return related
 
     def launch(self) -> Self:
         from machinable.execution import Execution
 
-        execution = Execution.get()
-
-        execution.add(self)
+        self.execution.add(self)
 
         if Execution.is_connected():
             # commit only, defer execution
+            Execution.get().add(self)
             self.commit()
         else:
-            execution.dispatch()
+            self.current_execution_context.add(self)
+            self.current_execution_context.dispatch()
 
         return self
 
+    @property
+    def seed(self) -> int:
+        return self.__model__.seed
+
+    @property
+    def nickname(self) -> str:
+        return self.__model__.nickname
+
     @classmethod
     def collect(cls, components) -> "ComponentCollection":
         return ComponentCollection(components)
 
-    def resources(
-        self, execution: Optional["Execution"] = None
-    ) -> Optional[Dict]:
-        if execution is None:
-            execution = self.execution
-        if execution is None:
-            return None
-        return self.load_file(f"resources/{execution.id}.json", None)
-
     def dispatch(self) -> Self:
         """Dispatch the component lifecycle"""
         writes_meta_data = (
             self.on_write_meta_data() is not False and self.is_mounted()
         )
         try:
             self.on_before_dispatch()
 
             self.on_seeding()
 
             # meta-data
             if writes_meta_data:
-                self.update_status("started")
-                self.save_file(
-                    "host.json",
+                if not self.execution.is_started():
+                    self.execution.update_status(status="started")
+                else:
+                    self.execution.update_status(status="resumed")
+
+                self.execution.save_file(
+                    [self.id, "host.json"],
                     data=Project.get().provider().get_host_info(),
                 )
 
             def beat():
                 t = threading.Timer(15, beat)
                 t.daemon = True
                 t.start()
                 self.on_heartbeat()
                 if self.on_write_meta_data() is not False and self.is_mounted():
-                    self.update_status("heartbeat")
+                    self.execution.update_status(status="heartbeat")
                 return t
 
             heartbeat = beat()
 
             self.__call__()
 
             self.on_success()
             self.on_finish(success=True)
 
             if heartbeat is not None:
                 heartbeat.cancel()
 
             if writes_meta_data:
-                self.update_status("finished")
+                self.execution.update_status(status="finished")
+                self.cached(True, reason="finished")
 
             self.on_after_dispatch(success=True)
         except BaseException as _ex:  # pylint: disable=broad-except
             self.on_failure(exception=_ex)
             self.on_finish(success=False)
             self.on_after_dispatch(success=False)
             raise errors.ComponentException(
@@ -155,20 +183,26 @@
             ) from _ex
         finally:
             if writes_meta_data:
                 # propagate changes
                 for storage in Storage.connected():
                     storage.update(self)
 
-    @property
-    def host_info(self) -> Optional[Dict]:
-        return self.load_file("host.json", None)
+    def cached(
+        self, cached: Optional[bool] = None, reason: str = "user"
+    ) -> bool:
+        if cached is None:
+            return self.load_file("cached", None) is not None
+        elif cached is True:
+            self.save_file("cached", str(reason))
+            return True
+        elif cached is False:
+            os.remove(self.local_directory("cached"), ignore_errors=True)
 
-    def cached(self) -> bool:
-        return self.is_finished()
+        return cached
 
     def dispatch_code(self, inline: bool = True) -> Optional[str]:
         connections = [f"Project('{Project.get().path()}').__enter__()"]
         for kind, elements in connected_elements.items():
             if kind in ["Project", "Execution"]:
                 continue
             for element in elements:
@@ -184,151 +218,19 @@
 
         if inline:
             code = code.replace("\n        ", ";")[1:-1]
             return f'{sys.executable} -c "{code}"'
 
         return code.replace("        ", "")[1:-1]
 
-    def output(self, incremental: bool = False) -> Optional[str]:
-        """Returns the output log"""
-        if not self.is_mounted():
-            return None
-        if incremental:
-            read_length = self._cache.get("output_read_length", 0)
-            if read_length == -1:
-                return ""
-            output = self.load_file("output.log", None)
-            if output is None:
-                return None
-
-            if self.is_finished():
-                self._cache["output_read_length"] = -1
-            else:
-                self._cache["output_read_length"] = len(output)
-            return output[read_length:]
-
-        if "output" in self._cache:
-            return self._cache["output"]
-
-        output = self.load_file("output.log", None)
-
-        if self.is_finished():
-            self._cache["output"] = output
-
-        return output
-
-    def update_status(
-        self,
-        status: Literal["started", "heartbeat", "finished"] = "heartbeat",
-        timestamp: Optional[TimestampType] = None,
-    ) -> None:
-        if timestamp is None:
-            timestamp = arrow.now()
-        if isinstance(timestamp, arrow.Arrow):
-            timestamp = arrow.get(timestamp)
-
-        if status == "started":
-            save_file(
-                self.local_directory("started_at"),
-                str(timestamp) + "\n",
-                # starting event can occur multiple times
-                mode="a",
-            )
-        elif status == "heartbeat":
-            save_file(
-                self.local_directory("heartbeat_at"),
-                str(timestamp),
-                mode="w",
-            )
-        elif status == "finished":
-            save_file(
-                self.local_directory("finished_at"),
-                str(timestamp),
-                mode="w",
-            )
-        else:
-            raise ValueError(
-                f"Invalid status {status}; must be one of 'started', 'heartbeat', 'finished'"
-            )
-
-    def created_at(self) -> Optional[DatetimeType]:
-        if self.timestamp is None:
-            return None
-
-        return arrow.get(self.timestamp)
-
-    def started_at(self) -> Optional[DatetimeType]:
-        """Returns the starting time"""
-        if not self.is_mounted():
-            return None
-        return self._retrieve_status("started")
-
-    def heartbeat_at(self):
-        """Returns the last heartbeat time"""
-        if not self.is_mounted():
-            return None
-        return self._retrieve_status("heartbeat")
-
-    def finished_at(self):
-        """Returns the finishing time"""
-        if not self.is_mounted():
-            return None
-        return self._retrieve_status("finished")
-
-    def _retrieve_status(self, field: str) -> Optional[DatetimeType]:
-        fields = ["started", "heartbeat", "finished"]
-        if field not in fields:
-            raise ValueError(f"Invalid field: {field}. Must be on of {fields}")
-        status = load_file(self.local_directory(f"{field}_at"), default=None)
-        if status is None:
-            return None
-        if field == "started":
-            # can have multiple rows, return latest
-            status = status.strip("\n").split("\n")[-1]
-
-        try:
-            return arrow.get(status)
-        except arrow.ParserError:
-            return None
-
-    def is_finished(self):
-        """True if finishing time has been written"""
-        return bool(self.finished_at())
-
-    def is_started(self):
-        """True if starting time has been written"""
-        return bool(self.started_at())
-
-    def is_active(self):
-        """True if not finished and last heartbeat occurred less than 30 seconds ago"""
-        if not self.heartbeat_at():
-            return False
-
-        return (not self.is_finished()) and (
-            (arrow.now() - self.heartbeat_at()).seconds < 30
-        )
-
-    def is_live(self):
-        """True if active or finished"""
-        return self.is_finished() or self.is_active()
-
-    def is_incomplete(self):
-        """Shorthand for is_started() and not (is_active() or is_finished())"""
-        return self.is_started() and not (
-            self.is_active() or self.is_finished()
-        )
-
     # life cycle
 
     def __call__(self) -> None:
         ...
 
-    def on_before_commit(self) -> Optional[bool]:
-        """Event triggered before the commit of the component"""
-
     def on_before_dispatch(self) -> Optional[bool]:
         """Event triggered before the dispatch of the component"""
 
     def on_success(self):
         """Lifecycle event triggered iff execution finishes successfully"""
 
     def on_finish(self, success: bool):
```

### Comparing `machinable-4.3.1/src/machinable/config.py` & `machinable-4.4.0/src/machinable/config.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/src/machinable/element.py` & `machinable-4.4.0/src/machinable/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import collections
 import copy
 import json
-import os
-import stat
 import sys
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 import arrow
 import dill as pickle
 import machinable
 import omegaconf
-import pydantic
 from machinable import schema
 from machinable.collection import ElementCollection
 from machinable.config import from_element, match_method, rewrite_config_methods
 from machinable.errors import ConfigurationError, MachinableError
 from machinable.mixin import Mixin
-from machinable.settings import get_settings
 from machinable.types import DatetimeType, ElementType, VersionType
 from machinable.utils import Jsonable, sentinel, unflatten_dict, update_dict
 from omegaconf import DictConfig, OmegaConf
 
 
 class ConfigMethod:
     def __init__(self, element: "Element", prefix="config") -> None:
@@ -214,15 +210,27 @@
     result = ""
     for i in range(0, 6 * 2, 2):
         result += alphabet[int(uuid[i : i + 2], 16) % 62]
 
     return result
 
 
-def resolve_custom_predicate(predicate: str, element: "Element"):
+def resolve_custom_predicate(
+    predicate: Optional[str], element: "Element"
+) -> Optional[List[str]]:
+    # predicate may look like this "example,test,*"
+    #  where * represents a placeholder for all the custom predicates
+    #  that are marked with a trailing * (i.e. default predicates)
+    # $ is a shorthand for inferring the predicate from the element
+    if predicate == "$":
+        predicate = element.default_predicate
+
+    if predicate is None:
+        return None
+
     from machinable.project import Project
 
     custom = element.on_compute_predicate() or {}
     if isinstance(element, Project):
         custom.update(element.global_predicate() or {})
     else:
         custom.update(Project.get().provider().global_predicate() or {})
@@ -258,14 +266,15 @@
 
 
 class Element(Mixin, Jsonable):
     """Element baseclass"""
 
     kind: Optional[str] = "Element"
     default: Optional["Element"] = None
+    default_predicate: Optional[str] = "config,*"
     _module_: Optional[str] = None
 
     def __init__(self, version: VersionType = None):
         super().__init__()
         if Element._module_ is None:
             Element._module_ = self.__module__
         self.__model__ = schema.Element(
@@ -293,15 +302,15 @@
     def id(self) -> str:
         return self.uuid[:6]
 
     @property
     def timestamp(self) -> float:
         return self.__model__.timestamp
 
-    def timestamp_at(self) -> DatetimeType:
+    def created_at(self) -> DatetimeType:
         return arrow.get(self.__model__.timestamp)
 
     def version(
         self, version: VersionType = sentinel, overwrite: bool = False
     ) -> List[Union[str, dict]]:
         if version is sentinel:
             return self.__model__.version
@@ -342,15 +351,15 @@
         return _CONNECTIONS[cls.kind]
 
     @classmethod
     def get(
         cls,
         module: Union[str, "Element", None] = None,
         version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
+        predicate: Optional[str] = "$",
         **kwargs,
     ) -> "Element":
         if module is None and version is None:
             if len(_CONNECTIONS[cls.kind]) > 0:
                 return _CONNECTIONS[cls.kind][-1]
 
         if module is None or predicate is None:
@@ -396,15 +405,15 @@
         return cls.make(module, version, base_class=cls, **kwargs)
 
     @classmethod
     def singleton(
         cls,
         module: Union[str, "Element"],
         version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
+        predicate: Optional[str] = "$",
         **kwargs,
     ) -> "Element":
         # no-op as elements do not have a storage representation
         return cls.make(module, version, **kwargs)
 
     @classmethod
     def from_model(cls, model: schema.Element) -> "Element":
@@ -565,15 +574,19 @@
 
         if cls.kind is None:
             return schema.Element
 
         return getattr(schema, cls.kind)
 
     def matches(self, element: "Element", predicate: str) -> bool:
-        for p in resolve_custom_predicate(predicate, element):
+        predicate_fields = resolve_custom_predicate(predicate, element)
+        if predicate_fields is None:
+            return False
+
+        for p in predicate_fields:
             if not equalversion(self.predicate[p], element.predicate[p]):
                 return False
 
         return True
 
     def set_model(self, model: schema.Element) -> Self:
         self.__model__ = model
@@ -671,15 +684,15 @@
     def __setstate__(self, state):
         self.__model__ = self.__class__.model()(**state)
 
     def __repr__(self):
         return f"{self.kind} [{self.id}]"
 
     def __str__(self):
-        return self.__repr__()
+        return self.id
 
     def __eq__(self, other):
         return self.uuid == other.uuid
 
     def __ne__(self, other):
         return self.uuid != other.uuid
```

### Comparing `machinable-4.3.1/src/machinable/errors.py` & `machinable-4.4.0/src/machinable/errors.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/src/machinable/group.py` & `machinable-4.4.0/src/machinable/group.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/src/machinable/index.py` & `machinable-4.4.0/src/machinable/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, List, Optional, Union
 
 import json
 import os
+from contextlib import contextmanager
 from datetime import datetime
 
 try:
     from pysqlite3 import dbapi2 as sqlite3
 except ModuleNotFoundError:
     import sqlite3
 
@@ -83,14 +84,24 @@
             else:
                 os.makedirs(os.path.dirname(database), exist_ok=True)
     db = sqlite3.connect(database)
     migrate(db)
     return db
 
 
+@contextmanager
+def db(database: str, create=False) -> Optional[sqlite3.Connection]:
+    try:
+        database = load(database, create)
+        yield database
+        database.close()
+    except FileNotFoundError:
+        yield None
+
+
 class Index(Interface):
     kind = "Index"
     default = get_settings().default_index
 
     class Config:
         directory: str = "./storage"
         database: str = "in_directory('index.sqlite')"
@@ -119,126 +130,138 @@
         return self._db
 
     def local_directory(self, uuid: str, *append: str) -> str:
         # TODO: allow custom directory mappings
         return os.path.join(self.config.directory, uuid, *append)
 
     def commit(self, model: schema.Interface) -> bool:
-        cur = self.db.cursor()
-        if cur.execute(
-            """SELECT uuid FROM 'index' WHERE uuid=?""", (model.uuid,)
-        ).fetchone():
-            # already exists
-            return False
-        cur.execute(
-            """INSERT INTO 'index' (
-                uuid,
-                kind,
-                module,
-                config,
-                version,
-                predicate,
-                lineage,
-                'timestamp'
-            ) VALUES (?,?,?,?,?,?,?,?)""",
-            (
-                model.uuid,
-                model.kind,
-                model.module,
-                _jn(model.config),
-                _jn(model.version),
-                _jn(model.predicate),
-                _jn(model.lineage),
-                model.timestamp,
-            ),
-        )
-        self.db.commit()
+        with db(self.config.database, create=True) as _db:
+            cur = _db.cursor()
+            if cur.execute(
+                """SELECT uuid FROM 'index' WHERE uuid=?""", (model.uuid,)
+            ).fetchone():
+                # already exists
+                return False
+            cur.execute(
+                """INSERT INTO 'index' (
+                    uuid,
+                    kind,
+                    module,
+                    config,
+                    version,
+                    predicate,
+                    lineage,
+                    'timestamp'
+                ) VALUES (?,?,?,?,?,?,?,?)""",
+                (
+                    model.uuid,
+                    model.kind,
+                    model.module,
+                    _jn(model.config),
+                    _jn(model.version),
+                    _jn(model.predicate),
+                    _jn(model.lineage),
+                    model.timestamp,
+                ),
+            )
+            _db.commit()
         return True
 
     def create_relation(
         self,
         relation: str,
         uuid: str,
         related_uuid: Union[str, List[str]],
         priority: int = 0,
         timestamp: Optional[float] = None,
     ) -> None:
         if isinstance(related_uuid, (list, tuple)):
             for r in related_uuid:
                 self.create_relation(relation, uuid, r, priority, timestamp)
             return
-
-        cur = self.db.cursor()
-        if cur.execute(
-            """SELECT id FROM 'relations' WHERE uuid=? AND related_uuid=? AND relation=?""",
-            (uuid, related_uuid, relation),
-        ).fetchone():
-            # already exists
-            return
-        if timestamp is None:
-            timestamp = datetime.now().timestamp()
-        cur.execute(
-            """INSERT INTO 'relations' (
-                relation,
-                uuid,
-                related_uuid,
-                priority,
-                timestamp
-            ) VALUES (?,?,?,?,?)""",
-            (relation, uuid, related_uuid, priority, timestamp),
-        )
-        self.db.commit()
+        with db(self.config.database, create=True) as _db:
+            cur = _db.cursor()
+            if cur.execute(
+                """SELECT id FROM 'relations' WHERE uuid=? AND related_uuid=? AND relation=?""",
+                (uuid, related_uuid, relation),
+            ).fetchone():
+                # already exists
+                return
+            if timestamp is None:
+                timestamp = datetime.now().timestamp()
+            cur.execute(
+                """INSERT INTO 'relations' (
+                    relation,
+                    uuid,
+                    related_uuid,
+                    priority,
+                    timestamp
+                ) VALUES (?,?,?,?,?)""",
+                (relation, uuid, related_uuid, priority, timestamp),
+            )
+            _db.commit()
 
     def find(self, uuid: str) -> Optional[schema.Interface]:
-        cur = self.db.cursor()
-        row = cur.execute(
-            """SELECT * FROM 'index' WHERE uuid=?""", (uuid,)
-        ).fetchone()
-        if row is None:
-            return None
-        return interface_row_factory(cur, row)
+        with db(self.config.database, create=False) as _db:
+            if not _db:
+                return None
+            cur = _db.cursor()
+            row = cur.execute(
+                """SELECT * FROM 'index' WHERE uuid=?""", (uuid,)
+            ).fetchone()
+            if row is None:
+                return None
+            return interface_row_factory(cur, row)
 
     def find_by_predicate(
         self, module: str, predicate: Optional[Dict] = None
     ) -> List[schema.Interface]:
-        cur = self.db.cursor()
-        if predicate:
-            keys = ["module=?"]
-            values = [module]
-            for p, v in predicate.items():
-                keys.append(f"json_extract(predicate, '$.{p}')=?")
-                values.append(v if isinstance(v, (str, int, float)) else _jn(v))
-            query = cur.execute(
-                """SELECT * FROM 'index' WHERE """ + (" AND ".join(keys)),
-                values,
-            )
-        else:
-            query = cur.execute(
-                """SELECT * FROM 'index' WHERE module=?""",
-                (module,),
-            )
+        with db(self.config.database, create=False) as _db:
+            if not _db:
+                return []
+            cur = _db.cursor()
+            if predicate:
+                keys = ["module=?"]
+                values = [module]
+                for p, v in predicate.items():
+                    keys.append(f"json_extract(predicate, '$.{p}')=?")
+                    values.append(
+                        v if isinstance(v, (str, int, float)) else _jn(v)
+                    )
+                query = cur.execute(
+                    """SELECT * FROM 'index' WHERE """ + (" AND ".join(keys)),
+                    values,
+                )
+            else:
+                query = cur.execute(
+                    """SELECT * FROM 'index' WHERE module=?""",
+                    (module,),
+                )
 
-        return [interface_row_factory(cur, row) for row in query.fetchall()]
+            return [interface_row_factory(cur, row) for row in query.fetchall()]
 
     def find_related(
         self, relation: str, uuid: str, inverse: bool = False
     ) -> Union[None, List[schema.Interface]]:
-        cur = self.db.cursor()
-        if not inverse:
-            rows = cur.execute(
-                """SELECT * FROM 'index' WHERE uuid IN
-                    (
-                    SELECT related_uuid FROM relations WHERE uuid=? AND relation=?
-                    )  ORDER BY 'timestamp' ASC
-                """,
-                (uuid, relation),
-            ).fetchall()
-        else:
-            rows = cur.execute(
-                """SELECT * FROM 'index' WHERE uuid IN
-                    (
-                    SELECT uuid FROM relations WHERE related_uuid=? AND relation=? ORDER BY 'timestamp' DESC
-                    )  ORDER BY 'timestamp' ASC
-                """,
-                (uuid, relation),
-            ).fetchall()
-        return [interface_row_factory(cur, row) for row in rows or []]
+        with db(self.config.database, create=False) as _db:
+            if not _db:
+                return None
+            cur = _db.cursor()
+            if not inverse:
+                rows = cur.execute(
+                    """SELECT * FROM 'index' WHERE uuid IN
+                        (
+                        SELECT related_uuid FROM relations WHERE uuid=? AND relation=?
+                        )  ORDER BY 'timestamp' DESC
+                    """,
+                    (uuid, relation),
+                ).fetchall()
+            else:
+                rows = cur.execute(
+                    """SELECT * FROM 'index' WHERE uuid IN
+                        (
+                        SELECT uuid FROM relations WHERE related_uuid=? AND relation=?
+                        )  ORDER BY 'timestamp' DESC
+                    """,
+                    (uuid, relation),
+                ).fetchall()
+            return [interface_row_factory(cur, row) for row in rows or []]
```

### Comparing `machinable-4.3.1/src/machinable/interface.py` & `machinable-4.4.0/src/machinable/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,30 @@
     from typing_extensions import Self
 
 from typing import Callable
 
 import os
 from functools import partial, wraps
 
-from machinable import schema
+from machinable import errors, schema
 from machinable.collection import Collection, InterfaceCollection
 from machinable.element import (
     Element,
     get_dump,
     get_lineage,
     resolve_custom_predicate,
 )
 from machinable.settings import get_settings
 from machinable.types import VersionType
-from machinable.utils import is_directory_version, load_file, save_file
+from machinable.utils import (
+    is_directory_version,
+    joinpath,
+    load_file,
+    save_file,
+)
 from omegaconf import OmegaConf
 
 
 class Relation:
     inverse: bool = False
     multiple: bool = False
 
@@ -64,14 +69,16 @@
     def collect(self, elements: List["Interface"]) -> Collection:
         if self.collection is None:
             return self.related_cls.collect(elements)
         return self.collection(elements)
 
     def __set_name__(self, cls, name):
         self.cls = cls
+        if cls.__relations__ is None:
+            cls.__relations__ = {}
         cls.__relations__[name] = self
 
     def __get__(self, instance, owner):
         if (
             not instance._relation_cache.get(self.fn.__name__, None)
             and instance.is_mounted()
         ):
@@ -136,15 +143,15 @@
 
 class Interface(Element):
     kind = "Interface"
     default = get_settings().default_interface
     # class level relationship information
     # note that the actual data is kept
     # in the __related__ object propery
-    __relations__: Dict[str, Relation] = {}
+    __relations__: Optional[Dict[str, Relation]] = None
 
     def __init__(
         self,
         version: VersionType = None,
         uses: Union[None, "Interface", List["Interface"]] = None,
         derived_from: Optional["Interface"] = None,
     ):
@@ -157,37 +164,54 @@
             lineage=get_lineage(self),
         )
         self.__model__._dump = get_dump(self)
 
         # initialize relation data
         self.__related__ = {}
         self._relation_cache = {}
+        if self.__relations__ is None:
+            self.__relations__ = {}
         for name, relation in self.__relations__.items():
             if relation.multiple:
                 self.__related__[name] = relation.collect([])
             else:
                 self.__related__[name] = None
         if uses:
-            self.use(uses)
-        self.push_related("ancestor", derived_from)
+            if not isinstance(uses, (list, tuple)):
+                uses = [uses]
+            for use in uses:
+                self.__related__["uses"].append(use)
+            self._relation_cache["uses"] = True
+
+        if derived_from:
+            self.__related__["ancestor"] = derived_from
+            self._relation_cache["ancestor"] = True
 
         self._deferred_data = {}
 
     @classmethod
     def collect(cls, elements) -> InterfaceCollection:
         return InterfaceCollection(elements)
 
     def push_related(self, key: str, value: "Interface") -> None:
-        # todo: check for editablility
+        if self.is_committed():
+            raise errors.MachinableError(
+                f"{repr(self)} already exists and cannot be modified."
+            )
         if self.__relations__[key].multiple:
             self.__related__[key].append(value)
         else:
             self.__related__[key] = value
         self._relation_cache[key] = True
 
+    def is_committed(self) -> bool:
+        from machinable.index import Index
+
+        return Index.get().find(self.uuid) is not None
+
     def commit(self) -> Self:
         from machinable.index import Index
 
         # ensure that configuration has been parsed
         assert self.config is not None
         assert self.predicate is not None
 
@@ -256,46 +280,34 @@
                         f"{key}={shlex.quote(str(val))}"
                         for key, val in flatten(v, reducer="dot").items()
                     ]
                 )
 
         return " ".join(cli)
 
-    def use(self, use: Union[Element, List[Element]]) -> Self:
-        # todo: check for editablility
-
-        if isinstance(use, (list, tuple)):
-            for _use in use:
-                self.use(_use)
-            return self
-
-        self.push_related("uses", use)
-
-        return self
-
     def derive(
         self,
         module: Union[str, Element, None] = None,
         version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
+        predicate: Optional[str] = "$",
         **kwargs,
     ) -> Self:
         if module is None or predicate is None:
             return self.make(module, version, derived_from=self, **kwargs)
 
         return self.derived.singleton(
             module, version, predicate, derived_from=self, **kwargs
         )
 
     @classmethod
     def singleton(
         cls,
         module: Union[str, "Element"],
         version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
+        predicate: Optional[str] = "$",
         **kwargs,
     ) -> "Collection":
         if module in [
             "machinable.index",
             "machinable.project",
         ] and is_directory_version(version):
             # interpret as shortcut for directory
@@ -348,78 +360,79 @@
         return cls.collect([cls.find(uuid) for uuid in uuids])
 
     @classmethod
     def find_by_predicate(
         cls,
         module: Union[str, "Element"],
         version: VersionType = None,
-        predicate: Optional[str] = get_settings().default_predicate,
+        predicate: Optional[str] = "$",
         **kwargs,
     ) -> "Collection":
         from machinable.index import Index
 
         try:
             candidate = cls.make(module, version, **kwargs)
         except ModuleNotFoundError:
             return cls.collect([])
 
-        if predicate:
-            predicate = OmegaConf.to_container(
-                OmegaConf.create(
-                    {
-                        p: candidate.predicate[p]
-                        for p in resolve_custom_predicate(predicate, candidate)
-                    }
-                )
+        predicate_fields = resolve_custom_predicate(predicate, candidate)
+
+        if predicate_fields is None:
+            return cls.collect([])
+
+        predicate_data = OmegaConf.to_container(
+            OmegaConf.create(
+                {p: candidate.predicate[p] for p in predicate_fields}
             )
+        )
 
         return cls.collect(
             [
                 cls.find(interface.uuid)
                 for interface in Index.get().find_by_predicate(
                     module
                     if isinstance(module, str)
                     else f"__session__{module.__name__}",
-                    predicate,
+                    predicate_data,
                 )
             ]
         )
 
     @classmethod
     def from_directory(cls, directory: str) -> "Element":
         """Returns an interface from a storage directory
 
         Note that this does not verify the integrity of the directory.
         In particular, the interface may be missing or not be indexed.
         """
-        data = load_file(os.path.join(directory, "model.json"))
+        data = load_file([directory, "model.json"])
 
         model = getattr(schema, data["kind"], None)
         if model is None:
             # TODO: users should have an option to register custom interface types
             raise ValueError(f"Invalid interface kind: {model['kind']}")
 
         interface = model(**data)
         if interface.module.startswith("__session__"):
-            interface._dump = load_file(os.path.join(directory, "dump.p"), None)
+            interface._dump = load_file([directory, "dump.p"], None)
 
         return cls.from_model(interface)
 
     def to_directory(self, directory: str, relations=True) -> Self:
-        save_file(os.path.join(directory, ".machinable"), self.__model__.uuid)
-        save_file(os.path.join(directory, "model.json"), self.__model__)
+        save_file([directory, ".machinable"], self.__model__.uuid)
+        save_file([directory, "model.json"], self.__model__)
         if self.__model__._dump is not None:
-            save_file(os.path.join(directory, "dump.p"), self.__model__._dump)
+            save_file([directory, "dump.p"], self.__model__._dump)
         if relations:
             for k, v in self.__related__.items():
                 if hasattr(v, "uuid"):
-                    save_file(os.path.join(directory, "related", k), v.uuid)
+                    save_file([directory, "related", k], v.uuid)
                 elif v:
                     save_file(
-                        os.path.join(directory, "related", k),
+                        [directory, "related", k],
                         "\n".join([i.uuid for i in v]),
                         mode="w",
                     )
 
         return self
 
     def local_directory(self, *append: str, create: bool = False) -> str:
@@ -428,27 +441,32 @@
         directory = Index.get().local_directory(self.uuid, *append)
 
         if create:
             os.makedirs(directory, exist_ok=True)
 
         return directory
 
-    def load_file(self, filepath: str, default=None) -> Optional[Any]:
+    def load_file(
+        self, filepath: Union[str, List[str]], default=None
+    ) -> Optional[Any]:
+        filepath = joinpath(filepath)
         if not self.is_mounted():
             # has write been deferred?
             if filepath in self._deferred_data:
                 return self._deferred_data[filepath]
 
             return default
 
         data = load_file(self.local_directory(filepath), default=None)
 
         return data if data is not None else default
 
-    def save_file(self, filepath: str, data: Any) -> str:
+    def save_file(self, filepath: Union[str, List[str]], data: Any) -> str:
+        filepath = joinpath(filepath)
+
         if os.path.isabs(filepath):
             raise ValueError("Filepath must be relative")
 
         if not self.is_mounted():
             # defer writes until interface storage is mounted
             self._deferred_data[filepath] = data
             return "$deferred"
```

### Comparing `machinable-4.3.1/src/machinable/mixin.py` & `machinable-4.4.0/src/machinable/mixin.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/src/machinable/project.py` & `machinable-4.4.0/src/machinable/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,17 +292,14 @@
         element = instantiate(
             module,
             element_class,
             version,
             **constructor_kwargs,
         )
 
-        if isinstance(element, Interface):
-            element.push_related("project", self)
-
         return element
 
     def get_diff(self) -> Union[str, None]:
         return get_diff(self.path())
 
     def exists(self) -> bool:
         return os.path.exists(self.config.directory)
```

### Comparing `machinable-4.3.1/src/machinable/schedule.py` & `machinable-4.4.0/src/machinable/schedule.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/src/machinable/schema.py` & `machinable-4.4.0/src/machinable/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 class Project(Interface):
     kind: str = "Project"
 
 
 class Execution(Interface):
     kind: str = "Execution"
+    seed: int = Field(default_factory=generate_seed)
     resources: Optional[Dict] = None
 
 
 class Schedule(Interface):
     kind: str = "Schedule"
```

### Comparing `machinable-4.3.1/src/machinable/settings.py` & `machinable-4.4.0/src/machinable/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from machinable.errors import ConfigurationError
 from machinable.types import ElementType
 from pydantic import BaseModel, Field
 
 
 class Settings(BaseModel):
-    default_predicate: Optional[str] = "config,*"
     default_execution: Optional[ElementType] = None
     default_component: Optional[ElementType] = None
     default_interface: Optional[ElementType] = None
     default_schedule: Optional[ElementType] = None
     default_group: Optional[str] = "%Y_%U_%a/"
     default_storage: Optional[ElementType] = None
     default_index: Optional[ElementType] = None
```

### Comparing `machinable-4.3.1/src/machinable/storage.py` & `machinable-4.4.0/src/machinable/storage.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.1/src/machinable/utils.py` & `machinable-4.4.0/src/machinable/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,21 @@
         return True
     if "/" in version or "\\" in version or version == "~":
         return True
 
     return False
 
 
+def joinpath(filepath: Union[str, List[str]]) -> str:
+    if isinstance(filepath, str):
+        return filepath
+
+    return os.path.join(*[str(p) for p in filepath if p is not None])
+
+
 def random_str(length: int, random_state=None):
     if random_state is None or isinstance(random_state, int):
         random_state = random.Random(random_state)
 
     return "".join(
         random_state.choice(
             string.ascii_uppercase + string.ascii_lowercase + string.digits
@@ -209,29 +216,30 @@
         if category not in _WORDS:
             raise KeyError(f"Invalid category: {category}")
         picks.append(random.choice(_WORDS[category]))
     return glue.join(picks)
 
 
 def load_file(
-    filepath: str,
+    filepath: Union[str, List[str]],
     default: Any = sentinel,
     opener=open,
     **opener_kwargs,
 ) -> Any:
     """Loads a data object from file
 
     # Arguments
     filepath: Target filepath. The extension is being used to determine
         the file format. Supported formats are:
         .json (JSON), .jsonl (JSON-lines), .npy (numpy), .p (pickle); all other will be loaded as plain text (e.g. .txt|.log|.diff|.sh)
     default: Optional default if reading fails
     opener: Customer file opener
     opener_kwargs: Optional arguments to pass to the opener
     """
+    filepath = joinpath(filepath)
     _, ext = os.path.splitext(filepath)
     mode = opener_kwargs.pop("mode", "r")
     try:
         if ext == ".p":
             if "b" not in mode:
                 mode = mode + "b"
             with opener(filepath, mode, **opener_kwargs) as f:
@@ -258,15 +266,15 @@
     except (FileNotFoundError, Exception) as _ex:
         if default is not sentinel:
             return default
         raise _ex
 
 
 def save_file(
-    filepath: str,
+    filepath: Union[str, List[str]],
     data: Any,
     makedirs: Union[bool, Callable] = True,
     opener=open,
     **opener_kwargs,
 ) -> str:
     """Saves a data object to file
 
@@ -277,14 +285,15 @@
     data: The data object
     makedirs: If True or Callable, path will be created
     opener: Customer file opener
     opener_kwargs: Optional arguments to pass to the opener
 
     Returns the absolute path to the written file
     """
+    filepath = joinpath(filepath)
     path = os.path.dirname(filepath)
     name = os.path.basename(filepath)
     _, ext = os.path.splitext(name)
     mode = opener_kwargs.pop("mode", "w")
 
     if path != "":
         if makedirs is True:
```

### Comparing `machinable-4.3.1/PKG-INFO` & `machinable-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machinable
-Version: 4.3.1
+Version: 4.4.0
 Summary: A modular configuration system for research projects
 Home-page: https://machinable.org
 License: MIT
 Keywords: machine-learning,research
 Author: Frithjof Gressmann
 Author-email: hello@machinable.org
 Maintainer: Frithjof Gressmann
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Requires-Dist: arrow (>=1.2,<2.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: flatten-dict (>=0.4,<0.5)
-Requires-Dist: importlib-metadata (>=6.6,<7.0) ; python_version < "3.8"
+Requires-Dist: importlib-metadata (>=6.7,<7.0) ; python_version < "3.8"
 Requires-Dist: jsonlines (>=3.1,<4.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Documentation, https://machinable.org
 Project-URL: Repository, https://github.com/machinable-org/machinable
 Description-Content-Type: text/markdown
```

