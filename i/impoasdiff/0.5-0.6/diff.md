# Comparing `tmp/impoasdiff-0.5.tar.gz` & `tmp/impoasdiff-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impoasdiff-0.5.tar", last modified: Wed Jun 21 18:17:49 2023, max compression
+gzip compressed data, was "impoasdiff-0.6.tar", last modified: Wed Jun 21 18:56:12 2023, max compression
```

## Comparing `impoasdiff-0.5.tar` & `impoasdiff-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:17:49.410260 impoasdiff-0.5/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:17:49.410071 impoasdiff-0.5/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.5/README.md
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:17:49.406587 impoasdiff-0.5/impoasdiff.egg-info/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      313 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/SOURCES.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/dependency_links.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/requires.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       18 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/top_level.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 18:17:49.410304 impoasdiff-0.5/setup.cfg
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1003 2023-06-21 18:17:44.000000 impoasdiff-0.5/setup.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:17:49.409779 impoasdiff-0.5/src/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      306 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/__init__.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 18:17:12.000000 impoasdiff-0.5/src/_version.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/args_manager.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/diff_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/file_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/generate_diff.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/utils.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:56:12.593366 impoasdiff-0.6/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:56:12.593110 impoasdiff-0.6/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.6/README.md
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:56:12.589162 impoasdiff-0.6/impoasdiff.egg-info/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:56:12.000000 impoasdiff-0.6/impoasdiff.egg-info/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      313 2023-06-21 18:56:12.000000 impoasdiff-0.6/impoasdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 18:56:12.000000 impoasdiff-0.6/impoasdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 18:56:12.000000 impoasdiff-0.6/impoasdiff.egg-info/requires.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       63 2023-06-21 18:56:12.000000 impoasdiff-0.6/impoasdiff.egg-info/top_level.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 18:56:12.593423 impoasdiff-0.6/setup.cfg
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1060 2023-06-21 18:55:27.000000 impoasdiff-0.6/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:56:12.592665 impoasdiff-0.6/src/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      306 2023-06-21 18:05:33.000000 impoasdiff-0.6/src/__init__.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 18:17:12.000000 impoasdiff-0.6/src/_version.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.6/src/args_manager.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.6/src/diff_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.6/src/file_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:23:53.000000 impoasdiff-0.6/src/generate_diff.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.6/src/utils.py
```

### Comparing `impoasdiff-0.5/setup.py` & `impoasdiff-0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impoasdiff",
-    version=os.environ.get("VER", "0.5"),
+    version=os.environ.get("VER", "0.6"),
     author="Yash Thadani",
     author_email="yash.thadani@imperva.com",
     description="Open API diff tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    py_modules=["generate_diff"], 
+    py_modules=["generate_diff", "file_handler", "diff_handler", "args_manager", "utils"], 
     # package_dir={'':''},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
```

### Comparing `impoasdiff-0.5/src/args_manager.py` & `impoasdiff-0.6/src/args_manager.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.5/src/diff_handler.py` & `impoasdiff-0.6/src/diff_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.5/src/file_handler.py` & `impoasdiff-0.6/src/file_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.5/src/generate_diff.py` & `impoasdiff-0.6/src/generate_diff.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.5/src/utils.py` & `impoasdiff-0.6/src/utils.py`

 * *Files identical despite different names*

