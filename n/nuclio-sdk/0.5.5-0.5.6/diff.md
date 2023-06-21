# Comparing `tmp/nuclio_sdk-0.5.5.tar.gz` & `tmp/nuclio_sdk-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-h4g9w1wc/nuclio_sdk-0.5.5.tar", last modified: Thu Jun  8 09:45:43 2023, max compression
+gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-xd6fod4j/nuclio_sdk-0.5.6.tar", last modified: Wed Jun 21 07:52:57 2023, max compression
```

## Comparing `nuclio_sdk-0.5.5.tar` & `nuclio_sdk-0.5.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/mock_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/nuclio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/mock_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/test_qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/nuclio_sdk/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/nuclio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/nuclio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/nuclio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/nuclio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/nuclio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 07:52:57.000000 nuclio_sdk-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-21 07:52:21.000000 nuclio_sdk-0.5.6/setup.py
```

### Comparing `nuclio_sdk-0.5.5/LICENSE.txt` & `nuclio_sdk-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/PKG-INFO` & `nuclio_sdk-0.5.6/nuclio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nuclio_sdk
-Version: 0.5.5
+Name: nuclio-sdk
+Version: 0.5.6
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.5/Pipfile` & `nuclio_sdk-0.5.6/Pipfile`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/Pipfile.lock` & `nuclio_sdk-0.5.6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/__init__.py` & `nuclio_sdk-0.5.6/nuclio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/context.py` & `nuclio_sdk-0.5.6/nuclio_sdk/context.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/event.py` & `nuclio_sdk-0.5.6/nuclio_sdk/event.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/exceptions.py` & `nuclio_sdk-0.5.6/nuclio_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/helpers.py` & `nuclio_sdk-0.5.6/nuclio_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/json_encoder.py` & `nuclio_sdk-0.5.6/nuclio_sdk/json_encoder.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/logger.py` & `nuclio_sdk-0.5.6/nuclio_sdk/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,34 +54,33 @@
 
 
 class Logger(object):
     def __init__(self, level, name="nuclio_sdk"):
         self._logger = logging.getLogger(name)
         self._logger.setLevel(level)
         self._bound_variables = {}
-        self._handlers = {}
 
     def set_handler(self, handler_name, file, formatter):
 
         # check if there's a handler by this name
-        if handler_name in self._handlers:
-            self._logger.removeHandler(self._handlers[handler_name])
+        for handler in self._logger.handlers:
+            if handler.name == handler_name:
+                self._logger.removeHandler(handler)
+                break
 
         # create a stream handler from the file
         stream_handler = logging.StreamHandler(file)
+        stream_handler.name = handler_name
 
         # set the formatter
         stream_handler.setFormatter(formatter)
 
         # add the handler to the logger
         self._logger.addHandler(stream_handler)
 
-        # save as the named output
-        self._handlers[handler_name] = stream_handler
-
     def debug(self, message, *args):
         self._update_bound_vars_and_log(logging.DEBUG, message, *args)
 
     def info(self, message, *args):
         self._update_bound_vars_and_log(logging.INFO, message, *args)
 
     def warn(self, message, *args):
```

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/platform.py` & `nuclio_sdk-0.5.6/nuclio_sdk/platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/qualified_offset.py` & `nuclio_sdk-0.5.6/nuclio_sdk/qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/response.py` & `nuclio_sdk-0.5.6/nuclio_sdk/response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/test/__init__.py` & `nuclio_sdk-0.5.6/nuclio_sdk/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/test/mock_platform.py` & `nuclio_sdk-0.5.6/nuclio_sdk/test/mock_platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/test/test_case.py` & `nuclio_sdk-0.5.6/nuclio_sdk/test/test_case.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/test/test_event.py` & `nuclio_sdk-0.5.6/nuclio_sdk/test/test_event.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/test/test_logger.py` & `nuclio_sdk-0.5.6/nuclio_sdk/test/test_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -106,7 +106,25 @@
 
         self._logger.debug_with("TestD", some_instance=SomeObject())
         self.assertIn("TestD", self._io.getvalue())
         self.assertIn(
             '"with": {"some_instance": "Unable to serialize object: I am not a string"}',
             self._io.getvalue(),
         )
+
+    def test_redundant_logger_creation(self):
+
+        # create 3 loggers with the same name
+        logger1 = nuclio_sdk.Logger(logging.DEBUG, "test-logger")
+        logger1.set_handler("default", self._io, nuclio_sdk.logger.JSONFormatter())
+        logger2 = nuclio_sdk.Logger(logging.DEBUG, "test-logger")
+        logger2.set_handler("default", self._io, nuclio_sdk.logger.JSONFormatter())
+        logger3 = nuclio_sdk.Logger(logging.DEBUG, "test-logger")
+        logger3.set_handler("default", self._io, nuclio_sdk.logger.JSONFormatter())
+
+        # log from each logger and make sure only one log line is printed
+        logger1.info("1")
+        assert self._io.getvalue().count('"level": "info", "message": "1"') == 1
+        logger2.info("2")
+        assert self._io.getvalue().count('"level": "info", "message": "2"') == 1
+        logger3.info("3")
+        assert self._io.getvalue().count('"level": "info", "message": "3"') == 1
```

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/test/test_qualified_offset.py` & `nuclio_sdk-0.5.6/nuclio_sdk/test/test_qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk/test/test_response.py` & `nuclio_sdk-0.5.6/nuclio_sdk/test/test_response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk.egg-info/PKG-INFO` & `nuclio_sdk-0.5.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nuclio-sdk
-Version: 0.5.5
+Name: nuclio_sdk
+Version: 0.5.6
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.5/nuclio_sdk.egg-info/SOURCES.txt` & `nuclio_sdk-0.5.6/nuclio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.5/setup.py` & `nuclio_sdk-0.5.6/setup.py`

 * *Files identical despite different names*

