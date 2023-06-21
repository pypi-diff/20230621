# Comparing `tmp/spatiafi-1.1.5.tar.gz` & `tmp/spatiafi-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatiafi-1.1.5.tar", last modified: Sun Jun 18 01:05:07 2023, max compression
+gzip compressed data, was "spatiafi-1.1.7.tar", last modified: Wed Jun 21 21:51:04 2023, max compression
```

## Comparing `spatiafi-1.1.5.tar` & `spatiafi-1.1.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.298801 spatiafi-1.1.5/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.1.5/.dockerignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.1.5/.gitignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.1.5/.pre-commit-config.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-06-17 16:21:46.000000 spatiafi-1.1.5/.requirements.sha256
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.1.5/Dockerfile
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.1.5/LICENSE
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-18 01:05:07.302801 spatiafi-1.1.5/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-06-17 16:27:30.000000 spatiafi-1.1.5/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-06-12 18:08:33.000000 spatiafi-1.1.5/pyproject.toml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-06-17 16:21:46.000000 spatiafi-1.1.5/requirements-dev.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-06-17 16:20:25.000000 spatiafi-1.1.5/requirements.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.298801 spatiafi-1.1.5/scripts/
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.1.5/scripts/bootstrap_dev.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.1.5/scripts/build_docker.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-06-12 18:08:33.000000 spatiafi-1.1.5/scripts/gen_requirements.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.1.5/scripts/install_package.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.1.5/scripts/test.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-06-17 16:44:05.000000 spatiafi-1.1.5/scripts/upload_pypi.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      935 2023-06-18 01:05:07.302801 spatiafi-1.1.5/setup.cfg
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.1.5/setup.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.294801 spatiafi-1.1.5/src/
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.298801 spatiafi-1.1.5/src/spatiafi/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-06-17 16:27:44.000000 spatiafi-1.1.5/src/spatiafi/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:12:50.000000 spatiafi-1.1.5/src/spatiafi/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-06-18 01:05:07.000000 spatiafi-1.1.5/src/spatiafi/_version.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.1.5/src/spatiafi/auth.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.298801 spatiafi-1.1.5/src/spatiafi/gdal_auth/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       79 2023-06-18 01:03:50.000000 spatiafi-1.1.5/src/spatiafi/gdal_auth/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:27:45.000000 spatiafi-1.1.5/src/spatiafi/gdal_auth/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-06-17 16:27:45.000000 spatiafi-1.1.5/src/spatiafi/gdal_auth/cli.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4730 2023-06-18 01:03:50.000000 spatiafi-1.1.5/src/spatiafi/gdal_auth/gdal_auth.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-06-17 16:27:45.000000 spatiafi-1.1.5/src/spatiafi/session.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.298801 spatiafi-1.1.5/src/spatiafi.egg-info/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-18 01:05:07.000000 spatiafi-1.1.5/src/spatiafi.egg-info/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-06-18 01:05:07.000000 spatiafi-1.1.5/src/spatiafi.egg-info/SOURCES.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-06-18 01:05:07.000000 spatiafi-1.1.5/src/spatiafi.egg-info/dependency_links.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-06-18 01:05:07.000000 spatiafi-1.1.5/src/spatiafi.egg-info/entry_points.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      235 2023-06-18 01:05:07.000000 spatiafi-1.1.5/src/spatiafi.egg-info/requires.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-06-18 01:05:07.000000 spatiafi-1.1.5/src/spatiafi.egg-info/top_level.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.298801 spatiafi-1.1.5/tests/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.1.5/tests/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.1.5/tests/test_dummy.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 01:05:07.298801 spatiafi-1.1.5/workflows/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.1.5/workflows/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.1.5/workflows/delpoy-sensor.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-12 18:08:33.000000 spatiafi-1.1.5/workflows/kustomization.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.1.5/workflows/py-spfi-api-build-wf.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.1.5/workflows/repo-sensor.yaml
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.1.5/workflows/submit-wf.sh
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.1.7/.dockerignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.1.7/.gitignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.1.7/.pre-commit-config.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-06-17 16:21:46.000000 spatiafi-1.1.7/.requirements.sha256
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.1.7/Dockerfile
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.1.7/LICENSE
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-21 21:51:04.464701 spatiafi-1.1.7/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-06-17 16:27:30.000000 spatiafi-1.1.7/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-06-12 18:08:33.000000 spatiafi-1.1.7/pyproject.toml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-06-17 16:21:46.000000 spatiafi-1.1.7/requirements-dev.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-06-17 16:20:25.000000 spatiafi-1.1.7/requirements.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.460701 spatiafi-1.1.7/scripts/
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/bootstrap_dev.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/build_docker.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/gen_requirements.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/install_package.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/test.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-06-21 17:00:42.000000 spatiafi-1.1.7/scripts/upload_pypi.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      935 2023-06-21 21:51:04.464701 spatiafi-1.1.7/setup.cfg
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.1.7/setup.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.460701 spatiafi-1.1.7/src/
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/src/spatiafi/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-06-17 16:27:44.000000 spatiafi-1.1.7/src/spatiafi/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:12:50.000000 spatiafi-1.1.7/src/spatiafi/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi/_version.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.1.7/src/spatiafi/auth.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/src/spatiafi/gdal_auth/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       79 2023-06-18 01:03:50.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:27:45.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-06-17 16:27:45.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/cli.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4742 2023-06-21 21:50:25.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/gdal_auth.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-06-17 16:27:45.000000 spatiafi-1.1.7/src/spatiafi/session.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/src/spatiafi.egg-info/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/entry_points.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      235 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/requires.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/top_level.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/tests/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.1.7/tests/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.1.7/tests/test_dummy.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/workflows/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/delpoy-sensor.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/kustomization.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/py-spfi-api-build-wf.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/repo-sensor.yaml
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/submit-wf.sh
```

### Comparing `spatiafi-1.1.5/.dockerignore` & `spatiafi-1.1.7/.dockerignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/.gitignore` & `spatiafi-1.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/.pre-commit-config.yaml` & `spatiafi-1.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/Dockerfile` & `spatiafi-1.1.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/LICENSE` & `spatiafi-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/PKG-INFO` & `spatiafi-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.5
+Version: 1.1.7
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.5/README.md` & `spatiafi-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/pyproject.toml` & `spatiafi-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/requirements-dev.txt` & `spatiafi-1.1.7/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/requirements.txt` & `spatiafi-1.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/scripts/bootstrap_dev.sh` & `spatiafi-1.1.7/scripts/bootstrap_dev.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/scripts/gen_requirements.sh` & `spatiafi-1.1.7/scripts/gen_requirements.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/setup.cfg` & `spatiafi-1.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/src/spatiafi/auth.py` & `spatiafi-1.1.7/src/spatiafi/auth.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/src/spatiafi/gdal_auth/cli.py` & `spatiafi-1.1.7/src/spatiafi/gdal_auth/cli.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/src/spatiafi/gdal_auth/gdal_auth.py` & `spatiafi-1.1.7/src/spatiafi/gdal_auth/gdal_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 logger = logging.getLogger(__name__)
 
 _GDAL_SCOPES = [
     "https://www.googleapis.com/auth/devstorage.read_write",
     "https://www.googleapis.com/auth/userinfo.email",
     "https://www.googleapis.com/auth/userinfo.profile",
+    "https://www.googleapis.com/auth/accounts.reauth",
     "https://www.googleapis.com/auth/earthengine",
     "openid",
 ]
 
 _on_gcp = None
 
 on_gcp_file = os.path.join(
@@ -79,17 +80,15 @@
     """Get or refresh credentials"""
 
     if os.path.exists(user_credentials_file):
         with open(user_credentials_file, "r") as f:
             info = json.load(f)
 
         quota_project_id = info.get("quota_project_id", None)
-        credentials = UserCredentials.from_authorized_user_info(
-            info=info, scopes=_GDAL_SCOPES
-        )
+        credentials = UserCredentials.from_authorized_user_info(info=info)
 
         if project and project != quota_project_id:
             credentials = credentials.with_quota_project(quota_project_id=project)
         if credentials.expired:
             credentials.refresh(google.auth.transport.requests.Request())
         return credentials, project
```

### Comparing `spatiafi-1.1.5/src/spatiafi/session.py` & `spatiafi-1.1.7/src/spatiafi/session.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/src/spatiafi.egg-info/PKG-INFO` & `spatiafi-1.1.7/src/spatiafi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.5
+Version: 1.1.7
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.5/src/spatiafi.egg-info/SOURCES.txt` & `spatiafi-1.1.7/src/spatiafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/workflows/README.md` & `spatiafi-1.1.7/workflows/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/workflows/delpoy-sensor.sh` & `spatiafi-1.1.7/workflows/delpoy-sensor.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/workflows/repo-sensor.yaml` & `spatiafi-1.1.7/workflows/repo-sensor.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.5/workflows/submit-wf.sh` & `spatiafi-1.1.7/workflows/submit-wf.sh`

 * *Files identical despite different names*

