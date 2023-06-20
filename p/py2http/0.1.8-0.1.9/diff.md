# Comparing `tmp/py2http-0.1.8.tar.gz` & `tmp/py2http-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py2http-0.1.8.tar", last modified: Fri Oct 30 02:18:35 2020, max compression
+gzip compressed data, was "dist/py2http-0.1.9.tar", last modified: Sat Nov  7 21:22:43 2020, max compression
```

## Comparing `py2http-0.1.8.tar` & `py2http-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-10-30 02:18:35.424224 py2http-0.1.8/
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      234 2020-10-30 02:18:35.424389 py2http-0.1.8/PKG-INFO
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     5117 2020-08-14 19:53:05.000000 py2http-0.1.8/README.md
-drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-10-30 02:18:35.404698 py2http-0.1.8/py2http/
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      384 2020-10-01 18:47:47.000000 py2http-0.1.8/py2http/__init__.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2603 2020-10-30 02:17:06.000000 py2http-0.1.8/py2http/bottle_plugins.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2645 2020-09-22 20:42:47.000000 py2http-0.1.8/py2http/config.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)    36704 2020-10-01 20:39:26.000000 py2http-0.1.8/py2http/decorators.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2836 2020-10-07 01:11:56.000000 py2http-0.1.8/py2http/default_configs.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      109 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/diagnosis.py
-drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-10-30 02:18:35.415189 py2http-0.1.8/py2http/examples/
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/examples/__init__.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/examples/custom_input_mapper.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)       39 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/examples/custom_input_mappers.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      484 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/examples/example_service.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      850 2020-08-24 19:36:29.000000 py2http-0.1.8/py2http/examples/example_service_bottle.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      707 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/examples/example_service_flask.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     1340 2020-10-30 02:17:06.000000 py2http-0.1.8/py2http/middleware.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     9266 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/openapi_utils.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     1226 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/route_utils.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     9339 2020-09-22 20:42:47.000000 py2http-0.1.8/py2http/schema_tools.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)    15187 2020-10-21 19:57:13.000000 py2http-0.1.8/py2http/service.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)       28 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/signatures.py
-drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-10-30 02:18:35.423608 py2http-0.1.8/py2http/tests/
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/tests/__init__.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      996 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/tests/example_service_test.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     1492 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/tests/objects_for_testing.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2641 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/tests/simple_run_process_test.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2400 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/tests/test_decorators.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/tests/test_flask.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     4312 2020-09-22 20:42:47.000000 py2http-0.1.8/py2http/tests/test_p2h2p.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      827 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/tests/utils_for_testing.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      603 2020-08-14 19:53:05.000000 py2http-0.1.8/py2http/types.py
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)    18988 2020-09-22 20:42:47.000000 py2http-0.1.8/py2http/util.py
-drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-10-30 02:18:35.408469 py2http-0.1.8/py2http.egg-info/
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      234 2020-10-30 02:18:34.000000 py2http-0.1.8/py2http.egg-info/PKG-INFO
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      951 2020-10-30 02:18:35.000000 py2http-0.1.8/py2http.egg-info/SOURCES.txt
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)        1 2020-10-30 02:18:34.000000 py2http-0.1.8/py2http.egg-info/dependency_links.txt
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)        8 2020-10-30 02:18:34.000000 py2http-0.1.8/py2http.egg-info/top_level.txt
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)      306 2020-10-30 02:18:35.425022 py2http-0.1.8/setup.cfg
--rw-r--r--   0 Steve.Herzog   (502) staff       (20)     3235 2020-10-30 02:18:03.000000 py2http-0.1.8/setup.py
+drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-11-07 21:22:43.775609 py2http-0.1.9/
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      234 2020-11-07 21:22:43.775941 py2http-0.1.9/PKG-INFO
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     5117 2020-08-14 19:53:05.000000 py2http-0.1.9/README.md
+drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-11-07 21:22:43.737497 py2http-0.1.9/py2http/
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      384 2020-10-01 18:47:47.000000 py2http-0.1.9/py2http/__init__.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2603 2020-10-30 02:17:06.000000 py2http-0.1.9/py2http/bottle_plugins.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2645 2020-09-22 20:42:47.000000 py2http-0.1.9/py2http/config.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)    36704 2020-10-01 20:39:26.000000 py2http-0.1.9/py2http/decorators.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2843 2020-11-05 06:50:22.000000 py2http-0.1.9/py2http/default_configs.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      109 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/diagnosis.py
+drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-11-07 21:22:43.753925 py2http-0.1.9/py2http/examples/
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/examples/__init__.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/examples/custom_input_mapper.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)       39 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/examples/custom_input_mappers.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      484 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/examples/example_service.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      850 2020-08-24 19:36:29.000000 py2http-0.1.9/py2http/examples/example_service_bottle.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      707 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/examples/example_service_flask.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     1340 2020-10-30 02:17:06.000000 py2http-0.1.9/py2http/middleware.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     9266 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/openapi_utils.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     1226 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/route_utils.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     9339 2020-09-22 20:42:47.000000 py2http-0.1.9/py2http/schema_tools.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)    15187 2020-10-21 19:57:13.000000 py2http-0.1.9/py2http/service.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)       28 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/signatures.py
+drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-11-07 21:22:43.774312 py2http-0.1.9/py2http/tests/
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/tests/__init__.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      996 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/tests/example_service_test.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     1492 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/tests/objects_for_testing.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2641 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/tests/simple_run_process_test.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     2400 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/tests/test_decorators.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)        0 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/tests/test_flask.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     4312 2020-09-22 20:42:47.000000 py2http-0.1.9/py2http/tests/test_p2h2p.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      827 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/tests/utils_for_testing.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      603 2020-08-14 19:53:05.000000 py2http-0.1.9/py2http/types.py
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)    18988 2020-09-22 20:42:47.000000 py2http-0.1.9/py2http/util.py
+drwxr-xr-x   0 Steve.Herzog   (502) staff       (20)        0 2020-11-07 21:22:43.742085 py2http-0.1.9/py2http.egg-info/
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      234 2020-11-07 21:22:43.000000 py2http-0.1.9/py2http.egg-info/PKG-INFO
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      951 2020-11-07 21:22:43.000000 py2http-0.1.9/py2http.egg-info/SOURCES.txt
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)        1 2020-11-07 21:22:43.000000 py2http-0.1.9/py2http.egg-info/dependency_links.txt
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)        8 2020-11-07 21:22:43.000000 py2http-0.1.9/py2http.egg-info/top_level.txt
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)      306 2020-11-07 21:22:43.776913 py2http-0.1.9/setup.cfg
+-rw-r--r--   0 Steve.Herzog   (502) staff       (20)     3235 2020-11-07 21:22:03.000000 py2http-0.1.9/setup.py
```

### Comparing `py2http-0.1.8/README.md` & `py2http-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/bottle_plugins.py` & `py2http-0.1.9/py2http/bottle_plugins.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/config.py` & `py2http-0.1.9/py2http/config.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/decorators.py` & `py2http-0.1.9/py2http/decorators.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/default_configs.py` & `py2http-0.1.9/py2http/default_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from aiohttp import web
 from bottle import response
 import json
 import os
+import traceback
 
 from i2.errors import AuthorizationError, ForbiddenError, InputError, NotFoundError, DuplicateRecordError
 
 from py2http.decorators import handle_json_req, send_json_resp, JsonRespEncoder
 from py2http.config import AIOHTTP, BOTTLE, FLASK
 
 
@@ -34,28 +35,28 @@
         content_type="application/json",
         reason=reason
     )
 
 
 def aiohttp_error_handler(error: Exception):
     message = str(error)
+    traceback.print_exc()
     if isinstance(error, (AuthorizationError, InputError, DuplicateRecordError)):
         _raise_http_client_error(web.HTTPBadRequest, message, reason=type(error).__name__)
     elif isinstance(error, ForbiddenError):
         _raise_http_client_error(web.HTTPForbidden, message)
     elif isinstance(error, NotFoundError):
         _raise_http_client_error(web.HTTPNotFound, message)
     else:
         _raise_http_client_error(web.HTTPInternalServerError, message)
 
 
 def bottle_error_handler(error: Exception):
     message = str(error)
-    print(f'Error: {error}')
-    print(f'Message: {message}')
+    traceback.print_exc()
     if isinstance(error, (AuthorizationError, InputError, DuplicateRecordError)):
         response.status = f'400 {type(error).__name__}'
         # response.reason = type(error).__name__
     elif isinstance(error, ForbiddenError):
         response.status = 403
     elif isinstance(error, NotFoundError):
         response.status = 404
```

### Comparing `py2http-0.1.8/py2http/examples/example_service_bottle.py` & `py2http-0.1.9/py2http/examples/example_service_bottle.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/examples/example_service_flask.py` & `py2http-0.1.9/py2http/examples/example_service_flask.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/middleware.py` & `py2http-0.1.9/py2http/middleware.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/openapi_utils.py` & `py2http-0.1.9/py2http/openapi_utils.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/route_utils.py` & `py2http-0.1.9/py2http/route_utils.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/schema_tools.py` & `py2http-0.1.9/py2http/schema_tools.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/service.py` & `py2http-0.1.9/py2http/service.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/tests/example_service_test.py` & `py2http-0.1.9/py2http/tests/example_service_test.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/tests/objects_for_testing.py` & `py2http-0.1.9/py2http/tests/objects_for_testing.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/tests/simple_run_process_test.py` & `py2http-0.1.9/py2http/tests/simple_run_process_test.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/tests/test_decorators.py` & `py2http-0.1.9/py2http/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/tests/test_p2h2p.py` & `py2http-0.1.9/py2http/tests/test_p2h2p.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/tests/utils_for_testing.py` & `py2http-0.1.9/py2http/tests/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/types.py` & `py2http-0.1.9/py2http/types.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http/util.py` & `py2http-0.1.9/py2http/util.py`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/py2http.egg-info/SOURCES.txt` & `py2http-0.1.9/py2http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2http-0.1.8/setup.py` & `py2http-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import os
 # from configparser import ConfigParser
 from setuptools import find_packages, setup
 # from pack import read_configs
 
 # uncomment this for manual build
 setup_configs = dict(
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     include_package_data=True,
     platforms='any'
 )
 setup(**setup_configs)
```

