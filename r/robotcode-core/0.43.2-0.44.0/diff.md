# Comparing `tmp/robotcode_core-0.43.2.tar.gz` & `tmp/robotcode_core-0.44.0.tar.gz`

## Comparing `robotcode_core-0.43.2.tar` & `robotcode_core-0.44.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/async_cache.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/async_itertools.py
--rw-r--r--   0        0        0    21626 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0    15582 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/dataclasses.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/event.py
--rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/logging.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/py.typed
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/types.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/uri.py
--rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/lsp/types.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/LICENSE.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/README.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/pyproject.toml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.43.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/async_cache.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/async_itertools.py
+-rw-r--r--   0        0        0    21626 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0    15582 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/dataclasses.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/event.py
+-rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/logging.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/types.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/lsp/types.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/process.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/LICENSE.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/README.md
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.44.0/PKG-INFO
```

### Comparing `robotcode_core-0.43.2/src/robotcode/core/async_cache.py` & `robotcode_core-0.44.0/src/robotcode/core/async_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/async_itertools.py` & `robotcode_core-0.44.0/src/robotcode/core/async_itertools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/async_tools.py` & `robotcode_core-0.44.0/src/robotcode/core/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/dataclasses.py` & `robotcode_core-0.44.0/src/robotcode/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/event.py` & `robotcode_core-0.44.0/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/logging.py` & `robotcode_core-0.44.0/src/robotcode/core/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     __owner: Any = None
     __owner_name: Optional[str] = None
     __postfix: str = ""
     __logger: Optional[logging.Logger] = None
 
     def __init__(
         self,
-        _func: _FUNC_TYPE = None,
+        _func: Optional[_FUNC_TYPE] = None,
         *,
         name: Optional[str] = None,
         postfix: str = "",
         level: int = logging.NOTSET,
     ) -> None:
         self.__func = _func
 
@@ -168,15 +168,15 @@
 
         return self.__logger
 
     def __set_name__(self, owner: Any, name: str) -> None:
         self.__owner = owner
         self.__owner_name = name
 
-    def __call__(self, _func: _FUNC_TYPE = None) -> LoggingDescriptor:
+    def __call__(self, _func: Optional[_FUNC_TYPE] = None) -> LoggingDescriptor:
         if _func is not None:
             self.__func = _func
 
         return self
 
     def __get__(self, obj: Any, objtype: Type[Any]) -> LoggingDescriptor:
         return self
```

### Comparing `robotcode_core-0.43.2/src/robotcode/core/uri.py` & `robotcode_core-0.44.0/src/robotcode/core/uri.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/lsp/types.py` & `robotcode_core-0.44.0/src/robotcode/core/lsp/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.44.0/src/robotcode/core/utils/debugpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Sequence, Tuple, Union
+from typing import Optional, Sequence, Tuple, Union
 
 from ..logging import LoggingDescriptor
 from .net import find_free_port
 
 _logger = LoggingDescriptor(name=__name__)
 
 
@@ -39,24 +39,23 @@
         for address in addresses:
             debugpy.listen((address, port))
 
         return True
     return False
 
 
-def start_debugpy(end_point: Union[Tuple[str, int], int], wait_for_client: bool) -> bool:
+def start_debugpy(end_point: Union[Tuple[str, int], int], wait_for_client: bool) -> Optional[int]:
     if is_debugpy_installed():
         import debugpy
 
         if isinstance(end_point, int):
             end_point = ("127.0.0.1", end_point)
 
         real_port = find_free_port(end_point[1])
-        if real_port != end_point[1]:
-            _logger.warning(lambda: f"start debugpy session on port {real_port}")
+
         debugpy.listen((end_point[0], real_port))
 
         if wait_for_client:
             _logger.info("wait for debugpy client")
             debugpy.wait_for_client()
-        return True
-    return False
+        return real_port
+    return None
```

### Comparing `robotcode_core-0.43.2/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.44.0/src/robotcode/core/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.44.0/src/robotcode/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/utils/net.py` & `robotcode_core-0.44.0/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.44.0/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/src/robotcode/core/utils/version.py` & `robotcode_core-0.44.0/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/.gitignore` & `robotcode_core-0.44.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/LICENSE.txt` & `robotcode_core-0.44.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/README.md` & `robotcode_core-0.44.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/pyproject.toml` & `robotcode_core-0.44.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.43.2/PKG-INFO` & `robotcode_core-0.44.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-core
-Version: 0.43.2
+Version: 0.44.0
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

