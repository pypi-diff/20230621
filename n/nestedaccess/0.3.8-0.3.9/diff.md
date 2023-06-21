# Comparing `tmp/nestedaccess-0.3.8.tar.gz` & `tmp/nestedaccess-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.3.8.tar", last modified: Wed Jun 21 07:02:36 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.3.9.tar", last modified: Wed Jun 21 07:05:36 2023, max compression
```

## Comparing `nestedaccess-0.3.8.tar` & `nestedaccess-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:02:36.475431 nestedaccess-0.3.8/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.3.8/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.3.8/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 07:02:36.475183 nestedaccess-0.3.8/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:41.000000 nestedaccess-0.3.8/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:02:36.473378 nestedaccess-0.3.8/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       41 2023-06-21 05:49:21.000000 nestedaccess-0.3.8/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:00.000000 nestedaccess-0.3.8/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:02:36.474774 nestedaccess-0.3.8/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-21 07:02:36.475510 nestedaccess-0.3.8/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3482 2023-06-21 07:02:33.000000 nestedaccess-0.3.8/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:05:36.566434 nestedaccess-0.3.9/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.3.9/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.3.9/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 07:05:36.566143 nestedaccess-0.3.9/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:41.000000 nestedaccess-0.3.9/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:05:36.564370 nestedaccess-0.3.9/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-21 07:04:44.000000 nestedaccess-0.3.9/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1496 2023-06-21 07:04:48.000000 nestedaccess-0.3.9/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:05:36.565671 nestedaccess-0.3.9/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 07:05:36.000000 nestedaccess-0.3.9/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-21 07:05:36.000000 nestedaccess-0.3.9/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-21 07:05:36.000000 nestedaccess-0.3.9/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-21 07:05:36.000000 nestedaccess-0.3.9/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-21 07:05:36.566526 nestedaccess-0.3.9/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3482 2023-06-21 07:05:33.000000 nestedaccess-0.3.9/setup.py
```

### Comparing `nestedaccess-0.3.8/LICENSE` & `nestedaccess-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.3.8/PKG-INFO` & `nestedaccess-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.3.8
+Version: 0.3.9
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.3.8/README.md` & `nestedaccess-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.3.8/nestedaccess/nestedaccess.py` & `nestedaccess-0.3.9/nestedaccess/nestedaccess.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def get(data, keys, default=None):
+def nestedaccess(data, keys, default=None):
     """
     get nested data
 
     Args:
         data (dict or list): Nested data objects, which can be dictionaries or lists
         keys (list): list of keys or indices to fetch nested data
         default (any, optional): The default value, returned when the acquisition fails, the default is None
```

### Comparing `nestedaccess-0.3.8/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.3.9/nestedaccess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.3.8
+Version: 0.3.9
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.3.8/setup.py` & `nestedaccess-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.3.8"
+VERSION = "0.3.9"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
```

