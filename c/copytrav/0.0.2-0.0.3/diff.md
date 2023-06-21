# Comparing `tmp/copytrav-0.0.2.tar.gz` & `tmp/copytrav-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copytrav-0.0.2.tar", last modified: Tue Jun 20 21:44:43 2023, max compression
+gzip compressed data, was "copytrav-0.0.3.tar", last modified: Wed Jun 21 17:42:18 2023, max compression
```

## Comparing `copytrav-0.0.2.tar` & `copytrav-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 21:44:21.000000 copytrav-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 21:44:43.078216 copytrav-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-20 21:44:21.000000 copytrav-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-20 21:44:21.000000 copytrav-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:44:43.078216 copytrav-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.074216 copytrav-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.074216 copytrav-0.0.2/src/copytrav/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.074216 copytrav-0.0.2/src/copytrav/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav/data/one/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/one/data1.rst
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/one/data1.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav/data/two/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/data2.rst
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav/data/two/even_more_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/even_more_data/data3.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/even_more_data/data3.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-20 21:44:21.000000 copytrav-0.0.2/tests/test_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 17:42:00.000000 copytrav-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-21 17:42:18.279693 copytrav-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-21 17:42:00.000000 copytrav-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-21 17:42:00.000000 copytrav-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:42:18.279693 copytrav-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.275693 copytrav-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.275693 copytrav-0.0.3/src/copytrav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.275693 copytrav-0.0.3/src/copytrav/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav/data/one/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/one/data1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/one/data1.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav/data/two/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/data2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav/data/two/even_more_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/even_more_data/data3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/even_more_data/data3.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-21 17:42:00.000000 copytrav-0.0.3/tests/test_copy.py
```

### Comparing `copytrav-0.0.2/LICENSE` & `copytrav-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `copytrav-0.0.2/README.md` & `copytrav-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `copytrav-0.0.2/pyproject.toml` & `copytrav-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "copytrav"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Owen Shepherd", email="oshepengineering@gmail.com" },
 ]
 description = "Copy traversables as directories."
+readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 
 [project.optional-dependencies]
```

### Comparing `copytrav-0.0.2/src/copytrav/__init__.py` & `copytrav-0.0.3/src/copytrav/__init__.py`

 * *Files identical despite different names*

### Comparing `copytrav-0.0.2/tests/test_copy.py` & `copytrav-0.0.3/tests/test_copy.py`

 * *Files identical despite different names*

