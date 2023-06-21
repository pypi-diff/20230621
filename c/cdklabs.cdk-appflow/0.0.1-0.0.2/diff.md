# Comparing `tmp/cdklabs.cdk-appflow-0.0.1.tar.gz` & `tmp/cdklabs.cdk-appflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-appflow-0.0.1.tar", last modified: Wed Jun 21 00:29:09 2023, max compression
+gzip compressed data, was "cdklabs.cdk-appflow-0.0.2.tar", last modified: Wed Jun 21 14:21:46 2023, max compression
```

## Comparing `cdklabs.cdk-appflow-0.0.1.tar` & `cdklabs.cdk-appflow-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:28:57.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs/cdk_appflow/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:29:09.155612 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 00:29:09.000000 cdklabs.cdk-appflow-0.0.1/src/cdklabs.cdk_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:46.076801 cdklabs.cdk-appflow-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-21 14:21:46.076801 cdklabs.cdk-appflow-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:21:46.076801 cdklabs.cdk-appflow-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:46.072801 cdklabs.cdk-appflow-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:46.072801 cdklabs.cdk-appflow-0.0.2/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:46.072801 cdklabs.cdk-appflow-0.0.2/src/cdklabs/cdk_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   463711 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs/cdk_appflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:46.072801 cdklabs.cdk-appflow-0.0.2/src/cdklabs/cdk_appflow/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs/cdk_appflow/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173447 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:34.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs/cdk_appflow/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:46.072801 cdklabs.cdk-appflow-0.0.2/src/cdklabs.cdk_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-21 14:21:46.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-21 14:21:46.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:46.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 14:21:46.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs.cdk_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 14:21:46.000000 cdklabs.cdk-appflow-0.0.2/src/cdklabs.cdk_appflow.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-appflow-0.0.1/LICENSE` & `cdklabs.cdk-appflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.1/setup.py` & `cdklabs.cdk-appflow-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-appflow",
-    "version": "0.0.1",
+    "version": "0.0.2",
     "description": "@cdklabs/cdk-appflow",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-appflow.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,25 @@
     },
     "packages": [
         "cdklabs.cdk_appflow",
         "cdklabs.cdk_appflow._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_appflow._jsii": [
-            "cdk-appflow@0.0.1.jsii.tgz"
+            "cdk-appflow@0.0.2.jsii.tgz"
         ],
         "cdklabs.cdk_appflow": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.83.0, <3.0.0",
+        "aws-cdk-lib>=2.84.0, <3.0.0",
+        "aws-cdk.aws-glue-alpha==2.84.0.a0",
+        "aws-cdk.aws-redshift-alpha==2.84.0.a0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

