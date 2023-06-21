# Comparing `tmp/E620py-0.9.1.tar.gz` & `tmp/E620py-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E620py-0.9.1.tar", last modified: Mon May 29 17:45:54 2023, max compression
+gzip compressed data, was "E620py-0.9.2.tar", last modified: Wed Jun 21 17:54:52 2023, max compression
```

## Comparing `E620py-0.9.1.tar` & `E620py-0.9.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 17:45:43.000000 E620py-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-29 17:45:54.638410 E620py-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-29 17:45:43.000000 E620py-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-29 17:45:43.000000 E620py-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:45:54.638410 E620py-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/src/E620py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/src/e620py/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 17:54:42.000000 E620py-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 17:54:52.263161 E620py-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 17:54:42.000000 E620py-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 17:54:42.000000 E620py-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:54:52.263161 E620py-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/src/E620py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/src/e620py/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/objects.py
```

### Comparing `E620py-0.9.1/LICENSE` & `E620py-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/PKG-INFO` & `E620py-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 0.9.1
+Version: 0.9.2
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `E620py-0.9.1/README.md` & `E620py-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/pyproject.toml` & `E620py-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/src/E620py.egg-info/PKG-INFO` & `E620py-0.9.2/src/E620py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 0.9.1
+Version: 0.9.2
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `E620py-0.9.1/src/e620py/api.py` & `E620py-0.9.2/src/e620py/api.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/src/e620py/downloader.py` & `E620py-0.9.2/src/e620py/downloader.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/src/e620py/exceptions.py` & `E620py-0.9.2/src/e620py/exceptions.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/src/e620py/file_handling.py` & `E620py-0.9.2/src/e620py/file_handling.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/src/e620py/networking.py` & `E620py-0.9.2/src/e620py/networking.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.1/src/e620py/objects.py` & `E620py-0.9.2/src/e620py/objects.py`

 * *Files identical despite different names*

