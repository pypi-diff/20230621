# Comparing `tmp/aws-cdk.aws-iotevents-actions-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-iotevents-actions-alpha-2.85.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-iotevents-actions-alpha/dist/python/aws-cdk.aws-iotevents-actions-alph", last modified: Tue Jun 13 23:47:31 2023, max compression
+gzip compressed data, was "/codebuild/output/src913890871/src/packages/@aws-cdk/aws-iotevents-actions-alpha/dist/python/aws-cdk.aws-iotevents-actions-alph", last modified: Wed Jun 21 13:32:44 2023, max compression
```

## Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0.tar` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5723 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4705 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1987 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/aws_iotevents_actions_alpha/
--rw-r--r--   0 root         (0) root         (0)    19108 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      502 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30977 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:21.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/aws_iotevents_actions_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5723 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      631 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:31.000000 aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5723 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/aws_iotevents_actions_alpha/
+-rw-r--r--   0 root         (0) root         (0)    19108 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      502 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30976 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.85.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:35.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/aws_iotevents_actions_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5723 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      631 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 13:32:44.000000 aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iotevents-actions-alpha
-Version: 2.84.0a0
+Version: 2.85.0a0
 Summary: Receipt Detector Model actions for AWS IoT Events
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/README.md` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-iotevents-actions-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.85.0.a0",
     "description": "Receipt Detector Model actions for AWS IoT Events",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_cdk.aws_iotevents_actions_alpha",
         "aws_cdk.aws_iotevents_actions_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_iotevents_actions_alpha._jsii": [
-            "aws-iotevents-actions-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-iotevents-actions-alpha@2.85.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_iotevents_actions_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.84.0",
-        "aws-cdk.aws-iotevents-alpha==2.84.0.a0",
+        "aws-cdk-lib==2.85.0",
+        "aws-cdk.aws-iotevents-alpha==2.85.0.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iotevents-actions-alpha
-Version: 2.84.0a0
+Version: 2.85.0a0
 Summary: Receipt Detector Model actions for AWS IoT Events
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.84.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-iotevents-actions-alpha-2.85.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/requires.txt
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_iotevents_actions_alpha/__init__.py
 src/aws_cdk/aws_iotevents_actions_alpha/py.typed
 src/aws_cdk/aws_iotevents_actions_alpha/_jsii/__init__.py
-src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.85.0-alpha.0.jsii.tgz
```

