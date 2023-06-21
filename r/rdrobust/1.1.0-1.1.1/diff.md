# Comparing `tmp/rdrobust-1.1.0.tar.gz` & `tmp/rdrobust-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rmasini/Library/CloudStorage/Dropbox/rdrobust/Python/rdrobust/dist/.tmp-fqtwfoa2/rdrobust-1.1.0.tar", last modified: Tue Jun 20 19:06:16 2023, max compression
+gzip compressed data, was "/Users/rmasini/Library/CloudStorage/Dropbox/rdrobust/Python/rdrobust/dist/.tmp-tvwevzj5/rdrobust-1.1.1.tar", last modified: Wed Jun 21 19:11:09 2023, max compression
```

## Comparing `rdrobust-1.1.0.tar` & `rdrobust-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.137838 rdrobust-1.1.0/
--rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-20 19:06:16.138263 rdrobust-1.1.0/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)     5912 2021-07-26 21:54:29.000000 rdrobust-1.1.0/README.md
--rw-r--r--   0 rmasini    (501) staff       (20)      108 2022-08-11 22:11:33.000000 rdrobust-1.1.0/pyproject.toml
--rw-r--r--   0 rmasini    (501) staff       (20)      828 2023-06-20 19:06:16.140038 rdrobust-1.1.0/setup.cfg
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.119851 rdrobust-1.1.0/src/
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.130376 rdrobust-1.1.0/src/rdrobust/
--rwxr-xr-x   0 rmasini    (501) staff       (20)      142 2023-06-07 15:28:53.000000 rdrobust-1.1.0/src/rdrobust/__init__.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    18074 2023-06-07 15:14:29.000000 rdrobust-1.1.0/src/rdrobust/funs.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    27460 2023-06-07 15:50:22.000000 rdrobust-1.1.0/src/rdrobust/rdbwselect.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    30156 2023-06-07 15:50:48.000000 rdrobust-1.1.0/src/rdrobust/rdplot.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    30968 2023-06-20 03:34:30.000000 rdrobust-1.1.0/src/rdrobust/rdrobust.py
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.136754 rdrobust-1.1.0/src/rdrobust.egg-info/
--rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)      334 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/SOURCES.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/dependency_links.txt
--rw-r--r--   0 rmasini    (501) staff       (20)       55 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/requires.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        9 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/top_level.txt
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 19:11:09.166081 rdrobust-1.1.1/
+-rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-21 19:11:09.166315 rdrobust-1.1.1/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)     5912 2021-07-26 21:54:29.000000 rdrobust-1.1.1/README.md
+-rw-r--r--   0 rmasini    (501) staff       (20)      108 2022-08-11 22:11:33.000000 rdrobust-1.1.1/pyproject.toml
+-rw-r--r--   0 rmasini    (501) staff       (20)      828 2023-06-21 19:11:09.167258 rdrobust-1.1.1/setup.cfg
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 19:11:09.153332 rdrobust-1.1.1/src/
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 19:11:09.160891 rdrobust-1.1.1/src/rdrobust/
+-rwxr-xr-x   0 rmasini    (501) staff       (20)      142 2023-06-07 15:28:53.000000 rdrobust-1.1.1/src/rdrobust/__init__.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    18074 2023-06-07 15:14:29.000000 rdrobust-1.1.1/src/rdrobust/funs.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    27475 2023-06-21 19:02:24.000000 rdrobust-1.1.1/src/rdrobust/rdbwselect.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    30199 2023-06-21 19:09:39.000000 rdrobust-1.1.1/src/rdrobust/rdplot.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    30983 2023-06-21 19:03:11.000000 rdrobust-1.1.1/src/rdrobust/rdrobust.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 19:11:09.165575 rdrobust-1.1.1/src/rdrobust.egg-info/
+-rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-21 19:11:09.000000 rdrobust-1.1.1/src/rdrobust.egg-info/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)      334 2023-06-21 19:11:09.000000 rdrobust-1.1.1/src/rdrobust.egg-info/SOURCES.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-21 19:11:09.000000 rdrobust-1.1.1/src/rdrobust.egg-info/dependency_links.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)       55 2023-06-21 19:11:09.000000 rdrobust-1.1.1/src/rdrobust.egg-info/requires.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        9 2023-06-21 19:11:09.000000 rdrobust-1.1.1/src/rdrobust.egg-info/top_level.txt
```

### Comparing `rdrobust-1.1.0/PKG-INFO` & `rdrobust-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdrobust
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 Home-page: https://github.com/rdpackages/rdrobust
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdrobust/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rdrobust-1.1.0/README.md` & `rdrobust-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rdrobust-1.1.0/setup.cfg` & `rdrobust-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rdrobust
-version = 1.1.0
+version = 1.1.1
 author = Ricardo Masini
 author_email = rmasini@princeton.edu
 description = Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rdpackages/rdrobust
 project_urls =
```

### Comparing `rdrobust-1.1.0/src/rdrobust/funs.py` & `rdrobust-1.1.1/src/rdrobust/funs.py`

 * *Files identical despite different names*

### Comparing `rdrobust-1.1.0/src/rdrobust/rdbwselect.py` & `rdrobust-1.1.1/src/rdrobust/rdbwselect.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             fuzzy = np.array(fuzzy).reshape(-1,1)
             if subset is not None: fuzzy = fuzzy[subset]
             na_ok = na_ok & complete_cases(fuzzy)
       
         if weights is not None:
             weights = np.array(weights).reshape(-1,1)
             if subset is not None: weights = weights[subset]
-            na_ok = na_ok & complete_cases(weights) & weights>=0
+            na_ok = na_ok & complete_cases(weights) & (weights>=0).reshape(-1,)
         
         x = x[na_ok]
         y = y[na_ok]
     
         if covs is not None: covs = covs[na_ok,:]
         if fuzzy is not None: fuzzy   = fuzzy[na_ok]
         if cluster is not None: cluster = cluster[na_ok]
```

### Comparing `rdrobust-1.1.0/src/rdrobust/rdplot.py` & `rdrobust-1.1.1/src/rdrobust/rdplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         if subset is not None: covs = covs[subset,:]
         na_ok = na_ok & complete_cases(covs)
     
     if weights is not None:
         weights = np.array(weights).reshape(-1,1)
         if subset is not None:
             weights = weights[subset]
-        na_ok = na_ok & complete_cases(weights) & weights>=0
+        na_ok = na_ok & complete_cases(weights) & (weights>=0).reshape(-1,)
         
     x = x[na_ok]
     y = y[na_ok]    
     
     if covs is not None: covs = covs[na_ok,:]
     if weights is not None: weights = weights[na_ok]
     
@@ -355,16 +355,16 @@
     W_h_l = rdrobust_kweight(x_l,c,h_l,kernel).reshape(-1,1)
     W_h_r = rdrobust_kweight(x_r,c,h_r,kernel).reshape(-1,1)
 	
     n_h_l = np.sum(W_h_l>0)
     n_h_r = np.sum(W_h_r>0)
 	
     if weights is not None:
-        fw_l = weights[x<c]
-        fw_r = weights[x>=c]
+        fw_l = weights[x<c].reshape(-1,1)
+        fw_r = weights[x>=c].reshape(-1,1)
         W_h_l = fw_l*W_h_l
         W_h_r = fw_r*W_h_r
 	
     invG_p_l  = qrXXinv(np.sqrt(W_h_l)*R_p_l)
     invG_p_r  = qrXXinv(np.sqrt(W_h_r)*R_p_r)
 	
     if covs is None:
```

### Comparing `rdrobust-1.1.0/src/rdrobust/rdrobust.py` & `rdrobust-1.1.1/src/rdrobust/rdrobust.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
             fuzzy = fuzzy[subset]
         na_ok = na_ok & complete_cases(fuzzy)
   
     if weights is not None:
         weights = np.array(weights).reshape(-1,1)
         if subset is not None:
             weights = weights[subset]
-        na_ok = na_ok & complete_cases(weights) & weights>=0
+        na_ok = na_ok & complete_cases(weights) & (weights>=0).reshape(-1,)
     
     x = x[na_ok]
     y = y[na_ok]
     
     if covs is not None: covs = covs[na_ok,:]
     if fuzzy is not None: fuzzy   = fuzzy[na_ok]
     if cluster is not None: cluster = cluster[na_ok]
```

### Comparing `rdrobust-1.1.0/src/rdrobust.egg-info/PKG-INFO` & `rdrobust-1.1.1/src/rdrobust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdrobust
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 Home-page: https://github.com/rdpackages/rdrobust
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdrobust/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

