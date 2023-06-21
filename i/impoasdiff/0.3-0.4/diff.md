# Comparing `tmp/impoasdiff-0.3.tar.gz` & `tmp/impoasdiff-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impoasdiff-0.3.tar", last modified: Wed Jun 21 17:54:47 2023, max compression
+gzip compressed data, was "impoasdiff-0.4.tar", last modified: Wed Jun 21 18:11:32 2023, max compression
```

## Comparing `impoasdiff-0.3.tar` & `impoasdiff-0.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.699797 impoasdiff-0.3/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      386 2023-06-21 17:54:47.699884 impoasdiff-0.3/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)       46 2023-06-20 18:51:42.000000 impoasdiff-0.3/README.rst
--rw-r--r--   0 yash.thadani   (503) staff       (20)      148 2023-06-21 17:54:47.700413 impoasdiff-0.3/setup.cfg
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1019 2023-06-21 17:54:43.000000 impoasdiff-0.3/setup.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.693481 impoasdiff-0.3/src/
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.695781 impoasdiff-0.3/src/imp_oasdiffgen/
--rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 08:42:31.000000 impoasdiff-0.3/src/imp_oasdiffgen/generate_diff.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.699574 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      386 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      329 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/SOURCES.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/dependency_links.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/requires.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       14 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/top_level.txt
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:11:32.285930 impoasdiff-0.4/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:11:32.285709 impoasdiff-0.4/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.4/README.md
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:11:32.281966 impoasdiff-0.4/impoasdiff.egg-info/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      422 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      297 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/requires.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       18 2023-06-21 18:11:32.000000 impoasdiff-0.4/impoasdiff.egg-info/top_level.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 18:11:32.285985 impoasdiff-0.4/setup.cfg
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1003 2023-06-21 18:11:29.000000 impoasdiff-0.4/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 18:11:32.285336 impoasdiff-0.4/src/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      306 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/__init__.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/args_manager.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/diff_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/file_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/generate_diff.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.4/src/utils.py
```

### Comparing `impoasdiff-0.3/setup.py` & `impoasdiff-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impoasdiff",
-    version=os.environ.get("VER", "0.3"),
+    version=os.environ.get("VER", "0.4"),
     author="Yash Thadani",
     author_email="yash.thadani@imperva.com",
     description="Open API diff tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     py_modules=["generate_diff"], 
-    package_dir={'':'src/imp_oasdiffgen'},
+    # package_dir={'':''},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
 
     # entry_points = {
```

### Comparing `impoasdiff-0.3/src/imp_oasdiffgen/generate_diff.py` & `impoasdiff-0.4/src/generate_diff.py`

 * *Files identical despite different names*

