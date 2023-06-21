# Comparing `tmp/xdatasets-0.2.8.tar.gz` & `tmp/xdatasets-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdatasets-0.2.8.tar", last modified: Fri Jun 16 19:02:46 2023, max compression
+gzip compressed data, was "xdatasets-0.2.9.tar", last modified: Wed Jun 21 16:27:00 2023, max compression
```

## Comparing `xdatasets-0.2.8.tar` & `xdatasets-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:46.247897 xdatasets-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 19:02:42.000000 xdatasets-0.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-16 19:02:42.000000 xdatasets-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 19:02:42.000000 xdatasets-0.2.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 19:02:42.000000 xdatasets-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 19:02:42.000000 xdatasets-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-16 19:02:46.247897 xdatasets-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-16 19:02:42.000000 xdatasets-0.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 19:02:46.247897 xdatasets-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-16 19:02:42.000000 xdatasets-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:46.247897 xdatasets-0.2.8/xdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-16 19:02:42.000000 xdatasets-0.2.8/xdatasets/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:46.247897 xdatasets-0.2.8/xdatasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 19:02:46.000000 xdatasets-0.2.8/xdatasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:27:00.074075 xdatasets-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 16:26:52.000000 xdatasets-0.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-21 16:26:52.000000 xdatasets-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-21 16:26:52.000000 xdatasets-0.2.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-21 16:26:52.000000 xdatasets-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 16:26:52.000000 xdatasets-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-21 16:27:00.074075 xdatasets-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 16:26:52.000000 xdatasets-0.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-21 16:27:00.074075 xdatasets-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-21 16:26:52.000000 xdatasets-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:27:00.074075 xdatasets-0.2.9/xdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-21 16:26:52.000000 xdatasets-0.2.9/xdatasets/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:27:00.074075 xdatasets-0.2.9/xdatasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-21 16:27:00.000000 xdatasets-0.2.9/xdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-21 16:27:00.000000 xdatasets-0.2.9/xdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:27:00.000000 xdatasets-0.2.9/xdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:27:00.000000 xdatasets-0.2.9/xdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-21 16:27:00.000000 xdatasets-0.2.9/xdatasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 16:27:00.000000 xdatasets-0.2.9/xdatasets.egg-info/top_level.txt
```

### Comparing `xdatasets-0.2.8/CONTRIBUTING.rst` & `xdatasets-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/LICENSE` & `xdatasets-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/PKG-INFO` & `xdatasets-0.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.8
+Version: 0.2.9
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.8/README.rst` & `xdatasets-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/setup.py` & `xdatasets-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,10 +72,10 @@
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords=KEYWORDS,
     name=NAME,
     packages=find_packages(),
     extras_require={"dev": dev_requirements},
     url=URL,
-    version='0.2.8',
+    version='0.2.9',
     zip_safe=False,
 )
```

### Comparing `xdatasets-0.2.8/xdatasets/core.py` & `xdatasets-0.2.9/xdatasets/core.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/xdatasets/scripting.py` & `xdatasets-0.2.9/xdatasets/scripting.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/xdatasets/spatial.py` & `xdatasets-0.2.9/xdatasets/spatial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/xdatasets/temporal.py` & `xdatasets-0.2.9/xdatasets/temporal.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,12 +101,15 @@
 
 
 def minimum_duration(ds,
                      time):
 
     minimum_duration_value, unit = time['minimum_duration']
 
+    indexer = (ds.end_date - ds.start_date) > pd.to_timedelta(minimum_duration_value, unit=unit)
+    
+    if indexer.chunks is not None:
+        indexer = indexer.compute()
 
-    return ds.where(
-    (ds.end_date - ds.start_date) > pd.to_timedelta(minimum_duration_value, unit=unit), 
-    drop=True
-    )
+    return ds.where(indexer,
+                    drop=True
+                    )
```

### Comparing `xdatasets-0.2.8/xdatasets/tutorial.py` & `xdatasets-0.2.9/xdatasets/tutorial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/xdatasets/utils.py` & `xdatasets-0.2.9/xdatasets/utils.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/xdatasets/validations.py` & `xdatasets-0.2.9/xdatasets/validations.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/xdatasets/workflows.py` & `xdatasets-0.2.9/xdatasets/workflows.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.8/xdatasets.egg-info/PKG-INFO` & `xdatasets-0.2.9/xdatasets.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.8
+Version: 0.2.9
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.8/xdatasets.egg-info/requires.txt` & `xdatasets-0.2.9/xdatasets.egg-info/requires.txt`

 * *Files identical despite different names*

