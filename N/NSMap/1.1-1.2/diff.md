# Comparing `tmp/NSMap-1.1.tar.gz` & `tmp/NSMap-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NSMap-1.1.tar", last modified: Wed Jun 21 21:20:25 2023, max compression
+gzip compressed data, was "NSMap-1.2.tar", last modified: Wed Jun 21 21:29:12 2023, max compression
```

## Comparing `NSMap-1.1.tar` & `NSMap-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        0 2023-06-21 21:20:25.219879 NSMap-1.1/
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)     1086 2023-06-16 03:58:12.000000 NSMap-1.1/LICENSE
-drwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        0 2023-06-21 21:20:24.825928 NSMap-1.1/NSMap/
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)    12163 2023-06-20 23:51:55.000000 NSMap-1.1/NSMap/NSMapToolkit.py
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      237 2023-06-20 23:59:43.000000 NSMap-1.1/NSMap/__init__.py
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)     3843 2023-06-20 23:38:20.000000 NSMap-1.1/NSMap/modelSystems.py
-drwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        0 2023-06-21 21:20:25.142407 NSMap-1.1/NSMap.egg-info/
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      631 2023-06-21 21:20:24.000000 NSMap-1.1/NSMap.egg-info/PKG-INFO
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      232 2023-06-21 21:20:24.000000 NSMap-1.1/NSMap.egg-info/SOURCES.txt
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        1 2023-06-21 21:20:24.000000 NSMap-1.1/NSMap.egg-info/dependency_links.txt
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)       22 2023-06-21 21:20:24.000000 NSMap-1.1/NSMap.egg-info/requires.txt
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        6 2023-06-21 21:20:24.000000 NSMap-1.1/NSMap.egg-info/top_level.txt
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      631 2023-06-21 21:20:25.203312 NSMap-1.1/PKG-INFO
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      120 2023-06-16 03:58:12.000000 NSMap-1.1/README.md
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)       38 2023-06-21 21:20:25.223921 NSMap-1.1/setup.cfg
--rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      909 2023-06-21 20:50:23.000000 NSMap-1.1/setup.py
+drwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        0 2023-06-21 21:29:12.913489 NSMap-1.2/
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)     1086 2023-06-16 03:58:12.000000 NSMap-1.2/LICENSE
+drwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        0 2023-06-21 21:29:12.500109 NSMap-1.2/NSMap/
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)    12163 2023-06-20 23:51:55.000000 NSMap-1.2/NSMap/NSMapToolkit.py
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      237 2023-06-20 23:59:43.000000 NSMap-1.2/NSMap/__init__.py
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)     3843 2023-06-20 23:38:20.000000 NSMap-1.2/NSMap/modelSystems.py
+drwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        0 2023-06-21 21:29:12.827504 NSMap-1.2/NSMap.egg-info/
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      631 2023-06-21 21:29:11.000000 NSMap-1.2/NSMap.egg-info/PKG-INFO
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      232 2023-06-21 21:29:12.000000 NSMap-1.2/NSMap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        1 2023-06-21 21:29:11.000000 NSMap-1.2/NSMap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)       12 2023-06-21 21:29:11.000000 NSMap-1.2/NSMap.egg-info/requires.txt
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)        6 2023-06-21 21:29:11.000000 NSMap-1.2/NSMap.egg-info/top_level.txt
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      631 2023-06-21 21:29:12.897486 NSMap-1.2/PKG-INFO
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      120 2023-06-16 03:58:12.000000 NSMap-1.2/README.md
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)       38 2023-06-21 21:29:12.918484 NSMap-1.2/setup.cfg
+-rwxrwxrwx   0 kenflat2  (1000) kenflat2  (1000)      899 2023-06-21 21:29:06.000000 NSMap-1.2/setup.py
```

### Comparing `NSMap-1.1/LICENSE` & `NSMap-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NSMap-1.1/NSMap/NSMapToolkit.py` & `NSMap-1.2/NSMap/NSMapToolkit.py`

 * *Files identical despite different names*

### Comparing `NSMap-1.1/NSMap/modelSystems.py` & `NSMap-1.2/NSMap/modelSystems.py`

 * *Files identical despite different names*

### Comparing `NSMap-1.1/NSMap.egg-info/PKG-INFO` & `NSMap-1.2/NSMap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NSMap
-Version: 1.1
+Version: 1.2
 Summary: Implementation of NS-Map
 Home-page: UNKNOWN
 Author: Kenneth Gee
 Author-email: kenflat2@gmail.com
 License: UNKNOWN
 Keywords: Ecology,Forecasting,EDM,Empirical Dynamical Modeling,Nonstationarity
 Platform: UNKNOWN
```

### Comparing `NSMap-1.1/PKG-INFO` & `NSMap-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NSMap
-Version: 1.1
+Version: 1.2
 Summary: Implementation of NS-Map
 Home-page: UNKNOWN
 Author: Kenneth Gee
 Author-email: kenflat2@gmail.com
 License: UNKNOWN
 Keywords: Ecology,Forecasting,EDM,Empirical Dynamical Modeling,Nonstationarity
 Platform: UNKNOWN
```

### Comparing `NSMap-1.1/setup.py` & `NSMap-1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1'
+VERSION = '1.2'
 DESCRIPTION = 'Implementation of NS-Map'
 LONG_DESCRIPTION = 'Implementation of NS-Map, a nonstationary extension of the ecological forecasting method S-Map.'
 
 setup(
     name = 'NSMap',
     version = VERSION,
     author = 'Kenneth Gee',
     author_email = 'kenflat2@gmail.com',
     description = DESCRIPTION,
     long_description = LONG_DESCRIPTION,
     packages = find_packages(),
-    install_requires = ['numpy', 'scipy.integrate'],
+    install_requires = ['numpy', 'scipy'],
     keywords = ['Ecology', 'Forecasting', 'EDM', 'Empirical Dynamical Modeling', 'Nonstationarity'],
     classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Science/Research",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
```

