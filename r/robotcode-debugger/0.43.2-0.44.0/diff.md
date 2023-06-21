# Comparing `tmp/robotcode_debugger-0.43.2.tar.gz` & `tmp/robotcode_debugger-0.44.0.tar.gz`

## Comparing `robotcode_debugger-0.43.2.tar` & `robotcode_debugger-0.44.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    49522 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/README.md
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.43.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    49549 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/README.md
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.44.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/debugger.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,15 +844,15 @@
             return
 
         if self.debug and entry.source and entry.line is not None:
             self.process_start_state(entry.source, entry.line, entry.type, status)
 
             self.wait_for_running()
 
-    CAUGHTED_KEYWORDS: ClassVar = [
+    CAUGHTED_KEYWORDS: ClassVar[List[str]] = [
         "BuiltIn.Run Keyword And Expect Error",
         "BuiltIn.Run Keyword And Ignore Error",
         "BuiltIn.Run Keyword And Warn On Failure",
         "BuiltIn.Wait Until Keyword Succeeds",
         "BuiltIn.Run Keyword And Continue On Failure",
     ]
 
@@ -980,15 +980,15 @@
                         module_id=v.libname,
                     )
 
         frames = list(yield_stack())
 
         return StackTraceResult(frames, len(self.stack_frames))
 
-    MESSAGE_COLORS: ClassVar = {
+    MESSAGE_COLORS: ClassVar[Dict[str, str]] = {
         "INFO": "\u001b[38;5;2m",
         "WARN": "\u001b[38;5;3m",
         "ERROR": "\u001b[38;5;1m",
         "TRACE": "\u001b[38;5;4m",
         "FAIL": "\u001b[38;5;5m\u001b[1m",
         "DEBUG": "\u001b[38;5;8m",
     }
```

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/run.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/server.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.44.0/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/.gitignore` & `robotcode_debugger-0.44.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/LICENSE.txt` & `robotcode_debugger-0.44.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/README.md` & `robotcode_debugger-0.44.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.43.2/pyproject.toml` & `robotcode_debugger-0.44.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.43.2",
-  "robotcode-runner==0.43.2",
+  "robotcode-jsonrpc2==0.44.0",
+  "robotcode-runner==0.44.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.43.2/PKG-INFO` & `robotcode_debugger-0.44.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.43.2
+Version: 0.44.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.43.2
-Requires-Dist: robotcode-runner==0.43.2
+Requires-Dist: robotcode-jsonrpc2==0.44.0
+Requires-Dist: robotcode-runner==0.44.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

