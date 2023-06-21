# Comparing `tmp/omniValidator-0.0.17.tar.gz` & `tmp/omniValidator-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniValidator-0.0.17.tar", last modified: Fri Jun 16 07:33:45 2023, max compression
+gzip compressed data, was "omniValidator-0.0.18.tar", last modified: Wed Jun 21 05:10:42 2023, max compression
```

## Comparing `omniValidator-0.0.17.tar` & `omniValidator-0.0.18.tar`

### file list

```diff
@@ -1,47 +1,20 @@
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.626109 omniValidator-0.0.17/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.17/LICENSE
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.17/MANIFEST.in
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-16 07:33:45.626109 omniValidator-0.0.17/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4236 2023-02-24 06:47:34.000000 omniValidator-0.0.17/README.md
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.17/pyproject.toml
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      103 2023-06-15 12:44:01.000000 omniValidator-0.0.17/requirements.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-06-16 07:33:45.626109 omniValidator-0.0.17/setup.cfg
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-06-15 13:35:10.000000 omniValidator-0.0.17/setup.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      163 2023-06-15 13:35:59.000000 omniValidator-0.0.17/src/omniValidator/__init__.py
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    13484 2023-06-15 13:34:32.000000 omniValidator-0.0.17/src/omniValidator/core.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_data/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1600 2022-12-15 13:02:07.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_method/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1549 2022-12-15 14:02:57.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1163 2022-12-15 14:03:17.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.610109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1698 2022-12-15 14:18:47.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_data/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1536 2022-12-15 14:18:29.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1447 2022-12-15 14:24:03.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_method/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1207 2022-12-16 15:05:19.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.614109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.622109 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1273 2022-12-15 14:52:01.000000 omniValidator-0.0.17/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1897 2023-05-12 08:35:05.000000 omniValidator-0.0.17/src/omniValidator/utils.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-16 07:33:45.618109 omniValidator-0.0.17/src/omniValidator.egg-info/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1051 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/SOURCES.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/dependency_links.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       61 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/requires.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-06-16 07:33:45.000000 omniValidator-0.0.17/src/omniValidator.egg-info/top_level.txt
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.017459 omniValidator-0.0.18/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.18/LICENSE
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.18/MANIFEST.in
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-21 05:10:42.017459 omniValidator-0.0.18/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4236 2023-02-24 06:47:34.000000 omniValidator-0.0.18/README.md
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.18/pyproject.toml
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      139 2023-06-20 14:42:08.000000 omniValidator-0.0.18/requirements.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-06-21 05:10:42.017459 omniValidator-0.0.18/setup.cfg
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-06-20 14:43:16.000000 omniValidator-0.0.18/setup.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.009459 omniValidator-0.0.18/src/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.017459 omniValidator-0.0.18/src/omniValidator/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      163 2023-06-15 13:35:59.000000 omniValidator-0.0.18/src/omniValidator/__init__.py
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    13584 2023-06-20 13:53:36.000000 omniValidator-0.0.18/src/omniValidator/core.py
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     2647 2023-06-20 14:47:14.000000 omniValidator-0.0.18/src/omniValidator/utils.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-06-21 05:10:42.017459 omniValidator-0.0.18/src/omniValidator.egg-info/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      357 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       96 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/requires.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-06-21 05:10:41.000000 omniValidator-0.0.18/src/omniValidator.egg-info/top_level.txt
```

### Comparing `omniValidator-0.0.17/LICENSE` & `omniValidator-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.17/PKG-INFO` & `omniValidator-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniValidator
-Version: 0.0.17
+Version: 0.0.18
 Summary: Validator of output files for Omnibencharmk.
 Home-page: https://github.com/omnibenchmark/omniValidator
 Author: A. Sonrel
 Author-email: anthony.sonrel@uzh.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `omniValidator-0.0.17/README.md` & `omniValidator-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.17/setup.py` & `omniValidator-0.0.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     name="omniValidator",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.17",  # Required
+    version="0.0.18",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Validator of output files for Omnibencharmk.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `omniValidator-0.0.17/src/omniValidator/core.py` & `omniValidator-0.0.18/src/omniValidator/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 import warnings
 from json2table import convert
 from IPython.core.display import display, HTML
 from omniValidator.utils import get_avail_keywords, get_avail_benchmarks, schema_exist
 from urllib.parse import urlparse
 import requests
 
+# Global variables for github links
+raw_github = 'https://raw.githubusercontent.com/omnibenchmark/omni_essentials/main/'
+
 class ValidationError(Exception):
      def __init__(self, value):
          self.value = value
      def __str__(self):
          return repr(self.value)
 
 
@@ -66,15 +69,15 @@
     Args: 
         benchmark: omnibenchmark name. 
         keyword: keyword associated to the project (i.e., keyword specific to 'data', 'method', etc)
         ftype: file type name. 
         github: boolean, whether to fetch the content from github. 
     """
     if github == True: 
-        schema_path = os.path.join('https://raw.githubusercontent.com/omnibenchmark/omni_essentials/main/', 'schemas', benchmark, keyword, ftype+'.json')
+        schema_path = os.path.join(raw_github, 'schemas', benchmark, keyword, ftype+'.json')
     else: 
         from omniValidator import __path__ as omni_val_path     
         schema_path = os.path.join(omni_val_path[0], 'schemas', benchmark, keyword, ftype+'.json')
     return(schema_path)
 
 
 def validate_json_file(json_input_path, json_schema_path):
@@ -116,15 +119,14 @@
         data_folder (str): path to the output files that need to be validated.
 
     Returns: 
         Raises an Exception error is an output file is missing. Else, returns True.
 
 
     """
-    from omniValidator import __path__ as omni_val_path   
 
      # args requirements
     if omni_obj is None:
         if benchmark is None and keyword is None and data_folder is None: 
             msg = " if `omni_obj` is not specified, the other arguments are required."
             raise Exception(msg)
     if data_folder is not None and omni_obj is not None: 
@@ -149,17 +151,15 @@
         else: 
             benchmark = omni_obj.benchmark_name        
 
     ## Checks validity of benchmark and keyword
     schema_exist(benchmark, keyword)
 
     ## Loads requir file
-    requir = os.path.join(omni_val_path[0], 'schemas', benchmark, keyword, 'output',  'requirements.json')
-    f = open(requir)
-    requir = json.load(f)
+    requir = read_json_file(os.path.join(raw_github, 'schemas', benchmark, keyword, 'output/requirements.json'))
 
     ## Parse requirements into regex
     requir_names = list(requir['outputs_files'].keys())
     requir_end = [requir['outputs_files'][sub]['end'] for sub in requir['outputs_files']]
     regx = [a_ + ".*" + b_ for a_, b_ in zip(requir_names, requir_end)] 
 
     ## list
@@ -202,14 +202,16 @@
                 msg = "no files associated to "+ regx[i]
                 raise Exception(msg)
 
         elif len(files_found[i]) > 1: 
             msg = "Multiple files associated to "+ regx[i] +":\n"+str(files_found[i])
             warnings.warn(msg)
     print("\nValidated! All outputs meet the requirements of '", keyword, "'\n")
+    if omni_obj is not None: 
+        print("You can now run the workflow for this omni object.")
     return True
 
 
 def validate_all(benchmark, keyword, data_folder): 
     """
     Simultaneous vadlidation of requirements and JSON files using the JSON schemas of Omnivalidator.
     
@@ -229,17 +231,15 @@
         msg = "`data_folder` or `omni_obj` are required."
         raise Exception(msg)
     if data_folder is not None: 
         msg = "both `data_folder` and `omni_obj` are provided but only 1 required. Only `omni_obj` will be used."
         warnings.warn(msg)
         
     ## Loads requir file
-    requir = os.path.join(omni_val_path[0], 'schemas', benchmark, keyword, 'output',  'requirements.json')
-    f = open(requir)
-    requir = json.load(f)
+    requir = read_json_file(os.path.join(raw_github, 'schemas', benchmark, keyword, 'output/requirements.json'))
 
     ## Parse requirements into regex
     requir_names = list(requir['outputs_files'].keys())
     requir_end = [requir['outputs_files'][sub]['end'] for sub in requir['required']]
     regx = [a_ + ".*" + b_ for a_, b_ in zip(requir_names, requir_end)] 
     requir_dict = dict(zip(requir_names, requir_end))
 
@@ -315,24 +315,25 @@
                 else:
                     msg = "File '"+ v + "' not following the requirements."
                     raise Exception(msg)
     
     return True
 
 
-def display_requirements(omni_obj=None, benchmark=None, keyword=None):
+def display_requirements(omni_obj=None, benchmark=None, keyword=None, raw_html = False):
     """
     Displays the requirements of an Omnibenchmark's module, fetched from https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas.
 
     If `omni_obj` is not specified, all other arguments should be provided. 
 
     Args: 
         omni_obj (omniObject): omni object from the omnibenchmark module
         benchmark (str):  benchmark name
         keyword (str): keyword that defines the current step of the benchmark 
+        raw_html (bool): return the html object. 
 
     Returns: 
         A parsed table of the requirements in an `IPython.core.display.HTML` object.
 
 
     """
     from omniValidator import __path__ as omni_val_path   
@@ -348,15 +349,17 @@
         if benchmark is not None: 
             msg = "both `omni_obj` and `benchmark` are provided. Using `benchmark` argument only."
             warnings.warn(msg)
         else: 
             benchmark = omni_obj.benchmark_name        
 
     ## Loads requir file
-    requir = os.path.join(omni_val_path[0], 'schemas', benchmark, keyword, 'output',  'requirements.json')
-    f = open(requir)
-    requir = json.load(f)
+    requir = read_json_file(os.path.join(raw_github, 'schemas', benchmark, keyword, 'output/requirements.json'))
+
     build_direction = "LEFT_TO_RIGHT"
     table_attributes = {"style" : "width:100%"}
     html = convert(requir, build_direction=build_direction, table_attributes=table_attributes)
-    display(HTML(html))
+    if raw_html: 
+        return(html)
+    else: 
+        display(HTML(html))
```

### Comparing `omniValidator-0.0.17/src/omniValidator.egg-info/PKG-INFO` & `omniValidator-0.0.18/src/omniValidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniValidator
-Version: 0.0.17
+Version: 0.0.18
 Summary: Validator of output files for Omnibencharmk.
 Home-page: https://github.com/omnibenchmark/omniValidator
 Author: A. Sonrel
 Author-email: anthony.sonrel@uzh.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

