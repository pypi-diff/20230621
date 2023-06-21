# Comparing `tmp/typedparser-0.2.7.tar.gz` & `tmp/typedparser-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedparser-0.2.7.tar", last modified: Wed Jun 21 09:37:18 2023, max compression
+gzip compressed data, was "typedparser-0.2.8.tar", last modified: Wed Jun 21 09:41:51 2023, max compression
```

## Comparing `typedparser-0.2.7.tar` & `typedparser-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:37:18.121847 typedparser-0.2.7/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.2.7/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     6218 2023-06-21 09:37:18.117847 typedparser-0.2.7/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5405 2023-06-21 09:33:18.000000 typedparser-0.2.7/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.2.7/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 09:33:18.000000 typedparser-0.2.7/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-21 09:37:18.121847 typedparser-0.2.7/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:37:18.049845 typedparser-0.2.7/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:37:18.093846 typedparser-0.2.7/src/typedparser/
--rw-------   0 gings    (14999) lmb-mit   (1061)      391 2023-06-21 09:33:18.000000 typedparser-0.2.7/src/typedparser/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    12145 2023-06-21 09:33:18.000000 typedparser-0.2.7/src/typedparser/_typedattr.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3513 2023-06-21 09:33:18.000000 typedparser-0.2.7/src/typedparser/_typedparser.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-06-21 09:33:18.000000 typedparser-0.2.7/src/typedparser/custom_format.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5393 2023-06-21 09:33:18.000000 typedparser-0.2.7/src/typedparser/funcs.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     9485 2023-06-21 09:33:18.000000 typedparser-0.2.7/src/typedparser/objects.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:37:18.113846 typedparser-0.2.7/src/typedparser.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     6218 2023-06-21 09:37:17.000000 typedparser-0.2.7/src/typedparser.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      452 2023-06-21 09:37:17.000000 typedparser-0.2.7/src/typedparser.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:37:17.000000 typedparser-0.2.7/src/typedparser.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 09:37:17.000000 typedparser-0.2.7/src/typedparser.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-06-21 09:37:17.000000 typedparser-0.2.7/src/typedparser.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:37:17.000000 typedparser-0.2.7/src/typedparser.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.863883 typedparser-0.2.8/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.2.8/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5960 2023-06-21 09:41:51.863883 typedparser-0.2.8/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5147 2023-06-21 09:41:35.000000 typedparser-0.2.8/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.2.8/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 09:41:35.000000 typedparser-0.2.8/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-21 09:41:51.867883 typedparser-0.2.8/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.807881 typedparser-0.2.8/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.835882 typedparser-0.2.8/src/typedparser/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      391 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    12145 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/_typedattr.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3513 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/_typedparser.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/custom_format.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5393 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/funcs.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     9485 2023-06-21 09:41:35.000000 typedparser-0.2.8/src/typedparser/objects.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 09:41:51.859883 typedparser-0.2.8/src/typedparser.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5960 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      452 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-06-21 09:41:51.000000 typedparser-0.2.8/src/typedparser.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:37:17.000000 typedparser-0.2.8/src/typedparser.egg-info/zip-safe
```

### Comparing `typedparser-0.2.7/LICENSE` & `typedparser-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.7/PKG-INFO` & `typedparser-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.2.7
+Version: 0.2.8
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -157,22 +157,14 @@
 
 * New attributes cannot to be added after class definition to an attrs instance,
   unless it is created with `@define(slots=False)`
   [Explanation](https://www.attrs.org/en/21.2.0/glossary.html#term-slotted-classes)
 * Untyped fields or "ClassVar" typed fields will be ignored by @attrs.define
   and therefore also by this library.
 
-### Other utilities in the package 
-
-* `Const`: An alternative to `enum.Enum` for defining constants
-* `cacheutils`: Cache objects to disk / to memory
-* `objutils`: Various utilities like nested modification of dicts
-* Type definitions and other utilities
-
-
 ## Install locally and run tests
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
```

### Comparing `typedparser-0.2.7/README.md` & `typedparser-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -135,22 +135,14 @@
 
 * New attributes cannot to be added after class definition to an attrs instance,
   unless it is created with `@define(slots=False)`
   [Explanation](https://www.attrs.org/en/21.2.0/glossary.html#term-slotted-classes)
 * Untyped fields or "ClassVar" typed fields will be ignored by @attrs.define
   and therefore also by this library.
 
-### Other utilities in the package 
-
-* `Const`: An alternative to `enum.Enum` for defining constants
-* `cacheutils`: Cache objects to disk / to memory
-* `objutils`: Various utilities like nested modification of dicts
-* Type definitions and other utilities
-
-
 ## Install locally and run tests
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
```

### Comparing `typedparser-0.2.7/pyproject.toml` & `typedparser-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.7/src/typedparser/_typedattr.py` & `typedparser-0.2.8/src/typedparser/_typedattr.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.7/src/typedparser/_typedparser.py` & `typedparser-0.2.8/src/typedparser/_typedparser.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.7/src/typedparser/custom_format.py` & `typedparser-0.2.8/src/typedparser/custom_format.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.7/src/typedparser/funcs.py` & `typedparser-0.2.8/src/typedparser/funcs.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.7/src/typedparser/objects.py` & `typedparser-0.2.8/src/typedparser/objects.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.2.7/src/typedparser.egg-info/PKG-INFO` & `typedparser-0.2.8/src/typedparser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.2.7
+Version: 0.2.8
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -157,22 +157,14 @@
 
 * New attributes cannot to be added after class definition to an attrs instance,
   unless it is created with `@define(slots=False)`
   [Explanation](https://www.attrs.org/en/21.2.0/glossary.html#term-slotted-classes)
 * Untyped fields or "ClassVar" typed fields will be ignored by @attrs.define
   and therefore also by this library.
 
-### Other utilities in the package 
-
-* `Const`: An alternative to `enum.Enum` for defining constants
-* `cacheutils`: Cache objects to disk / to memory
-* `objutils`: Various utilities like nested modification of dicts
-* Type definitions and other utilities
-
-
 ## Install locally and run tests
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
```

