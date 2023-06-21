# Comparing `tmp/robotcode_jsonrpc2-0.43.2.tar.gz` & `tmp/robotcode_jsonrpc2-0.44.0.tar.gz`

## Comparing `robotcode_jsonrpc2-0.43.2.tar` & `robotcode_jsonrpc2-0.44.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/src/robotcode/jsonrpc2/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/src/robotcode/jsonrpc2/__version__.py
--rw-r--r--   0        0        0    27794 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/src/robotcode/jsonrpc2/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/src/robotcode/jsonrpc2/py.typed
--rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/src/robotcode/jsonrpc2/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/LICENSE.txt
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/pyproject.toml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.43.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/src/robotcode/jsonrpc2/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/src/robotcode/jsonrpc2/__version__.py
+-rw-r--r--   0        0        0    30450 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/src/robotcode/jsonrpc2/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/src/robotcode/jsonrpc2/py.typed
+-rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/src/robotcode/jsonrpc2/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/LICENSE.txt
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/pyproject.toml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.44.0/PKG-INFO
```

### Comparing `robotcode_jsonrpc2-0.43.2/src/robotcode/jsonrpc2/protocol.py` & `robotcode_jsonrpc2-0.44.0/src/robotcode/jsonrpc2/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -620,15 +620,73 @@
                     entry.future.set_exception(e)
                 else:
                     if entry.future.get_loop().is_running():
                         entry.future.get_loop().call_soon_threadsafe(entry.future.set_exception, e)
 
     @__logger.call
     async def handle_error(self, message: JsonRPCError) -> None:
-        raise JsonRPCErrorException(message.error.code, message.error.message, message.error.data)
+        if message.id is None:
+            error = "Invalid response. Response id is null."
+            self.__logger.warning(error)
+            raise JsonRPCErrorException(message.error.code, message.error.message, message.error.data)
+
+        with self._sended_request_lock:
+            entry = self._sended_request.pop(message.id, None)
+
+        if entry is None:
+            error = f"Invalid response. Could not find id '{message.id}' in request list."
+            self.__logger.warning(error)
+            raise JsonRPCErrorException(message.error.code, message.error.message, message.error.data)
+
+        try:
+            if not entry.future.done():
+                res = None
+                if message.result is not None:
+                    res = from_dict(message.result, entry.result_type)
+                if entry.future.get_loop() == asyncio.get_running_loop():
+                    entry.future.set_exception(
+                        JsonRPCErrorException(message.error.code, message.error.message, message.error.data)
+                    )
+                else:
+                    if entry.future.get_loop().is_running():
+
+                        def set_result(f: asyncio.Future[Any], r: Any, ev: threading.Event) -> None:
+                            try:
+                                if not f.done() and f.get_loop().is_running():
+                                    f.set_exception(
+                                        JsonRPCErrorException(
+                                            message.error.code, message.error.message, message.error.data
+                                        )
+                                    )
+                            finally:
+                                ev.set()
+
+                        done = threading.Event()
+
+                        entry.future.get_loop().call_soon_threadsafe(set_result, entry.future, res, done)
+
+                        start = time.monotonic()
+                        while not done.is_set():
+                            if time.monotonic() - start > 120:
+                                raise TimeoutError("Can't set future result.")
+
+                            await asyncio.sleep(0)
+
+                    else:
+                        self.__logger.warning(lambda: f"Response {entry!r} loop is not running.")
+
+        except (SystemExit, KeyboardInterrupt):
+            raise
+        except BaseException as e:
+            if not entry.future.done():
+                if entry.future.get_loop() == asyncio.get_running_loop():
+                    entry.future.set_exception(e)
+                else:
+                    if entry.future.get_loop().is_running():
+                        entry.future.get_loop().call_soon_threadsafe(entry.future.set_exception, e)
 
     @staticmethod
     def _convert_params(
         callable: Callable[..., Any], params_type: Optional[Type[Any]], params: Any
     ) -> Tuple[List[Any], Dict[str, Any]]:
         if params is None:
             return [], {}
```

### Comparing `robotcode_jsonrpc2-0.43.2/src/robotcode/jsonrpc2/server.py` & `robotcode_jsonrpc2-0.44.0/src/robotcode/jsonrpc2/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.43.2/.gitignore` & `robotcode_jsonrpc2-0.44.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.43.2/LICENSE.txt` & `robotcode_jsonrpc2-0.44.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.43.2/README.md` & `robotcode_jsonrpc2-0.44.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.43.2/pyproject.toml` & `robotcode_jsonrpc2-0.44.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotcode-core==0.43.2"]
+dependencies = ["robotcode-core==0.44.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
 Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
```

### Comparing `robotcode_jsonrpc2-0.43.2/PKG-INFO` & `robotcode_jsonrpc2-0.44.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-jsonrpc2
-Version: 0.43.2
+Version: 0.44.0
 Summary: JSONRPC Server for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.43.2
+Requires-Dist: robotcode-core==0.44.0
 Description-Content-Type: text/markdown
 
 # robotcode-jsonrpc2
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
```

