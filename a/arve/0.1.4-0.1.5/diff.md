# Comparing `tmp/arve-0.1.4.tar.gz` & `tmp/arve-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arve-0.1.4.tar", last modified: Wed Jun 21 11:38:16 2023, max compression
+gzip compressed data, was "arve-0.1.5.tar", last modified: Wed Jun 21 12:07:47 2023, max compression
```

## Comparing `arve-0.1.4.tar` & `arve-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.181456 arve-0.1.4/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1073 2023-05-25 00:29:02.000000 arve-0.1.4/LICENSE
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      640 2023-06-21 11:38:16.180907 arve-0.1.4/PKG-INFO
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      158 2023-05-14 10:56:51.000000 arve-0.1.4/README.md
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.168206 arve-0.1.4/arve/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      196 2023-06-21 11:30:52.000000 arve-0.1.4/arve/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1144 2023-06-06 11:45:15.000000 arve-0.1.4/arve/arve.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.166178 arve-0.1.4/arve/aux_data/
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.170151 arve-0.1.4/arve/aux_data/masks/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   254106 2023-06-19 13:12:55.000000 arve-0.1.4/arve/aux_data/masks/G2.csv.zip
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.173502 arve-0.1.4/arve/data/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      635 2023-06-16 12:57:16.000000 arve-0.1.4/arve/data/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3193 2023-06-21 11:12:54.000000 arve-0.1.4/arve/data/add_data.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3371 2023-06-20 12:13:03.000000 arve-0.1.4/arve/data/compute_spec_mast.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     6983 2023-06-21 08:40:36.000000 arve-0.1.4/arve/data/compute_vrad_ccf.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     8287 2023-06-21 08:39:29.000000 arve-0.1.4/arve/data/compute_vrad_lbl.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     5448 2023-06-21 09:52:22.000000 arve-0.1.4/arve/data/get_aux_data.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.176647 arve-0.1.4/arve/functions/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      649 2023-06-06 14:55:13.000000 arve-0.1.4/arve/functions/__init__.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      512 2023-05-24 14:59:20.000000 arve-0.1.4/arve/functions/convert_air_to_vac.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      470 2023-05-24 14:56:52.000000 arve-0.1.4/arve/functions/convert_vac_to_air.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      437 2023-06-07 13:53:46.000000 arve-0.1.4/arve/functions/doppler_shift.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3980 2023-05-12 12:11:07.000000 arve-0.1.4/arve/functions/gls_periodogram.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      702 2023-06-07 16:01:02.000000 arve-0.1.4/arve/functions/inverted_gaussian.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      319 2023-05-12 12:11:30.000000 arve-0.1.4/arve/functions/sptype_to_num.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.177506 arve-0.1.4/arve/planets/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      269 2023-06-06 12:02:18.000000 arve-0.1.4/arve/planets/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       81 2023-05-12 12:12:35.000000 arve-0.1.4/arve/planets/add_planet.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.180371 arve-0.1.4/arve/star/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      792 2023-06-06 12:01:31.000000 arve-0.1.4/arve/star/__init__.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     4279 2023-05-12 12:13:14.000000 arve-0.1.4/arve/star/add_vpsd_components.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     1503 2023-05-12 12:13:54.000000 arve-0.1.4/arve/star/compute_vpsd.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2946 2023-06-06 11:49:08.000000 arve-0.1.4/arve/star/fit_vpsd_coefficients.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3126 2023-06-16 09:02:29.000000 arve-0.1.4/arve/star/get_stellar_parameters.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2852 2023-05-12 12:15:31.000000 arve-0.1.4/arve/star/plot_vpsd_components.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 11:38:16.169832 arve-0.1.4/arve.egg-info/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      640 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/PKG-INFO
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      860 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/SOURCES.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)        1 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/dependency_links.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       58 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/requires.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)        5 2023-06-21 11:38:16.000000 arve-0.1.4/arve.egg-info/top_level.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       38 2023-06-21 11:38:16.181614 arve-0.1.4/setup.cfg
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1251 2023-06-21 11:32:27.000000 arve-0.1.4/setup.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.641764 arve-0.1.5/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1073 2023-05-25 00:29:02.000000 arve-0.1.5/LICENSE
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      640 2023-06-21 12:07:47.641368 arve-0.1.5/PKG-INFO
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      158 2023-05-14 10:56:51.000000 arve-0.1.5/README.md
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.596831 arve-0.1.5/arve/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      196 2023-06-21 12:05:42.000000 arve-0.1.5/arve/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1144 2023-06-06 11:45:15.000000 arve-0.1.5/arve/arve.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.595274 arve-0.1.5/arve/aux_data/
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.598846 arve-0.1.5/arve/aux_data/masks/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   254106 2023-06-19 13:12:55.000000 arve-0.1.5/arve/aux_data/masks/G2.csv.zip
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.612862 arve-0.1.5/arve/aux_data/spectra/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)  2960850 2023-06-19 12:14:29.000000 arve-0.1.5/arve/aux_data/spectra/G2.csv.zip
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   856618 2023-06-19 11:32:35.000000 arve-0.1.5/arve/aux_data/spectra/WAVE.csv.zip
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.617584 arve-0.1.5/arve/aux_data/tellurics/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3544 2023-06-19 13:19:10.000000 arve-0.1.5/arve/aux_data/tellurics/TELL.csv.zip
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.622821 arve-0.1.5/arve/data/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      635 2023-06-16 12:57:16.000000 arve-0.1.5/arve/data/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3193 2023-06-21 11:12:54.000000 arve-0.1.5/arve/data/add_data.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3371 2023-06-20 12:13:03.000000 arve-0.1.5/arve/data/compute_spec_mast.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     6983 2023-06-21 08:40:36.000000 arve-0.1.5/arve/data/compute_vrad_ccf.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     8287 2023-06-21 08:39:29.000000 arve-0.1.5/arve/data/compute_vrad_lbl.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     5448 2023-06-21 09:52:22.000000 arve-0.1.5/arve/data/get_aux_data.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.629766 arve-0.1.5/arve/functions/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      649 2023-06-06 14:55:13.000000 arve-0.1.5/arve/functions/__init__.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      512 2023-05-24 14:59:20.000000 arve-0.1.5/arve/functions/convert_air_to_vac.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      470 2023-05-24 14:56:52.000000 arve-0.1.5/arve/functions/convert_vac_to_air.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      437 2023-06-07 13:53:46.000000 arve-0.1.5/arve/functions/doppler_shift.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3980 2023-05-12 12:11:07.000000 arve-0.1.5/arve/functions/gls_periodogram.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      702 2023-06-07 16:01:02.000000 arve-0.1.5/arve/functions/inverted_gaussian.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      319 2023-05-12 12:11:30.000000 arve-0.1.5/arve/functions/sptype_to_num.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.632499 arve-0.1.5/arve/planets/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      269 2023-06-06 12:02:18.000000 arve-0.1.5/arve/planets/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       81 2023-05-12 12:12:35.000000 arve-0.1.5/arve/planets/add_planet.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.640212 arve-0.1.5/arve/star/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      792 2023-06-06 12:01:31.000000 arve-0.1.5/arve/star/__init__.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     4279 2023-05-12 12:13:14.000000 arve-0.1.5/arve/star/add_vpsd_components.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     1503 2023-05-12 12:13:54.000000 arve-0.1.5/arve/star/compute_vpsd.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2946 2023-06-06 11:49:08.000000 arve-0.1.5/arve/star/fit_vpsd_coefficients.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3126 2023-06-16 09:02:29.000000 arve-0.1.5/arve/star/get_stellar_parameters.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2852 2023-05-12 12:15:31.000000 arve-0.1.5/arve/star/plot_vpsd_components.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-06-21 12:07:47.598456 arve-0.1.5/arve.egg-info/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      640 2023-06-21 12:07:47.000000 arve-0.1.5/arve.egg-info/PKG-INFO
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      965 2023-06-21 12:07:47.000000 arve-0.1.5/arve.egg-info/SOURCES.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)        1 2023-06-21 12:07:47.000000 arve-0.1.5/arve.egg-info/dependency_links.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       58 2023-06-21 12:07:47.000000 arve-0.1.5/arve.egg-info/requires.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)        5 2023-06-21 12:07:47.000000 arve-0.1.5/arve.egg-info/top_level.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       38 2023-06-21 12:07:47.641922 arve-0.1.5/setup.cfg
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1252 2023-06-21 12:05:25.000000 arve-0.1.5/setup.py
```

### Comparing `arve-0.1.4/LICENSE` & `arve-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/PKG-INFO` & `arve-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arve
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analyzing Radial Velocity Elements
 Home-page: https://github.com/almoulla/arve
 Author: Khaled Al Moulla
 Author-email: khaled.almoulla@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `arve-0.1.4/arve/arve.py` & `arve-0.1.5/arve/arve.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/aux_data/masks/G2.csv.zip` & `arve-0.1.5/arve/aux_data/masks/G2.csv.zip`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/data/__init__.py` & `arve-0.1.5/arve/data/__init__.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/data/add_data.py` & `arve-0.1.5/arve/data/add_data.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/data/compute_spec_mast.py` & `arve-0.1.5/arve/data/compute_spec_mast.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/data/compute_vrad_ccf.py` & `arve-0.1.5/arve/data/compute_vrad_ccf.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/data/compute_vrad_lbl.py` & `arve-0.1.5/arve/data/compute_vrad_lbl.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/data/get_aux_data.py` & `arve-0.1.5/arve/data/get_aux_data.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/functions/__init__.py` & `arve-0.1.5/arve/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/functions/convert_air_to_vac.py` & `arve-0.1.5/arve/functions/convert_air_to_vac.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/functions/gls_periodogram.py` & `arve-0.1.5/arve/functions/gls_periodogram.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/functions/inverted_gaussian.py` & `arve-0.1.5/arve/functions/inverted_gaussian.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/star/__init__.py` & `arve-0.1.5/arve/star/__init__.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/star/add_vpsd_components.py` & `arve-0.1.5/arve/star/add_vpsd_components.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/star/compute_vpsd.py` & `arve-0.1.5/arve/star/compute_vpsd.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/star/fit_vpsd_coefficients.py` & `arve-0.1.5/arve/star/fit_vpsd_coefficients.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/star/get_stellar_parameters.py` & `arve-0.1.5/arve/star/get_stellar_parameters.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve/star/plot_vpsd_components.py` & `arve-0.1.5/arve/star/plot_vpsd_components.py`

 * *Files identical despite different names*

### Comparing `arve-0.1.4/arve.egg-info/PKG-INFO` & `arve-0.1.5/arve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arve
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analyzing Radial Velocity Elements
 Home-page: https://github.com/almoulla/arve
 Author: Khaled Al Moulla
 Author-email: khaled.almoulla@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `arve-0.1.4/setup.py` & `arve-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as file:
     long_description = file.read()
 
 setup(
     name="arve",
-    version="0.1.4",
+    version="0.1.5",
     author="Khaled Al Moulla",
     author_email="khaled.almoulla@gmail.com",
     description="Analyzing Radial Velocity Elements",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/almoulla/arve",
     license="MIT License",
@@ -26,10 +26,10 @@
     classifiers=["Development Status :: 1 - Planning"    ,
                  "Intended Audience :: Science/Research" ,
                  "License :: OSI Approved :: MIT License",
                  "Programming Language :: Python :: 3"   ,
                  ],
     include_package_data=True,
     package_data={"arve": ["aux_data/masks/*.csv.zip",
-                           "aux_data/spectra/*.csv.zip"
+                           "aux_data/spectra/*.csv.zip",
                            "aux_data/tellurics/*.csv.zip"]}
 )
```

