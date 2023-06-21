# Comparing `tmp/PyPhotometry-0.0.5.tar.gz` & `tmp/PyPhotometry-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPhotometry-0.0.5.tar", last modified: Tue Jun 13 11:04:12 2023, max compression
+gzip compressed data, was "PyPhotometry-0.0.6.tar", last modified: Wed Jun 21 10:36:59 2023, max compression
```

## Comparing `PyPhotometry-0.0.5.tar` & `PyPhotometry-0.0.6.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 11:04:12.508811 PyPhotometry-0.0.5/
--rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-05 14:17:48.000000 PyPhotometry-0.0.5/LICENSE.txt
--rw-r--r--   0 jean      (1000) users      (100)    10425 2023-06-13 11:04:12.508811 PyPhotometry-0.0.5/PKG-INFO
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 11:04:12.504811 PyPhotometry-0.0.5/PyPhotometry.egg-info/
--rw-r--r--   0 jean      (1000) users      (100)    10425 2023-06-13 11:04:12.000000 PyPhotometry-0.0.5/PyPhotometry.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)     1272 2023-06-13 11:04:12.000000 PyPhotometry-0.0.5/PyPhotometry.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-13 11:04:12.000000 PyPhotometry-0.0.5/PyPhotometry.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1000) users      (100)       36 2023-06-13 11:04:12.000000 PyPhotometry-0.0.5/PyPhotometry.egg-info/requires.txt
--rw-r--r--   0 jean      (1000) users      (100)       13 2023-06-13 11:04:12.000000 PyPhotometry-0.0.5/PyPhotometry.egg-info/top_level.txt
--rw-r--r--   0 jean      (1000) users      (100)     9660 2023-06-13 11:02:41.000000 PyPhotometry-0.0.5/README.md
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 11:04:12.504811 PyPhotometry-0.0.5/data/
--rw-r--r--   0 jean      (1000) users      (100)     1391 2023-06-09 12:52:22.000000 PyPhotometry-0.0.5/data/2MASSH.txt
--rw-r--r--   0 jean      (1000) users      (100)     2421 2023-06-09 12:52:35.000000 PyPhotometry-0.0.5/data/2MASSJ.txt
--rw-r--r--   0 jean      (1000) users      (100)     1771 2023-06-09 12:52:52.000000 PyPhotometry-0.0.5/data/2MASSKs.txt
--rw-r--r--   0 jean      (1000) users      (100)      395 2023-06-09 12:54:11.000000 PyPhotometry-0.0.5/data/GalexFUV.txt
--rw-r--r--   0 jean      (1000) users      (100)      539 2023-06-09 12:53:58.000000 PyPhotometry-0.0.5/data/GalexNUV.txt
--rw-r--r--   0 jean      (1000) users      (100)     3411 2023-06-09 15:32:41.000000 PyPhotometry-0.0.5/data/Herschel_SPIRE.PLW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)     3403 2023-06-09 13:08:51.000000 PyPhotometry-0.0.5/data/Herschel_SPIRE.PMW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)     5330 2023-06-09 15:29:59.000000 PyPhotometry-0.0.5/data/Herschel_SPIRE.PSW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)      557 2022-06-28 09:30:49.000000 PyPhotometry-0.0.5/data/IRAS.100mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      562 2022-06-28 09:31:23.000000 PyPhotometry-0.0.5/data/IRAS.12mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      898 2022-06-28 09:31:43.000000 PyPhotometry-0.0.5/data/IRAS.25mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      634 2022-06-28 09:32:09.000000 PyPhotometry-0.0.5/data/IRAS.60mu.txt
--rw-------   0 jean      (1000) users      (100)      352 2023-06-09 16:11:38.000000 PyPhotometry-0.0.5/data/ListFilters.txt
--rw-------   0 jean      (1000) users      (100)     2327 2023-06-09 16:08:51.000000 PyPhotometry-0.0.5/data/SDSSg.txt
--rw-------   0 jean      (1000) users      (100)     2331 2023-06-09 16:09:13.000000 PyPhotometry-0.0.5/data/SDSSi.txt
--rw-------   0 jean      (1000) users      (100)     1975 2023-06-09 16:09:05.000000 PyPhotometry-0.0.5/data/SDSSr.txt
--rw-------   0 jean      (1000) users      (100)     1317 2023-06-09 16:08:58.000000 PyPhotometry-0.0.5/data/SDSSu.txt
--rw-------   0 jean      (1000) users      (100)     3750 2023-06-09 16:09:23.000000 PyPhotometry-0.0.5/data/SDSSz.txt
--rw-r--r--   0 jean      (1000) users      (100)     3137 2023-06-09 10:46:30.000000 PyPhotometry-0.0.5/data/WISE1.txt
--rw-r--r--   0 jean      (1000) users      (100)     3704 2023-06-09 10:46:43.000000 PyPhotometry-0.0.5/data/WISE2.txt
--rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:46:55.000000 PyPhotometry-0.0.5/data/WISE3.txt
--rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:47:05.000000 PyPhotometry-0.0.5/data/WISE4.txt
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 11:04:12.508811 PyPhotometry-0.0.5/data/calibration_stars/
--rw-------   0 jean      (1000) users      (100)    91797 2012-10-27 14:35:30.000000 PyPhotometry-0.0.5/data/calibration_stars/BD+17d4708.dat
--rw-------   0 jean      (1000) users      (100)     3957 2012-10-21 09:22:12.000000 PyPhotometry-0.0.5/data/calibration_stars/BD+17o4708.dat
--rw-------   0 jean      (1000) users      (100)     2018 2022-06-18 13:55:58.000000 PyPhotometry-0.0.5/data/calibration_stars/Filters_ReadMe.txt
--rw-r--r--   0 jean      (1000) users      (100)    61057 2022-06-16 07:14:27.000000 PyPhotometry-0.0.5/data/calibration_stars/Sun.dat
--rw-------   0 jean      (1000) users      (100)    24431 2012-10-21 08:57:22.000000 PyPhotometry-0.0.5/data/calibration_stars/Sun_LR.dat
--rw-r--r--   0 jean      (1000) users      (100)   441983 2022-06-13 11:36:36.000000 PyPhotometry-0.0.5/data/calibration_stars/VegaLR.dat
--rw-------   0 jean      (1000) users      (100)    24454 2012-10-22 16:22:29.000000 PyPhotometry-0.0.5/data/calibration_stars/VegaLR_OLD.dat
--rw-r--r--   0 jean      (1000) users      (100)   100800 2022-06-16 05:47:12.000000 PyPhotometry-0.0.5/data/calibration_stars/bd17d4708_stisnic_001.fits
--rw-------   0 jean      (1000) users      (100)    35409 2010-11-12 17:30:08.000000 PyPhotometry-0.0.5/data/calibration_stars/kp00_6000.ascii
--rw-r--r--   0 jean      (1000) users      (100)    51840 2022-06-16 06:01:27.000000 PyPhotometry-0.0.5/data/calibration_stars/sun_reference_stis_001.fits
--rw-r--r--   0 jean      (1000) users      (100)    77824 2023-06-09 20:58:36.000000 PyPhotometry-0.0.5/data/filters.db
--rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-13 11:04:12.508811 PyPhotometry-0.0.5/setup.cfg
--rw-r--r--   0 jean      (1000) users      (100)     2695 2023-06-13 09:46:13.000000 PyPhotometry-0.0.5/setup.py
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 11:04:12.504811 PyPhotometry-0.0.5/src/
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 11:04:12.508811 PyPhotometry-0.0.5/src/fortran/
--rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:58:20.000000 PyPhotometry-0.0.5/src/fortran/DataTypes.f90
--rw-r--r--   0 jean      (1000) users      (100)    17884 2023-06-13 09:40:28.000000 PyPhotometry-0.0.5/src/fortran/EvalFilters.f90
--rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyPhotometry-0.0.5/src/fortran/GaussLegendreQuadrature.f90
--rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyPhotometry-0.0.5/src/fortran/IntegralALL.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-05 14:17:48.000000 PyPhotometry-0.0.5/src/fortran/LINinterpol.f90
--rw-r--r--   0 jean      (1000) users      (100)    50092 2023-06-13 09:33:16.000000 PyPhotometry-0.0.5/src/fortran/PropFilters.f90
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 11:04:12.508811 PyPhotometry-0.0.5/src/python/
--rw-r--r--   0 jean      (1000) users      (100)    68809 2023-06-09 21:01:02.000000 PyPhotometry-0.0.5/src/python/Photometry.py
--rw-r--r--   0 jean      (1000) users      (100)        0 2023-06-09 18:01:42.000000 PyPhotometry-0.0.5/src/python/__init__.py
--rw-r--r--   0 jean      (1000) users      (100)        6 2023-06-13 11:02:09.000000 PyPhotometry-0.0.5/version.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-21 10:36:59.716946 PyPhotometry-0.0.6/
+-rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-05 14:17:48.000000 PyPhotometry-0.0.6/LICENSE.txt
+-rw-r--r--   0 jean      (1000) users      (100)       65 2023-06-20 11:24:55.000000 PyPhotometry-0.0.6/MANIFEST.in
+-rw-r--r--   0 jean      (1000) users      (100)    11096 2023-06-21 10:36:59.716946 PyPhotometry-0.0.6/PKG-INFO
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-21 10:36:59.712946 PyPhotometry-0.0.6/PyPhotometry.egg-info/
+-rw-r--r--   0 jean      (1000) users      (100)    11096 2023-06-21 10:36:59.000000 PyPhotometry-0.0.6/PyPhotometry.egg-info/PKG-INFO
+-rw-r--r--   0 jean      (1000) users      (100)     1284 2023-06-21 10:36:59.000000 PyPhotometry-0.0.6/PyPhotometry.egg-info/SOURCES.txt
+-rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-21 10:36:59.000000 PyPhotometry-0.0.6/PyPhotometry.egg-info/dependency_links.txt
+-rw-r--r--   0 jean      (1000) users      (100)       36 2023-06-21 10:36:59.000000 PyPhotometry-0.0.6/PyPhotometry.egg-info/requires.txt
+-rw-r--r--   0 jean      (1000) users      (100)       13 2023-06-21 10:36:59.000000 PyPhotometry-0.0.6/PyPhotometry.egg-info/top_level.txt
+-rw-r--r--   0 jean      (1000) users      (100)    10331 2023-06-21 10:34:13.000000 PyPhotometry-0.0.6/README.md
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-21 10:36:59.716946 PyPhotometry-0.0.6/data/
+-rw-r--r--   0 jean      (1000) users      (100)     1391 2023-06-09 12:52:22.000000 PyPhotometry-0.0.6/data/2MASSH.txt
+-rw-r--r--   0 jean      (1000) users      (100)     2421 2023-06-09 12:52:35.000000 PyPhotometry-0.0.6/data/2MASSJ.txt
+-rw-r--r--   0 jean      (1000) users      (100)     1771 2023-06-09 12:52:52.000000 PyPhotometry-0.0.6/data/2MASSKs.txt
+-rw-r--r--   0 jean      (1000) users      (100)      395 2023-06-09 12:54:11.000000 PyPhotometry-0.0.6/data/GalexFUV.txt
+-rw-r--r--   0 jean      (1000) users      (100)      539 2023-06-09 12:53:58.000000 PyPhotometry-0.0.6/data/GalexNUV.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3411 2023-06-09 15:32:41.000000 PyPhotometry-0.0.6/data/Herschel_SPIRE.PLW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3403 2023-06-09 13:08:51.000000 PyPhotometry-0.0.6/data/Herschel_SPIRE.PMW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5330 2023-06-09 15:29:59.000000 PyPhotometry-0.0.6/data/Herschel_SPIRE.PSW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)      557 2022-06-28 09:30:49.000000 PyPhotometry-0.0.6/data/IRAS.100mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      562 2022-06-28 09:31:23.000000 PyPhotometry-0.0.6/data/IRAS.12mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      898 2022-06-28 09:31:43.000000 PyPhotometry-0.0.6/data/IRAS.25mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      634 2022-06-28 09:32:09.000000 PyPhotometry-0.0.6/data/IRAS.60mu.txt
+-rw-------   0 jean      (1000) users      (100)      352 2023-06-09 16:11:38.000000 PyPhotometry-0.0.6/data/ListFilters.txt
+-rw-------   0 jean      (1000) users      (100)     2327 2023-06-09 16:08:51.000000 PyPhotometry-0.0.6/data/SDSSg.txt
+-rw-------   0 jean      (1000) users      (100)     2331 2023-06-09 16:09:13.000000 PyPhotometry-0.0.6/data/SDSSi.txt
+-rw-------   0 jean      (1000) users      (100)     1975 2023-06-09 16:09:05.000000 PyPhotometry-0.0.6/data/SDSSr.txt
+-rw-------   0 jean      (1000) users      (100)     1317 2023-06-09 16:08:58.000000 PyPhotometry-0.0.6/data/SDSSu.txt
+-rw-------   0 jean      (1000) users      (100)     3750 2023-06-09 16:09:23.000000 PyPhotometry-0.0.6/data/SDSSz.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3137 2023-06-09 10:46:30.000000 PyPhotometry-0.0.6/data/WISE1.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3704 2023-06-09 10:46:43.000000 PyPhotometry-0.0.6/data/WISE2.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:46:55.000000 PyPhotometry-0.0.6/data/WISE3.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:47:05.000000 PyPhotometry-0.0.6/data/WISE4.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-21 10:36:59.716946 PyPhotometry-0.0.6/data/calibration_stars/
+-rw-------   0 jean      (1000) users      (100)    91797 2012-10-27 14:35:30.000000 PyPhotometry-0.0.6/data/calibration_stars/BD+17d4708.dat
+-rw-------   0 jean      (1000) users      (100)     3957 2012-10-21 09:22:12.000000 PyPhotometry-0.0.6/data/calibration_stars/BD+17o4708.dat
+-rw-------   0 jean      (1000) users      (100)     2018 2022-06-18 13:55:58.000000 PyPhotometry-0.0.6/data/calibration_stars/Filters_ReadMe.txt
+-rw-r--r--   0 jean      (1000) users      (100)    61057 2022-06-16 07:14:27.000000 PyPhotometry-0.0.6/data/calibration_stars/Sun.dat
+-rw-------   0 jean      (1000) users      (100)    24431 2012-10-21 08:57:22.000000 PyPhotometry-0.0.6/data/calibration_stars/Sun_LR.dat
+-rw-r--r--   0 jean      (1000) users      (100)   441983 2022-06-13 11:36:36.000000 PyPhotometry-0.0.6/data/calibration_stars/VegaLR.dat
+-rw-------   0 jean      (1000) users      (100)    24454 2012-10-22 16:22:29.000000 PyPhotometry-0.0.6/data/calibration_stars/VegaLR_OLD.dat
+-rw-r--r--   0 jean      (1000) users      (100)   100800 2022-06-16 05:47:12.000000 PyPhotometry-0.0.6/data/calibration_stars/bd17d4708_stisnic_001.fits
+-rw-------   0 jean      (1000) users      (100)    35409 2010-11-12 17:30:08.000000 PyPhotometry-0.0.6/data/calibration_stars/kp00_6000.ascii
+-rw-r--r--   0 jean      (1000) users      (100)    51840 2022-06-16 06:01:27.000000 PyPhotometry-0.0.6/data/calibration_stars/sun_reference_stis_001.fits
+-rw-r--r--   0 jean      (1000) users      (100)    77824 2023-06-09 20:58:36.000000 PyPhotometry-0.0.6/data/filters.db
+-rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-21 10:36:59.716946 PyPhotometry-0.0.6/setup.cfg
+-rw-r--r--   0 jean      (1000) users      (100)     4089 2023-06-20 12:49:17.000000 PyPhotometry-0.0.6/setup.py
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-21 10:36:59.712946 PyPhotometry-0.0.6/src/
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-21 10:36:59.716946 PyPhotometry-0.0.6/src/fortran/
+-rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:58:20.000000 PyPhotometry-0.0.6/src/fortran/DataTypes.f90
+-rw-r--r--   0 jean      (1000) users      (100)    17884 2023-06-13 09:40:28.000000 PyPhotometry-0.0.6/src/fortran/EvalFilters.f90
+-rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyPhotometry-0.0.6/src/fortran/GaussLegendreQuadrature.f90
+-rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyPhotometry-0.0.6/src/fortran/IntegralALL.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-05 14:17:48.000000 PyPhotometry-0.0.6/src/fortran/LINinterpol.f90
+-rw-r--r--   0 jean      (1000) users      (100)    50092 2023-06-13 09:33:16.000000 PyPhotometry-0.0.6/src/fortran/PropFilters.f90
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-21 10:36:59.716946 PyPhotometry-0.0.6/src/python/
+-rw-r--r--   0 jean      (1000) users      (100)    76356 2023-06-21 10:24:31.000000 PyPhotometry-0.0.6/src/python/Photometry.py
+-rw-r--r--   0 jean      (1000) users      (100)        0 2023-06-09 18:01:42.000000 PyPhotometry-0.0.6/src/python/__init__.py
+-rw-r--r--   0 jean      (1000) users      (100)        6 2023-06-20 11:01:16.000000 PyPhotometry-0.0.6/version.txt
```

### Comparing `PyPhotometry-0.0.5/LICENSE.txt` & `PyPhotometry-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/PKG-INFO` & `PyPhotometry-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPhotometry
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.
 Home-page: https://github.com/neutrinomuon/PyPhotometry
 Download-URL: https://github.com/neutrinomuon/PyPhotometry
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 Maintainer: Jean Gomes
 Maintainer-email: antineutrinomuon@gmail.com
@@ -19,15 +19,15 @@
 
 ### PyPhotometry
 ####  Fully based on a Fortran legacy package to easily compute the photometric fluxes and magnitudes in different systems
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 github repository: <a href="https://github.com/neutrinomuon/PyPhotometry">PyPhotometry</a>
 
-last stable version: 0.0.5
+last stable version: 0.0.6
 
 © Copyright ®
 
 J.G. - Jean Gomes @ 2023
 
 <hr>
 
@@ -38,14 +38,39 @@
 
 <div align="center">
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
+#### Requirements
+
+The following packages are required to run this project:
+
+- astropy>=5.0.4
+- matplotlib>=3.7.1
+- setuptools>=61.2.0
+- SQLAlchemy>=1.4.32
+
+and pyphot may be used for comparison and tests:
+
+- pyphot>=1.4.4
+
+You can install all the required packages by running the following command:
+
+<pre>
+pip install -r requirements.txt
+</pre>
+
+Additionally, you may optionally install pyphot for testing or comparison
+purposes. 
+
+Please note that pyphot is not a mandatory requirement for running this
+project and is only recommended if you intend to test or compare with it.
+
 #### <b>RESUME</b>
 
 <strong>PyPhotometry</strong> is a Python package that builds upon a
 collection of Fortran 2003+ routines originally developed between 2003 and
 2004. These routines are the foundation of the package and can be traced back
 to that time period. The licensing details for the Fortran routines can be
 found in the LICENSE.txt file included with the package.
@@ -54,20 +79,15 @@
 fluxes and magnitudes in various photometric systems. It offers support for
 multiple magnitude systems, including the VEGA standard, the VEGA system
 proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
 (Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
 an option without any calibration.
 
 It's important to note that PyPhotometry does not include the Pyphot package
-developed by M. Fouesneau, but it can be used for comparison purposes. If you
-wish to install Pyphot for comparison, you can use the following command:
-
-<pre>
-pip install pyphot
-</pre>
+developed by M. Fouesneau, but it can be used for comparison purposes.
 
 However, it is not mandatory to install Pyphot in order to use PyPhotometry. The PyPhotometry package comes with its own set of accompanying routines that provide the necessary functionality.
 
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
 href='https://github.com/neutrinomuon/PyPhotometry/blob/main/LICENSE.txt'>LICENSE.txt</a>
 file.
 
@@ -88,14 +108,19 @@
 </pre>
 
 However, it is not necessary for the usage of this package. This package is
 meant for a comparison, but PyPhotometry legacy routines are more
 general. Accompanying there are several other routines.
 
 <hr>
+#### <b>Brief Tutorial</b>
+
+A brief tutorial can be found at <a
+href='https://github.com/neutrinomuon/PyPhotometry/blob/main/tutorials/PyPhotometry%20-%20Example%201.ipynb'>PyPhotometry
+Example1.ipynb</a>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/PyPhotometry/>PyPhotometry</a> by using pip -
 <a href='https://pypi.org/'>PyPI - The Python Package Index</a>:
```

#### html2text {}

```diff
@@ -1,63 +1,70 @@
-Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.5 Summary: PyPhotometry
+Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.6 Summary: PyPhotometry
 is a Python package based on a Fortran legacy package that allows you to
 compute photometric fluxes and magnitudes in various photometric systems. Home-
 page: https://github.com/neutrinomuon/PyPhotometry Download-URL: https://
 github.com/neutrinomuon/PyPhotometry Author: Jean Gomes Author-email:
 antineutrinomuon@gmail.com Maintainer: Jean Gomes Maintainer-email:
 antineutrinomuon@gmail.com License: UNKNOWN Keywords:
 photometry,stars,galaxies,magnitude,systems Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Fortran
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt ### PyPhotometry #### Fully based on a
 Fortran legacy package to easily compute the photometric fluxes and magnitudes
 in different systems email: [antineutrinomuon@gmail.com](mailto:
 antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt) github
-repository: PyPhotometry last stable version: 0.0.5 Â© Copyright Â® J.G. - Jean
+repository: PyPhotometry last stable version: 0.0.6 Â© Copyright Â® J.G. - Jean
 Gomes @ 2023
 ===============================================================================
 [https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
 [https://img.shields.io/pypi/pyversions/PyPhotometry][https://anaconda.org/
 neutrinomuon/PyPhotometry/badges/license.svg]
 ===============================================================================
        [https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/
                                PyPhotometry.png]
 ===============================================================================
+#### Requirements The following packages are required to run this project: -
+astropy>=5.0.4 - matplotlib>=3.7.1 - setuptools>=61.2.0 - SQLAlchemy>=1.4.32
+and pyphot may be used for comparison and tests: - pyphot>=1.4.4 You can
+install all the required packages by running the following command:
+pip install -r requirements.txt
+Additionally, you may optionally install pyphot for testing or comparison
+purposes. Please note that pyphot is not a mandatory requirement for running
+this project and is only recommended if you intend to test or compare with it.
 #### RESUME PyPhotometry is a Python package that builds upon a collection of
 Fortran 2003+ routines originally developed between 2003 and 2004. These
 routines are the foundation of the package and can be traced back to that time
 period. The licensing details for the Fortran routines can be found in the
 LICENSE.txt file included with the package. The main purpose of PyPhotometry is
 to enable the computation of photometric fluxes and magnitudes in various
 photometric systems. It offers support for multiple magnitude systems,
 including the VEGA standard, the VEGA system proposed by Bohlin and Gilland in
 2004, the AB system, the TG standard system (Thuan & Gunn), the WFPC2 system,
 the FOCA system at 2000, and also provides an option without any calibration.
 It's important to note that PyPhotometry does not include the Pyphot package
-developed by M. Fouesneau, but it can be used for comparison purposes. If you
-wish to install Pyphot for comparison, you can use the following command:
-pip install pyphot
-However, it is not mandatory to install Pyphot in order to use PyPhotometry.
-The PyPhotometry package comes with its own set of accompanying routines that
+developed by M. Fouesneau, but it can be used for comparison purposes. However,
+it is not mandatory to install Pyphot in order to use PyPhotometry. The
+PyPhotometry package comes with its own set of accompanying routines that
 provide the necessary functionality. Original Fortran 2003+ routines date back
 to 2003-2004. Read the LICENSE.txt file. PyPhotometry is a Python package based
 on a Fortran legacy package that allows you to compute photometric fluxes and
 magnitudes in various photometric systems. The package provides different
 magnitude systems, such as VEGA standard, VEGA proposed by Bohlin and Gilland
 2004, AB system, TG standard system (Thuan & Gunn), WFPC2 system, FOCA at 2000,
 and without any calibration. Pyphot from M. Fouesneau is *NOT* part of the
 distribution, but used as a comparison: https://mfouesneau.github.io/pyphot/
 index.html#package-main-content. If you want to install for comparison then:
 pip install pyphot
 However, it is not necessary for the usage of this package. This package is
 meant for a comparison, but PyPhotometry legacy routines are more general.
 Accompanying there are several other routines.
 ===============================================================================
-#### INSTALLATION You can easily install PyPhotometry by using pip - PyPI_-_The
-Python_Package_Index:
+#### Brief Tutorial A brief tutorial can be found at PyPhotometry
+Example1.ipynb #### INSTALLATION You can easily install PyPhotometry by using
+pip - PyPI_-_The_Python_Package_Index:
 pip install PyPhotometry
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
 PyPhotometry: [https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 version.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 latest_release_date.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 platforms.svg]
```

### Comparing `PyPhotometry-0.0.5/PyPhotometry.egg-info/PKG-INFO` & `PyPhotometry-0.0.6/PyPhotometry.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPhotometry
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.
 Home-page: https://github.com/neutrinomuon/PyPhotometry
 Download-URL: https://github.com/neutrinomuon/PyPhotometry
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 Maintainer: Jean Gomes
 Maintainer-email: antineutrinomuon@gmail.com
@@ -19,15 +19,15 @@
 
 ### PyPhotometry
 ####  Fully based on a Fortran legacy package to easily compute the photometric fluxes and magnitudes in different systems
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 github repository: <a href="https://github.com/neutrinomuon/PyPhotometry">PyPhotometry</a>
 
-last stable version: 0.0.5
+last stable version: 0.0.6
 
 © Copyright ®
 
 J.G. - Jean Gomes @ 2023
 
 <hr>
 
@@ -38,14 +38,39 @@
 
 <div align="center">
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
+#### Requirements
+
+The following packages are required to run this project:
+
+- astropy>=5.0.4
+- matplotlib>=3.7.1
+- setuptools>=61.2.0
+- SQLAlchemy>=1.4.32
+
+and pyphot may be used for comparison and tests:
+
+- pyphot>=1.4.4
+
+You can install all the required packages by running the following command:
+
+<pre>
+pip install -r requirements.txt
+</pre>
+
+Additionally, you may optionally install pyphot for testing or comparison
+purposes. 
+
+Please note that pyphot is not a mandatory requirement for running this
+project and is only recommended if you intend to test or compare with it.
+
 #### <b>RESUME</b>
 
 <strong>PyPhotometry</strong> is a Python package that builds upon a
 collection of Fortran 2003+ routines originally developed between 2003 and
 2004. These routines are the foundation of the package and can be traced back
 to that time period. The licensing details for the Fortran routines can be
 found in the LICENSE.txt file included with the package.
@@ -54,20 +79,15 @@
 fluxes and magnitudes in various photometric systems. It offers support for
 multiple magnitude systems, including the VEGA standard, the VEGA system
 proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
 (Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
 an option without any calibration.
 
 It's important to note that PyPhotometry does not include the Pyphot package
-developed by M. Fouesneau, but it can be used for comparison purposes. If you
-wish to install Pyphot for comparison, you can use the following command:
-
-<pre>
-pip install pyphot
-</pre>
+developed by M. Fouesneau, but it can be used for comparison purposes.
 
 However, it is not mandatory to install Pyphot in order to use PyPhotometry. The PyPhotometry package comes with its own set of accompanying routines that provide the necessary functionality.
 
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
 href='https://github.com/neutrinomuon/PyPhotometry/blob/main/LICENSE.txt'>LICENSE.txt</a>
 file.
 
@@ -88,14 +108,19 @@
 </pre>
 
 However, it is not necessary for the usage of this package. This package is
 meant for a comparison, but PyPhotometry legacy routines are more
 general. Accompanying there are several other routines.
 
 <hr>
+#### <b>Brief Tutorial</b>
+
+A brief tutorial can be found at <a
+href='https://github.com/neutrinomuon/PyPhotometry/blob/main/tutorials/PyPhotometry%20-%20Example%201.ipynb'>PyPhotometry
+Example1.ipynb</a>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/PyPhotometry/>PyPhotometry</a> by using pip -
 <a href='https://pypi.org/'>PyPI - The Python Package Index</a>:
```

#### html2text {}

```diff
@@ -1,63 +1,70 @@
-Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.5 Summary: PyPhotometry
+Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.6 Summary: PyPhotometry
 is a Python package based on a Fortran legacy package that allows you to
 compute photometric fluxes and magnitudes in various photometric systems. Home-
 page: https://github.com/neutrinomuon/PyPhotometry Download-URL: https://
 github.com/neutrinomuon/PyPhotometry Author: Jean Gomes Author-email:
 antineutrinomuon@gmail.com Maintainer: Jean Gomes Maintainer-email:
 antineutrinomuon@gmail.com License: UNKNOWN Keywords:
 photometry,stars,galaxies,magnitude,systems Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Fortran
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt ### PyPhotometry #### Fully based on a
 Fortran legacy package to easily compute the photometric fluxes and magnitudes
 in different systems email: [antineutrinomuon@gmail.com](mailto:
 antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt) github
-repository: PyPhotometry last stable version: 0.0.5 Â© Copyright Â® J.G. - Jean
+repository: PyPhotometry last stable version: 0.0.6 Â© Copyright Â® J.G. - Jean
 Gomes @ 2023
 ===============================================================================
 [https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
 [https://img.shields.io/pypi/pyversions/PyPhotometry][https://anaconda.org/
 neutrinomuon/PyPhotometry/badges/license.svg]
 ===============================================================================
        [https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/
                                PyPhotometry.png]
 ===============================================================================
+#### Requirements The following packages are required to run this project: -
+astropy>=5.0.4 - matplotlib>=3.7.1 - setuptools>=61.2.0 - SQLAlchemy>=1.4.32
+and pyphot may be used for comparison and tests: - pyphot>=1.4.4 You can
+install all the required packages by running the following command:
+pip install -r requirements.txt
+Additionally, you may optionally install pyphot for testing or comparison
+purposes. Please note that pyphot is not a mandatory requirement for running
+this project and is only recommended if you intend to test or compare with it.
 #### RESUME PyPhotometry is a Python package that builds upon a collection of
 Fortran 2003+ routines originally developed between 2003 and 2004. These
 routines are the foundation of the package and can be traced back to that time
 period. The licensing details for the Fortran routines can be found in the
 LICENSE.txt file included with the package. The main purpose of PyPhotometry is
 to enable the computation of photometric fluxes and magnitudes in various
 photometric systems. It offers support for multiple magnitude systems,
 including the VEGA standard, the VEGA system proposed by Bohlin and Gilland in
 2004, the AB system, the TG standard system (Thuan & Gunn), the WFPC2 system,
 the FOCA system at 2000, and also provides an option without any calibration.
 It's important to note that PyPhotometry does not include the Pyphot package
-developed by M. Fouesneau, but it can be used for comparison purposes. If you
-wish to install Pyphot for comparison, you can use the following command:
-pip install pyphot
-However, it is not mandatory to install Pyphot in order to use PyPhotometry.
-The PyPhotometry package comes with its own set of accompanying routines that
+developed by M. Fouesneau, but it can be used for comparison purposes. However,
+it is not mandatory to install Pyphot in order to use PyPhotometry. The
+PyPhotometry package comes with its own set of accompanying routines that
 provide the necessary functionality. Original Fortran 2003+ routines date back
 to 2003-2004. Read the LICENSE.txt file. PyPhotometry is a Python package based
 on a Fortran legacy package that allows you to compute photometric fluxes and
 magnitudes in various photometric systems. The package provides different
 magnitude systems, such as VEGA standard, VEGA proposed by Bohlin and Gilland
 2004, AB system, TG standard system (Thuan & Gunn), WFPC2 system, FOCA at 2000,
 and without any calibration. Pyphot from M. Fouesneau is *NOT* part of the
 distribution, but used as a comparison: https://mfouesneau.github.io/pyphot/
 index.html#package-main-content. If you want to install for comparison then:
 pip install pyphot
 However, it is not necessary for the usage of this package. This package is
 meant for a comparison, but PyPhotometry legacy routines are more general.
 Accompanying there are several other routines.
 ===============================================================================
-#### INSTALLATION You can easily install PyPhotometry by using pip - PyPI_-_The
-Python_Package_Index:
+#### Brief Tutorial A brief tutorial can be found at PyPhotometry
+Example1.ipynb #### INSTALLATION You can easily install PyPhotometry by using
+pip - PyPI_-_The_Python_Package_Index:
 pip install PyPhotometry
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
 PyPhotometry: [https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 version.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 latest_release_date.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 platforms.svg]
```

### Comparing `PyPhotometry-0.0.5/PyPhotometry.egg-info/SOURCES.txt` & `PyPhotometry-0.0.6/PyPhotometry.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.txt
+MANIFEST.in
 README.md
 setup.py
 version.txt
 PyPhotometry.egg-info/PKG-INFO
 PyPhotometry.egg-info/SOURCES.txt
 PyPhotometry.egg-info/dependency_links.txt
 PyPhotometry.egg-info/requires.txt
```

### Comparing `PyPhotometry-0.0.5/README.md` & `PyPhotometry-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ### PyPhotometry
 ####  Fully based on a Fortran legacy package to easily compute the photometric fluxes and magnitudes in different systems
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 github repository: <a href="https://github.com/neutrinomuon/PyPhotometry">PyPhotometry</a>
 
-last stable version: 0.0.5
+last stable version: 0.0.6
 
 © Copyright ®
 
 J.G. - Jean Gomes @ 2023
 
 <hr>
 
@@ -19,14 +19,39 @@
 
 <div align="center">
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
+#### Requirements
+
+The following packages are required to run this project:
+
+- astropy>=5.0.4
+- matplotlib>=3.7.1
+- setuptools>=61.2.0
+- SQLAlchemy>=1.4.32
+
+and pyphot may be used for comparison and tests:
+
+- pyphot>=1.4.4
+
+You can install all the required packages by running the following command:
+
+<pre>
+pip install -r requirements.txt
+</pre>
+
+Additionally, you may optionally install pyphot for testing or comparison
+purposes. 
+
+Please note that pyphot is not a mandatory requirement for running this
+project and is only recommended if you intend to test or compare with it.
+
 #### <b>RESUME</b>
 
 <strong>PyPhotometry</strong> is a Python package that builds upon a
 collection of Fortran 2003+ routines originally developed between 2003 and
 2004. These routines are the foundation of the package and can be traced back
 to that time period. The licensing details for the Fortran routines can be
 found in the LICENSE.txt file included with the package.
@@ -35,20 +60,15 @@
 fluxes and magnitudes in various photometric systems. It offers support for
 multiple magnitude systems, including the VEGA standard, the VEGA system
 proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
 (Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
 an option without any calibration.
 
 It's important to note that PyPhotometry does not include the Pyphot package
-developed by M. Fouesneau, but it can be used for comparison purposes. If you
-wish to install Pyphot for comparison, you can use the following command:
-
-<pre>
-pip install pyphot
-</pre>
+developed by M. Fouesneau, but it can be used for comparison purposes.
 
 However, it is not mandatory to install Pyphot in order to use PyPhotometry. The PyPhotometry package comes with its own set of accompanying routines that provide the necessary functionality.
 
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
 href='https://github.com/neutrinomuon/PyPhotometry/blob/main/LICENSE.txt'>LICENSE.txt</a>
 file.
 
@@ -69,14 +89,19 @@
 </pre>
 
 However, it is not necessary for the usage of this package. This package is
 meant for a comparison, but PyPhotometry legacy routines are more
 general. Accompanying there are several other routines.
 
 <hr>
+#### <b>Brief Tutorial</b>
+
+A brief tutorial can be found at <a
+href='https://github.com/neutrinomuon/PyPhotometry/blob/main/tutorials/PyPhotometry%20-%20Example%201.ipynb'>PyPhotometry
+Example1.ipynb</a>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/PyPhotometry/>PyPhotometry</a> by using pip -
 <a href='https://pypi.org/'>PyPI - The Python Package Index</a>:
```

#### html2text {}

```diff
@@ -1,52 +1,59 @@
 ### PyPhotometry #### Fully based on a Fortran legacy package to easily compute
 the photometric fluxes and magnitudes in different systems email:
 [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
 [jean@astro.up.pt](mailto:jean@astro.up.pt) github repository: PyPhotometry
-last stable version: 0.0.5 Â© Copyright Â® J.G. - Jean Gomes @ 2023
+last stable version: 0.0.6 Â© Copyright Â® J.G. - Jean Gomes @ 2023
 ===============================================================================
 [https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
 [https://img.shields.io/pypi/pyversions/PyPhotometry][https://anaconda.org/
 neutrinomuon/PyPhotometry/badges/license.svg]
 ===============================================================================
        [https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/
                                PyPhotometry.png]
 ===============================================================================
+#### Requirements The following packages are required to run this project: -
+astropy>=5.0.4 - matplotlib>=3.7.1 - setuptools>=61.2.0 - SQLAlchemy>=1.4.32
+and pyphot may be used for comparison and tests: - pyphot>=1.4.4 You can
+install all the required packages by running the following command:
+pip install -r requirements.txt
+Additionally, you may optionally install pyphot for testing or comparison
+purposes. Please note that pyphot is not a mandatory requirement for running
+this project and is only recommended if you intend to test or compare with it.
 #### RESUME PyPhotometry is a Python package that builds upon a collection of
 Fortran 2003+ routines originally developed between 2003 and 2004. These
 routines are the foundation of the package and can be traced back to that time
 period. The licensing details for the Fortran routines can be found in the
 LICENSE.txt file included with the package. The main purpose of PyPhotometry is
 to enable the computation of photometric fluxes and magnitudes in various
 photometric systems. It offers support for multiple magnitude systems,
 including the VEGA standard, the VEGA system proposed by Bohlin and Gilland in
 2004, the AB system, the TG standard system (Thuan & Gunn), the WFPC2 system,
 the FOCA system at 2000, and also provides an option without any calibration.
 It's important to note that PyPhotometry does not include the Pyphot package
-developed by M. Fouesneau, but it can be used for comparison purposes. If you
-wish to install Pyphot for comparison, you can use the following command:
-pip install pyphot
-However, it is not mandatory to install Pyphot in order to use PyPhotometry.
-The PyPhotometry package comes with its own set of accompanying routines that
+developed by M. Fouesneau, but it can be used for comparison purposes. However,
+it is not mandatory to install Pyphot in order to use PyPhotometry. The
+PyPhotometry package comes with its own set of accompanying routines that
 provide the necessary functionality. Original Fortran 2003+ routines date back
 to 2003-2004. Read the LICENSE.txt file. PyPhotometry is a Python package based
 on a Fortran legacy package that allows you to compute photometric fluxes and
 magnitudes in various photometric systems. The package provides different
 magnitude systems, such as VEGA standard, VEGA proposed by Bohlin and Gilland
 2004, AB system, TG standard system (Thuan & Gunn), WFPC2 system, FOCA at 2000,
 and without any calibration. Pyphot from M. Fouesneau is *NOT* part of the
 distribution, but used as a comparison: https://mfouesneau.github.io/pyphot/
 index.html#package-main-content. If you want to install for comparison then:
 pip install pyphot
 However, it is not necessary for the usage of this package. This package is
 meant for a comparison, but PyPhotometry legacy routines are more general.
 Accompanying there are several other routines.
 ===============================================================================
-#### INSTALLATION You can easily install PyPhotometry by using pip - PyPI_-_The
-Python_Package_Index:
+#### Brief Tutorial A brief tutorial can be found at PyPhotometry
+Example1.ipynb #### INSTALLATION You can easily install PyPhotometry by using
+pip - PyPI_-_The_Python_Package_Index:
 pip install PyPhotometry
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
 PyPhotometry: [https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 version.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 latest_release_date.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 platforms.svg]
```

### Comparing `PyPhotometry-0.0.5/data/2MASSH.txt` & `PyPhotometry-0.0.6/data/2MASSH.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/2MASSJ.txt` & `PyPhotometry-0.0.6/data/2MASSJ.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/2MASSKs.txt` & `PyPhotometry-0.0.6/data/2MASSKs.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/GalexNUV.txt` & `PyPhotometry-0.0.6/data/GalexNUV.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/Herschel_SPIRE.PLW_ext.txt` & `PyPhotometry-0.0.6/data/Herschel_SPIRE.PLW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/Herschel_SPIRE.PMW_ext.txt` & `PyPhotometry-0.0.6/data/Herschel_SPIRE.PMW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/Herschel_SPIRE.PSW_ext.txt` & `PyPhotometry-0.0.6/data/Herschel_SPIRE.PSW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/IRAS.100mu.txt` & `PyPhotometry-0.0.6/data/IRAS.100mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/IRAS.12mu.txt` & `PyPhotometry-0.0.6/data/IRAS.12mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/IRAS.25mu.txt` & `PyPhotometry-0.0.6/data/IRAS.25mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/IRAS.60mu.txt` & `PyPhotometry-0.0.6/data/IRAS.60mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/SDSSg.txt` & `PyPhotometry-0.0.6/data/SDSSg.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/SDSSi.txt` & `PyPhotometry-0.0.6/data/SDSSi.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/SDSSr.txt` & `PyPhotometry-0.0.6/data/SDSSr.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/SDSSu.txt` & `PyPhotometry-0.0.6/data/SDSSu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/SDSSz.txt` & `PyPhotometry-0.0.6/data/SDSSz.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/WISE1.txt` & `PyPhotometry-0.0.6/data/WISE1.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/WISE2.txt` & `PyPhotometry-0.0.6/data/WISE2.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/WISE3.txt` & `PyPhotometry-0.0.6/data/WISE3.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/WISE4.txt` & `PyPhotometry-0.0.6/data/WISE4.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/BD+17d4708.dat` & `PyPhotometry-0.0.6/data/calibration_stars/BD+17d4708.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/BD+17o4708.dat` & `PyPhotometry-0.0.6/data/calibration_stars/BD+17o4708.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/Filters_ReadMe.txt` & `PyPhotometry-0.0.6/data/calibration_stars/Filters_ReadMe.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/Sun.dat` & `PyPhotometry-0.0.6/data/calibration_stars/Sun.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/Sun_LR.dat` & `PyPhotometry-0.0.6/data/calibration_stars/Sun_LR.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/VegaLR.dat` & `PyPhotometry-0.0.6/data/calibration_stars/VegaLR.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/VegaLR_OLD.dat` & `PyPhotometry-0.0.6/data/calibration_stars/VegaLR_OLD.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/bd17d4708_stisnic_001.fits` & `PyPhotometry-0.0.6/data/calibration_stars/bd17d4708_stisnic_001.fits`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/kp00_6000.ascii` & `PyPhotometry-0.0.6/data/calibration_stars/kp00_6000.ascii`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/calibration_stars/sun_reference_stis_001.fits` & `PyPhotometry-0.0.6/data/calibration_stars/sun_reference_stis_001.fits`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/data/filters.db` & `PyPhotometry-0.0.6/data/filters.db`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/setup.py` & `PyPhotometry-0.0.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     for root, _, filenames in os.walk(directory):
         for filename in filenames:
             files.append(os.path.join(root, filename))
     return files
 
 # Define the directories you want to include
 data_directory = 'data'
-calibration_directory = 'data/calibration'
+calibration_directory = 'data/calibration_stars'
 
 # Get all files within the data directory and its subdirectories
 data_files = get_files(data_directory)
 
 # Get all files within the calibration directory
 calibration_files = get_files(calibration_directory)
 
@@ -48,20 +48,34 @@
        maintainer='Jean Gomes',
        maintainer_email='antineutrinomuon@gmail.com',
        keywords='photometry,stars,galaxies,magnitude,systems',
        url='https://github.com/neutrinomuon/PyPhotometry',
        docs_url='https://github.com/neutrinomuon/PyPhotometry',
        download_url='https://github.com/neutrinomuon/PyPhotometry',
        install_requires=[ 'numpy','matplotlib','sqlalchemy','astropy' ],
-       requires_python='>3.9',
+       requires_python='>=3.9',
        classifiers=[
            "Programming Language :: Python :: 3",
            "Programming Language :: Fortran",
            "Operating System :: OS Independent",
                    ],
        package_dir={"PyPhotometry": "src/python"},
        packages=['PyPhotometry'],
-       data_files=[ ('', ['version.txt','LICENSE.txt']),
-                    ('data', data_files),
-                    ('data/calibration', calibration_files) ],
+       data_files=[('PyPhotometry/data', data_files), ('PyPhotometry/data/calibration_stars', calibration_files)],
+       include_package_data=True,
+       #data_files=[ ('', ['version.txt','LICENSE.txt']),
+       #             ('data', data_files),
+       #             ('data/calibration', calibration_files) ],
+       #package_data={'PyPhotometry': [
+       #                               'data/*',
+       #                               'data/calibration/*',
+       #                              ],
+       #             },
+       #package_data={'PyPhotometry': [                                                                                                                                                                                               
+       #                               'data/*',                                                                                                                                                                                      
+       #                               'data/calibration/*',                                                                                                                                                                          
+       #                              ],                                                                                                                                               
+       #             },                          
+       #include_package_data=True,
+       #data_files=[('', ['version.txt', 'LICENSE.txt'])]
       )
```

### Comparing `PyPhotometry-0.0.5/src/fortran/DataTypes.f90` & `PyPhotometry-0.0.6/src/fortran/DataTypes.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/src/fortran/EvalFilters.f90` & `PyPhotometry-0.0.6/src/fortran/EvalFilters.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/src/fortran/GaussLegendreQuadrature.f90` & `PyPhotometry-0.0.6/src/fortran/GaussLegendreQuadrature.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/src/fortran/IntegralALL.f90` & `PyPhotometry-0.0.6/src/fortran/IntegralALL.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/src/fortran/LINinterpol.f90` & `PyPhotometry-0.0.6/src/fortran/LINinterpol.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/src/fortran/PropFilters.f90` & `PyPhotometry-0.0.6/src/fortran/PropFilters.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.5/src/python/Photometry.py` & `PyPhotometry-0.0.6/src/python/Photometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Revised interface on Sat Jan 30 12:07:21 2021
 
 @author: Jean Gomes
 
 RESUME :  Filters
 
-Version: v01 beta
+Version: v0.0.6
 
 PYTHON : Python compatibility using f2py revised. Better usage  with numpy.  
 
 Written: Jean Michel Gomes © Copyright
 Created on Sat Jan 30 12:07:21 2021
 """
 
@@ -88,18 +88,31 @@
 
 # General Database Class
 class create_database_filters(object):
     
     global Base
     Base = declarative_base()
     
-    def __init__( self, database_path='../../data',database_filename='filters.db' ):
+    def __init__( self, database_path=None,database_filename='filters.db' ):
         self.store_filters = 0
         self.readfilters = 0
         
+        # database_path by default is define as None, if so, look for installation of PyPhotometry
+        # Specify the package name
+        if database_path == None:
+            package_name = 'PyPhotometry'
+
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+
+            # Get the base directory path of the package
+            database_path = package_dist.location + '/' + package_name + '/data/'
+
+            print("... Package directory:", database_path)
+        
         self.database_path = database_path
         self.database_filename = database_filename
         self.database_filters = os.path.join(database_path, database_filename)
         
         # By using pkg_resources.resource_filename(__name__, 'filters.db'), the code retrieves the 
         # absolute file path of 'filters.db' within the package or module. This path is then assigned 
         # to self.database_filters for further use, such as creating an SQLAlchemy engine with the 
@@ -149,15 +162,82 @@
         lbd_units = Column(String)
         
         wavelength = Column(PickleType)
         fluxes = Column(PickleType)
 
         N_lambda = Column(Integer)
                 
-    def read_spectra( self, path_Vega='../../data/calibration_stars/VegaLR.dat',path_Sun='../../data/calibration_stars/Sun_LR.dat',path1Sun='../../data/calibration_stars/Sun.dat',path2Sun='/../../data/calibration_stars/sun_reference_stis_001.fits',path_BD='../../data/calibration_stars/BD+17d4708.dat', verbose=False ):
+    #def read_spectra( self, path_Vega='../../data/calibration_stars/VegaLR.dat',path_Sun='../../data/calibration_stars/Sun_LR.dat',path1Sun='../../data/calibration_stars/Sun.dat',path2Sun='/../../data/calibration_stars/sun_reference_stis_001.fits',path_BD='../../data/calibration_stars/BD+17d4708.dat', verbose=False ):
+    def read_spectra( self, path_Vega=None,path_Sun=None,path1Sun=None,path2Sun=None,path_BD=None, verbose=False ):
+        
+        # Read Vega *******************************************************************
+        if path_Vega == None:
+            package_name = 'PyPhotometry'
+
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+
+            # Get the base directory path of the package
+            path_Vega = package_dist.location + '/' + package_name + '/data/calibration_stars/VegaLR.dat'
+
+            print("... path_Vega directory:", path_Vega)
+        # Read Vega *******************************************************************
+
+        # Read Sun ********************************************************************
+        if path_Sun == None:
+            package_name = 'PyPhotometry'
+
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+
+            # Get the base directory path of the package
+            path_Sun = package_dist.location + '/' + package_name + '/data/calibration_stars/Sun_LR.dat'
+
+            print("... path_Sun directory:", path_Sun)
+        # Read Sun ********************************************************************
+        
+        # Read Sun_1 ******************************************************************
+        if path1Sun == None:
+            package_name = 'PyPhotometry'
+
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+
+            # Get the base directory path of the package
+            path1Sun = package_dist.location + '/' + package_name + '/data/calibration_stars/Sun.dat'
+
+            print("... path1Sun directory:", path1Sun)
+        # Read Sun_1 ******************************************************************
+        
+        # Read Sun_2 ******************************************************************
+        if path2Sun == None:
+            package_name = 'PyPhotometry'
+
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+
+            # Get the base directory path of the package
+            path2Sun = package_dist.location + '/' + package_name + '/data/calibration_stars/sun_reference_stis_001.fits'
+
+            print("... path2Sun directory:", path2Sun)
+        # Read Sun_2 ******************************************************************
+        
+        # Read BD *********************************************************************
+        if path_BD == None:
+            package_name = 'PyPhotometry'
+
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+
+            # Get the base directory path of the package
+            path_BD = package_dist.location + '/' + package_name + '/data/calibration_stars/BD+17d4708.dat'
+
+            print("... path_BD directory:", path2Sun)
+        # Read BD *********************************************************************
+        
         o = Filters( )
         o.ReadCalibrationStars(  path_Vega=path_Vega,path_Sun=path_Sun,path1Sun=path1Sun,path2Sun=path2Sun,path_BD=path_BD )
         
         self.lambVega = o.lambVega
         self.fluxVega =o.fluxVega
         self.lambvega = self.lambVega
         self.fluxvega = self.fluxVega
@@ -182,20 +262,33 @@
         if verbose:
             print("[read_spectra]")
             print("... Read spectra of calibration stars")
             print("[read_spectra]")
             
         return
         
-    def read_filters( self, path_data='../../data/',N_lambda=500,verbose=False ):
+    def read_filters( self, path_data=None,N_lambda=500,verbose=False ):
                 
         if verbose:
             print("[read_filters]")
             print("... Reading filters")
         
+        # database_path by default is define as None, if so, look for installation of PyPhotometry
+        # Specify the package name
+        if path_data == None:
+            package_name = 'PyPhotometry'
+
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+
+            # Get the base directory path of the package
+            path_data = package_dist.location + '/' + package_name + '/data/'
+
+            print("... path_data directory:", path_data)
+        
         # Verify if database contains models for Draine and Li (2007)
         try:
             read = self.session.query(self._filters_class).filter( np.size(self._filters_class.name_filter) > 0 )
         except:
             read = 'ERROR' #np.zeros()
             
         # print('###########################################')
@@ -436,15 +529,19 @@
         
             metadata = Base.metadata.create_all(self.Engine)
         
             o = Filters()
             #print(o)
             path = path_data #'../../data/'
             arq_fil1 = 'ListFilters.txt'
-            o.ReadFilters( path,arq_fil1,verbose=verbose )
+            IsKeepOn = o.ReadFilters( path,arq_fil1,verbose=verbose )
+        
+            if IsKeepOn != 1:
+                print("... Problem running filters database")
+                return
         
             # 4 different entry for each filter
             N_entries = int( len(o.filters) / 4 )
             # print( len(o.filters) )
             print("... N_entries: {0:}".format(N_entries))
 
             self.N_filters = N_entries
@@ -596,18 +693,19 @@
                 
         #self.T_lambda = self.filters
         #self.T_fluxes =
         
         Figure = plt.figure( figsize=(12,10),dpi=120,facecolor='w',edgecolor='w' )
         plt.subplots_adjust(bottom=.02, left=.06, right=.95, top=.98, wspace=0.0, hspace=0.0) 
         
-        ax = plt.subplot(111)
+        #ax = plt.subplot(111)
 
         # Top plot ###########################################################
-        ax1_top = subplot2grid( (20,20), (0,0), colspan=20, rowspan=10 )                                           
+        ax1_top = subplot2grid( (20,20), (0,0), colspan=20, rowspan=10 )
+                                        
         # Sets the position and size of the panel for Plot #01
         #ax1_top.axis('on')
         #ax1_top.axes.get_xaxis().set_visible(False)
 
         #ax1_top.set_xscale('log')
         
         #ax1_top.xaxis.set_major_formatter(matplotlib.ticker.ScalarFormatter())
@@ -933,15 +1031,15 @@
             print( "... arq_fil1: {0:}".format(arq_fil1) ) #arq_fil1 = file_dir(1:ilastnum)//'ListFilters.txt'
         
         try:
             o_filter = open(path + arq_fil1,'r')
         except:
             print('... Filter List does not exist')
             o_filter.close()
-            return
+            return -999
         
         r_filter = o_filter.readlines()
         Nfilters = int(r_filter[0].split()[0])
         self.Nfilters = Nfilters
         if verbose:
             print("... Nfilters: {0:d}".format(Nfilters))
                 
@@ -1064,15 +1162,15 @@
             # fill_character = ' '  # Specify the character you want to use for filling
 
             # print( "{0:0>4} {1:<30} {2:<30} {3:<30}".format( i, self.name_fil[i].ljust(40, fill_character), str(self.name_of_filter[i]) , str(self.name_fil[i]).split('.txt')[0] ) )
             
         # print( "N_filters: ----- DEBUG: ",len(self.filters) )
         print("[ReadFilters]")
 
-        return
+        return 1
     
     def ReadONEFilter( self,path,arq_fil1,N_lambda=500 ):
         print("")
         print( "... Reading One Filter " )
         print( "... arq_fil1: {0:}".format(arq_fil1) )
                 
         Nfilters =1
@@ -1164,15 +1262,16 @@
             self.onefilter[ i ] = [ str(self.name1fil[i]).split('.txt')[0],self.detector1type[i],self.T1lambda[0:N_lambda,i], self.T1fluxes[0:N_lambda,i], d ]
             self.onefilter[ str(self.name1fil[i]) + '.txt' ] = self.onefilter[ i ]
             self.onefilter[ self.name1fil[i] ] = self.onefilter[ i ]
             
             #print( self.onefilter )
             return
             
-    def ReadCalibrationStars( self,path_Vega='../../data/calibration_stars/VegaLR.dat',path_Sun='../../data/calibration_stars/Sun_LR.dat',path1Sun='../../data/calibration_stars/Sun.dat',path2Sun='../../data/sun_reference_stis_001.fits',path_BD='../../data/calibration_stars/BD+17d4708.dat',verbose=0 ):
+    #def ReadCalibrationStars( self,path_Vega='../../data/calibration_stars/VegaLR.dat',path_Sun='../../data/calibration_stars/Sun_LR.dat',path1Sun='../../data/calibration_stars/Sun.dat',path2Sun='../../data/sun_reference_stis_001.fits',path_BD='../../data/calibration_stars/BD+17d4708.dat',verbose=0 ):
+    def ReadCalibrationStars( self,path_Vega=None,path_Sun=None,path1Sun=None,path2Sun=None,path_BD=None,verbose=0 ):
 # ! *** Read calibration stars ************************************************
 # !     RESUME : VEGA spectrum.                                               !
 # !              Intrinsic Flux: erg/s/cm2/A                                  !
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 #     !arq_fil1 = file_dir(1:ilastnum)//'VegaLR.dat'
 #     !open  (21,status='old',file=arq_fil1,ERR=22)
 #     !read  (21,*,ERR=22) arq_lixo,NVegalbd
@@ -1215,14 +1314,79 @@
 #     !    read(21,*,ERR=22) lamb_FBD(i_lambda),flux_FBD(i_lambda)
 #     !end do
 #     !close(21)
 # ! *** Read calibration stars ************************************************
         
 # https://www.stsci.edu/hst/instrumentation/reference-data-for-calibration-and-tools/astronomical-catalogs/calspec
 
+# Read Vega *******************************************************************
+        if path_Vega == None:
+            package_name = 'PyPhotometry'
+        
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+        
+            # Get the base directory path of the package
+            path_Vega = package_dist.location + '/' + package_name + '/data/calibration_stars/VegaLR.dat'
+        
+            print("... path_Vega directory:", path_Vega)
+# Read Vega *******************************************************************
+
+# Read Sun ********************************************************************
+        if path_Sun == None:
+            package_name = 'PyPhotometry'
+        
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+        
+            # Get the base directory path of the package
+            path_Sun = package_dist.location + '/' + package_name + '/data/calibration_stars/Sun_LR.dat'
+        
+            print("... path_Sun directory:", path_Sun)
+# Read Sun ********************************************************************
+
+# Read Sun_1 ******************************************************************
+        if path1Sun == None:
+            package_name = 'PyPhotometry'
+        
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+        
+            # Get the base directory path of the package
+            path1Sun = package_dist.location + '/' + package_name + '/data/calibration_stars/Sun.dat'
+        
+            print("... path1Sun directory:", path1Sun)
+# Read Sun_1 ******************************************************************
+
+# Read Sun_2 ******************************************************************
+        if path2Sun == None:
+            package_name = 'PyPhotometry'
+        
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+        
+            # Get the base directory path of the package
+            path2Sun = package_dist.location + '/' + package_name + '/data/calibration_stars/sun_reference_stis_001.fits'
+        
+            print("... path2Sun directory:", path2Sun)
+# Read Sun_2 ******************************************************************
+
+# Read BD *********************************************************************
+        if path_BD == None:
+            package_name = 'PyPhotometry'
+        
+            # Get the distribution object for the package
+            package_dist = pkg_resources.get_distribution(package_name)
+        
+            # Get the base directory path of the package
+            path_BD = package_dist.location + '/' + package_name + '/data/calibration_stars/BD+17d4708.dat'
+        
+            print("... path_BD directory:", path2Sun)
+# Read BD *********************************************************************
+
 #  *** VEGA spectrum ***************************************************************
 #         Intrinsic Flux: erg/s/cm2/A                                                                                                                  !
 ######################################################################
         o = open(path_Vega,'r')
         r = o.readlines()
         r_split  = r[0].split()[1]
```

