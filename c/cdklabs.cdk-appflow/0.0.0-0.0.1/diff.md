# Comparing `tmp/cdklabs.cdk-appflow-0.0.0.tar.gz` & `tmp/cdklabs.cdk-appflow-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-appflow-0.0.0.tar", last modified: Tue Jun 20 10:52:26 2023, max compression
+gzip compressed data, was "cdklabs.cdk-appflow-0.0.1.tar", last modified: Wed Jun 21 00:29:09 2023, max compression
```

## Comparing `cdklabs.cdk-appflow-0.0.0.tar` & `cdklabs.cdk-appflow-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:52:26.716743 cdklabs.cdk-appflow-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-20 10:52:26.716743 cdklabs.cdk-appflow-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:52:26.716743 cdklabs.cdk-appflow-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:52:26.712743 cdklabs.cdk-appflow-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:52:26.712743 cdklabs.cdk-appflow-0.0.0/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:52:26.716743 cdklabs.cdk-appflow-0.0.0/src/cdklabs/cdk_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs/cdk_appflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:52:26.716743 cdklabs.cdk-appflow-0.0.0/src/cdklabs/cdk_appflow/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs/cdk_appflow/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:52:12.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs/cdk_appflow/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:52:26.716743 cdklabs.cdk-appflow-0.0.0/src/cdklabs.cdk_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-20 10:52:26.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 10:52:26.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:52:26.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 10:52:26.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs.cdk_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 10:52:26.000000 cdklabs.cdk-appflow-0.0.0/src/cdklabs.cdk_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-appflow-0.0.0/LICENSE` & `cdklabs.cdk-appflow-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.0/PKG-INFO` & `cdklabs.cdk-appflow-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.0
+Version: 0.0.1
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-appflow-0.0.0/setup.py` & `cdklabs.cdk-appflow-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-appflow",
-    "version": "0.0.0",
+    "version": "0.0.1",
     "description": "@cdklabs/cdk-appflow",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-appflow.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_appflow",
         "cdklabs.cdk_appflow._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_appflow._jsii": [
-            "cdk-appflow@0.0.0.jsii.tgz"
+            "cdk-appflow@0.0.1.jsii.tgz"
         ],
         "cdklabs.cdk_appflow": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdklabs.cdk-appflow-0.0.0/src/cdklabs/cdk_appflow/__init__.py` & `cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.0/src/cdklabs.cdk_appflow.egg-info/PKG-INFO` & `cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.0
+Version: 0.0.1
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

