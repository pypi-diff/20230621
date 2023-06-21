# Comparing `tmp/shadems-0.5.2.tar.gz` & `tmp/shadems-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadems-0.5.2.tar", max compression
+gzip compressed data, was "shadems-0.5.3.tar", max compression
```

## Comparing `shadems-0.5.2.tar` & `shadems-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    15283 2023-05-02 09:42:52.194320 shadems-0.5.2/README.md
--rwxr-xr-x   0        0        0      109 2023-05-02 09:42:52.194320 shadems-0.5.2/bin/shadems
--rw-r--r--   0        0        0     1663 2023-05-02 09:42:52.222319 shadems-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1092 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/__init__.py
--rw-r--r--   0        0        0    20832 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/__main__.py
--rw-r--r--   0        0        0     8415 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/dask_utils.py
--rw-r--r--   0        0        0    19026 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/data_mappers.py
--rw-r--r--   0        0        0    27196 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/data_plots.py
--rw-r--r--   0        0        0     6787 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/ds_ext.py
--rw-r--r--   0        0        0    26242 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/main.py
--rw-r--r--   0        0        0     8564 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/ms_info.py
--rw-r--r--   0        0        0      528 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/Makefile
--rw-r--r--   0        0        0      711 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/README.md
--rw-r--r--   0        0        0        0 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/__init__.py
--rwxr-xr-x   0        0        0     7568 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/check-shadems-functionality.sh
--rw-r--r--   0        0        0     3537 2023-05-02 09:42:52.222319 shadems-0.5.2/shade_ms/tests/test_dask_utils.py
--rw-r--r--   0        0        0    16827 1970-01-01 00:00:00.000000 shadems-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    15283 2023-06-21 16:53:29.217061 shadems-0.5.3/README.md
+-rw-r--r--   0        0        0     1323 2023-06-21 16:53:29.245060 shadems-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1078 2023-06-21 16:53:29.245060 shadems-0.5.3/shade_ms/__init__.py
+-rw-r--r--   0        0        0    20832 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/__main__.py
+-rw-r--r--   0        0        0     8415 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/dask_utils.py
+-rw-r--r--   0        0        0    19026 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/data_mappers.py
+-rw-r--r--   0        0        0    27196 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/data_plots.py
+-rw-r--r--   0        0        0     6787 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/ds_ext.py
+-rw-r--r--   0        0        0    26293 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/main.py
+-rw-r--r--   0        0        0     8564 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/ms_info.py
+-rw-r--r--   0        0        0      528 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/tests/Makefile
+-rw-r--r--   0        0        0      711 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/tests/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/tests/__init__.py
+-rwxr-xr-x   0        0        0     7568 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/tests/check-shadems-functionality.sh
+-rw-r--r--   0        0        0     3549 2023-06-21 16:53:29.249060 shadems-0.5.3/shade_ms/tests/test_dask_utils.py
+-rw-r--r--   0        0        0    16742 1970-01-01 00:00:00.000000 shadems-0.5.3/PKG-INFO
```

### Comparing `shadems-0.5.2/README.md` & `shadems-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/pyproject.toml` & `shadems-0.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shadems"
-version = "0.5.2"
+version = "0.5.3"
 description = "Rapid Measurement Set plotting with dask-ms and datashader"
 authors = ["Ian Heywood & RATT <ian.heywood@physics.ox.ac.uk>"]
 license = "GPL-2.0-only"
 homepage = "https://github.com/ratt-ru/shadeMS"
 repository = "https://github.com/ratt-ru/shadeMS"
 readme = "README.md"
 keywords = ["Astronomy", "Visualisation", "Packaging"]
@@ -17,28 +17,25 @@
         "Topic :: Scientific/Engineering :: Astronomy"
 ]
 packages = [
     { include = "shade_ms" },
 ]
 
 [tool.poetry.scripts]
-shadems = {reference = "bin/shadems", type = "file"}
+shadems = "shade_ms.main:driver"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-datashader = "*"
-dask-ms = { version = "^0.2.15", extras = ["xarray"] }
+datashader = "^0.15.0"
+dask-ms = { version = "^0.2.16", extras = ["xarray"] }
 holoviews = "^1.14.9"
 matplotlib = { version = "^3.6.0" }
 cmasher = "^1.6.3"
 future-fstrings = "^1.2.0"
 requests = "^2.27.1"
-pandas = "1.5.3" # Datashader is broken with the latest pandas
-numpy = "1.23.5" # Datashader installs the latest numpy which is in conflict with <=1.35.5 required by numba 
-dask = { extras = ["array"], version = "2022.9.1" } # Datashader installs the latest dask which is in conflict with <2023.0.0 required by dask-ms[array]
 pytest = { version = "^7.2.2", optional=true }
 pytest-flake8 = { version = "^1.1.1", optional=true }
 
 [tool.poetry.extras]
 testing = ["pytest", "pytest-flake8"]
 
 [build-system]
```

### Comparing `shadems-0.5.2/shade_ms/__init__.py` & `shadems-0.5.3/shade_ms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 
 # set default number of renderers to half the available cores
 DEFAULT_CNUM = 16
-DEFAULT_NUM_RENDERS = max(1, len(os.sched_getaffinity(0))//2)
+DEFAULT_NUM_RENDERS = max(1, os.cpu_count()//2)
 
 from .__main__ import cli, parse_plot_spec, parse_slice_spec  # noqa
 
 # create logger with 'spam_application'
 log = logging.getLogger('shadems')
 log.setLevel(logging.DEBUG)
 # create file handler which logs even debug messages
```

### Comparing `shadems-0.5.2/shade_ms/__main__.py` & `shadems-0.5.3/shade_ms/__main__.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/dask_utils.py` & `shadems-0.5.3/shade_ms/dask_utils.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/data_mappers.py` & `shadems-0.5.3/shade_ms/data_mappers.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/data_plots.py` & `shadems-0.5.3/shade_ms/data_plots.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/ds_ext.py` & `shadems-0.5.3/shade_ms/ds_ext.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/main.py` & `shadems-0.5.3/shade_ms/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,7 +569,10 @@
 
         with open(cache_file, "wt") as file:
             json.dump(minmax_cache, file, sort_keys=True, indent=4, separators=(',', ': '))
         log.info(f"Saved minmax cache to {cache_file} (disable with --no-lim-save)")
 
     log.info('Finished')
     separator()
+
+def driver():
+    main([a for a in sys.argv[1:]])
```

### Comparing `shadems-0.5.2/shade_ms/ms_info.py` & `shadems-0.5.3/shade_ms/ms_info.py`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/tests/Makefile` & `shadems-0.5.3/shade_ms/tests/Makefile`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/tests/README.md` & `shadems-0.5.3/shade_ms/tests/README.md`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/tests/check-shadems-functionality.sh` & `shadems-0.5.3/shade_ms/tests/check-shadems-functionality.sh`

 * *Files identical despite different names*

### Comparing `shadems-0.5.2/shade_ms/tests/test_dask_utils.py` & `shadems-0.5.3/shade_ms/tests/test_dask_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     assert_array_equal(df['x'].min(), data1a.min())
     assert_array_equal(df['x'].max(), data1a.max())
     assert_array_equal(df['y'].min(), data1b.min())
     assert_array_equal(df['y'].max(), data1b.max())
     assert_array_equal(df['c0'].min(), data1c.min())
     assert_array_equal(df['c0'].max(), data1c.max())
 
-    df = df.append(df)
+    df = dd.multi.concat([df, df])
 
     assert_array_equal(df['x'].min(), data1a.min())
     assert_array_equal(df['x'].max(), data1a.max())
     assert_array_equal(df['y'].min(), data1b.min())
     assert_array_equal(df['y'].max(), data1b.max())
     assert_array_equal(df['c0'].min(), data1c.min())
     assert_array_equal(df['c0'].max(), data1c.max())
```

### Comparing `shadems-0.5.2/PKG-INFO` & `shadems-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadems
-Version: 0.5.2
+Version: 0.5.3
 Summary: Rapid Measurement Set plotting with dask-ms and datashader
 Home-page: https://github.com/ratt-ru/shadeMS
 License: GPL-2.0-only
 Keywords: Astronomy,Visualisation,Packaging
 Author: Ian Heywood & RATT
 Author-email: ian.heywood@physics.ox.ac.uk
 Requires-Python: >=3.8,<4.0
@@ -17,22 +17,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Provides-Extra: testing
 Requires-Dist: cmasher (>=1.6.3,<2.0.0)
-Requires-Dist: dask-ms[xarray] (>=0.2.15,<0.3.0)
-Requires-Dist: dask[array] (==2022.9.1)
-Requires-Dist: datashader
+Requires-Dist: dask-ms[xarray] (>=0.2.16,<0.3.0)
+Requires-Dist: datashader (>=0.15.0,<0.16.0)
 Requires-Dist: future-fstrings (>=1.2.0,<2.0.0)
 Requires-Dist: holoviews (>=1.14.9,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
-Requires-Dist: numpy (==1.23.5)
-Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pytest (>=7.2.2,<8.0.0) ; extra == "testing"
 Requires-Dist: pytest-flake8 (>=1.1.1,<2.0.0) ; extra == "testing"
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Repository, https://github.com/ratt-ru/shadeMS
 Description-Content-Type: text/markdown
 
 # shadems
```

