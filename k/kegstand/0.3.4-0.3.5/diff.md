# Comparing `tmp/kegstand-0.3.4.tar.gz` & `tmp/kegstand-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstand-0.3.4.tar", max compression
+gzip compressed data, was "kegstand-0.3.5.tar", max compression
```

## Comparing `kegstand-0.3.4.tar` & `kegstand-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.4/LICENSE
--rw-r--r--   0        0        0     1141 2023-06-20 22:24:15.131013 kegstand-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.4/src/kegstand/__init__.py
--rw-r--r--   0        0        0     2928 2023-06-20 22:21:15.544181 kegstand-0.3.4/src/kegstand/api.py
--rw-r--r--   0        0        0     9982 2023-06-20 21:54:06.742326 kegstand-0.3.4/src/kegstand/decorators.py
--rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.4/src/kegstand/utils.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.4/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1141 2023-06-20 23:30:32.094298 kegstand-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.5/src/kegstand/__init__.py
+-rw-r--r--   0        0        0     3139 2023-06-20 23:29:29.942870 kegstand-0.3.5/src/kegstand/api.py
+-rw-r--r--   0        0        0     9982 2023-06-20 21:54:06.742326 kegstand-0.3.5/src/kegstand/decorators.py
+-rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.5/src/kegstand/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.5/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.5/PKG-INFO
```

### Comparing `kegstand-0.3.4/LICENSE` & `kegstand-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.4/pyproject.toml` & `kegstand-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstand"
-version = "0.3.4"
+version = "0.3.5"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand-framework-python"
 homepage = "https://kegstand.dev"
 #readme = "README.md"
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
```

### Comparing `kegstand-0.3.4/src/kegstand/api.py` & `kegstand-0.3.5/src/kegstand/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,20 @@
         self.resources = []
         if root is not None:
             source_path = os.path.dirname(os.path.dirname(os.path.abspath(root)))
             logger.info(f"Adding resources from {root} : source_path={source_path}")
             self.find_and_add_resources(source_path)
 
 
-    def add_resource(self, resource):
+    def add_resource(self, resource, is_public: bool = False):
         # Resource is a ApiResource object
-        self.resources.append(resource)
+        self.resources.append({
+            "resource": resource,
+            "is_public": is_public,
+        })
 
 
     def find_and_add_resources(self, api_source_root: str):
         # Look through folder structure, importing and adding resources to the API.
         # Expects a folder structure like this:
         # api/
         #   [resource_name].py which exposes a resource object named `api`
@@ -33,39 +36,40 @@
         #   [resource_name].py which exposes a resource object named `api`
         resource_module_folders = find_resource_modules(api_source_root)
 
         for resource_module_folder in resource_module_folders:
             # Import the resource module
             resource_module = __import__(resource_module_folder['module_path'], fromlist=resource_module_folder['fromlist'])
             # Get the resource object from the module and add it to the API
-            self.add_resource(getattr(resource_module, 'api'))
+            self.add_resource(getattr(resource_module, 'api'), resource_module_folder['is_public'])
 
         return self.resources
 
 
     def export(self):
         # Export the API as a single Lambda-compatible handler function
         def handler(event, context):
             logger.debug(f"event={event}")
             logger.debug(f"context={context}")
-            method_resource = None
+            resource_is_public = False
             method = None
-            for resource in self.resources:
+            for resource_tuple in self.resources:
+                resource = resource_tuple["resource"]
                 if event["path"].startswith(resource.prefix):
                     method, params = resource.get_matching_route(event["httpMethod"], event["path"])
                     if method is not None:
-                        method_resource = resource
+                        resource_is_public = resource_tuple["is_public"]
                         break
 
             if method is None:
                 logger.error(f"No matching route found for {event['httpMethod']} {event['path']}")
                 return api_response({"error": f"Not found: {event['httpMethod']} {event['path']}"}, 404)
 
             # Check if the resource is public and if not, check that the user is authenticated
-            if not method_resource["is_public"]:
+            if not resource_is_public:
                 # Check that the user is authenticated
                 if "authorizer" not in event["requestContext"]:
                     logger.error("User is not authenticated")
                     return api_response({"error": f"User is not authenticated"}, 401)
 
             # Call the method's handler function
             return method["handler"](params, event, context)
```

### Comparing `kegstand-0.3.4/src/kegstand/decorators.py` & `kegstand-0.3.5/src/kegstand/decorators.py`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.4/src/kegstand/utils.py` & `kegstand-0.3.5/src/kegstand/utils.py`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.4/setup.py` & `kegstand-0.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aws-lambda-powertools[aws-sdk]>=2.10.0,<3.0.0', 'pyjwt>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'kegstand',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
     'long_description': 'None',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
```

### Comparing `kegstand-0.3.4/PKG-INFO` & `kegstand-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstand
-Version: 0.3.4
+Version: 0.3.5
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

