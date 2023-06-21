# Comparing `tmp/omniValidator-0.0.18.tar.gz` & `tmp/omniValidator-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniValidator-0.0.18.tar", last modified: Wed Jun 21 05:10:42 2023, max compression
+gzip compressed data, was "omniValidator-0.0.19.tar", last modified: Wed Jun 21 05:24:49 2023, max compression
```

## Comparing `omniValidator-0.0.18.tar` & `omniValidator-0.0.19.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.017459 omniValidator-0.0.18/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.18/LICENSE
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.18/MANIFEST.in
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-21 05:10:42.017459 omniValidator-0.0.18/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4236 2023-02-24 06:47:34.000000 omniValidator-0.0.18/README.md
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.18/pyproject.toml
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      139 2023-06-20 14:42:08.000000 omniValidator-0.0.18/requirements.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-06-21 05:10:42.017459 omniValidator-0.0.18/setup.cfg
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-06-20 14:43:16.000000 omniValidator-0.0.18/setup.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.009459 omniValidator-0.0.18/src/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.017459 omniValidator-0.0.18/src/omniValidator/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      163 2023-06-15 13:35:59.000000 omniValidator-0.0.18/src/omniValidator/__init__.py
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    13584 2023-06-20 13:53:36.000000 omniValidator-0.0.18/src/omniValidator/core.py
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     2647 2023-06-20 14:47:14.000000 omniValidator-0.0.18/src/omniValidator/utils.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.017459 omniValidator-0.0.18/src/omniValidator.egg-info/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      357 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/SOURCES.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/dependency_links.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       96 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/requires.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/top_level.txt
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:24:49.169277 omniValidator-0.0.19/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.19/LICENSE
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.19/MANIFEST.in
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-21 05:24:49.169277 omniValidator-0.0.19/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4236 2023-02-24 06:47:34.000000 omniValidator-0.0.19/README.md
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.19/pyproject.toml
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      139 2023-06-21 05:23:56.000000 omniValidator-0.0.19/requirements.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-06-21 05:24:49.169277 omniValidator-0.0.19/setup.cfg
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-06-21 05:23:37.000000 omniValidator-0.0.19/setup.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:24:49.161280 omniValidator-0.0.19/src/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:24:49.169277 omniValidator-0.0.19/src/omniValidator/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      163 2023-06-15 13:35:59.000000 omniValidator-0.0.19/src/omniValidator/__init__.py
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    13584 2023-06-20 13:53:36.000000 omniValidator-0.0.19/src/omniValidator/core.py
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     2647 2023-06-20 14:47:14.000000 omniValidator-0.0.19/src/omniValidator/utils.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:24:49.169277 omniValidator-0.0.19/src/omniValidator.egg-info/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-21 05:24:49.000000 omniValidator-0.0.19/src/omniValidator.egg-info/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      357 2023-06-21 05:24:49.000000 omniValidator-0.0.19/src/omniValidator.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-06-21 05:24:49.000000 omniValidator-0.0.19/src/omniValidator.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       96 2023-06-21 05:24:49.000000 omniValidator-0.0.19/src/omniValidator.egg-info/requires.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-06-21 05:24:49.000000 omniValidator-0.0.19/src/omniValidator.egg-info/top_level.txt
```

### Comparing `omniValidator-0.0.18/LICENSE` & `omniValidator-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.18/PKG-INFO` & `omniValidator-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniValidator
-Version: 0.0.18
+Version: 0.0.19
 Summary: Validator of output files for Omnibencharmk.
 Home-page: https://github.com/omnibenchmark/omniValidator
 Author: A. Sonrel
 Author-email: anthony.sonrel@uzh.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `omniValidator-0.0.18/README.md` & `omniValidator-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.18/setup.py` & `omniValidator-0.0.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     name="omniValidator",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.18",  # Required
+    version="0.0.19",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Validator of output files for Omnibencharmk.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `omniValidator-0.0.18/src/omniValidator/core.py` & `omniValidator-0.0.19/src/omniValidator/core.py`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.18/src/omniValidator/utils.py` & `omniValidator-0.0.19/src/omniValidator/utils.py`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.18/src/omniValidator.egg-info/PKG-INFO` & `omniValidator-0.0.19/src/omniValidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniValidator
-Version: 0.0.18
+Version: 0.0.19
 Summary: Validator of output files for Omnibencharmk.
 Home-page: https://github.com/omnibenchmark/omniValidator
 Author: A. Sonrel
 Author-email: anthony.sonrel@uzh.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

