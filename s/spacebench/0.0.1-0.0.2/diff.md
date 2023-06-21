# Comparing `tmp/spacebench-0.0.1.tar.gz` & `tmp/spacebench-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacebench-0.0.1.tar", last modified: Thu Apr 20 15:26:15 2023, max compression
+gzip compressed data, was "spacebench-0.0.2.tar", last modified: Wed Jun 21 02:49:54 2023, max compression
```

## Comparing `spacebench-0.0.1.tar` & `spacebench-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-20 15:26:15.975992 spacebench-0.0.1/
--rw-r--r--   0 nak443     (502) staff       (20)     1071 2023-04-05 23:54:49.000000 spacebench-0.0.1/LICENSE
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-20 14:30:45.000000 spacebench-0.0.1/MANIFEST.in
--rw-r--r--   0 nak443     (502) staff       (20)     1529 2023-04-20 15:26:15.975696 spacebench-0.0.1/PKG-INFO
--rw-r--r--   0 nak443     (502) staff       (20)     2945 2023-04-20 15:24:55.000000 spacebench-0.0.1/README.md
--rw-r--r--   0 nak443     (502) staff       (20)       38 2023-04-20 15:26:15.976098 spacebench-0.0.1/setup.cfg
--rw-r--r--   0 nak443     (502) staff       (20)     2021 2023-04-20 13:11:36.000000 spacebench-0.0.1/setup.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-20 15:26:15.969438 spacebench-0.0.1/spacebench/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-20 13:11:36.000000 spacebench-0.0.1/spacebench/__init__.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-20 15:26:15.971401 spacebench-0.0.1/spacebench/algorithm/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-20 14:30:45.000000 spacebench-0.0.1/spacebench/algorithm/__init__.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-20 15:26:15.973078 spacebench-0.0.1/spacebench/datasets/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-20 14:30:45.000000 spacebench-0.0.1/spacebench/datasets/__init__.py
--rw-r--r--   0 nak443     (502) staff       (20)     8605 2023-04-20 14:30:45.000000 spacebench-0.0.1/spacebench/datasets/datasets.py
--rw-r--r--   0 nak443     (502) staff       (20)     1919 2023-04-20 14:30:45.000000 spacebench-0.0.1/spacebench/datasets/error_sampler.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-20 15:26:15.973740 spacebench-0.0.1/spacebench/evaluation/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-20 14:30:45.000000 spacebench-0.0.1/spacebench/evaluation/__init__.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-20 15:26:15.974362 spacebench-0.0.1/spacebench/synthetic_data_generation/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-20 14:30:45.000000 spacebench-0.0.1/spacebench/synthetic_data_generation/__init__.py
--rw-r--r--   0 nak443     (502) staff       (20)    24764 2023-04-20 13:11:36.000000 spacebench-0.0.1/spacebench/synthetic_data_generation/nn_and_xgboost.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-20 15:26:15.970954 spacebench-0.0.1/spacebench.egg-info/
--rw-r--r--   0 nak443     (502) staff       (20)     1529 2023-04-20 15:26:15.000000 spacebench-0.0.1/spacebench.egg-info/PKG-INFO
--rw-r--r--   0 nak443     (502) staff       (20)      469 2023-04-20 15:26:15.000000 spacebench-0.0.1/spacebench.egg-info/SOURCES.txt
--rw-r--r--   0 nak443     (502) staff       (20)        1 2023-04-20 15:26:15.000000 spacebench-0.0.1/spacebench.egg-info/dependency_links.txt
--rw-r--r--   0 nak443     (502) staff       (20)       11 2023-04-20 15:26:15.000000 spacebench-0.0.1/spacebench.egg-info/top_level.txt
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-21 02:49:54.042310 spacebench-0.0.2/
+-rw-r--r--   0 nak443     (502) staff       (20)     1071 2023-04-05 23:54:49.000000 spacebench-0.0.2/LICENSE
+-rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-24 13:20:22.000000 spacebench-0.0.2/MANIFEST.in
+-rw-r--r--   0 nak443     (502) staff       (20)     1584 2023-06-21 02:49:54.042032 spacebench-0.0.2/PKG-INFO
+-rw-r--r--   0 nak443     (502) staff       (20)     5496 2023-06-21 02:44:38.000000 spacebench-0.0.2/README.md
+-rw-r--r--   0 nak443     (502) staff       (20)       38 2023-06-21 02:49:54.042415 spacebench-0.0.2/setup.cfg
+-rw-r--r--   0 nak443     (502) staff       (20)     2500 2023-06-21 02:48:05.000000 spacebench-0.0.2/setup.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-21 02:49:54.034954 spacebench-0.0.2/spacebench/
+-rw-r--r--   0 nak443     (502) staff       (20)      717 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/__init__.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-21 02:49:54.040072 spacebench-0.0.2/spacebench/algorithms/
+-rw-r--r--   0 nak443     (502) staff       (20)        0 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/algorithms/__init__.py
+-rw-r--r--   0 nak443     (502) staff       (20)      459 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/algorithms/classes.py
+-rw-r--r--   0 nak443     (502) staff       (20)    11918 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/algorithms/dapsm.py
+-rw-r--r--   0 nak443     (502) staff       (20)     7789 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/algorithms/gcn.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3705 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/algorithms/ols.py
+-rw-r--r--   0 nak443     (502) staff       (20)     1547 2023-06-21 02:44:38.000000 spacebench-0.0.2/spacebench/algorithms/spatial.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3941 2023-06-21 02:44:38.000000 spacebench-0.0.2/spacebench/algorithms/spatialplus.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-21 02:49:54.041418 spacebench-0.0.2/spacebench/api/
+-rw-r--r--   0 nak443     (502) staff       (20)        0 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/api/__init__.py
+-rw-r--r--   0 nak443     (502) staff       (20)     5798 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/api/cli.py
+-rw-r--r--   0 nak443     (502) staff       (20)     5535 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/api/dataverse.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3824 2023-06-21 02:44:38.000000 spacebench-0.0.2/spacebench/datamaster.py
+-rw-r--r--   0 nak443     (502) staff       (20)    14565 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/env.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3659 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/eval.py
+-rw-r--r--   0 nak443     (502) staff       (20)      620 2023-06-20 21:37:54.000000 spacebench-0.0.2/spacebench/log.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-21 02:49:54.036896 spacebench-0.0.2/spacebench.egg-info/
+-rw-r--r--   0 nak443     (502) staff       (20)     1584 2023-06-21 02:49:53.000000 spacebench-0.0.2/spacebench.egg-info/PKG-INFO
+-rw-r--r--   0 nak443     (502) staff       (20)      613 2023-06-21 02:49:53.000000 spacebench-0.0.2/spacebench.egg-info/SOURCES.txt
+-rw-r--r--   0 nak443     (502) staff       (20)        1 2023-06-21 02:49:53.000000 spacebench-0.0.2/spacebench.egg-info/dependency_links.txt
+-rw-r--r--   0 nak443     (502) staff       (20)      378 2023-06-21 02:49:53.000000 spacebench-0.0.2/spacebench.egg-info/requires.txt
+-rw-r--r--   0 nak443     (502) staff       (20)       11 2023-06-21 02:49:53.000000 spacebench-0.0.2/spacebench.egg-info/top_level.txt
```

### Comparing `spacebench-0.0.1/LICENSE` & `spacebench-0.0.2/LICENSE`

 * *Files identical despite different names*

