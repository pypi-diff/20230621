# Comparing `tmp/getpaper-0.0.4.tar.gz` & `tmp/getpaper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.0.4.tar", last modified: Tue Jun 20 23:35:35 2023, max compression
+gzip compressed data, was "getpaper-0.0.5.tar", last modified: Wed Jun 21 00:15:39 2023, max compression
```

## Comparing `getpaper-0.0.4.tar` & `getpaper-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 23:35:35.530794 getpaper-0.0.4/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.4/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-20 23:35:35.530794 getpaper-0.0.4/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1344 2023-06-20 23:35:34.000000 getpaper-0.0.4/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 23:35:35.530794 getpaper-0.0.4/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.4/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3544 2023-06-20 22:10:24.000000 getpaper-0.0.4/getpaper/download.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3162 2023-06-20 23:27:35.000000 getpaper-0.0.4/getpaper/parse.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 23:35:35.530794 getpaper-0.0.4/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      280 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      142 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-20 23:35:35.530794 getpaper-0.0.4/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1472 2023-06-20 23:35:34.000000 getpaper-0.0.4/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 00:15:39.092116 getpaper-0.0.5/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.5/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-21 00:15:39.092116 getpaper-0.0.5/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1344 2023-06-20 23:35:34.000000 getpaper-0.0.5/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 00:15:39.088116 getpaper-0.0.5/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.5/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3544 2023-06-20 22:10:24.000000 getpaper-0.0.5/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1306 2023-06-21 00:13:24.000000 getpaper-0.0.5/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     4810 2023-06-21 00:06:28.000000 getpaper-0.0.5/getpaper/parse.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 00:15:39.092116 getpaper-0.0.5/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      298 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      142 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 00:15:39.000000 getpaper-0.0.5/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 00:15:39.092116 getpaper-0.0.5/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1472 2023-06-21 00:06:39.000000 getpaper-0.0.5/setup.py
```

### Comparing `getpaper-0.0.4/LICENSE` & `getpaper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.4/PKG-INFO` & `getpaper-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.4
+Version: 0.0.5
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.0.4/README.md` & `getpaper-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.4/getpaper/download.py` & `getpaper-0.0.5/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.4/getpaper.egg-info/PKG-INFO` & `getpaper-0.0.5/getpaper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.4
+Version: 0.0.5
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.0.4/setup.py` & `getpaper-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

