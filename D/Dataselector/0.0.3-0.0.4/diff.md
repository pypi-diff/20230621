# Comparing `tmp/Dataselector-0.0.3.tar.gz` & `tmp/Dataselector-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dataselector-0.0.3.tar", last modified: Wed Jun 21 09:26:42 2023, max compression
+gzip compressed data, was "Dataselector-0.0.4.tar", last modified: Wed Jun 21 11:13:08 2023, max compression
```

## Comparing `Dataselector-0.0.3.tar` & `Dataselector-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 09:26:42.804730 Dataselector-0.0.3/
--rw-rw-rw-   0        0        0      252 2023-06-21 09:24:52.000000 Dataselector-0.0.3/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 09:26:42.794365 Dataselector-0.0.3/Dataselector/
--rw-rw-rw-   0        0        0     3337 2023-06-21 09:23:35.000000 Dataselector-0.0.3/Dataselector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 09:26:42.801726 Dataselector-0.0.3/Dataselector.egg-info/
--rw-rw-rw-   0        0        0      941 2023-06-21 09:26:42.000000 Dataselector-0.0.3/Dataselector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-21 09:26:42.000000 Dataselector-0.0.3/Dataselector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 09:26:42.000000 Dataselector-0.0.3/Dataselector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-21 09:26:42.000000 Dataselector-0.0.3/Dataselector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-21 09:26:42.000000 Dataselector-0.0.3/Dataselector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-06-20 12:22:56.000000 Dataselector-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-21 04:11:24.000000 Dataselector-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      941 2023-06-21 09:26:42.803732 Dataselector-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      123 2023-06-20 12:15:51.000000 Dataselector-0.0.3/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 09:26:42.804730 Dataselector-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-06-21 09:16:08.000000 Dataselector-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:13:08.115739 Dataselector-0.0.4/
+-rw-rw-rw-   0        0        0      367 2023-06-21 11:12:02.000000 Dataselector-0.0.4/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 11:13:08.107272 Dataselector-0.0.4/Dataselector/
+-rw-rw-rw-   0        0        0     3337 2023-06-21 11:11:30.000000 Dataselector-0.0.4/Dataselector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:13:08.115739 Dataselector-0.0.4/Dataselector.egg-info/
+-rw-rw-rw-   0        0        0     1056 2023-06-21 11:13:08.000000 Dataselector-0.0.4/Dataselector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-21 11:13:08.000000 Dataselector-0.0.4/Dataselector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 11:13:08.000000 Dataselector-0.0.4/Dataselector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-21 11:13:08.000000 Dataselector-0.0.4/Dataselector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 11:13:08.000000 Dataselector-0.0.4/Dataselector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-06-20 12:22:56.000000 Dataselector-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-21 04:11:24.000000 Dataselector-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1056 2023-06-21 11:13:08.115739 Dataselector-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2023-06-20 12:15:51.000000 Dataselector-0.0.4/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 11:13:08.115739 Dataselector-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-06-21 11:12:28.000000 Dataselector-0.0.4/setup.py
```

### Comparing `Dataselector-0.0.3/Dataselector/__init__.py` & `Dataselector-0.0.4/Dataselector/__init__.py`

 * *Files identical despite different names*

### Comparing `Dataselector-0.0.3/Dataselector.egg-info/PKG-INFO` & `Dataselector-0.0.4/Dataselector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dataselector
-Version: 0.0.3
+Version: 0.0.4
 Summary: A handy library to import dataset from various excel file types and URls
 Home-page: 
 Author: Siddharth Mishra
 Author-email: Siddharth.mishra@ganitinc.co.in
 License: MIT
 Keywords: Dataset
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,7 +27,12 @@
 -------------------
 - Beta test release two
 
 0.0.3 (21/06/2023)
 -------------------
 - Beta test release two point one
 - fixing several bugs 
+
+0.0.4 (21/06/2023)
+-------------------
+- Beta test release two point one
+- excluded all the system libraries
```

### Comparing `Dataselector-0.0.3/LICENSE.txt` & `Dataselector-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Dataselector-0.0.3/PKG-INFO` & `Dataselector-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dataselector
-Version: 0.0.3
+Version: 0.0.4
 Summary: A handy library to import dataset from various excel file types and URls
 Home-page: 
 Author: Siddharth Mishra
 Author-email: Siddharth.mishra@ganitinc.co.in
 License: MIT
 Keywords: Dataset
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,7 +27,12 @@
 -------------------
 - Beta test release two
 
 0.0.3 (21/06/2023)
 -------------------
 - Beta test release two point one
 - fixing several bugs 
+
+0.0.4 (21/06/2023)
+-------------------
+- Beta test release two point one
+- excluded all the system libraries
```

