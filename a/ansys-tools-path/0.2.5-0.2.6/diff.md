# Comparing `tmp/ansys_tools_path-0.2.5.tar.gz` & `tmp/ansys_tools_path-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_path-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_path-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_path-0.2.5.tar` & `ansys_tools_path-0.2.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/LICENSE
--rw-r--r--   0        0        0     4691 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/README.rst
--rw-r--r--   0        0        0     1843 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      919 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      648 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    26232 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4691 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/README.rst
+-rw-r--r--   0        0        0     1843 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      919 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      648 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    26251 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.2.6/PKG-INFO
```

### Comparing `ansys_tools_path-0.2.5/LICENSE` & `ansys_tools_path-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.5/README.rst` & `ansys_tools_path-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.5/pyproject.toml` & `ansys_tools_path-0.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.2.5"
+version = "0.2.6"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys_tools_path-0.2.5/src/ansys/tools/path/__init__.py` & `ansys_tools_path-0.2.6/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.5/src/ansys/tools/path/misc.py` & `ansys_tools_path-0.2.6/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.5/src/ansys/tools/path/path.py` & `ansys_tools_path-0.2.6/src/ansys/tools/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 LINUX_DEFAULT_DIRS = [["/", "usr", "ansys_inc"], ["/", "ansys_inc"], ["/", "install", "ansys_inc"]]
 LINUX_DEFAULT_DIRS = [os.path.join(*each) for each in LINUX_DEFAULT_DIRS]
 
 CONFIG_FILE_NAME = "config.txt"
 
 SUPPORTED_ANSYS_VERSIONS = {
+    241: "2024R1",
     232: "2023R2",
     231: "2023R1",
     222: "2022R2",
     221: "2022R1",
     212: "2021R2",
     211: "2021R1",
     202: "2020R2",
```

### Comparing `ansys_tools_path-0.2.5/PKG-INFO` & `ansys_tools_path-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.2.5
+Version: 0.2.6
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

