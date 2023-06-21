# Comparing `tmp/typedparser-0.2.8.tar.gz` & `tmp/typedparser-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedparser-0.2.8.tar", last modified: Wed Jun 21 09:41:51 2023, max compression
+gzip compressed data, was "typedparser-0.2.9.tar", last modified: Wed Jun 21 09:47:26 2023, max compression
```

## Comparing `typedparser-0.2.8.tar` & `typedparser-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.863883 typedparser-0.2.8/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.2.8/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     5960 2023-06-21 09:41:51.863883 typedparser-0.2.8/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5147 2023-06-21 09:41:35.000000 typedparser-0.2.8/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.2.8/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 09:41:35.000000 typedparser-0.2.8/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-21 09:41:51.867883 typedparser-0.2.8/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.807881 typedparser-0.2.8/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.835882 typedparser-0.2.8/src/typedparser/
--rw-------   0 gings    (14999) lmb-mit   (1061)      391 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    12145 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/_typedattr.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3513 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/_typedparser.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/custom_format.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5393 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/funcs.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     9485 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/objects.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.859883 typedparser-0.2.8/src/typedparser.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     5960 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      452 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:37:17.000000 typedparser-0.2.8/src/typedparser.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:47:26.379238 typedparser-0.2.9/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.2.9/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5960 2023-06-21 09:47:26.375238 typedparser-0.2.9/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5147 2023-06-21 09:45:39.000000 typedparser-0.2.9/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.2.9/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-06-21 09:45:39.000000 typedparser-0.2.9/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-21 09:47:26.379238 typedparser-0.2.9/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:47:26.323237 typedparser-0.2.9/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:47:26.347237 typedparser-0.2.9/src/typedparser/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      391 2023-06-21 09:45:39.000000 typedparser-0.2.9/src/typedparser/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    12145 2023-06-21 09:45:39.000000 typedparser-0.2.9/src/typedparser/_typedattr.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3513 2023-06-21 09:45:39.000000 typedparser-0.2.9/src/typedparser/_typedparser.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-06-21 09:45:39.000000 typedparser-0.2.9/src/typedparser/custom_format.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5393 2023-06-21 09:45:39.000000 typedparser-0.2.9/src/typedparser/funcs.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     9485 2023-06-21 09:45:39.000000 typedparser-0.2.9/src/typedparser/objects.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:47:26.371238 typedparser-0.2.9/src/typedparser.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5960 2023-06-21 09:47:26.000000 typedparser-0.2.9/src/typedparser.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      452 2023-06-21 09:47:26.000000 typedparser-0.2.9/src/typedparser.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:47:26.000000 typedparser-0.2.9/src/typedparser.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-06-21 09:47:26.000000 typedparser-0.2.9/src/typedparser.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-06-21 09:47:26.000000 typedparser-0.2.9/src/typedparser.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:37:17.000000 typedparser-0.2.9/src/typedparser.egg-info/zip-safe
```

### Comparing `typedparser-0.2.8/LICENSE` & `typedparser-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/PKG-INFO` & `typedparser-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `typedparser-0.2.8/README.md` & `typedparser-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/pyproject.toml` & `typedparser-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/src/typedparser/_typedattr.py` & `typedparser-0.2.9/src/typedparser/_typedattr.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/src/typedparser/_typedparser.py` & `typedparser-0.2.9/src/typedparser/_typedparser.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/src/typedparser/custom_format.py` & `typedparser-0.2.9/src/typedparser/custom_format.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/src/typedparser/funcs.py` & `typedparser-0.2.9/src/typedparser/funcs.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/src/typedparser/objects.py` & `typedparser-0.2.9/src/typedparser/objects.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.8/src/typedparser.egg-info/PKG-INFO` & `typedparser-0.2.9/src/typedparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

