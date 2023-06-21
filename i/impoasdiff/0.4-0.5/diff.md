# Comparing `tmp/impoasdiff-0.4.tar.gz` & `tmp/impoasdiff-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impoasdiff-0.4.tar", last modified: Wed Jun 21 18:11:32 2023, max compression
+gzip compressed data, was "impoasdiff-0.5.tar", last modified: Wed Jun 21 18:17:49 2023, max compression
```

## Comparing `impoasdiff-0.4.tar` & `impoasdiff-0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:11:32.285930 impoasdiff-0.4/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:11:32.285709 impoasdiff-0.4/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.4/README.md
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:11:32.281966 impoasdiff-0.4/impoasdiff.egg-info/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      297 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/SOURCES.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/dependency_links.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/requires.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       18 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/top_level.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 18:11:32.285985 impoasdiff-0.4/setup.cfg
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1003 2023-06-21 18:11:29.000000 impoasdiff-0.4/setup.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:11:32.285336 impoasdiff-0.4/src/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      306 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/__init__.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/args_manager.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/diff_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/file_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/generate_diff.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/utils.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:17:49.410260 impoasdiff-0.5/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:17:49.410071 impoasdiff-0.5/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.5/README.md
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:17:49.406587 impoasdiff-0.5/impoasdiff.egg-info/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      313 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/requires.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       18 2023-06-21 18:17:49.000000 impoasdiff-0.5/impoasdiff.egg-info/top_level.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 18:17:49.410304 impoasdiff-0.5/setup.cfg
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1003 2023-06-21 18:17:44.000000 impoasdiff-0.5/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:17:49.409779 impoasdiff-0.5/src/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      306 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/__init__.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 18:17:12.000000 impoasdiff-0.5/src/_version.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/args_manager.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/diff_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/file_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/generate_diff.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.5/src/utils.py
```

### Comparing `impoasdiff-0.4/setup.py` & `impoasdiff-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impoasdiff",
-    version=os.environ.get("VER", "0.4"),
+    version=os.environ.get("VER", "0.5"),
     author="Yash Thadani",
     author_email="yash.thadani@imperva.com",
     description="Open API diff tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     py_modules=["generate_diff"],
```

### Comparing `impoasdiff-0.4/src/args_manager.py` & `impoasdiff-0.5/src/args_manager.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.4/src/diff_handler.py` & `impoasdiff-0.5/src/diff_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.4/src/file_handler.py` & `impoasdiff-0.5/src/file_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.4/src/generate_diff.py` & `impoasdiff-0.5/src/generate_diff.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.4/src/utils.py` & `impoasdiff-0.5/src/utils.py`

 * *Files identical despite different names*

