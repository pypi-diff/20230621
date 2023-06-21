# Comparing `tmp/h3result-0.2.0.tar.gz` & `tmp/h3result-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h3result-0.2.0.tar", max compression
+gzip compressed data, was "h3result-0.3.0.tar", max compression
```

## Comparing `h3result-0.2.0.tar` & `h3result-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       34 2023-06-15 20:47:23.576073 h3result-0.2.0/README.md
--rw-r--r--   0        0        0     4297 2023-06-21 10:26:45.409404 h3result-0.2.0/build_ext.py
--rw-r--r--   0        0        0        0 2023-06-15 20:47:23.719071 h3result-0.2.0/h3result/__init__.py
--rw-r--r--   0        0        0      242 2023-06-15 21:23:57.265652 h3result-0.2.0/h3result/error.py
--rw-r--r--   0        0        0     1520 2023-06-19 09:24:28.280320 h3result-0.2.0/h3result/h3result.py
--rw-r--r--   0        0        0      970 2023-06-15 21:24:22.759664 h3result-0.2.0/h3result/interface.h
--rw-r--r--   0        0        0       72 2023-06-15 20:47:23.718229 h3result-0.2.0/h3result/path_like.py
--rw-r--r--   0        0        0      850 2023-06-19 09:51:43.238565 h3result-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 h3result-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-06-15 20:47:23.576073 h3result-0.3.0/README.md
+-rw-r--r--   0        0        0     4297 2023-06-21 10:26:45.409404 h3result-0.3.0/build_ext.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:47:23.719071 h3result-0.3.0/h3result/__init__.py
+-rw-r--r--   0        0        0      242 2023-06-15 21:23:57.265652 h3result-0.3.0/h3result/error.py
+-rw-r--r--   0        0        0     1513 2023-06-21 11:21:21.364139 h3result-0.3.0/h3result/h3result.py
+-rw-r--r--   0        0        0      970 2023-06-15 21:24:22.759664 h3result-0.3.0/h3result/interface.h
+-rw-r--r--   0        0        0       72 2023-06-15 20:47:23.718229 h3result-0.3.0/h3result/path_like.py
+-rw-r--r--   0        0        0      645 2023-06-21 11:22:35.090117 h3result-0.3.0/h3result/read_h3result.py
+-rw-r--r--   0        0        0      850 2023-06-21 11:13:55.176931 h3result-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 h3result-0.3.0/PKG-INFO
```

### Comparing `h3result-0.2.0/build_ext.py` & `h3result-0.3.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `h3result-0.2.0/h3result/interface.h` & `h3result-0.3.0/h3result/interface.h`

 * *Files identical despite different names*

### Comparing `h3result-0.2.0/pyproject.toml` & `h3result-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "h3result"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python wrapper for h3result library."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "h3result" }]
 include = [
 	{ path = "h3result/*.so", format = "wheel" },
```

### Comparing `h3result-0.2.0/PKG-INFO` & `h3result-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h3result
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python wrapper for h3result library.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

