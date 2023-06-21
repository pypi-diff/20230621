# Comparing `tmp/sysml2py-0.2.3.tar.gz` & `tmp/sysml2py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.2.3.tar", last modified: Wed Jun 21 03:30:22 2023, max compression
+gzip compressed data, was "sysml2py-0.3.0.tar", last modified: Wed Jun 21 03:26:33 2023, max compression
```

## Comparing `sysml2py-0.2.3.tar` & `sysml2py-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:30:22.788157 sysml2py-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 03:30:11.000000 sysml2py-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:30:22.788157 sysml2py-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-21 03:30:11.000000 sysml2py-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 03:30:11.000000 sysml2py-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:30:22.792157 sysml2py-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:30:22.784157 sysml2py-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:30:22.788157 sysml2py-0.2.3/src/sysml2py/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:30:22.788157 sysml2py-0.2.3/src/sysml2py/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/grammar/SysML.tx
--rw-r--r--   0 runner    (1001) docker     (123)    80969 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/grammar/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:30:22.788157 sysml2py-0.2.3/src/sysml2py/textx/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-21 03:30:11.000000 sysml2py-0.2.3/src/sysml2py/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:30:22.788157 sysml2py-0.2.3/sysml2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:30:22.000000 sysml2py-0.2.3/sysml2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 03:30:22.000000 sysml2py-0.2.3/sysml2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:30:22.000000 sysml2py-0.2.3/sysml2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 03:30:22.000000 sysml2py-0.2.3/sysml2py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.945388 sysml2py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 03:26:26.000000 sysml2py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:26:33.945388 sysml2py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-21 03:26:26.000000 sysml2py-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 03:26:26.000000 sysml2py-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:26:33.945388 sysml2py-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.937388 sysml2py-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.941388 sysml2py-0.3.0/src/sysml2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.941388 sysml2py-0.3.0/src/sysml2py/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    80969 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.941388 sysml2py-0.3.0/src/sysml2py/textx/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.945388 sysml2py-0.3.0/sysml2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/top_level.txt
```

### Comparing `sysml2py-0.2.3/LICENSE` & `sysml2py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/PKG-INFO` & `sysml2py-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.2.3
+Version: 0.3.0
 Summary: SysML v2.0 Parser
 Author-email: Christopher Cox <chris.cox@westfall.io>
 Project-URL: Homepage, https://github.com/Westfall-io/sysml2py
 Project-URL: Bug Tracker, https://github.com/Westfall-io/sysml2py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sysml2py-0.2.3/README.md` & `sysml2py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/pyproject.toml` & `sysml2py-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysml2py"
-version = "0.2.3"
+version = "0.3.0"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sysml2py-0.2.3/src/sysml2py/__init__.py` & `sysml2py-0.3.0/src/sysml2py/__init__.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/src/sysml2py/formatting.py` & `sysml2py-0.3.0/src/sysml2py/formatting.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.3.0/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.3.0/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.3.0/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/src/sysml2py/grammar/classes.py` & `sysml2py-0.3.0/src/sysml2py/grammar/classes.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.3.0/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/src/sysml2py/types.py` & `sysml2py-0.3.0/src/sysml2py/types.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.3/sysml2py.egg-info/PKG-INFO` & `sysml2py-0.3.0/sysml2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.2.3
+Version: 0.3.0
 Summary: SysML v2.0 Parser
 Author-email: Christopher Cox <chris.cox@westfall.io>
 Project-URL: Homepage, https://github.com/Westfall-io/sysml2py
 Project-URL: Bug Tracker, https://github.com/Westfall-io/sysml2py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

