# Comparing `tmp/sorcerun-0.2.6.tar.gz` & `tmp/sorcerun-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.6.tar", last modified: Mon Jun  5 07:34:02 2023, max compression
+gzip compressed data, was "sorcerun-0.2.7.tar", last modified: Wed Jun 21 17:31:06 2023, max compression
```

## Comparing `sorcerun-0.2.6.tar` & `sorcerun-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:02.833937 sorcerun-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-05 07:33:51.000000 sorcerun-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 07:34:02.833937 sorcerun-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-05 07:33:51.000000 sorcerun-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:34:02.833937 sorcerun-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-05 07:33:51.000000 sorcerun-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:02.829937 sorcerun-0.2.6/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:02.833937 sorcerun-0.2.6/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:06.581747 sorcerun-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 17:30:55.000000 sorcerun-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 17:31:06.581747 sorcerun-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-21 17:30:55.000000 sorcerun-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:31:06.581747 sorcerun-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 17:30:55.000000 sorcerun-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:06.577747 sorcerun-0.2.7/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:06.581747 sorcerun-0.2.7/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.2.6/LICENSE` & `sorcerun-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.6/PKG-INFO` & `sorcerun-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.6
+Version: 0.2.7
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.6/README.md` & `sorcerun-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.6/setup.py` & `sorcerun-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.6",
+    version="0.2.7",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
```

### Comparing `sorcerun-0.2.6/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.7/sorcerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.6
+Version: 0.2.7
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.6/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.7/sorcerun_package/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.6/sorcerun_package/cli.py` & `sorcerun-0.2.7/sorcerun_package/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+import time
 from sklearn.model_selection import ParameterGrid
 import os
 import subprocess
 import json, yaml
 from contextlib import ExitStack
 from .mongodb_utils import mongodb_server, init_mongodb
 from .sacred_utils import load_adapter_function, run_sacred_experiment
@@ -102,17 +103,16 @@
 def start():
     with open(AUTH_FILE, "r") as f:
         authjson = json.loads(f.read())
         conf_path = authjson["conf_path"]
 
     print(conf_path)
     with mongodb_server(conf_path):
-        # TODO pipe log outputs to stdout or something nicely
         while True:
-            pass
+            time.sleep(10)
 
 
 @sorcerun.command()
 def omniboard():
     """
     Run Omniboard using the details saved in {AUTH_FILE}.
     """
```

### Comparing `sorcerun-0.2.6/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.7/sorcerun_package/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.6/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.7/sorcerun_package/sacred_utils.py`

 * *Files identical despite different names*

