# Comparing `tmp/serverless-sdk-0.5.0.tar.gz` & `tmp/serverless-sdk-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-fyjwcwni/serverless-sdk-0.5.0.tar", last modified: Sat Jun 17 19:45:58 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-56sixmp4/serverless-sdk-0.5.1.tar", last modified: Wed Jun 21 14:58:53 2023, max compression
```

## Comparing `serverless-sdk-0.5.0.tar` & `serverless-sdk-0.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/tag_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/warning_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:58:53.000000 serverless-sdk-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-21 14:58:29.000000 serverless-sdk-0.5.1/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.5.0/PKG-INFO` & `serverless-sdk-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.5.0
+Version: 0.5.1
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.5.0/README.md` & `serverless-sdk-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/pyproject.toml` & `serverless-sdk-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.5.1/serverless_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.5.0
+Version: 0.5.1
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.5.0/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.5.1/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/__init__.py` & `serverless-sdk-0.5.1/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/base.py` & `serverless-sdk-0.5.1/sls_sdk/base.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/exceptions.py` & `serverless-sdk-0.5.1/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.5.1/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/emitter.py` & `serverless-sdk-0.5.1/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/error.py` & `serverless-sdk-0.5.1/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.5.1/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/imports.py` & `serverless-sdk-0.5.1/sls_sdk/lib/imports.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,16 @@
 
 class NativeAIOHTTPInstrumenter(BaseInstrumenter):
     def __init__(self):
         super().__init__("aiohttp")
         self._original_init = None
 
     async def _capture_response_body(self, trace_span, response):
+        # TODO: Turned off temporarily, until we have response body observation fixed
+        return
         # response is a aiohttp.ClientResponse object
         if not self.should_monitor_request_response:
             return
         if (
             response.content_length
             and response.content_length > SDK._maximum_body_byte_length
         ):
@@ -308,14 +310,16 @@
             finally:
                 if trace_span.end_time is None:
                     trace_span.close()
 
         return _func
 
     def _capture_response_body(self, trace_span, response):
+        # TODO: Turned off temporarily, until we have response body observation fixed
+        return
         if not self.should_monitor_request_response:
             return
         if response.length > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
                 "OUTPUT_BODY_TOO_LARGE",
                 trace_span,
@@ -409,14 +413,16 @@
             trace_span.tags["http.error_code"] = ex.__class__.__name__
             raise
         finally:
             if trace_span.end_time is None:
                 trace_span.close()
 
     def _capture_response_body(self, trace_span, response):
+        # TODO: Turned off temporarily, until we have response body observation fixed
+        return
         if not self.should_monitor_request_response:
             return
 
         response_length = int(response.headers.get("Content-Length", 0))
         if response_length > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
```

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/wrapper.py` & `serverless-sdk-0.5.1/sls_sdk/lib/instrumentation/wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/name.py` & `serverless-sdk-0.5.1/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/notice.py` & `serverless-sdk-0.5.1/sls_sdk/lib/notice.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.5.1/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/tags.py` & `serverless-sdk-0.5.1/sls_sdk/lib/tags.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/trace.py` & `serverless-sdk-0.5.1/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/warning.py` & `serverless-sdk-0.5.1/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.5.1/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/tests/test_sdk.py` & `serverless-sdk-0.5.1/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.0/tests/test_thread_safety.py` & `serverless-sdk-0.5.1/tests/test_thread_safety.py`

 * *Files identical despite different names*

