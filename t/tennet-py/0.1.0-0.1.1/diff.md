# Comparing `tmp/tennet-py-0.1.0.tar.gz` & `tmp/tennet-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tennet-py-0.1.0.tar", last modified: Mon Dec 13 17:47:13 2021, max compression
+gzip compressed data, was "tennet-py-0.1.1.tar", last modified: Wed Jun 21 11:51:48 2023, max compression
```

## Comparing `tennet-py-0.1.0.tar` & `tennet-py-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 17:47:13.034027 tennet-py-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-12-13 17:46:49.000000 tennet-py-0.1.0/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2021-12-13 17:47:13.034027 tennet-py-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-12-13 17:46:49.000000 tennet-py-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-13 17:47:13.034027 tennet-py-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2021-12-13 17:46:49.000000 tennet-py-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 17:47:13.030027 tennet-py-0.1.0/tennet/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-12-13 17:46:49.000000 tennet-py-0.1.0/tennet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2021-12-13 17:46:49.000000 tennet-py-0.1.0/tennet/tennet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 17:47:13.030027 tennet-py-0.1.0/tennet_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2021-12-13 17:47:12.000000 tennet-py-0.1.0/tennet_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      239 2021-12-13 17:47:12.000000 tennet-py-0.1.0/tennet_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 17:47:12.000000 tennet-py-0.1.0/tennet_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-13 17:47:12.000000 tennet-py-0.1.0/tennet_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-13 17:47:12.000000 tennet-py-0.1.0/tennet_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:51:48.957063 tennet-py-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 11:51:37.000000 tennet-py-0.1.1/LICENSE.MD
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-21 11:51:48.957063 tennet-py-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-21 11:51:37.000000 tennet-py-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 11:51:48.961063 tennet-py-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-21 11:51:37.000000 tennet-py-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:51:48.957063 tennet-py-0.1.1/tennet/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 11:51:37.000000 tennet-py-0.1.1/tennet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-21 11:51:37.000000 tennet-py-0.1.1/tennet/tennet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 11:51:37.000000 tennet-py-0.1.1/tennet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:51:48.957063 tennet-py-0.1.1/tennet_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-21 11:51:48.000000 tennet-py-0.1.1/tennet_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 11:51:48.000000 tennet-py-0.1.1/tennet_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:51:48.000000 tennet-py-0.1.1/tennet_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 11:51:48.000000 tennet-py-0.1.1/tennet_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 11:51:48.000000 tennet-py-0.1.1/tennet_py.egg-info/top_level.txt
```

### Comparing `tennet-py-0.1.0/LICENSE.MD` & `tennet-py-0.1.1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `tennet-py-0.1.0/PKG-INFO` & `tennet-py-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tennet-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python API wrapper for TenneT System & transmission data
 Home-page: https://github.com/fboerman/tennet-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: TenneT data api energy
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
@@ -54,8 +53,7 @@
 
 # retrieve same data as a dataframe
 df = client.query_df(DataType.settlementprices, d_from=start, d_to=end)
 ```
 
 ## Disclaimer
 This is an unoffical package which is not supported or endorsed in any way by TenneT TSO.
-
```

### Comparing `tennet-py-0.1.0/README.md` & `tennet-py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tennet-py-0.1.0/setup.py` & `tennet-py-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tennet-py-0.1.0/tennet_py.egg-info/PKG-INFO` & `tennet-py-0.1.1/tennet_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tennet-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python API wrapper for TenneT System & transmission data
 Home-page: https://github.com/fboerman/tennet-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: TenneT data api energy
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
@@ -54,8 +53,7 @@
 
 # retrieve same data as a dataframe
 df = client.query_df(DataType.settlementprices, d_from=start, d_to=end)
 ```
 
 ## Disclaimer
 This is an unoffical package which is not supported or endorsed in any way by TenneT TSO.
-
```

