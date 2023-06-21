# Comparing `tmp/impoasdiff-0.18.tar.gz` & `tmp/impoasdiff-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impoasdiff-0.18.tar", last modified: Wed Jun 21 20:25:36 2023, max compression
+gzip compressed data, was "impoasdiff-0.19.tar", last modified: Wed Jun 21 20:28:59 2023, max compression
```

## Comparing `impoasdiff-0.18.tar` & `impoasdiff-0.19.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:25:36.973240 impoasdiff-0.18/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      423 2023-06-21 20:25:36.973050 impoasdiff-0.18/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.18/README.md
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:25:36.969079 impoasdiff-0.18/impoasdiff/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      489 2023-06-21 19:42:52.000000 impoasdiff-0.18/impoasdiff/__init__.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 19:34:04.000000 impoasdiff-0.18/impoasdiff/_version.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.18/impoasdiff/args_manager.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.18/impoasdiff/diff_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.18/impoasdiff/file_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     4710 2023-06-21 18:23:53.000000 impoasdiff-0.18/impoasdiff/generate_diff.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:25:36.972757 impoasdiff-0.18/impoasdiff/templates/
--rw-r--r--   0 yash.thadani   (503) staff       (20)    10919 2023-06-21 18:05:33.000000 impoasdiff-0.18/impoasdiff/templates/report_v3.html
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.18/impoasdiff/utils.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:25:36.972414 impoasdiff-0.18/impoasdiff.egg-info/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      423 2023-06-21 20:25:36.000000 impoasdiff-0.18/impoasdiff.egg-info/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      398 2023-06-21 20:25:36.000000 impoasdiff-0.18/impoasdiff.egg-info/SOURCES.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 20:25:36.000000 impoasdiff-0.18/impoasdiff.egg-info/dependency_links.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 20:25:36.000000 impoasdiff-0.18/impoasdiff.egg-info/requires.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       70 2023-06-21 20:25:36.000000 impoasdiff-0.18/impoasdiff.egg-info/top_level.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 20:25:36.973345 impoasdiff-0.18/setup.cfg
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1008 2023-06-21 20:25:24.000000 impoasdiff-0.18/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:28:59.889760 impoasdiff-0.19/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      423 2023-06-21 20:28:59.889556 impoasdiff-0.19/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      125 2023-06-21 18:09:12.000000 impoasdiff-0.19/README.md
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:28:59.886747 impoasdiff-0.19/impoasdiff/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      489 2023-06-21 19:42:52.000000 impoasdiff-0.19/impoasdiff/__init__.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 19:34:04.000000 impoasdiff-0.19/impoasdiff/_version.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.19/impoasdiff/args_manager.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.19/impoasdiff/diff_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.19/impoasdiff/file_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     4777 2023-06-21 20:27:53.000000 impoasdiff-0.19/impoasdiff/generate_diff.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:28:59.889263 impoasdiff-0.19/impoasdiff/templates/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    10919 2023-06-21 18:05:33.000000 impoasdiff-0.19/impoasdiff/templates/report_v3.html
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.19/impoasdiff/utils.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-21 20:28:59.888780 impoasdiff-0.19/impoasdiff.egg-info/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      423 2023-06-21 20:28:59.000000 impoasdiff-0.19/impoasdiff.egg-info/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      398 2023-06-21 20:28:59.000000 impoasdiff-0.19/impoasdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-21 20:28:59.000000 impoasdiff-0.19/impoasdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-21 20:28:59.000000 impoasdiff-0.19/impoasdiff.egg-info/requires.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       70 2023-06-21 20:28:59.000000 impoasdiff-0.19/impoasdiff.egg-info/top_level.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-21 20:28:59.889817 impoasdiff-0.19/setup.cfg
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1008 2023-06-21 20:28:51.000000 impoasdiff-0.19/setup.py
```

### Comparing `impoasdiff-0.18/impoasdiff/args_manager.py` & `impoasdiff-0.19/impoasdiff/args_manager.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.18/impoasdiff/diff_handler.py` & `impoasdiff-0.19/impoasdiff/diff_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.18/impoasdiff/file_handler.py` & `impoasdiff-0.19/impoasdiff/file_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.18/impoasdiff/generate_diff.py` & `impoasdiff-0.19/impoasdiff/generate_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import os
 import json
 
 from file_handler import FileManager, build_file_path
 from args_manager import is_valid_args, get_argument_type
 from diff_handler import OASDiffAnalyser, scan_all_paths, _summary
 from utils import get_diff_mapping, get_src_tar_file_relative
 
@@ -31,15 +32,15 @@
             print(f"Unknown argument passed of type {arg_type}")
     else:
         print("Invalid arguments")
 
 
 def render_template(summary):
     from jinja2 import Environment, FileSystemLoader
-    env = Environment(loader=FileSystemLoader('templates/'))
+    env = Environment(loader=FileSystemLoader(os.path.abspath(os.path.join(os.path.dirname(__file__), 'templates'))))
     template = env.get_template('report_v3.html')
     rendered_template = template.render(summary)
     output_file_path = 'summary.html'
     with open(output_file_path, 'w') as file:
         file.write(rendered_template)
     print(f"Template rendered and saved to '{output_file_path}'.")
```

### Comparing `impoasdiff-0.18/impoasdiff/templates/report_v3.html` & `impoasdiff-0.19/impoasdiff/templates/report_v3.html`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.18/impoasdiff/utils.py` & `impoasdiff-0.19/impoasdiff/utils.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.18/setup.py` & `impoasdiff-0.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impoasdiff",
-    version=os.environ.get("VER", "0.18"),
+    version=os.environ.get("VER", "0.19"),
     author="Yash Thadani",
     author_email="yash.thadani@imperva.com",
     description="Open API diff tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     py_modules=["generate_diff", "file_handler", "diff_handler", "args_manager", "utils"],
```

