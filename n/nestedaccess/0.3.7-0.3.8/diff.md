# Comparing `tmp/nestedaccess-0.3.7.tar.gz` & `tmp/nestedaccess-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.3.7.tar", last modified: Wed Jun 21 05:54:08 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.3.8.tar", last modified: Wed Jun 21 07:02:36 2023, max compression
```

## Comparing `nestedaccess-0.3.7.tar` & `nestedaccess-0.3.8.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 05:54:08.737162 nestedaccess-0.3.7/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.3.7/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.3.7/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 05:54:08.736873 nestedaccess-0.3.7/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:41.000000 nestedaccess-0.3.7/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 05:54:08.736388 nestedaccess-0.3.7/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 05:54:08.000000 nestedaccess-0.3.7/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      221 2023-06-21 05:54:08.000000 nestedaccess-0.3.7/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-21 05:54:08.000000 nestedaccess-0.3.7/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-21 05:54:08.000000 nestedaccess-0.3.7/nestedaccess.egg-info/entry_points.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-21 05:54:08.000000 nestedaccess-0.3.7/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-21 05:54:08.737252 nestedaccess-0.3.7/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3479 2023-06-21 05:54:04.000000 nestedaccess-0.3.7/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:02:36.475431 nestedaccess-0.3.8/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.3.8/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.3.8/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 07:02:36.475183 nestedaccess-0.3.8/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:41.000000 nestedaccess-0.3.8/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:02:36.473378 nestedaccess-0.3.8/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       41 2023-06-21 05:49:21.000000 nestedaccess-0.3.8/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:00.000000 nestedaccess-0.3.8/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:02:36.474774 nestedaccess-0.3.8/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-21 07:02:36.000000 nestedaccess-0.3.8/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-21 07:02:36.475510 nestedaccess-0.3.8/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3482 2023-06-21 07:02:33.000000 nestedaccess-0.3.8/setup.py
```

### Comparing `nestedaccess-0.3.7/LICENSE` & `nestedaccess-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.3.7/PKG-INFO` & `nestedaccess-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.3.7
+Version: 0.3.8
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.3.7/README.md` & `nestedaccess-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.3.7/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.3.8/nestedaccess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.3.7
+Version: 0.3.8
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
```

### Comparing `nestedaccess-0.3.7/setup.py` & `nestedaccess-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.3.7"
+VERSION = "0.3.8"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
@@ -92,20 +92,20 @@
     description=DESCRIPTION,
     long_description=readme,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    py_modules=["nestedaccess"],
+    packages=find_packages(),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=[NAME],
-    entry_points={
-        "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
-    },
+    # entry_points={
+    #     "console_scripts": ["nestedaccess=nestedaccess.nestedaccess:nestedaccess"],
+    # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license=LICENSE,
     classifiers=[
         f"License :: OSI Approved :: {LICENSE} License",
         "Development Status :: 3 - Alpha",
```

