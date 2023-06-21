# Comparing `tmp/impoasdiff-0.2.tar.gz` & `tmp/impoasdiff-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impoasdiff-0.2.tar", last modified: Wed Jun 21 17:14:25 2023, max compression
+gzip compressed data, was "impoasdiff-0.3.tar", last modified: Wed Jun 21 17:54:47 2023, max compression
```

## Comparing `impoasdiff-0.2.tar` & `impoasdiff-0.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:14:25.441246 impoasdiff-0.2/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      317 2023-06-21 17:14:25.441350 impoasdiff-0.2/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)       46 2023-06-20 18:51:42.000000 impoasdiff-0.2/README.rst
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:14:25.440990 impoasdiff-0.2/impoasdiff.egg-info/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      317 2023-06-21 17:14:25.000000 impoasdiff-0.2/impoasdiff.egg-info/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      235 2023-06-21 17:14:25.000000 impoasdiff-0.2/impoasdiff.egg-info/SOURCES.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 17:14:25.000000 impoasdiff-0.2/impoasdiff.egg-info/dependency_links.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       72 2023-06-21 17:14:25.000000 impoasdiff-0.2/impoasdiff.egg-info/entry_points.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 17:14:25.000000 impoasdiff-0.2/impoasdiff.egg-info/requires.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 17:14:25.000000 impoasdiff-0.2/impoasdiff.egg-info/top_level.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      148 2023-06-21 17:14:25.441908 impoasdiff-0.2/setup.cfg
--rw-r--r--   0 yash.thadani   (503) staff       (20)      933 2023-06-21 17:13:58.000000 impoasdiff-0.2/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.699797 impoasdiff-0.3/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      386 2023-06-21 17:54:47.699884 impoasdiff-0.3/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       46 2023-06-20 18:51:42.000000 impoasdiff-0.3/README.rst
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      148 2023-06-21 17:54:47.700413 impoasdiff-0.3/setup.cfg
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1019 2023-06-21 17:54:43.000000 impoasdiff-0.3/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.693481 impoasdiff-0.3/src/
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.695781 impoasdiff-0.3/src/imp_oasdiffgen/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 08:42:31.000000 impoasdiff-0.3/src/imp_oasdiffgen/generate_diff.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 17:54:47.699574 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      386 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      329 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/requires.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       14 2023-06-21 17:54:47.000000 impoasdiff-0.3/src/imp_oasdiffgen/impoasdiff.egg-info/top_level.txt
```

### Comparing `impoasdiff-0.2/setup.py` & `impoasdiff-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impoasdiff",
-    version=os.environ.get("VER", "0.2"),
+    version=os.environ.get("VER", "0.3"),
     author="Yash Thadani",
     author_email="yash.thadani@imperva.com",
     description="Open API diff tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
+    py_modules=["generate_diff"], 
+    package_dir={'':'src/imp_oasdiffgen'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
 
-    entry_points = {
-        'console_scripts':
-        ['generate_diff=src.imp_oasdiffgen.generate_diff:main']
+    # entry_points = {
+    #     'console_scripts':
+    #     ['generate_diff=src.imp_oasdiffgen.generate_diff:main']
 
-    },
+    # },
     install_requires = [
         "idna==2.10",
         "Jinja2==3.1.2",
         "macholib==1.16.2",
         "MarkupSafe==2.1.3",
         "pyinstaller==5.12.0",
         "pyinstaller-hooks-contrib==2023.3",
```

