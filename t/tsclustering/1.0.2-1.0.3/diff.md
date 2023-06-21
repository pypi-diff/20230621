# Comparing `tmp/tsclustering-1.0.2.tar.gz` & `tmp/tsclustering-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsclustering-1.0.2.tar", last modified: Sun Jun 18 20:01:00 2023, max compression
+gzip compressed data, was "tsclustering-1.0.3.tar", last modified: Wed Jun 21 14:14:36 2023, max compression
```

## Comparing `tsclustering-1.0.2.tar` & `tsclustering-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 20:01:00.840526 tsclustering-1.0.2/
--rw-r--r--   0 grant      (501) staff       (20)     1068 2023-06-13 14:54:38.000000 tsclustering-1.0.2/LICENSE
--rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-18 20:01:00.840987 tsclustering-1.0.2/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)     2390 2023-06-18 19:39:13.000000 tsclustering-1.0.2/README.md
--rw-r--r--   0 grant      (501) staff       (20)       79 2023-06-18 20:01:00.842609 tsclustering-1.0.2/setup.cfg
--rw-r--r--   0 grant      (501) staff       (20)     1058 2023-06-18 20:00:54.000000 tsclustering-1.0.2/setup.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 20:01:00.832950 tsclustering-1.0.2/tsclustering/
--rw-r--r--   0 grant      (501) staff       (20)       38 2023-06-18 19:38:33.000000 tsclustering-1.0.2/tsclustering/__init__.py
--rw-r--r--   0 grant      (501) staff       (20)     2406 2023-06-13 14:54:38.000000 tsclustering-1.0.2/tsclustering/functions.py
--rw-r--r--   0 grant      (501) staff       (20)     4285 2023-06-13 14:54:38.000000 tsclustering-1.0.2/tsclustering/kmeans.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 20:01:00.839462 tsclustering-1.0.2/tsclustering.egg-info/
--rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)      289 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/SOURCES.txt
--rw-r--r--   0 grant      (501) staff       (20)        1 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/dependency_links.txt
--rw-r--r--   0 grant      (501) staff       (20)       20 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/requires.txt
--rw-r--r--   0 grant      (501) staff       (20)       13 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/top_level.txt
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-21 14:14:36.372928 tsclustering-1.0.3/
+-rw-r--r--   0 grant      (501) staff       (20)     1068 2023-06-13 14:54:38.000000 tsclustering-1.0.3/LICENSE
+-rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-21 14:14:36.373184 tsclustering-1.0.3/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)     2507 2023-06-21 14:08:15.000000 tsclustering-1.0.3/README.md
+-rw-r--r--   0 grant      (501) staff       (20)       79 2023-06-21 14:14:36.373899 tsclustering-1.0.3/setup.cfg
+-rw-r--r--   0 grant      (501) staff       (20)     1058 2023-06-21 14:12:16.000000 tsclustering-1.0.3/setup.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-21 14:14:36.370416 tsclustering-1.0.3/tsclustering/
+-rw-r--r--   0 grant      (501) staff       (20)       38 2023-06-18 19:38:33.000000 tsclustering-1.0.3/tsclustering/__init__.py
+-rw-r--r--   0 grant      (501) staff       (20)     2409 2023-06-21 14:04:55.000000 tsclustering-1.0.3/tsclustering/functions.py
+-rw-r--r--   0 grant      (501) staff       (20)     4285 2023-06-13 14:54:38.000000 tsclustering-1.0.3/tsclustering/kmeans.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-21 14:14:36.372485 tsclustering-1.0.3/tsclustering.egg-info/
+-rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-21 14:14:36.000000 tsclustering-1.0.3/tsclustering.egg-info/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)      289 2023-06-21 14:14:36.000000 tsclustering-1.0.3/tsclustering.egg-info/SOURCES.txt
+-rw-r--r--   0 grant      (501) staff       (20)        1 2023-06-21 14:14:36.000000 tsclustering-1.0.3/tsclustering.egg-info/dependency_links.txt
+-rw-r--r--   0 grant      (501) staff       (20)       20 2023-06-21 14:14:36.000000 tsclustering-1.0.3/tsclustering.egg-info/requires.txt
+-rw-r--r--   0 grant      (501) staff       (20)       13 2023-06-21 14:14:36.000000 tsclustering-1.0.3/tsclustering.egg-info/top_level.txt
```

### Comparing `tsclustering-1.0.2/LICENSE` & `tsclustering-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsclustering-1.0.2/PKG-INFO` & `tsclustering-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tsclustering
-Version: 1.0.2
+Version: 1.0.3
 Summary: A clustering tool for timeseries data with temporal distortions.
 Home-page: https://github.com/gellison321/tsclustering
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.3.tar.gz
 Keywords: timeseries,barycenter,clustering,data science,data analysis,kmeans,time series clustering
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
```

### Comparing `tsclustering-1.0.2/README.md` & `tsclustering-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 <p>
 <img alt="GitHub" src="https://img.shields.io/github/license/gellison321/tsclustering">
 </p>
 </div>
 
 ## <p align="center"> A clustering tool for timeseries data with temporal distortions.
 
+### <p align="center">[Install From pip](https://pypi.org/project/tsclustering/)
+```
+$ pip install tsclustering
+```
+
 ### <p align="center"> Handling Data with Temporal Distortions
 
-KMean implemenation using DTW and interpolated averaging. This package is able to efficiently handle arrays of varied length.
+KMeans implemenation using DTW and interpolated averaging. This package is able to efficiently handle arrays of varied length.
 
 <div align="center">
 <p>
 <img alt="GitHub" src="https://github.com/gellison321/tsclustering/blob/main/data/resources/varied-length.png?raw=true" width = 75%; height = auto>
 <img alt="GitHub" src="https://github.com/gellison321/tsclustering/blob/main/data/resources/clustered-varied-length.png?raw=true" width = 75%; height = auto>
 </p>
 </div>
@@ -43,24 +48,23 @@
 - SciPy
 - TSLearn
 
 ##  <p align="center"> IMPLEMENTATION
 ### <p align="center"> [Full Implementation](https://github.com/gellison321/tsclustering/blob/main/implementation.ipynb)
 
 ```python
-import pickle
 from tsclustering import KMeans
+import pickle
 
 # Loading Example Data 
 with open('./data/sample_data/X.pickle','rb') as file:
     X = pickle.load(file)
 with open('./data/sample_data/y.pickle','rb') as file:
     y = pickle.load(file)
 
-
 # Clustering with KMeans 
 km = KMeans(k_clusters = 3, n_init = 10, max_iter = 100,
             centroids = [], metric = 'dtw', averaging = 'interpolated')
 km.fit(X)
 
 # Computing Inertia
 km.get_inertia()
```

### Comparing `tsclustering-1.0.2/setup.py` & `tsclustering-1.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
   name = 'tsclustering',
   packages = find_packages(),
-  version = '1.0.2',
+  version = '1.0.3',
   license='',
   description = 'A clustering tool for timeseries data with temporal distortions.',
   author = 'Grant Ellison',
   author_email = 'gellison321@gmail.com',
   url = 'https://github.com/gellison321/tsclustering',
-  download_url = 'https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.2.tar.gz',
+  download_url = 'https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.3.tar.gz',
   keywords = ['timeseries', 'barycenter', 'clustering', 'data science','data analysis', 'kmeans', 'time series clustering'],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
     'Operating System :: OS Independent',
```

### Comparing `tsclustering-1.0.2/tsclustering/functions.py` & `tsclustering-1.0.3/tsclustering/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from pyts.metrics import dtw
+from tslearn.metrics import dtw
 from scipy.interpolate import interp1d
 from scipy.signal import correlate
 
 ''' Array Manipulations '''
 
 def interpolate(array, length):
     if type(array) != np.array:
```

### Comparing `tsclustering-1.0.2/tsclustering/kmeans.py` & `tsclustering-1.0.3/tsclustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `tsclustering-1.0.2/tsclustering.egg-info/PKG-INFO` & `tsclustering-1.0.3/tsclustering.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tsclustering
-Version: 1.0.2
+Version: 1.0.3
 Summary: A clustering tool for timeseries data with temporal distortions.
 Home-page: https://github.com/gellison321/tsclustering
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.3.tar.gz
 Keywords: timeseries,barycenter,clustering,data science,data analysis,kmeans,time series clustering
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
```

