# Comparing `tmp/packg-0.2.11.tar.gz` & `tmp/packg-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.11.tar", last modified: Wed Jun 21 10:06:30 2023, max compression
+gzip compressed data, was "packg-0.2.12.tar", last modified: Wed Jun 21 10:46:28 2023, max compression
```

## Comparing `packg-0.2.11.tar` & `packg-0.2.12.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:06:30.539190 packg-0.2.11/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.11/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2233 2023-06-21 10:06:30.539190 packg-0.2.11/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1437 2023-06-21 10:05:29.000000 packg-0.2.11/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2317 2023-06-21 09:57:15.000000 packg-0.2.11/pyproject.toml
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 10:05:29.000000 packg-0.2.11/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-21 10:06:30.543190 packg-0.2.11/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:06:30.439188 packg-0.2.11/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:06:30.511190 packg-0.2.11/src/packg/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      129 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/dtime.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      297 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/files.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7252 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/import_from_source.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     4229 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/misc.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      472 2023-06-21 10:05:29.000000 packg-0.2.11/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:06:30.535190 packg-0.2.11/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2233 2023-06-21 10:06:30.000000 packg-0.2.11/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      453 2023-06-21 10:06:30.000000 packg-0.2.11/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 10:06:30.000000 packg-0.2.11/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 10:06:30.000000 packg-0.2.11/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-06-21 10:06:30.000000 packg-0.2.11/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 10:00:06.000000 packg-0.2.11/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.196900 packg-0.2.12/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.12/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2102 2023-06-21 10:46:28.196900 packg-0.2.12/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1306 2023-06-21 10:46:12.000000 packg-0.2.12/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2317 2023-06-21 09:57:15.000000 packg-0.2.12/pyproject.toml
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 10:46:12.000000 packg-0.2.12/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-21 10:46:28.196900 packg-0.2.12/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.120899 packg-0.2.12/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.164900 packg-0.2.12/src/packg/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      129 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/dtime.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      297 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/files.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7270 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/import_from_source.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     4229 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/misc.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      472 2023-06-21 10:46:12.000000 packg-0.2.12/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-21 10:46:28.192900 packg-0.2.12/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2102 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      453 2023-06-21 10:46:28.000000 packg-0.2.12/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-06-21 10:46:27.000000 packg-0.2.12/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 10:00:06.000000 packg-0.2.12/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.11/LICENSE` & `packg-0.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.11/PKG-INFO` & `packg-0.2.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.11
+Version: 0.2.12
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -36,16 +36,16 @@
 </p>
 
 Collection of utilities used in other python projects. 
 
 ## Features
 
 * `caching`: Cache objects to disk / to memory
-* `Const`: Class for defining constants, as alternative to `enum.Enum` 
-* `typext` Type definitions and other utilities
+* `Const`: Base class for defining constants, as alternative to `enum.Enum` 
+* `typext`: Type definitions
 * etc
 
 ## Install
 
 Requires `python>=3.7`
 
 ```bash
@@ -55,18 +55,13 @@
 ## Dev install
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
-pylint gpack
+pylint packg
 
-# run tests for python>=3.7
+# run tests
 python -m pytest --cov
 pylint tests
-
-# run tests for python>=3.9
-python -m pytest tests tests_py39 --cov
-pylint tests 
-pylint tests_py39
 ~~~
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.11 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.12 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development :: Version Control :: Git Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE # packg
           [build_3.7_status] [build_3.9_status] [coverage] [version]
 Collection of utilities used in other python projects. ## Features * `caching`:
-Cache objects to disk / to memory * `Const`: Class for defining constants, as
-alternative to `enum.Enum` * `typext` Type definitions and other utilities *
-etc ## Install Requires `python>=3.7` ```bash pip install packg ``` ## Dev
-install Clone repository and cd into, then: ~~~bash pip install -e . pip
-install pytest pytest-cov pylint pytest-lazy-fixture pylint gpack # run tests
-for python>=3.7 python -m pytest --cov pylint tests # run tests for python>=3.9
-python -m pytest tests tests_py39 --cov pylint tests pylint tests_py39 ~~~
+Cache objects to disk / to memory * `Const`: Base class for defining constants,
+as alternative to `enum.Enum` * `typext`: Type definitions * etc ## Install
+Requires `python>=3.7` ```bash pip install packg ``` ## Dev install Clone
+repository and cd into, then: ~~~bash pip install -e . pip install pytest
+pytest-cov pylint pytest-lazy-fixture pylint packg # run tests python -m pytest
+--cov pylint tests ~~~
```

### Comparing `packg-0.2.11/pyproject.toml` & `packg-0.2.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.11/src/packg/caching.py` & `packg-0.2.12/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.11/src/packg/constclass.py` & `packg-0.2.12/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.11/src/packg/import_from_source.py` & `packg-0.2.12/src/packg/import_from_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
 
 def _apply_visitor(module: str, visitor: NodeVisitor) -> None:
     module_spec = import_util.find_spec(module)
     assert module_spec is not None
     assert module_spec.origin is not None
 
-    with open(module_spec.origin, "r") as source_file:
+    with open(module_spec.origin, "r", encoding="utf-8") as source_file:
         ast = parse(source=source_file.read(), filename=module_spec.origin)
 
     visitor.visit(ast)
 
 
 # unprivate some stuff
 apply_visitor = _apply_visitor
```

### Comparing `packg-0.2.11/src/packg/log.py` & `packg-0.2.12/src/packg/log.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.11/src/packg/system.py` & `packg-0.2.12/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.11/src/packg.egg-info/PKG-INFO` & `packg-0.2.12/src/packg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.11
+Version: 0.2.12
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -36,16 +36,16 @@
 </p>
 
 Collection of utilities used in other python projects. 
 
 ## Features
 
 * `caching`: Cache objects to disk / to memory
-* `Const`: Class for defining constants, as alternative to `enum.Enum` 
-* `typext` Type definitions and other utilities
+* `Const`: Base class for defining constants, as alternative to `enum.Enum` 
+* `typext`: Type definitions
 * etc
 
 ## Install
 
 Requires `python>=3.7`
 
 ```bash
@@ -55,18 +55,13 @@
 ## Dev install
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
-pylint gpack
+pylint packg
 
-# run tests for python>=3.7
+# run tests
 python -m pytest --cov
 pylint tests
-
-# run tests for python>=3.9
-python -m pytest tests tests_py39 --cov
-pylint tests 
-pylint tests_py39
 ~~~
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.11 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.12 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development :: Version Control :: Git Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE # packg
           [build_3.7_status] [build_3.9_status] [coverage] [version]
 Collection of utilities used in other python projects. ## Features * `caching`:
-Cache objects to disk / to memory * `Const`: Class for defining constants, as
-alternative to `enum.Enum` * `typext` Type definitions and other utilities *
-etc ## Install Requires `python>=3.7` ```bash pip install packg ``` ## Dev
-install Clone repository and cd into, then: ~~~bash pip install -e . pip
-install pytest pytest-cov pylint pytest-lazy-fixture pylint gpack # run tests
-for python>=3.7 python -m pytest --cov pylint tests # run tests for python>=3.9
-python -m pytest tests tests_py39 --cov pylint tests pylint tests_py39 ~~~
+Cache objects to disk / to memory * `Const`: Base class for defining constants,
+as alternative to `enum.Enum` * `typext`: Type definitions * etc ## Install
+Requires `python>=3.7` ```bash pip install packg ``` ## Dev install Clone
+repository and cd into, then: ~~~bash pip install -e . pip install pytest
+pytest-cov pylint pytest-lazy-fixture pylint packg # run tests python -m pytest
+--cov pylint tests ~~~
```

