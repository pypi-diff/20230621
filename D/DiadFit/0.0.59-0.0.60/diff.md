# Comparing `tmp/DiadFit-0.0.59.tar.gz` & `tmp/DiadFit-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiadFit-0.0.59.tar", last modified: Fri May 19 22:41:59 2023, max compression
+gzip compressed data, was "DiadFit-0.0.60.tar", last modified: Wed Jun 21 02:56:01 2023, max compression
```

## Comparing `DiadFit-0.0.59.tar` & `DiadFit-0.0.60.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.802765 DiadFit-0.0.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 22:41:59.802765 DiadFit-0.0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 22:41:45.000000 DiadFit-0.0.59/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:41:59.802765 DiadFit-0.0.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-19 22:41:48.000000 DiadFit-0.0.59/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.798765 DiadFit-0.0.59/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.802765 DiadFit-0.0.59/src/DiadFit/
--rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/CO2_EOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/H2O_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/Psensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/argon_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/cosmicray_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/densimeters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/density_depth_crustal_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   162634 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/diads.py
--rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/error_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35199 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/importing_data_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    63568 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/ne_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.802765 DiadFit-0.0.59/src/DiadFit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-21 02:56:01.320636 DiadFit-0.0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 02:55:46.000000 DiadFit-0.0.60/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 02:56:01.320636 DiadFit-0.0.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-21 02:55:49.000000 DiadFit-0.0.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/src/DiadFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/CO2_EOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/CO2_in_bubble_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/H2O_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/Psensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/argon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/cosmicray_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/densimeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/density_depth_crustal_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162634 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/diads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/error_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35199 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/importing_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63568 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/ne_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/src/DiadFit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-21 02:56:01.000000 DiadFit-0.0.60/src/DiadFit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/top_level.txt
```

### Comparing `DiadFit-0.0.59/PKG-INFO` & `DiadFit-0.0.60/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.59
+Version: 0.0.60
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.59/README.md` & `DiadFit-0.0.60/README.md`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/setup.py` & `DiadFit-0.0.60/setup.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/CO2_EOS.py` & `DiadFit-0.0.60/src/DiadFit/CO2_EOS.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/H2O_fitting.py` & `DiadFit-0.0.60/src/DiadFit/H2O_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/Psensor.py` & `DiadFit-0.0.60/src/DiadFit/Psensor.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/__init__.py` & `DiadFit-0.0.60/src/DiadFit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,12 +32,14 @@
 
 # Monte Carlo Error propagation
 from DiadFit.error_propagation import *
 
 from DiadFit.density_depth_crustal_profiles import *
 from DiadFit.CO2_EOS import *
 
+from DiadFit.CO2_in_bubble_error import *
+
 # version
 from ._version import __version__
```

### Comparing `DiadFit-0.0.59/src/DiadFit/argon_lines.py` & `DiadFit-0.0.60/src/DiadFit/argon_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/cosmicray_filter.py` & `DiadFit-0.0.60/src/DiadFit/cosmicray_filter.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/densimeters.py` & `DiadFit-0.0.60/src/DiadFit/densimeters.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/density_depth_crustal_profiles.py` & `DiadFit-0.0.60/src/DiadFit/density_depth_crustal_profiles.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/diads.py` & `DiadFit-0.0.60/src/DiadFit/diads.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/error_propagation.py` & `DiadFit-0.0.60/src/DiadFit/error_propagation.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/importing_data_files.py` & `DiadFit-0.0.60/src/DiadFit/importing_data_files.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit/ne_lines.py` & `DiadFit-0.0.60/src/DiadFit/ne_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.59/src/DiadFit.egg-info/PKG-INFO` & `DiadFit-0.0.60/src/DiadFit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.59
+Version: 0.0.60
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.59/src/DiadFit.egg-info/SOURCES.txt` & `DiadFit-0.0.60/src/DiadFit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 src/DiadFit/CO2_EOS.py
+src/DiadFit/CO2_in_bubble_error.py
 src/DiadFit/H2O_fitting.py
 src/DiadFit/Psensor.py
 src/DiadFit/__init__.py
 src/DiadFit/_version.py
 src/DiadFit/argon_lines.py
 src/DiadFit/cosmicray_filter.py
 src/DiadFit/densimeters.py
```

