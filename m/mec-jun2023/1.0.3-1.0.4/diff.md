# Comparing `tmp/mec_jun2023-1.0.3.tar.gz` & `tmp/mec_jun2023-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mec_jun2023-1.0.3.tar", last modified: Wed Jun 21 12:39:39 2023, max compression
+gzip compressed data, was "mec_jun2023-1.0.4.tar", last modified: Wed Jun 21 12:56:13 2023, max compression
```

## Comparing `mec_jun2023-1.0.3.tar` & `mec_jun2023-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:39:39.131891 mec_jun2023-1.0.3/
--rw-r--r--   0 antoine    (501) staff       (20)    35138 2023-06-21 09:21:00.000000 mec_jun2023-1.0.3/LICENSE
--rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:39:39.131789 mec_jun2023-1.0.3/PKG-INFO
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:39:39.131624 mec_jun2023-1.0.3/mec_jun2023.egg-info/
--rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/PKG-INFO
--rw-r--r--   0 antoine    (501) staff       (20)      168 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/SOURCES.txt
--rw-r--r--   0 antoine    (501) staff       (20)        1 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/dependency_links.txt
--rw-r--r--   0 antoine    (501) staff       (20)        9 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/top_level.txt
--rw-r--r--   0 antoine    (501) staff       (20)     7508 2023-06-21 12:39:21.000000 mec_jun2023-1.0.3/pymec_lp.py
--rw-r--r--   0 antoine    (501) staff       (20)       38 2023-06-21 12:39:39.131926 mec_jun2023-1.0.3/setup.cfg
--rw-r--r--   0 antoine    (501) staff       (20)      340 2023-06-21 12:39:26.000000 mec_jun2023-1.0.3/setup.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:56:13.399250 mec_jun2023-1.0.4/
+-rw-r--r--   0 antoine    (501) staff       (20)    35138 2023-06-21 09:21:00.000000 mec_jun2023-1.0.4/LICENSE
+-rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:56:13.399147 mec_jun2023-1.0.4/PKG-INFO
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:56:13.398970 mec_jun2023-1.0.4/mec_jun2023.egg-info/
+-rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:56:13.000000 mec_jun2023-1.0.4/mec_jun2023.egg-info/PKG-INFO
+-rw-r--r--   0 antoine    (501) staff       (20)      168 2023-06-21 12:56:13.000000 mec_jun2023-1.0.4/mec_jun2023.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        1 2023-06-21 12:56:13.000000 mec_jun2023-1.0.4/mec_jun2023.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        9 2023-06-21 12:56:13.000000 mec_jun2023-1.0.4/mec_jun2023.egg-info/top_level.txt
+-rw-r--r--   0 antoine    (501) staff       (20)     7538 2023-06-21 12:55:53.000000 mec_jun2023-1.0.4/pymec_lp.py
+-rw-r--r--   0 antoine    (501) staff       (20)       38 2023-06-21 12:56:13.399284 mec_jun2023-1.0.4/setup.cfg
+-rw-r--r--   0 antoine    (501) staff       (20)      340 2023-06-21 12:56:04.000000 mec_jun2023-1.0.4/setup.py
```

### Comparing `mec_jun2023-1.0.3/LICENSE` & `mec_jun2023-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mec_jun2023-1.0.3/pymec_lp.py` & `mec_jun2023-1.0.4/pymec_lp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 import scipy.sparse as spr
 #import gurobipy as grb
 import sympy
 from sympy.solvers import solve
 from sympy import *
 import matplotlib.pyplot as plt
+from tabulate import tabulate
 
 
 #############################
 # LP1: Intro to linear programming #
 #############################
 
 def load_stigler_data(verbose=False):
```

