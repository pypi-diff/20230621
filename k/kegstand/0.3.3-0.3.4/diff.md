# Comparing `tmp/kegstand-0.3.3.tar.gz` & `tmp/kegstand-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstand-0.3.3.tar", max compression
+gzip compressed data, was "kegstand-0.3.4.tar", max compression
```

## Comparing `kegstand-0.3.3.tar` & `kegstand-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.3/LICENSE
--rw-r--r--   0        0        0     1141 2023-06-20 21:56:47.295159 kegstand-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.3/src/kegstand/__init__.py
--rw-r--r--   0        0        0     2831 2023-06-20 21:47:15.563797 kegstand-0.3.3/src/kegstand/api.py
--rw-r--r--   0        0        0     9982 2023-06-20 21:54:06.742326 kegstand-0.3.3/src/kegstand/decorators.py
--rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.3/src/kegstand/utils.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.3/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1141 2023-06-20 22:24:15.131013 kegstand-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.4/src/kegstand/__init__.py
+-rw-r--r--   0        0        0     2928 2023-06-20 22:21:15.544181 kegstand-0.3.4/src/kegstand/api.py
+-rw-r--r--   0        0        0     9982 2023-06-20 21:54:06.742326 kegstand-0.3.4/src/kegstand/decorators.py
+-rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.4/src/kegstand/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.4/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.4/PKG-INFO
```

### Comparing `kegstand-0.3.3/LICENSE` & `kegstand-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.3/pyproject.toml` & `kegstand-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstand"
-version = "0.3.3"
+version = "0.3.4"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand-framework-python"
 homepage = "https://kegstand.dev"
 #readme = "README.md"
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
```

### Comparing `kegstand-0.3.3/src/kegstand/api.py` & `kegstand-0.3.4/src/kegstand/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,27 +43,29 @@
 
 
     def export(self):
         # Export the API as a single Lambda-compatible handler function
         def handler(event, context):
             logger.debug(f"event={event}")
             logger.debug(f"context={context}")
+            method_resource = None
             method = None
             for resource in self.resources:
                 if event["path"].startswith(resource.prefix):
                     method, params = resource.get_matching_route(event["httpMethod"], event["path"])
                     if method is not None:
+                        method_resource = resource
                         break
 
             if method is None:
                 logger.error(f"No matching route found for {event['httpMethod']} {event['path']}")
                 return api_response({"error": f"Not found: {event['httpMethod']} {event['path']}"}, 404)
 
-            # Check if the method is public and if not, check that the user is authenticated
-            if not method["is_public"]:
+            # Check if the resource is public and if not, check that the user is authenticated
+            if not method_resource["is_public"]:
                 # Check that the user is authenticated
                 if "authorizer" not in event["requestContext"]:
                     logger.error("User is not authenticated")
                     return api_response({"error": f"User is not authenticated"}, 401)
 
             # Call the method's handler function
             return method["handler"](params, event, context)
```

### Comparing `kegstand-0.3.3/src/kegstand/decorators.py` & `kegstand-0.3.4/src/kegstand/decorators.py`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.3/src/kegstand/utils.py` & `kegstand-0.3.4/src/kegstand/utils.py`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.3/setup.py` & `kegstand-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aws-lambda-powertools[aws-sdk]>=2.10.0,<3.0.0', 'pyjwt>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'kegstand',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
     'long_description': 'None',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
```

### Comparing `kegstand-0.3.3/PKG-INFO` & `kegstand-0.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstand
-Version: 0.3.3
+Version: 0.3.4
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

