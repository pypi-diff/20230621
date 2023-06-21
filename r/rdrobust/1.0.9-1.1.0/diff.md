# Comparing `tmp/rdrobust-1.0.9.tar.gz` & `tmp/rdrobust-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rmasini/Dropbox/rdrobust/Python/rdrobust/dist/.tmp-eh1x9bbg/rdrobust-1.0.9.tar", last modified: Wed Jun  7 15:53:54 2023, max compression
+gzip compressed data, was "/Users/rmasini/Library/CloudStorage/Dropbox/rdrobust/Python/rdrobust/dist/.tmp-fqtwfoa2/rdrobust-1.1.0.tar", last modified: Tue Jun 20 19:06:16 2023, max compression
```

## Comparing `rdrobust-1.0.9.tar` & `rdrobust-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.696076 rdrobust-1.0.9/
--rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-07 15:53:54.696326 rdrobust-1.0.9/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)     5912 2021-07-26 21:54:29.000000 rdrobust-1.0.9/README.md
--rw-r--r--   0 rmasini    (501) staff       (20)      108 2022-08-11 22:11:33.000000 rdrobust-1.0.9/pyproject.toml
--rw-r--r--   0 rmasini    (501) staff       (20)      828 2023-06-07 15:53:54.697313 rdrobust-1.0.9/setup.cfg
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.665420 rdrobust-1.0.9/src/
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.690528 rdrobust-1.0.9/src/rdrobust/
--rwxr-xr-x   0 rmasini    (501) staff       (20)      142 2023-06-07 15:51:19.000000 rdrobust-1.0.9/src/rdrobust/__init__.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    18074 2023-06-07 15:51:02.000000 rdrobust-1.0.9/src/rdrobust/funs.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    27460 2023-06-07 15:50:22.000000 rdrobust-1.0.9/src/rdrobust/rdbwselect.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    30156 2023-06-07 15:50:48.000000 rdrobust-1.0.9/src/rdrobust/rdplot.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    30912 2023-06-07 15:50:40.000000 rdrobust-1.0.9/src/rdrobust/rdrobust.py
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.695546 rdrobust-1.0.9/src/rdrobust.egg-info/
--rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)      334 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/SOURCES.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/dependency_links.txt
--rw-r--r--   0 rmasini    (501) staff       (20)       55 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/requires.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        9 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/top_level.txt
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.137838 rdrobust-1.1.0/
+-rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-20 19:06:16.138263 rdrobust-1.1.0/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)     5912 2021-07-26 21:54:29.000000 rdrobust-1.1.0/README.md
+-rw-r--r--   0 rmasini    (501) staff       (20)      108 2022-08-11 22:11:33.000000 rdrobust-1.1.0/pyproject.toml
+-rw-r--r--   0 rmasini    (501) staff       (20)      828 2023-06-20 19:06:16.140038 rdrobust-1.1.0/setup.cfg
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.119851 rdrobust-1.1.0/src/
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.130376 rdrobust-1.1.0/src/rdrobust/
+-rwxr-xr-x   0 rmasini    (501) staff       (20)      142 2023-06-07 15:28:53.000000 rdrobust-1.1.0/src/rdrobust/__init__.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    18074 2023-06-07 15:14:29.000000 rdrobust-1.1.0/src/rdrobust/funs.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    27460 2023-06-07 15:50:22.000000 rdrobust-1.1.0/src/rdrobust/rdbwselect.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    30156 2023-06-07 15:50:48.000000 rdrobust-1.1.0/src/rdrobust/rdplot.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    30968 2023-06-20 03:34:30.000000 rdrobust-1.1.0/src/rdrobust/rdrobust.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-20 19:06:16.136754 rdrobust-1.1.0/src/rdrobust.egg-info/
+-rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)      334 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/SOURCES.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/dependency_links.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)       55 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/requires.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        9 2023-06-20 19:06:16.000000 rdrobust-1.1.0/src/rdrobust.egg-info/top_level.txt
```

### Comparing `rdrobust-1.0.9/PKG-INFO` & `rdrobust-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdrobust
-Version: 1.0.9
+Version: 1.1.0
 Summary: Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 Home-page: https://github.com/rdpackages/rdrobust
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdrobust/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rdrobust-1.0.9/README.md` & `rdrobust-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rdrobust-1.0.9/setup.cfg` & `rdrobust-1.1.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rdrobust
-version = 1.0.9
+version = 1.1.0
 author = Ricardo Masini
 author_email = rmasini@princeton.edu
 description = Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rdpackages/rdrobust
 project_urls =
```

### Comparing `rdrobust-1.0.9/src/rdrobust/funs.py` & `rdrobust-1.1.0/src/rdrobust/funs.py`

 * *Files identical despite different names*

### Comparing `rdrobust-1.0.9/src/rdrobust/rdbwselect.py` & `rdrobust-1.1.0/src/rdrobust/rdbwselect.py`

 * *Files identical despite different names*

### Comparing `rdrobust-1.0.9/src/rdrobust/rdplot.py` & `rdrobust-1.1.0/src/rdrobust/rdplot.py`

 * *Files identical despite different names*

### Comparing `rdrobust-1.0.9/src/rdrobust/rdrobust.py` & `rdrobust-1.1.0/src/rdrobust/rdrobust.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,16 @@
         y = y[subset]
     na_ok = complete_cases(x) & complete_cases(y)
     
     if cluster is not None:
         cluster = np.array(cluster).reshape(-1,1)
         if subset is not None:
             cluster = cluster[subset]
-        na_ok = na_ok & complete_cases(cluster)
+        if np.issubdtype(cluster.dtype, np.number):
+            na_ok = na_ok & complete_cases(cluster)
     
     if covs is not None:
         try: covs_names = list(covs.columns)
         except: covs_names = ['z' + str(i+1) for i in range(ncol(covs))]         
         covs = np.array(covs).reshape(len(covs),-1)  
         covs_order = np.argsort([len(i) for i in covs_names])
         covs = covs[:,covs_order]
```

### Comparing `rdrobust-1.0.9/src/rdrobust.egg-info/PKG-INFO` & `rdrobust-1.1.0/src/rdrobust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdrobust
-Version: 1.0.9
+Version: 1.1.0
 Summary: Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 Home-page: https://github.com/rdpackages/rdrobust
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdrobust/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

