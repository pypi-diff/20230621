# Comparing `tmp/logger-local-0.0.5.tar.gz` & `tmp/logger-local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-local-0.0.5.tar", last modified: Thu Jun  1 06:38:34 2023, max compression
+gzip compressed data, was "logger-local-0.0.6.tar", last modified: Wed Jun 21 11:03:51 2023, max compression
```

## Comparing `logger-local-0.0.5.tar` & `logger-local-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.261656 logger-local-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 06:38:24.000000 logger-local-0.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.257656 logger-local-0.0.5/LoggerLocalPythonPackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:24.000000 logger-local-0.0.5/LoggerLocalPythonPackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 06:38:34.261656 logger-local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-01 06:38:24.000000 logger-local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.257656 logger-local-0.0.5/logger_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 06:38:34.000000 logger-local-0.0.5/logger_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 06:38:34.261656 logger-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 06:38:24.000000 logger-local-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:38:34.257656 logger-local-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-01 06:38:24.000000 logger-local-0.0.5/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:03:51.863735 logger-local-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 11:03:42.000000 logger-local-0.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:03:51.863735 logger-local-0.0.6/LoggerLocalPythonPackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-21 11:03:42.000000 logger-local-0.0.6/LoggerLocalPythonPackage/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-21 11:03:42.000000 logger-local-0.0.6/LoggerLocalPythonPackage/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 11:03:42.000000 logger-local-0.0.6/LoggerLocalPythonPackage/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-21 11:03:42.000000 logger-local-0.0.6/LoggerLocalPythonPackage/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:03:42.000000 logger-local-0.0.6/LoggerLocalPythonPackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 11:03:51.863735 logger-local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-21 11:03:42.000000 logger-local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:03:51.863735 logger-local-0.0.6/logger_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 11:03:51.000000 logger-local-0.0.6/logger_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 11:03:51.000000 logger-local-0.0.6/logger_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:03:51.000000 logger-local-0.0.6/logger_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 11:03:51.000000 logger-local-0.0.6/logger_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:03:51.863735 logger-local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 11:03:42.000000 logger-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:03:51.863735 logger-local-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-21 11:03:42.000000 logger-local-0.0.6/tests/test_writer.py
```

### Comparing `logger-local-0.0.5/LICENSE` & `logger-local-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.5/LoggerLocalPythonPackage/LoggerService.py` & `logger-local-0.0.6/LoggerLocalPythonPackage/LoggerService.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.5/LoggerLocalPythonPackage/Writer.py` & `logger-local-0.0.6/LoggerLocalPythonPackage/Writer.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.5/PKG-INFO` & `logger-local-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.5/README.md` & `logger-local-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.5/logger_local.egg-info/PKG-INFO` & `logger-local-0.0.6/logger_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.5/setup.py` & `logger-local-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='logger-local',
-    version='0.0.5',
+    version='0.0.6',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Logger Python Local",
     long_description="This is a package for sharing common Logger function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles-zone/logger-local-python-package",
     packages=setuptools.find_packages(),
```

### Comparing `logger-local-0.0.5/tests/test_writer.py` & `logger-local-0.0.6/tests/test_writer.py`

 * *Files identical despite different names*

