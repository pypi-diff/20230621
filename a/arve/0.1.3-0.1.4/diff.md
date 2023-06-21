# Comparing `tmp/arve-0.1.3.tar.gz` & `tmp/arve-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arve-0.1.3.tar", last modified: Fri May 12 14:11:21 2023, max compression
+gzip compressed data, was "arve-0.1.4.tar", last modified: Wed Jun 21 11:38:16 2023, max compression
```

## Comparing `arve-0.1.3.tar` & `arve-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,43 @@
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.949378 arve-0.1.3/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1073 2023-02-02 15:37:16.000000 arve-0.1.3/LICENSE
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      597 2023-05-12 14:11:21.948915 arve-0.1.3/PKG-INFO
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      115 2023-02-06 14:14:55.000000 arve-0.1.3/README.md
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.924071 arve-0.1.3/arve/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      251 2023-05-12 13:53:39.000000 arve-0.1.3/arve/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1827 2023-05-12 12:45:58.000000 arve-0.1.3/arve/arve.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.922104 arve-0.1.3/arve/aux_data/
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.939235 arve-0.1.3/arve/aux_data/masks/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    18615 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/A0_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    27356 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/A2_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    43308 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/A5_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    52490 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/A7_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    74648 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/F0_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    76147 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/F2_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    98242 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/F5_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   113164 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/F8_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   128904 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/G0_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   149481 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/G2_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   149481 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/G5_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   165192 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/G8_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   183696 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K0_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   200200 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K2_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   200200 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K3_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   237329 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K5_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   237329 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K7_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   235852 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/M0_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   450099 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/M2_3500-7000.csv
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   427005 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/M5_3500-7000.csv
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.941733 arve-0.1.3/arve/data/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      233 2023-05-12 12:39:33.000000 arve-0.1.3/arve/data/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1057 2023-05-12 09:58:19.000000 arve-0.1.3/arve/data/add_spec.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      872 2023-05-12 12:04:26.000000 arve-0.1.3/arve/data/add_vrad.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     4634 2023-05-12 12:56:35.000000 arve-0.1.3/arve/data/compute_vrad_ccf.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.943587 arve-0.1.3/arve/functions/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      362 2023-05-12 12:43:02.000000 arve-0.1.3/arve/functions/__init__.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      412 2023-05-12 12:10:56.000000 arve-0.1.3/arve/functions/doppler_shift.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3980 2023-05-12 12:11:07.000000 arve-0.1.3/arve/functions/gls_periodogram.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      696 2023-05-12 12:10:30.000000 arve-0.1.3/arve/functions/inverted_gaussian.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      319 2023-05-12 12:11:30.000000 arve-0.1.3/arve/functions/sptype_to_num.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.944548 arve-0.1.3/arve/planets/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       80 2023-05-12 12:43:31.000000 arve-0.1.3/arve/planets/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       81 2023-05-12 12:12:35.000000 arve-0.1.3/arve/planets/add_planet.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.948066 arve-0.1.3/arve/star/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      450 2023-05-12 12:44:13.000000 arve-0.1.3/arve/star/__init__.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     4279 2023-05-12 12:13:14.000000 arve-0.1.3/arve/star/add_vpsd_components.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     1503 2023-05-12 12:13:54.000000 arve-0.1.3/arve/star/compute_vpsd.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2946 2023-05-12 12:14:29.000000 arve-0.1.3/arve/star/fit_vpsd_coefficients.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2808 2023-05-12 12:14:54.000000 arve-0.1.3/arve/star/get_stellar_parameters.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2852 2023-05-12 12:15:31.000000 arve-0.1.3/arve/star/plot_vpsd_components.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.925800 arve-0.1.3/arve.egg-info/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      597 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/PKG-INFO
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1430 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/SOURCES.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)        1 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/dependency_links.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       51 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/requires.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)        5 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/top_level.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       38 2023-05-12 14:11:21.949519 arve-0.1.3/setup.cfg
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1101 2023-05-12 13:52:33.000000 arve-0.1.3/setup.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.181456 arve-0.1.4/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1073 2023-05-25 00:29:02.000000 arve-0.1.4/LICENSE
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      640 2023-06-21 11:38:16.180907 arve-0.1.4/PKG-INFO
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      158 2023-05-14 10:56:51.000000 arve-0.1.4/README.md
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.168206 arve-0.1.4/arve/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      196 2023-06-21 11:30:52.000000 arve-0.1.4/arve/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1144 2023-06-06 11:45:15.000000 arve-0.1.4/arve/arve.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.166178 arve-0.1.4/arve/aux_data/
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.170151 arve-0.1.4/arve/aux_data/masks/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   254106 2023-06-19 13:12:55.000000 arve-0.1.4/arve/aux_data/masks/G2.csv.zip
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.173502 arve-0.1.4/arve/data/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      635 2023-06-16 12:57:16.000000 arve-0.1.4/arve/data/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3193 2023-06-21 11:12:54.000000 arve-0.1.4/arve/data/add_data.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3371 2023-06-20 12:13:03.000000 arve-0.1.4/arve/data/compute_spec_mast.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     6983 2023-06-21 08:40:36.000000 arve-0.1.4/arve/data/compute_vrad_ccf.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     8287 2023-06-21 08:39:29.000000 arve-0.1.4/arve/data/compute_vrad_lbl.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     5448 2023-06-21 09:52:22.000000 arve-0.1.4/arve/data/get_aux_data.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.176647 arve-0.1.4/arve/functions/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      649 2023-06-06 14:55:13.000000 arve-0.1.4/arve/functions/__init__.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      512 2023-05-24 14:59:20.000000 arve-0.1.4/arve/functions/convert_air_to_vac.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      470 2023-05-24 14:56:52.000000 arve-0.1.4/arve/functions/convert_vac_to_air.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      437 2023-06-07 13:53:46.000000 arve-0.1.4/arve/functions/doppler_shift.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3980 2023-05-12 12:11:07.000000 arve-0.1.4/arve/functions/gls_periodogram.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      702 2023-06-07 16:01:02.000000 arve-0.1.4/arve/functions/inverted_gaussian.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      319 2023-05-12 12:11:30.000000 arve-0.1.4/arve/functions/sptype_to_num.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.177506 arve-0.1.4/arve/planets/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      269 2023-06-06 12:02:18.000000 arve-0.1.4/arve/planets/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       81 2023-05-12 12:12:35.000000 arve-0.1.4/arve/planets/add_planet.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.180371 arve-0.1.4/arve/star/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      792 2023-06-06 12:01:31.000000 arve-0.1.4/arve/star/__init__.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     4279 2023-05-12 12:13:14.000000 arve-0.1.4/arve/star/add_vpsd_components.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     1503 2023-05-12 12:13:54.000000 arve-0.1.4/arve/star/compute_vpsd.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2946 2023-06-06 11:49:08.000000 arve-0.1.4/arve/star/fit_vpsd_coefficients.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3126 2023-06-16 09:02:29.000000 arve-0.1.4/arve/star/get_stellar_parameters.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2852 2023-05-12 12:15:31.000000 arve-0.1.4/arve/star/plot_vpsd_components.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.169832 arve-0.1.4/arve.egg-info/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      640 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/PKG-INFO
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      860 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/SOURCES.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)        1 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/dependency_links.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       58 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/requires.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)        5 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/top_level.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       38 2023-06-21 11:38:16.181614 arve-0.1.4/setup.cfg
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1251 2023-06-21 11:32:27.000000 arve-0.1.4/setup.py
```

### Comparing `arve-0.1.3/LICENSE` & `arve-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arve-0.1.3/PKG-INFO` & `arve-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: arve
-Version: 0.1.3
+Version: 0.1.4
 Summary: Analyzing Radial Velocity Elements
 Home-page: https://github.com/almoulla/arve
 Author: Khaled Al Moulla
 Author-email: khaled.almoulla@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Logo](arve/_logo/logo.png)
+![Logo](https://github.com/almoulla/arve/blob/main/arve/_logo/logo.png)
 # ARVE ~ Analyzing Radial Velocity Elements
 
 ## Installation
 
 ```
 pip install arve
 ```
```

### Comparing `arve-0.1.3/arve/arve.py` & `arve-0.1.4/arve/arve.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,56 @@
-from   .data      import _Data_classes
-from   .functions import _Functions_classes
-from   .planets   import _Planets_classes
-from   .star      import _Star_classes
+from .data      import Data
+from .functions import Functions
+from .planets   import Planets
+from .star      import Star
 
 import gc
 import pickle
 
+from typing import Optional
+
 class ARVE:
     """ARVE main class.
     """
 
     def __init__(self):
-        self.id: str = None
-        self.data = _Data(self)
-        self.functions = _Functions(self)
-        self.planets = _Planets(self)
-        self.star = _Star(self)
-
-def load(arve:str) -> ARVE:
-    """Load ARVE object.
-
-    :param arve: ARVE file to load
-    :type arve: str
-    :return: loaded ARVE object
-    :rtype: ARVE
-    """
-
-    return pickle.load(open(arve, 'rb'))
+        self.id       : Optional[str] = None
+        self.data     : Data          = Data(self)
+        self.functions: Functions     = Functions(self)
+        self.planets  : Planets       = Planets(self)
+        self.star     : Star          = Star(self)
 
 def save(arve:ARVE) -> None:
     """Save ARVE object.
 
     :param arve: ARVE object to save
     :type arve: ARVE
     :return: None
     :rtype: None
     """
 
     return pickle.dump(arve, open(arve.id+'.arve', 'wb'))
 
+def load(arve:str) -> ARVE:
+    """Load ARVE object.
+
+    :param arve: ARVE file to load
+    :type arve: str
+    :return: loaded ARVE object
+    :rtype: ARVE
+    """
+
+    return pickle.load(open(arve, 'rb'))
+
 def delete(arve:ARVE) -> None:
     """Delete ARVE object.
 
     :param arve: ARVE object to delete
     :type arve: ARVE
     :return: None
     :rtype: None
     """
     
     del arve
     gc.collect()
     
-    return None
-
-class _Data(_Data_classes):
-    """ARVE _Data sub-class.
-    """
-
-    def __init__(self, arve):
-        self.arve = arve
-        self.spec: dict = {}
-        self.vrad: dict = {}
-
-class _Functions(_Functions_classes):
-    """ARVE _Functions sub-class.
-    """
-
-    def __init__(self, arve):
-        self.arve = arve
-
-class _Planets(_Planets_classes):
-    """ARVE _Planets sub-class.
-    """
-    
-    def __init__(self, arve):
-        self.arve = arve
-        self.parameters: dict = {}
-
-class _Star(_Star_classes):
-    """ARVE _Star sub-class.
-    """
-
-    def __init__(self, arve):
-        self.arve = arve
-        self.target: str = None
-        self.stellar_parameters: dict = {}
-        self.vpsd: dict = {}
-        self.vpsd_components: dict = {}
+    return None
```

### Comparing `arve-0.1.3/arve/functions/gls_periodogram.py` & `arve-0.1.4/arve/functions/gls_periodogram.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.3/arve/functions/inverted_gaussian.py` & `arve-0.1.4/arve/functions/inverted_gaussian.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,19 @@
         :param params: tuple with continuum, contrast, RV and FWHM
         :type params: tuple of floats
         :return: inverted Gaussian evaluated at x
         :rtype: list
         """
         
         # unpack parameters
-        continuum, contrast, RV, FWHM = params
+        continuum, contrast, vrad, fwhm = params
         
         # rename parameters
         C = continuum
         a = contrast
-        b = RV
-        c = FWHM
+        b = vrad
+        c = fwhm
         
         # scale FWHM into sigma
         c /= 2*np.sqrt(2*np.log(2))
 
-        return C - a*np.exp(-((x-b)/c)**2/2)
+        return C*(1-a*np.exp(-((x-b)/c)**2/2))
```

### Comparing `arve-0.1.3/arve/star/add_vpsd_components.py` & `arve-0.1.4/arve/star/add_vpsd_components.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.3/arve/star/compute_vpsd.py` & `arve-0.1.4/arve/star/compute_vpsd.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.3/arve/star/fit_vpsd_coefficients.py` & `arve-0.1.4/arve/star/fit_vpsd_coefficients.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.3/arve/star/get_stellar_parameters.py` & `arve-0.1.4/arve/star/get_stellar_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,39 @@
     def get_stellar_parameters(self) -> None:
         """Get spectral type from SIMBAD query and stellar parameters from main-sequence table.
 
         :return: None
         :rtype: None
         """
 
+        # initiate dictionarty with stellar parameters
+        self.stellar_parameters = {}
+
         # Sun
         if self.target == "Sun":
 
             # save stellar parameters
-            self.stellar_parameters["sptype"] = "G2"
-            self.stellar_parameters["Teff"  ] = 5770
-            self.stellar_parameters["logg"  ] = 4.4
-            self.stellar_parameters["Fe_H"  ] = 0.0
-            self.stellar_parameters["M"     ] = 1.0
-            self.stellar_parameters["R"     ] = 1.0
-            self.stellar_parameters["vsini" ] = 1.63
+            self.stellar_parameters["sptype"  ] = "G2"
+            self.stellar_parameters["vrad_sys"] = 0.0
+            self.stellar_parameters["Teff"    ] = 5770
+            self.stellar_parameters["logg"    ] = 4.4
+            self.stellar_parameters["Fe_H"    ] = 0.0
+            self.stellar_parameters["M"       ] = 1.0
+            self.stellar_parameters["R"       ] = 1.0
+            self.stellar_parameters["vsini"   ] = 1.63
 
         # other stars
         else:
 
             # get spectral type from query
             simbad = Simbad()
-            simbad.add_votable_fields("sptype")
-            self.stellar_parameters["sptype"] = simbad.query_object(self.target)["SP_TYPE"][0][:2]
+            simbad.add_votable_fields("sptype"  )
+            simbad.add_votable_fields("velocity")
+            self.stellar_parameters["sptype"  ] = simbad.query_object(self.target)["SP_TYPE"   ][0][:2]
+            self.stellar_parameters["vrad_sys"] = simbad.query_object(self.target)["RVZ_RADVEL"][0]
 
             # convert spectral types to numbers
             sptype_num       =  self.arve.functions.sptype_to_num(sptype=self.stellar_parameters["sptype"])
             sptype_num_table = [self.arve.functions.sptype_to_num(sptype=sptype) for sptype in _table["sptype"]]
 
             # interpolate and save stellar parameters from table
             for key in ["Teff", "logg", "Fe_H", "M", "R", "vsini"]:
```

### Comparing `arve-0.1.3/arve/star/plot_vpsd_components.py` & `arve-0.1.4/arve/star/plot_vpsd_components.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.3/arve.egg-info/PKG-INFO` & `arve-0.1.4/arve.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: arve
-Version: 0.1.3
+Version: 0.1.4
 Summary: Analyzing Radial Velocity Elements
 Home-page: https://github.com/almoulla/arve
 Author: Khaled Al Moulla
 Author-email: khaled.almoulla@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Logo](arve/_logo/logo.png)
+![Logo](https://github.com/almoulla/arve/blob/main/arve/_logo/logo.png)
 # ARVE ~ Analyzing Radial Velocity Elements
 
 ## Installation
 
 ```
 pip install arve
 ```
```

### Comparing `arve-0.1.3/setup.py` & `arve-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import find_packages, setup
 
-with open("README.md", "r") as file:
+with open("README.md") as file:
     long_description = file.read()
 
 setup(
     name="arve",
-    version="0.1.3",
+    version="0.1.4",
     author="Khaled Al Moulla",
     author_email="khaled.almoulla@gmail.com",
     description="Analyzing Radial Velocity Elements",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/almoulla/arve",
     license="MIT License",
     packages=find_packages(),
     install_requires=["astroquery",
                       "lmfit"     ,
                       "matplotlib",
                       "numba"     ,
                       "numpy"     ,
+                      "pandas"    ,
                       "scipy"     ,
                       "tqdm"      ,
                      ],
     classifiers=["Development Status :: 1 - Planning"    ,
                  "Intended Audience :: Science/Research" ,
                  "License :: OSI Approved :: MIT License",
                  "Programming Language :: Python :: 3"   ,
                  ],
     include_package_data=True,
-    package_data={"arve": ["aux_data/masks/*.csv"]}
+    package_data={"arve": ["aux_data/masks/*.csv.zip",
+                           "aux_data/spectra/*.csv.zip"
+                           "aux_data/tellurics/*.csv.zip"]}
 )
```

