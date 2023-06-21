# Comparing `tmp/ecoscope-1.3.2.tar.gz` & `tmp/ecoscope-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.3.2.tar", last modified: Tue Jun 20 06:55:45 2023, max compression
+gzip compressed data, was "ecoscope-1.3.3.tar", last modified: Wed Jun 21 08:13:45 2023, max compression
```

## Comparing `ecoscope-1.3.2.tar` & `ecoscope-1.3.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.180349 ecoscope-1.3.2/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-22 06:13:31.000000 ecoscope-1.3.2/LICENSE
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-06-20 06:55:45.180349 ecoscope-1.3.2/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-22 06:13:31.000000 ecoscope-1.3.2/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.116339 ecoscope-1.3.2/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2023-06-16 19:26:49.000000 ecoscope-1.3.2/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2023-06-16 14:29:12.000000 ecoscope-1.3.2/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2023-06-16 20:17:33.000000 ecoscope-1.3.2/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.176348 ecoscope-1.3.2/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.176348 ecoscope-1.3.2/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    33370 2023-06-08 07:55:39.000000 ecoscope-1.3.2/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.176348 ecoscope-1.3.2/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.180349 ecoscope-1.3.2/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-06-16 20:24:07.000000 ecoscope-1.3.2/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope.egg-info/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-22 13:48:35.000000 ecoscope-1.3.2/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      289 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-22 06:13:31.000000 ecoscope-1.3.2/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-06-20 06:55:45.180349 ecoscope-1.3.2/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1945 2023-06-16 18:21:45.000000 ecoscope-1.3.2/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.180349 ecoscope-1.3.2/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6554 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6955 2023-05-24 09:30:01.000000 ecoscope-1.3.2/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-06-16 18:01:57.000000 ecoscope-1.3.2/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.940167 ecoscope-1.3.3/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-06-21 08:12:37.000000 ecoscope-1.3.3/LICENSE
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-06-21 08:13:45.940167 ecoscope-1.3.3/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-06-21 08:12:37.000000 ecoscope-1.3.3/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.936166 ecoscope-1.3.3/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.936166 ecoscope-1.3.3/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.936166 ecoscope-1.3.3/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.936166 ecoscope-1.3.3/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.936166 ecoscope-1.3.3/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.940167 ecoscope-1.3.3/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    33370 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.940167 ecoscope-1.3.3/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.940167 ecoscope-1.3.3/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-06-21 08:12:37.000000 ecoscope-1.3.3/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.936166 ecoscope-1.3.3/ecoscope.egg-info/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-06-21 08:13:45.000000 ecoscope-1.3.3/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-06-21 08:13:45.000000 ecoscope-1.3.3/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-06-21 08:13:45.000000 ecoscope-1.3.3/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-06-21 08:13:45.000000 ecoscope-1.3.3/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      289 2023-06-21 08:13:45.000000 ecoscope-1.3.3/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-06-21 08:13:45.000000 ecoscope-1.3.3/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-06-21 08:12:37.000000 ecoscope-1.3.3/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-06-21 08:13:45.940167 ecoscope-1.3.3/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1945 2023-06-21 08:12:37.000000 ecoscope-1.3.3/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-21 08:13:45.940167 ecoscope-1.3.3/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6554 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6955 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-06-21 08:12:37.000000 ecoscope-1.3.3/tests/test_utils.py
```

### Comparing `ecoscope-1.3.2/LICENSE` & `ecoscope-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/PKG-INFO` & `ecoscope-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.3.2
+Version: 1.3.3
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.3.2/README.rst` & `ecoscope-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/__init__.py` & `ecoscope-1.3.3/ecoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.3.3/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/astronomy.py` & `ecoscope-1.3.3/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/ecograph.py` & `ecoscope-1.3.3/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/geofence.py` & `ecoscope-1.3.3/ecoscope/analysis/geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/immobility.py` & `ecoscope-1.3.3/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/percentile.py` & `ecoscope-1.3.3/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/proximity.py` & `ecoscope-1.3.3/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/seasons.py` & `ecoscope-1.3.3/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/analysis/speed.py` & `ecoscope-1.3.3/ecoscope/analysis/speed.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/base/__init__.py` & `ecoscope-1.3.3/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/base/_dataclasses.py` & `ecoscope-1.3.3/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/base/base.py` & `ecoscope-1.3.3/ecoscope/base/base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/base/utils.py` & `ecoscope-1.3.3/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/contrib/basemaps.py` & `ecoscope-1.3.3/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/contrib/foliumap.py` & `ecoscope-1.3.3/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/contrib/legend.txt` & `ecoscope-1.3.3/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/io/earthranger.py` & `ecoscope-1.3.3/ecoscope/io/earthranger.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/io/eetools.py` & `ecoscope-1.3.3/ecoscope/io/eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/io/raster.py` & `ecoscope-1.3.3/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/io/utils.py` & `ecoscope-1.3.3/ecoscope/io/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/mapping/map.py` & `ecoscope-1.3.3/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope/plotting/plot.py` & `ecoscope-1.3.3/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.3.3/ecoscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.3.2
+Version: 1.3.3
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.3.2/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.3.3/ecoscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/pyproject.toml` & `ecoscope-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/setup.py` & `ecoscope-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_base.py` & `ecoscope-1.3.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_earthranger_io.py` & `ecoscope-1.3.3/tests/test_earthranger_io.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_ecodataframe.py` & `ecoscope-1.3.3/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_ecograph.py` & `ecoscope-1.3.3/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_eetools.py` & `ecoscope-1.3.3/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_geofence.py` & `ecoscope-1.3.3/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_immobility.py` & `ecoscope-1.3.3/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_seasons.py` & `ecoscope-1.3.3/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.2/tests/test_ud.py` & `ecoscope-1.3.3/tests/test_ud.py`

 * *Files identical despite different names*

