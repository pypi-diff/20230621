# Comparing `tmp/triplex-0.0.10.tar.gz` & `tmp/triplex-0.0.11.tar.gz`

## Comparing `triplex-0.0.10.tar` & `triplex-0.0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/README.md
--rwxr-xr-x   0        0        0    11637 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/dfas.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/exceptions.py
--rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/perturbations.py
--rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/triplex.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/parsers/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/parsers/clausie.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/parsers/ollie.py
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/parsers/openie.py
--rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/parsers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/probings/__init__.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/probings/esnli.py
--rwxr-xr-x   0        0        0     5611 2020-02-02 00:00:00.000000 triplex-0.0.10/src/triplex/scripts/extract_from_dataset.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 triplex-0.0.10/LICENSE
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 triplex-0.0.10/README.md
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 triplex-0.0.10/pyproject.toml
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 triplex-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/README.md
+-rwxr-xr-x   0        0        0    11637 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/dfas.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/exceptions.py
+-rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/perturbations.py
+-rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/triplex.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/parsers/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/parsers/clausie.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/parsers/ollie.py
+-rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/parsers/openie.py
+-rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/parsers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/probings/__init__.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/probings/esnli.py
+-rwxr-xr-x   0        0        0     5611 2020-02-02 00:00:00.000000 triplex-0.0.11/src/triplex/scripts/extract_from_dataset.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 triplex-0.0.11/LICENSE
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 triplex-0.0.11/README.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 triplex-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 triplex-0.0.11/PKG-INFO
```

### Comparing `triplex-0.0.10/src/triplex/README.md` & `triplex-0.0.11/src/triplex/README.md`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/dfas.py` & `triplex-0.0.11/src/triplex/dfas.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/perturbations.py` & `triplex-0.0.11/src/triplex/perturbations.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/triplex.py` & `triplex-0.0.11/src/triplex/triplex.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/parsers/ollie.py` & `triplex-0.0.11/src/triplex/parsers/ollie.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/parsers/openie.py` & `triplex-0.0.11/src/triplex/parsers/openie.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/parsers/utils.py` & `triplex-0.0.11/src/triplex/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/probings/esnli.py` & `triplex-0.0.11/src/triplex/probings/esnli.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/src/triplex/scripts/extract_from_dataset.py` & `triplex-0.0.11/src/triplex/scripts/extract_from_dataset.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/LICENSE` & `triplex-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/README.md` & `triplex-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `triplex-0.0.10/pyproject.toml` & `triplex-0.0.11/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "triplex"
-version = "0.0.10"
+version = "0.0.11"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@di.unipi.it" },
 ]
 description = "Explaining models, with Triples."
 readme = "README.md"
-requires-python = ">=3.10, <3.11"
+requires-python = ">=3.8, <3.11"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers"
 ]
```

### Comparing `triplex-0.0.10/PKG-INFO` & `triplex-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: triplex
-Version: 0.0.10
+Version: 0.0.11
 Summary: Explaining models, with Triples.
 Project-URL: Homepage, https://github.com/msetzu/triplex
 Project-URL: Bug Tracker, https://github.com/msetzu/triplex/issues
 Author-email: Mattia Setzu <mattia.setzu@di.unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.10
+Requires-Python: <3.11,>=3.8
 Requires-Dist: click==7.1.2
 Requires-Dist: fire
 Requires-Dist: huggingface-hub
 Requires-Dist: logzero
 Requires-Dist: nltk
 Requires-Dist: numpy
 Requires-Dist: pandas
```

