# Comparing `tmp/ansys_mechanical_core-0.9.0.tar.gz` & `tmp/ansys_mechanical_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_mechanical_core-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_mechanical_core-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_mechanical_core-0.9.0.tar` & `ansys_mechanical_core-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1089 2023-06-13 15:12:57.796721 ansys_mechanical_core-0.9.0/LICENSE
--rw-r--r--   0        0        0     5448 2023-06-13 15:12:57.796721 ansys_mechanical_core-0.9.0/README.rst
--rw-r--r--   0        0        0     4042 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1236 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      138 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     4266 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     3697 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     6761 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/__init__.py
--rw-r--r--   0        0        0     4603 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/environ.py
--rw-r--r--   0        0        0     4834 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/linux_api.py
--rw-r--r--   0        0        0      238 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/sinks.py
--rw-r--r--   0        0        0     4094 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/windows_api.py
--rw-r--r--   0        0        0      852 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2990 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    78531 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25279 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 ansys_mechanical_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-21 20:01:07.489448 ansys_mechanical_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5448 2023-06-21 20:01:07.489448 ansys_mechanical_core-0.9.1/README.rst
+-rw-r--r--   0        0        0     4042 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1236 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      138 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     4266 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     3697 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1958 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     6761 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/__init__.py
+-rw-r--r--   0        0        0     4603 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/environ.py
+-rw-r--r--   0        0        0     4834 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/linux_api.py
+-rw-r--r--   0        0        0      238 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/sinks.py
+-rw-r--r--   0        0        0     4094 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/windows_api.py
+-rw-r--r--   0        0        0      852 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2990 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    78531 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25279 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 ansys_mechanical_core-0.9.1/PKG-INFO
```

### Comparing `ansys_mechanical_core-0.9.0/LICENSE` & `ansys_mechanical_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/README.rst` & `ansys_mechanical_core-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/pyproject.toml` & `ansys_mechanical_core-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.9.0"
+version = "0.9.1"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "ansys_api_mechanical==0.1.0",
     "ansys-pythonnet>=3.1.0rc1",
-    "ansys-tools-path>=0.2.3",
+    "ansys-tools-path>=0.2.6",
     "importlib-metadata>=4.0",
     "appdirs>=1.4.0",
     "grpcio>=1.30.0",
     "protobuf>=3.12.2,<3.21.0",
     "ansys-platform-instancemanagement>=1.0.1",
     "tqdm>=4.45.0",
 ]
@@ -46,15 +46,15 @@
 Homepage = "https://github.com/ansys/pymechanical"
 Tracker = "https://github.com/ansys/pymechanical/issues"
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.3.2",
     "pytest-cov==4.1.0",
-    "pytest-print==0.3.1",
+    "pytest-print==0.3.2",
 ]
 doc = [
     "Sphinx==6.2.1", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
     "ansys-sphinx-theme==0.9.9",
     "grpcio==1.54.2",
     "imageio-ffmpeg==0.4.8",
     "imageio==2.31.1",
```

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/__init__.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/_version.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/app.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/app.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/config.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/imports.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/initializer.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/initializer.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/loader.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/loader.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/__init__.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/environ.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/environ.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/linux_api.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/linux_api.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/windows_api.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/windows_api.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/resolver.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/runtime.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/shims.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/errors.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/examples/downloads.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/launcher.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/logging.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/mechanical.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/misc.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/pool.py` & `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/pool.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.0/PKG-INFO` & `ansys_mechanical_core-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python wrapper for Ansys Mechanical
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ansys_api_mechanical==0.1.0
 Requires-Dist: ansys-pythonnet>=3.1.0rc1
-Requires-Dist: ansys-tools-path>=0.2.3
+Requires-Dist: ansys-tools-path>=0.2.6
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: protobuf>=3.12.2,<3.21.0
 Requires-Dist: ansys-platform-instancemanagement>=1.0.1
 Requires-Dist: tqdm>=4.45.0
 Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
@@ -44,15 +44,15 @@
 Requires-Dist: sphinx_design==0.4.1 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
 Requires-Dist: pytest==7.3.2 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
-Requires-Dist: pytest-print==0.3.1 ; extra == "tests"
+Requires-Dist: pytest-print==0.3.2 ; extra == "tests"
 Project-URL: Documentation, https://mechanical.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/pymechanical
 Project-URL: Source, https://github.com/ansys/pymechanical
 Project-URL: Tracker, https://github.com/ansys/pymechanical/issues
 Provides-Extra: doc
 Provides-Extra: tests
```

