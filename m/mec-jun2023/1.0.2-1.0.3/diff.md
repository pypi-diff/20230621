# Comparing `tmp/mec_jun2023-1.0.2.tar.gz` & `tmp/mec_jun2023-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mec_jun2023-1.0.2.tar", last modified: Wed Jun 21 12:36:43 2023, max compression
+gzip compressed data, was "mec_jun2023-1.0.3.tar", last modified: Wed Jun 21 12:39:39 2023, max compression
```

## Comparing `mec_jun2023-1.0.2.tar` & `mec_jun2023-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:36:43.070291 mec_jun2023-1.0.2/
--rw-r--r--   0 antoine    (501) staff       (20)    35138 2023-06-21 09:21:00.000000 mec_jun2023-1.0.2/LICENSE
--rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:36:43.070195 mec_jun2023-1.0.2/PKG-INFO
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:36:43.070025 mec_jun2023-1.0.2/mec_jun2023.egg-info/
--rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:36:43.000000 mec_jun2023-1.0.2/mec_jun2023.egg-info/PKG-INFO
--rw-r--r--   0 antoine    (501) staff       (20)      168 2023-06-21 12:36:43.000000 mec_jun2023-1.0.2/mec_jun2023.egg-info/SOURCES.txt
--rw-r--r--   0 antoine    (501) staff       (20)        1 2023-06-21 12:36:43.000000 mec_jun2023-1.0.2/mec_jun2023.egg-info/dependency_links.txt
--rw-r--r--   0 antoine    (501) staff       (20)        9 2023-06-21 12:36:43.000000 mec_jun2023-1.0.2/mec_jun2023.egg-info/top_level.txt
--rw-r--r--   0 antoine    (501) staff       (20)     7672 2023-06-21 12:36:12.000000 mec_jun2023-1.0.2/pymec_lp.py
--rw-r--r--   0 antoine    (501) staff       (20)       38 2023-06-21 12:36:43.070326 mec_jun2023-1.0.2/setup.cfg
--rw-r--r--   0 antoine    (501) staff       (20)      340 2023-06-21 12:36:20.000000 mec_jun2023-1.0.2/setup.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:39:39.131891 mec_jun2023-1.0.3/
+-rw-r--r--   0 antoine    (501) staff       (20)    35138 2023-06-21 09:21:00.000000 mec_jun2023-1.0.3/LICENSE
+-rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:39:39.131789 mec_jun2023-1.0.3/PKG-INFO
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:39:39.131624 mec_jun2023-1.0.3/mec_jun2023.egg-info/
+-rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/PKG-INFO
+-rw-r--r--   0 antoine    (501) staff       (20)      168 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        1 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        9 2023-06-21 12:39:39.000000 mec_jun2023-1.0.3/mec_jun2023.egg-info/top_level.txt
+-rw-r--r--   0 antoine    (501) staff       (20)     7508 2023-06-21 12:39:21.000000 mec_jun2023-1.0.3/pymec_lp.py
+-rw-r--r--   0 antoine    (501) staff       (20)       38 2023-06-21 12:39:39.131926 mec_jun2023-1.0.3/setup.cfg
+-rw-r--r--   0 antoine    (501) staff       (20)      340 2023-06-21 12:39:26.000000 mec_jun2023-1.0.3/setup.py
```

### Comparing `mec_jun2023-1.0.2/LICENSE` & `mec_jun2023-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mec_jun2023-1.0.2/pymec_lp.py` & `mec_jun2023-1.0.3/pymec_lp.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,16 @@
 
 
 #########################
 # LP2: The simplex algorithm #
 #########################
 
 def round_expr(expr, num_digits):
-    #---
-    #description of the function
-    #arg:
-    #   expr: meaning
-    #   num_digits: meaning
-    #return:
-    #   expr.xreplace: meaning & type
-    #---
     return expr.xreplace({n : round(n, num_digits) for n in expr.atoms(Number)})
 
-
-
 class Tableau():
     def __init__(self, names_basic, names_nonbasic, A_i_j, b_i, c_j): # z = d - A @ x
         self.nonbasic = list(symbols(names_nonbasic))
         self.base = { Symbol('obj') : c_j @ self.nonbasic }
         self.base.update( { list(symbols(names_basic))[i]: b_i[i]  - (A_i_j @ self.nonbasic)[i] for i in range(len(b_i))} )
 
     def variables(self):
```

