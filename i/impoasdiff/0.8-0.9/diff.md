# Comparing `tmp/impoasdiff-0.8.tar.gz` & `tmp/impoasdiff-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impoasdiff-0.8.tar", last modified: Wed Jun 21 19:16:27 2023, max compression
+gzip compressed data, was "impoasdiff-0.9.tar", last modified: Wed Jun 21 19:34:21 2023, max compression
```

## Comparing `impoasdiff-0.8.tar` & `impoasdiff-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 19:16:27.023174 impoasdiff-0.8/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 19:16:27.022971 impoasdiff-0.8/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.8/README.md
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 19:16:27.019561 impoasdiff-0.8/impoasdiff.egg-info/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 19:16:26.000000 impoasdiff-0.8/impoasdiff.egg-info/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      313 2023-06-21 19:16:26.000000 impoasdiff-0.8/impoasdiff.egg-info/SOURCES.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 19:16:26.000000 impoasdiff-0.8/impoasdiff.egg-info/dependency_links.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 19:16:26.000000 impoasdiff-0.8/impoasdiff.egg-info/requires.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       63 2023-06-21 19:16:26.000000 impoasdiff-0.8/impoasdiff.egg-info/top_level.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 19:16:27.023234 impoasdiff-0.8/setup.cfg
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1060 2023-06-21 19:16:22.000000 impoasdiff-0.8/setup.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 19:16:27.022657 impoasdiff-0.8/src/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      383 2023-06-21 19:15:57.000000 impoasdiff-0.8/src/__init__.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 18:17:12.000000 impoasdiff-0.8/src/_version.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.8/src/args_manager.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.8/src/diff_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.8/src/file_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:23:53.000000 impoasdiff-0.8/src/generate_diff.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.8/src/utils.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 19:34:21.103754 impoasdiff-0.9/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 19:34:21.102782 impoasdiff-0.9/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.9/README.md
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 19:34:21.099977 impoasdiff-0.9/impoasdiff.egg-info/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 19:34:21.000000 impoasdiff-0.9/impoasdiff.egg-info/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      313 2023-06-21 19:34:21.000000 impoasdiff-0.9/impoasdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 19:34:21.000000 impoasdiff-0.9/impoasdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 19:34:21.000000 impoasdiff-0.9/impoasdiff.egg-info/requires.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       63 2023-06-21 19:34:21.000000 impoasdiff-0.9/impoasdiff.egg-info/top_level.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 19:34:21.103839 impoasdiff-0.9/setup.cfg
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1060 2023-06-21 19:34:12.000000 impoasdiff-0.9/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 19:34:21.102447 impoasdiff-0.9/src/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      412 2023-06-21 19:32:17.000000 impoasdiff-0.9/src/__init__.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 19:34:04.000000 impoasdiff-0.9/src/_version.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.9/src/args_manager.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.9/src/diff_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.9/src/file_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:23:53.000000 impoasdiff-0.9/src/generate_diff.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.9/src/utils.py
```

### Comparing `impoasdiff-0.8/setup.py` & `impoasdiff-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impoasdiff",
-    version=os.environ.get("VER", "0.8"),
+    version=os.environ.get("VER", "0.9"),
     author="Yash Thadani",
     author_email="yash.thadani@imperva.com",
     description="Open API diff tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     py_modules=["generate_diff", "file_handler", "diff_handler", "args_manager", "utils"],
```

### Comparing `impoasdiff-0.8/src/args_manager.py` & `impoasdiff-0.9/src/args_manager.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.8/src/diff_handler.py` & `impoasdiff-0.9/src/diff_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.8/src/file_handler.py` & `impoasdiff-0.9/src/file_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.8/src/generate_diff.py` & `impoasdiff-0.9/src/generate_diff.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.8/src/utils.py` & `impoasdiff-0.9/src/utils.py`

 * *Files identical despite different names*

