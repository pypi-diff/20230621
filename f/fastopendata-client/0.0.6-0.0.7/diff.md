# Comparing `tmp/fastopendata_client-0.0.6.tar.gz` & `tmp/fastopendata_client-0.0.7.tar.gz`

## Comparing `fastopendata_client-0.0.6.tar` & `fastopendata_client-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastopendata_client-0.0.6/src/fastopendata-client/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastopendata_client-0.0.6/src/fastopendata-client/client.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastopendata_client-0.0.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastopendata_client-0.0.6/LICENSE
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastopendata_client-0.0.6/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastopendata_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fastopendata_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastopendata_client-0.0.7/src/fastopendata_client/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastopendata_client-0.0.7/src/fastopendata_client/client.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastopendata_client-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastopendata_client-0.0.7/LICENSE
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastopendata_client-0.0.7/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastopendata_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fastopendata_client-0.0.7/PKG-INFO
```

### Comparing `fastopendata_client-0.0.6/.gitignore` & `fastopendata_client-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fastopendata_client-0.0.6/LICENSE` & `fastopendata_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastopendata_client-0.0.6/pyproject.toml` & `fastopendata_client-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastopendata_client"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Zachary Ernst", email="zac.ernst@gmail.com" },
 ]
 description = "Client for the FastOpenData API service"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fastopendata_client-0.0.6/PKG-INFO` & `fastopendata_client-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastopendata_client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Client for the FastOpenData API service
 Project-URL: Homepage, https://github.com/zacernst/fastopendata
 Project-URL: Bug Tracker, https://github.com/zacernst/fastopendata/issues
 Author-email: Zachary Ernst <zac.ernst@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

