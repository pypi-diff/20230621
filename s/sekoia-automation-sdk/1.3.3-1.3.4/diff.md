# Comparing `tmp/sekoia_automation_sdk-1.3.3.tar.gz` & `tmp/sekoia_automation_sdk-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.3.3.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.3.4.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.3.3.tar` & `sekoia_automation_sdk-1.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/LICENSE
--rw-r--r--   0        0        0     8422 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/README.md
--rw-r--r--   0        0        0     2114 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11420 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/action.py
--rw-r--r--   0        0        0     5193 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/config.py
--rw-r--r--   0        0        0     6955 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15640 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-06-13 07:52:32.615261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      596 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10011 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/openapi.py
--rwxr-xr-x   0        0        0    13722 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/sync_library.py
--rw-r--r--   0        0        0     6094 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/storage.py
--rw-r--r--   0        0        0    14267 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-06-13 07:52:32.619261 sekoia_automation_sdk-1.3.3/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/LICENSE
+-rw-r--r--   0        0        0     8422 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/README.md
+-rw-r--r--   0        0        0     2114 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11420 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/action.py
+-rw-r--r--   0        0        0     5193 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6955 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      596 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    13709 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     6094 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    14267 2023-06-21 10:42:11.176765 sekoia_automation_sdk-1.3.4/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-06-21 10:42:11.176765 sekoia_automation_sdk-1.3.4/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.4/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.3.3/LICENSE` & `sekoia_automation_sdk-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/README.md` & `sekoia_automation_sdk-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/pyproject.toml` & `sekoia_automation_sdk-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.3.3"
+version = "1.3.4"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/action.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/cli.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/config.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/module.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/scripts/sync_library.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/sync_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
             image_name = docker_image
 
         token = base64.b64encode(self.registry_pat.encode()).decode()
         response = requests.get(
             f"https://{registry}/v2/{namespace}/{image_name}/manifests/{version}",
             headers={
                 "Authorization": f"Bearer {token}",
-                "Accept": "application/vnd.docker.distribution.manifest.v2+json",
+                "Accept": "application/vnd.oci.image.index.v1+json",
             },
         )
 
         return response.status_code == 200
 
     def load_module(self, module_path: Path):
         """Sync a module and its components (triggers, actions) using Playbook API
```

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/trigger.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.3.4/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.3/PKG-INFO` & `sekoia_automation_sdk-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

