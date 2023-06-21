# Comparing `tmp/botocore-a-la-carte-verifiedpermissions-1.29.156.tar.gz` & `tmp/botocore-a-la-carte-verifiedpermissions-1.29.157.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-verifiedpermissions-1.29.156.tar", last modified: Tue Jun 20 01:22:28 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-verifiedpermissions-1.29.157.tar", last modified: Wed Jun 21 01:25:05 2023, max compression
```

## Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156.tar` & `botocore-a-la-carte-verifiedpermissions-1.29.157.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-20 01:22:28.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-06-20 01:21:37.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-20 01:21:37.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   125360 2023-06-20 01:21:37.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 01:21:37.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore_a_la_carte_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 01:22:28.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-20 01:22:28.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:22:28.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore_a_la_carte_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 01:22:28.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/botocore_a_la_carte_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 01:22:28.277665 botocore-a-la-carte-verifiedpermissions-1.29.156/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-20 01:22:28.000000 botocore-a-la-carte-verifiedpermissions-1.29.156/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-21 01:25:05.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-06-21 01:24:02.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-21 01:24:02.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   125360 2023-06-21 01:24:02.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 01:24:02.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore_a_la_carte_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 01:25:05.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-21 01:25:05.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:25:05.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore_a_la_carte_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 01:25:05.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/botocore_a_la_carte_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:25:05.348207 botocore-a-la-carte-verifiedpermissions-1.29.157/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-21 01:25:05.000000 botocore-a-la-carte-verifiedpermissions-1.29.157/setup.py
```

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/LICENSE.txt` & `botocore-a-la-carte-verifiedpermissions-1.29.157/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/PKG-INFO` & `botocore-a-la-carte-verifiedpermissions-1.29.157/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-verifiedpermissions
-Version: 1.29.156
+Version: 1.29.157
 Summary: verifiedpermissions data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json` & `botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/botocore/data/verifiedpermissions/2021-12-01/service-2.json` & `botocore-a-la-carte-verifiedpermissions-1.29.157/botocore/data/verifiedpermissions/2021-12-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO` & `botocore-a-la-carte-verifiedpermissions-1.29.157/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-verifiedpermissions
-Version: 1.29.156
+Version: 1.29.157
 Summary: verifiedpermissions data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt` & `botocore-a-la-carte-verifiedpermissions-1.29.157/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.156/setup.py` & `botocore-a-la-carte-verifiedpermissions-1.29.157/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-verifiedpermissions',
-    version="1.29.156",
+    version="1.29.157",
     description='verifiedpermissions data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/verifiedpermissions/*/*.json'],
```

