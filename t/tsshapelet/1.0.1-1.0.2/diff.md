# Comparing `tmp/tsshapelet-1.0.1.tar.gz` & `tmp/tsshapelet-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsshapelet-1.0.1.tar", last modified: Fri Jun 16 00:52:32 2023, max compression
+gzip compressed data, was "tsshapelet-1.0.2.tar", last modified: Wed Jun 21 14:16:44 2023, max compression
```

## Comparing `tsshapelet-1.0.1.tar` & `tsshapelet-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-16 00:52:32.656648 tsshapelet-1.0.1/
--rw-r--r--   0 grant      (501) staff       (20)     1068 2023-06-13 14:54:57.000000 tsshapelet-1.0.1/LICENSE
--rw-r--r--   0 grant      (501) staff       (20)      882 2023-06-16 00:52:32.656948 tsshapelet-1.0.1/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)     2076 2023-06-16 00:44:40.000000 tsshapelet-1.0.1/README.md
--rw-r--r--   0 grant      (501) staff       (20)       79 2023-06-16 00:52:32.658199 tsshapelet-1.0.1/setup.cfg
--rw-r--r--   0 grant      (501) staff       (20)     1014 2023-06-16 00:52:29.000000 tsshapelet-1.0.1/setup.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-16 00:52:32.653710 tsshapelet-1.0.1/tsshapelet/
--rw-r--r--   0 grant      (501) staff       (20)      109 2023-06-16 00:50:36.000000 tsshapelet-1.0.1/tsshapelet/__init__.py
--rw-r--r--   0 grant      (501) staff       (20)     2627 2023-06-13 14:54:58.000000 tsshapelet-1.0.1/tsshapelet/functions.py
--rw-r--r--   0 grant      (501) staff       (20)     5771 2023-06-13 14:54:58.000000 tsshapelet-1.0.1/tsshapelet/shapelet.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-16 00:52:32.656149 tsshapelet-1.0.1/tsshapelet.egg-info/
--rw-r--r--   0 grant      (501) staff       (20)      882 2023-06-16 00:52:32.000000 tsshapelet-1.0.1/tsshapelet.egg-info/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)      275 2023-06-16 00:52:32.000000 tsshapelet-1.0.1/tsshapelet.egg-info/SOURCES.txt
--rw-r--r--   0 grant      (501) staff       (20)        1 2023-06-16 00:52:32.000000 tsshapelet-1.0.1/tsshapelet.egg-info/dependency_links.txt
--rw-r--r--   0 grant      (501) staff       (20)       30 2023-06-16 00:52:32.000000 tsshapelet-1.0.1/tsshapelet.egg-info/requires.txt
--rw-r--r--   0 grant      (501) staff       (20)       11 2023-06-16 00:52:32.000000 tsshapelet-1.0.1/tsshapelet.egg-info/top_level.txt
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-21 14:16:44.657081 tsshapelet-1.0.2/
+-rw-r--r--   0 grant      (501) staff       (20)     1068 2023-06-13 14:54:57.000000 tsshapelet-1.0.2/LICENSE
+-rw-r--r--   0 grant      (501) staff       (20)      872 2023-06-21 14:16:44.657351 tsshapelet-1.0.2/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)     2149 2023-06-21 14:08:20.000000 tsshapelet-1.0.2/README.md
+-rw-r--r--   0 grant      (501) staff       (20)       79 2023-06-21 14:16:44.658479 tsshapelet-1.0.2/setup.cfg
+-rw-r--r--   0 grant      (501) staff       (20)     1000 2023-06-21 14:16:39.000000 tsshapelet-1.0.2/setup.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-21 14:16:44.654259 tsshapelet-1.0.2/tsshapelet/
+-rw-r--r--   0 grant      (501) staff       (20)      109 2023-06-16 00:50:36.000000 tsshapelet-1.0.2/tsshapelet/__init__.py
+-rw-r--r--   0 grant      (501) staff       (20)     2630 2023-06-21 14:05:12.000000 tsshapelet-1.0.2/tsshapelet/functions.py
+-rw-r--r--   0 grant      (501) staff       (20)     5771 2023-06-13 14:54:58.000000 tsshapelet-1.0.2/tsshapelet/shapelet.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-21 14:16:44.656498 tsshapelet-1.0.2/tsshapelet.egg-info/
+-rw-r--r--   0 grant      (501) staff       (20)      872 2023-06-21 14:16:44.000000 tsshapelet-1.0.2/tsshapelet.egg-info/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)      275 2023-06-21 14:16:44.000000 tsshapelet-1.0.2/tsshapelet.egg-info/SOURCES.txt
+-rw-r--r--   0 grant      (501) staff       (20)        1 2023-06-21 14:16:44.000000 tsshapelet-1.0.2/tsshapelet.egg-info/dependency_links.txt
+-rw-r--r--   0 grant      (501) staff       (20)       30 2023-06-21 14:16:44.000000 tsshapelet-1.0.2/tsshapelet.egg-info/requires.txt
+-rw-r--r--   0 grant      (501) staff       (20)       11 2023-06-21 14:16:44.000000 tsshapelet-1.0.2/tsshapelet.egg-info/top_level.txt
```

### Comparing `tsshapelet-1.0.1/LICENSE` & `tsshapelet-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsshapelet-1.0.1/PKG-INFO` & `tsshapelet-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tsshapelet
-Version: 1.0.1
+Version: 1.0.2
 Summary: A timeseries shapelet extraction tool for python.
 Home-page: https://github.com/gellison321/tsshapelet
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsshapelet/archive/refs/tags/1.0.1.tar.gz
-Keywords: timeseries,barycenter,shapelets,data science,data analysis
+Download-URL: https://github.com/gellison321/tsshapelet/archive/refs/tags/1.0.2.tar.gz
+Keywords: timeseries,barycenter,data science,data analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tsshapelet-1.0.1/README.md` & `tsshapelet-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 <p>
 <img alt="GitHub" src="https://img.shields.io/github/license/gellison321/tsshapelet">
 </p>
 </div>
 
 ## <p align="center"> A timeseries shapelet extraction tool for python.
 
+### <p align="center">[Install From pip](https://pypi.org/project/tsshapelet/)
+```
+$ pip install tsshapelet
+```
+
 ### **FEATURES**
 
 #### Timeseries Preprocessing
 - Moving Average Smoothing
 - Quantile Normalization
 - Interpolation (downsampling)
 - Phase Syncing
@@ -38,17 +43,17 @@
 - TSLearn
 - PeakUtils
 
 ##  <p align="center"> IMPLEMENTATION
 ### <p align="center"> [Full Implementation](https://github.com/gellison321/tsshapelet/blob/main/implementation.ipynb)
 
 ```python
+
+from tsshapelet import Shapelet, manipulations, metrics, barycenters
 import pandas as pd
-from tsshapelet.shapelet import Shapelet
-from tsshapelet.functions import manipulations, metrics, barycenters
 
 df = pd.read_csv('./data/sample_data/001_labeled.csv')
 univariate_ts_array = df['waist_vm']
 
 
 ''' Example of barycenter averaging with peak extraction '''
```

### Comparing `tsshapelet-1.0.1/setup.py` & `tsshapelet-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
   name = 'tsshapelet',
   packages = find_packages(),
-  version = '1.0.1',
+  version = '1.0.2',
   license='',
   description = 'A timeseries shapelet extraction tool for python.',
   author = 'Grant Ellison',
   author_email = 'gellison321@gmail.com',
   url = 'https://github.com/gellison321/tsshapelet',
-  download_url = 'https://github.com/gellison321/tsshapelet/archive/refs/tags/1.0.1.tar.gz',
-  keywords = ['timeseries', 'barycenter', 'shapelets', 'data science','data analysis'],
+  download_url = 'https://github.com/gellison321/tsshapelet/archive/refs/tags/1.0.2.tar.gz',
+  keywords = ['timeseries', 'barycenter', 'data science','data analysis'],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
-
     'Topic :: Software Development :: Build Tools',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
   ],
```

### Comparing `tsshapelet-1.0.1/tsshapelet/functions.py` & `tsshapelet-1.0.2/tsshapelet/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from pyts.metrics import dtw
+from tslearn.metrics import dtw
 from scipy.interpolate import interp1d
 from scipy.signal import correlate
 import peakutils
 
 ''' Array Manipulations '''
 
 def interpolate(array, length):
```

### Comparing `tsshapelet-1.0.1/tsshapelet/shapelet.py` & `tsshapelet-1.0.2/tsshapelet/shapelet.py`

 * *Files identical despite different names*

### Comparing `tsshapelet-1.0.1/tsshapelet.egg-info/PKG-INFO` & `tsshapelet-1.0.2/tsshapelet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tsshapelet
-Version: 1.0.1
+Version: 1.0.2
 Summary: A timeseries shapelet extraction tool for python.
 Home-page: https://github.com/gellison321/tsshapelet
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsshapelet/archive/refs/tags/1.0.1.tar.gz
-Keywords: timeseries,barycenter,shapelets,data science,data analysis
+Download-URL: https://github.com/gellison321/tsshapelet/archive/refs/tags/1.0.2.tar.gz
+Keywords: timeseries,barycenter,data science,data analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

