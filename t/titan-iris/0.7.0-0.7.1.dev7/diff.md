# Comparing `tmp/titan-iris-0.7.0.tar.gz` & `tmp/titan-iris-0.7.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.7.0.tar", last modified: Wed Jun 21 08:53:44 2023, max compression
+gzip compressed data, was "titan-iris-0.7.1.dev7.tar", last modified: Wed Jun 21 09:07:39 2023, max compression
```

## Comparing `titan-iris-0.7.0.tar` & `titan-iris-0.7.1.dev7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:44.354278 titan-iris-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-21 08:53:26.000000 titan-iris-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 08:53:26.000000 titan-iris-0.7.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 08:53:26.000000 titan-iris-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-21 08:53:44.354278 titan-iris-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-21 08:53:26.000000 titan-iris-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 08:53:26.000000 titan-iris-0.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 08:53:26.000000 titan-iris-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 08:53:26.000000 titan-iris-0.7.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 08:53:44.354278 titan-iris-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 08:53:26.000000 titan-iris-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:44.346278 titan-iris-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:44.350278 titan-iris-0.7.0/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:44.350278 titan-iris-0.7.0/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:44.350278 titan-iris-0.7.0/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-21 08:53:26.000000 titan-iris-0.7.0/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:44.354278 titan-iris-0.7.0/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-21 08:53:44.000000 titan-iris-0.7.0/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 08:53:44.000000 titan-iris-0.7.0/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:53:44.000000 titan-iris-0.7.0/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 08:53:44.000000 titan-iris-0.7.0/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 08:53:44.000000 titan-iris-0.7.0/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 08:53:44.000000 titan-iris-0.7.0/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:44.354278 titan-iris-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-21 08:53:26.000000 titan-iris-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 08:53:26.000000 titan-iris-0.7.0/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.420360 titan-iris-0.7.1.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.420360 titan-iris-0.7.1.dev7/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.420360 titan-iris-0.7.1.dev7/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/tests/test_sdk.py
```

### Comparing `titan-iris-0.7.0/.gitignore` & `titan-iris-0.7.1.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/Dockerfile` & `titan-iris-0.7.1.dev7/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/PKG-INFO` & `titan-iris-0.7.1.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.7.0
+Version: 0.7.1.dev7
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.7.0/README.md` & `titan-iris-0.7.1.dev7/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/setup.py` & `titan-iris-0.7.1.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/config.yaml` & `titan-iris-0.7.1.dev7/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/gradio/run.py` & `titan-iris-0.7.1.dev7/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/main.py` & `titan-iris-0.7.1.dev7/src/iris/main.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/sdk/auth_utils.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/sdk/conf_manager.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/sdk/exception.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/sdk/iris_sdk.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/sdk/safe_convert.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/iris/sdk/utils.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.7.1.dev7/src/titan_iris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.7.0
+Version: 0.7.1.dev7
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.7.0/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.7.1.dev7/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/tests/test_cli.py` & `titan-iris-0.7.1.dev7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.0/tests/test_sdk.py` & `titan-iris-0.7.1.dev7/tests/test_sdk.py`

 * *Files identical despite different names*

