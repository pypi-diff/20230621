# Comparing `tmp/BulkRenamerPy-0.1.4.tar.gz` & `tmp/BulkRenamerPy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BulkRenamerPy-0.1.4.tar", last modified: Tue Jun 20 20:26:59 2023, max compression
+gzip compressed data, was "BulkRenamerPy-0.1.5.tar", last modified: Wed Jun 21 08:38:23 2023, max compression
```

## Comparing `BulkRenamerPy-0.1.4.tar` & `BulkRenamerPy-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:26:59.284618 BulkRenamerPy-0.1.4/
--rw-r--r--   0 frost     (1000) frost     (1000)    35149 2023-06-20 05:50:54.000000 BulkRenamerPy-0.1.4/LICENSE
--rw-r--r--   0 frost     (1000) frost     (1000)     1721 2023-06-20 20:26:59.284618 BulkRenamerPy-0.1.4/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)     1090 2023-06-20 20:23:27.000000 BulkRenamerPy-0.1.4/README.md
--rw-r--r--   0 frost     (1000) frost     (1000)      908 2023-06-20 20:24:35.000000 BulkRenamerPy-0.1.4/pyproject.toml
--rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-06-20 20:26:59.284618 BulkRenamerPy-0.1.4/setup.cfg
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:26:59.284618 BulkRenamerPy-0.1.4/src/
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:26:59.284618 BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/
--rw-r--r--   0 frost     (1000) frost     (1000)     1721 2023-06-20 20:26:59.000000 BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)      357 2023-06-20 20:26:59.000000 BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/SOURCES.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-06-20 20:26:59.000000 BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/dependency_links.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       56 2023-06-20 20:26:59.000000 BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/entry_points.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       71 2023-06-20 20:26:59.000000 BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/requires.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-06-20 20:26:59.000000 BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/top_level.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.4/src/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.4/src/__main__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2780 2023-06-20 17:54:27.000000 BulkRenamerPy-0.1.4/src/bulk_rename.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:26:59.284618 BulkRenamerPy-0.1.4/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)     2283 2023-06-20 19:43:22.000000 BulkRenamerPy-0.1.4/tests/test_bulk_rename.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-21 08:38:23.961206 BulkRenamerPy-0.1.5/
+-rw-r--r--   0 frost     (1000) frost     (1000)    35149 2023-06-20 05:50:54.000000 BulkRenamerPy-0.1.5/LICENSE
+-rw-r--r--   0 frost     (1000) frost     (1000)     1721 2023-06-21 08:38:23.961206 BulkRenamerPy-0.1.5/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)     1090 2023-06-20 20:23:27.000000 BulkRenamerPy-0.1.5/README.md
+-rw-r--r--   0 frost     (1000) frost     (1000)      908 2023-06-21 08:32:39.000000 BulkRenamerPy-0.1.5/pyproject.toml
+-rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-06-21 08:38:23.961206 BulkRenamerPy-0.1.5/setup.cfg
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-21 08:38:23.961206 BulkRenamerPy-0.1.5/src/
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-21 08:38:23.961206 BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/
+-rw-r--r--   0 frost     (1000) frost     (1000)     1721 2023-06-21 08:38:23.000000 BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)      357 2023-06-21 08:38:23.000000 BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/SOURCES.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-06-21 08:38:23.000000 BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/dependency_links.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       56 2023-06-21 08:38:23.000000 BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/entry_points.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       71 2023-06-21 08:38:23.000000 BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/requires.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-06-21 08:38:23.000000 BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/top_level.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.5/src/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.5/src/__main__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2780 2023-06-20 17:54:27.000000 BulkRenamerPy-0.1.5/src/bulk_rename.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-21 08:38:23.961206 BulkRenamerPy-0.1.5/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)     2459 2023-06-21 08:35:54.000000 BulkRenamerPy-0.1.5/tests/test_bulk_rename.py
```

### Comparing `BulkRenamerPy-0.1.4/LICENSE` & `BulkRenamerPy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.4/PKG-INFO` & `BulkRenamerPy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BulkRenamerPy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple tool to bulk rename files in a directory
 Author-email: Bruno Anesio <brunohanesio@gmail.com>
 Project-URL: Homepage, https://github.com/brunoanesio/bulk-rename
 Project-URL: Bug Tracker, https://github.com/brunoanesio/bulk-rename/issues
 Keywords: bulk rename,rename,rename files
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `BulkRenamerPy-0.1.4/README.md` & `BulkRenamerPy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.4/pyproject.toml` & `BulkRenamerPy-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BulkRenamerPy"
-version = "0.1.4"
+version = "0.1.5"
 authors = [{ name = "Bruno Anesio", email = "brunohanesio@gmail.com" }]
 description = "A simple tool to bulk rename files in a directory"
 keywords = ["bulk rename", "rename", "rename files"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `BulkRenamerPy-0.1.4/src/BulkRenamerPy.egg-info/PKG-INFO` & `BulkRenamerPy-0.1.5/src/BulkRenamerPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BulkRenamerPy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple tool to bulk rename files in a directory
 Author-email: Bruno Anesio <brunohanesio@gmail.com>
 Project-URL: Homepage, https://github.com/brunoanesio/bulk-rename
 Project-URL: Bug Tracker, https://github.com/brunoanesio/bulk-rename/issues
 Keywords: bulk rename,rename,rename files
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `BulkRenamerPy-0.1.4/src/bulk_rename.py` & `BulkRenamerPy-0.1.5/src/bulk_rename.py`

 * *Files identical despite different names*

