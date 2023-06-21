# Comparing `tmp/arcane-flask-1.9.0.tar.gz` & `tmp/arcane-flask-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane-flask-1.9.0.tar", max compression
+gzip compressed data, was "arcane-flask-1.9.1.tar", max compression
```

## Comparing `arcane-flask-1.9.0.tar` & `arcane-flask-1.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      368 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/README.md
--rw-r--r--   0        0        0      182 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/__init__.py
--rw-r--r--   0        0        0    11093 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/authentication.py
--rw-r--r--   0        0        0     2931 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/exception_decorator.py
--rw-r--r--   0        0        0     1638 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/http_response.py
--rw-r--r--   0        0        0      296 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/log.py
--rw-r--r--   0        0        0      775 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/services.py
--rw-r--r--   0        0        0     1576 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/tracking.py
--rw-r--r--   0        0        0      205 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/arcane/flask/types.py
--rw-r--r--   0        0        0      558 2022-03-03 14:18:50.520124 arcane-flask-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1232 2022-03-03 14:19:04.339854 arcane-flask-1.9.0/setup.py
--rw-r--r--   0        0        0     1236 2022-03-03 14:19:04.340153 arcane-flask-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      368 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/README.md
+-rw-r--r--   0        0        0      182 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/__init__.py
+-rw-r--r--   0        0        0    10583 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/authentication.py
+-rw-r--r--   0        0        0     2931 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/exception_decorator.py
+-rw-r--r--   0        0        0     1638 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/http_response.py
+-rw-r--r--   0        0        0      296 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/log.py
+-rw-r--r--   0        0        0      775 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/services.py
+-rw-r--r--   0        0        0     1576 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/tracking.py
+-rw-r--r--   0        0        0      205 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/arcane/flask/types.py
+-rw-r--r--   0        0        0      558 2022-03-03 14:59:58.772760 arcane-flask-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1232 2022-03-03 15:00:12.001809 arcane-flask-1.9.1/setup.py
+-rw-r--r--   0        0        0     1236 2022-03-03 15:00:12.002130 arcane-flask-1.9.1/PKG-INFO
```

### Comparing `arcane-flask-1.9.0/arcane/flask/authentication.py` & `arcane-flask-1.9.1/arcane/flask/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,28 +32,26 @@
     pass
 
 def check_access_rights(service: str,
                         required_rights: int,
                         service_user_right: str,  # should be something like ValueOf[UserRightsEnum]
                         datastore_client: DatastoreClient,
                         pubsub_client: PubSubClient,
-                        args_name_and_path_to_get: Dict[str, str] = {},
                         kwargs_name_and_path_to_get: Dict[str, str] = {},
                         receive_rights_per_client: bool=False,
                         auth_enabled: bool=True,
                         project: str = None
                         ) -> Callable[[Callable], Callable]:
     """
     This functions checks the authorizations from the current HTTP call.
     /!\ Must be the last decorator (right above the decorated function) when there are multiples decorators on
     a function in order to get job_func_signature.
     if receive_rights_per_client is set to True, function must accept an argument corresponding to CLIENTS_PARAM either
     as the last positional argument or as an named argument.
-    :param args_name_and_path_to_get: A dictionnary where the key is the name of the key we want to store the arg as and the value is the path to the value in the args ('[0].test.value'). The path must begin with an index value, like the example.
-    :param kwargs_name_and_path_to_get: A dictionnary where the key is the name of the key we want to store the kwarg as and the value is the path to the value in the args ('test.value'). Unlike args, the path must not begin with an index value, like the example.
+    :param kwargs_name_and_path_to_get: A dictionnary where the key is the name of the key we want to store the kwarg as and the value is the path to the value in the args ('test.value').
     """
     if required_rights == RightsLevelEnum.NONE and not receive_rights_per_client:
         def dummy_check_rights(job_func: Callable) -> Callable:
             return job_func
         return dummy_check_rights
 
     def check_rights(job_func: Callable) -> Callable:
@@ -137,19 +135,17 @@
                     authorized_clients = [client_entity.key.name for client_entity in clients_query.fetch()]
 
                 kwargs[CLIENTS_PARAM] = sorted(set(authorized_clients))
             executable = job_func(*args, **kwargs)
             end = time.time()
 
             additionnal_info = {}
-            for key, path in args_name_and_path_to_get.items():
-                additionnal_info[key] = get(args, path)
             for key, path in kwargs_name_and_path_to_get.items():
                 additionnal_info[key] = get(kwargs, path)
-            if len(additionnal_info.keys()):
+            if len(additionnal_info.keys()) == 0:
                 additionnal_info = None
 
             if auth_enabled:
                 try:
                     send_tracking_information(
                         email=claims['email'],
                         service=service,
```

### Comparing `arcane-flask-1.9.0/arcane/flask/exception_decorator.py` & `arcane-flask-1.9.1/arcane/flask/exception_decorator.py`

 * *Files identical despite different names*

### Comparing `arcane-flask-1.9.0/arcane/flask/http_response.py` & `arcane-flask-1.9.1/arcane/flask/http_response.py`

 * *Files identical despite different names*

### Comparing `arcane-flask-1.9.0/arcane/flask/services.py` & `arcane-flask-1.9.1/arcane/flask/services.py`

 * *Files identical despite different names*

### Comparing `arcane-flask-1.9.0/arcane/flask/tracking.py` & `arcane-flask-1.9.1/arcane/flask/tracking.py`

 * *Files identical despite different names*

### Comparing `arcane-flask-1.9.0/pyproject.toml` & `arcane-flask-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "arcane-flask"
 
-version = "1.9.0"
+version = "1.9.1"
 
 
 description = "Utility functions for flask apps."
 readme = "README.md"
 authors = ["Arcane <product@arcane.run>"]
 packages = [
     { include = "arcane" }
```

### Comparing `arcane-flask-1.9.0/setup.py` & `arcane-flask-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'firebase_admin==4.1.0',
  'flask>=1.1.4,<2.0.0',
  'flask_log_request_id>=0.10.1,<0.11.0',
  'pydash>=5.1.0,<6.0.0']
 
 setup_kwargs = {
     'name': 'arcane-flask',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'Utility functions for flask apps.',
     'long_description': "# Arcane flask\n\nThis package help us authenticate users\n\n## Get Started\n\n```sh\npip install arcane-flask\n```\n\n## Example Usage\n\n```python\nfrom arcane import flask\n\n@check_access_rights(service='function', required_rights='Viewer',\n                     receive_rights_per_client=True, project=Config.Project, adscale_key=Config.Key)\ndef function(params):\n    pass\n\n```\n\n",
     'author': 'Arcane',
     'author_email': 'product@arcane.run',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `arcane-flask-1.9.0/PKG-INFO` & `arcane-flask-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcane-flask
-Version: 1.9.0
+Version: 1.9.1
 Summary: Utility functions for flask apps.
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
```

