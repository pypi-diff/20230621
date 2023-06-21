# Comparing `tmp/roboflow-1.0.9.tar.gz` & `tmp/roboflow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.0.9.tar", last modified: Wed May 17 15:30:07 2023, max compression
+gzip compressed data, was "roboflow-1.1.0.tar", last modified: Wed Jun 21 16:51:26 2023, max compression
```

## Comparing `roboflow-1.0.9.tar` & `roboflow-1.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-17 15:29:32.000000 roboflow-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-17 15:30:07.218940 roboflow-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-17 15:29:32.000000 roboflow-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 15:29:32.000000 roboflow-1.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/archive/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-17 15:30:07.000000 roboflow-1.0.9/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:30:07.218940 roboflow-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-17 15:29:32.000000 roboflow-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-06-21 16:50:54.000000 roboflow-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-06-21 16:51:26.742029 roboflow-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-21 16:50:54.000000 roboflow-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 16:50:54.000000 roboflow-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.726028 roboflow-1.1.0/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.730028 roboflow-1.1.0/roboflow/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/archive/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23093 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/models/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-21 16:50:54.000000 roboflow-1.1.0/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.730028 roboflow-1.1.0/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 16:51:26.000000 roboflow-1.1.0/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:51:26.742029 roboflow-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-21 16:50:54.000000 roboflow-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.738029 roboflow-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:51:26.742029 roboflow-1.1.0/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 16:50:54.000000 roboflow-1.1.0/tests/util/test_versions.py
```

### Comparing `roboflow-1.0.9/LICENSE` & `roboflow-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/PKG-INFO` & `roboflow-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.9
+Version: 1.1.0
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.9 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.1.0 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.9/README.md` & `roboflow-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/__init__.py` & `roboflow-1.1.0/roboflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.util.general import write_line
 
-__version__ = "1.0.9"
+__version__ = "1.1.0"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
```

### Comparing `roboflow-1.0.9/roboflow/archive/plot.py` & `roboflow-1.1.0/roboflow/archive/plot.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/config.py` & `roboflow-1.1.0/roboflow/config.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/core/project.py` & `roboflow-1.1.0/roboflow/core/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         # stop on empty string
         if len(annotation_path) == 0:
             print("Please provide a non-empty string for annotation_path.")
             return {"result": "Please provide a non-empty string for annotation_path."}
 
         # check if annotation file exists
         elif os.path.exists(annotation_path):
-            print("-> found given annotation file")
+            # print("-> found given annotation file")
             annotation_string = open(annotation_path, "r").read()
 
         # if not annotation file, check if user wants to upload regular as classification annotation
         elif self.type == "classification":
             print(f"-> using {annotation_path} as classname for classification project")
             annotation_string = annotation_path
```

### Comparing `roboflow-1.0.9/roboflow/core/version.py` & `roboflow-1.1.0/roboflow/core/version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/core/workspace.py` & `roboflow-1.1.0/roboflow/core/workspace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+import concurrent.futures
 import glob
 import json
 import os
+import random
+import re
 import sys
 
 import requests
+import supervision as sv
 from numpy import ndarray
 from PIL import Image
+from tqdm import tqdm
 
 from roboflow.config import API_URL, CLIP_FEATURIZE_URL, DEMO_KEYS
 from roboflow.core.project import Project
 from roboflow.util.active_learning_utils import (
     check_box_size,
     clip_encode,
     count_comparisons,
 )
 from roboflow.util.clip_compare_utils import clip_encode
+from roboflow.util.general import write_line
 from roboflow.util.two_stage_utils import ocr_infer
 
 
 class Workspace:
     def __init__(self, info, api_key, default_workspace, model_format):
         if api_key in DEMO_KEYS:
             self.__api_key = api_key
@@ -238,14 +244,87 @@
         else:
             print(
                 "please use an object detection model--can only perform two stage with bounding box results"
             )
 
         return results
 
+    def upload_dataset(
+        self,
+        dataset_path,
+        project_name,
+        num_workers=10,
+        dataset_format="yolov8",
+        project_license="MIT",
+        project_type="object-detection",
+    ):
+        if project_type != "object-detection":
+            raise ("upload_dataset only supported for object-detection projects")
+
+        if dataset_format not in ["voc", "yolov8", "yolov5"]:
+            raise (
+                "dataset_format not supported - please use voc, yolov8, yolov5. PS, you can always convert your dataset in the Roboflow UI"
+            )
+
+        # check type stuff and convert
+        if dataset_format == "yolov8" or dataset_format == "yolov5":
+            # convert to voc
+            for split in ["train", "valid", "test"]:
+                dataset = sv.DetectionDataset.from_yolo(
+                    images_directory_path=dataset_path + "/" + split + "/images",
+                    annotations_directory_path=dataset_path + "/" + split + "/labels",
+                    data_yaml_path=dataset_path + "/data.yaml",
+                )
+
+                dataset.as_pascal_voc(
+                    images_directory_path=dataset_path + "_voc" + "/" + split,
+                    annotations_directory_path=dataset_path + "_voc" + "/" + split,
+                )
+
+            dataset_path = dataset_path + "_voc"
+
+        if project_name in self.project_list:
+            dataset_upload_project = self.project(project_name)
+        else:
+            dataset_upload_project = self.create_project(
+                project_name,
+                project_license=project_license,
+                annotation=project_name,
+                project_type=project_type,
+            )
+
+        def upload_file(img_file, split):
+            label_file = img_file.replace(".jpg", ".xml")
+            dataset_upload_project.upload(
+                image_path=img_file, annotation_path=label_file, split=split
+            )
+
+        def parallel_upload(file_list, split):
+            with concurrent.futures.ThreadPoolExecutor(
+                max_workers=num_workers
+            ) as executor:
+                list(
+                    tqdm(
+                        executor.map(upload_file, file_list, [split] * len(file_list)),
+                        total=len(file_list),
+                    )
+                )
+
+        write_line("uploading training set...")
+        file_list = glob.glob(dataset_path + "/train/*.jpg")
+        parallel_upload(file_list, "train")
+
+        write_line("uploading validation set...")
+        file_list = glob.glob(dataset_path + "/valid/*.jpg")
+        parallel_upload(file_list, "valid")
+
+        write_line("uploading test set...")
+        file_list = glob.glob(dataset_path + "/test/*.jpg")
+        parallel_upload(file_list, "test")
+
     def active_learning(
         self,
         raw_data_location: str = "",
         raw_data_extension: str = "",
         inference_endpoint: list = [],
         upload_destination: str = "",
         conditionals: dict = {},
```

### Comparing `roboflow-1.0.9/roboflow/models/classification.py` & `roboflow-1.1.0/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/models/inference.py` & `roboflow-1.1.0/roboflow/models/inference.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/models/instance_segmentation.py` & `roboflow-1.1.0/roboflow/models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/models/object_detection.py` & `roboflow-1.1.0/roboflow/models/object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/models/semantic_segmentation.py` & `roboflow-1.1.0/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/util/active_learning_utils.py` & `roboflow-1.1.0/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/util/clip_compare_utils.py` & `roboflow-1.1.0/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/util/image_utils.py` & `roboflow-1.1.0/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/util/prediction.py` & `roboflow-1.1.0/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/util/two_stage_utils.py` & `roboflow-1.1.0/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow/util/versions.py` & `roboflow-1.1.0/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/roboflow.egg-info/PKG-INFO` & `roboflow-1.1.0/roboflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.9
+Version: 1.1.0
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.9 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.1.0 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.9/roboflow.egg-info/SOURCES.txt` & `roboflow-1.1.0/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/setup.py` & `roboflow-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/models/test_instance_segmentation.py` & `roboflow-1.1.0/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/models/test_object_detection.py` & `roboflow-1.1.0/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/models/test_semantic_segmentation.py` & `roboflow-1.1.0/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/test_project.py` & `roboflow-1.1.0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/test_queries.py` & `roboflow-1.1.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/test_version.py` & `roboflow-1.1.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/util/test_image_utils.py` & `roboflow-1.1.0/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.9/tests/util/test_versions.py` & `roboflow-1.1.0/tests/util/test_versions.py`

 * *Files identical despite different names*

