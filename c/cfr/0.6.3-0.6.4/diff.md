# Comparing `tmp/cfr-0.6.3.tar.gz` & `tmp/cfr-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.6.3.tar", last modified: Tue Jun 20 23:47:31 2023, max compression
+gzip compressed data, was "cfr-0.6.4.tar", last modified: Wed Jun 21 18:27:14 2023, max compression
```

## Comparing `cfr-0.6.3.tar` & `cfr-0.6.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 23:47:31.400412 cfr-0.6.3/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.3/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-20 23:47:31.400229 cfr-0.6.3/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.3/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 23:47:31.392887 cfr-0.6.3/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.3/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 23:47:31.396870 cfr-0.6.3/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.6.3/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.3/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 23:47:31.399880 cfr-0.6.3/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.3/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.3/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.3/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.3/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    64854 2023-06-20 23:46:22.000000 cfr-0.6.3/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.3/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-19 02:39:39.000000 cfr-0.6.3/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.3/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.3/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26722 2023-06-20 23:08:04.000000 cfr-0.6.3/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.3/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 23:47:31.399124 cfr-0.6.3/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-20 23:47:31.000000 cfr-0.6.3/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-20 23:47:31.000000 cfr-0.6.3/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-20 23:47:31.000000 cfr-0.6.3/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.3/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-20 23:47:31.000000 cfr-0.6.3/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-20 23:47:31.000000 cfr-0.6.3/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-20 23:47:31.400473 cfr-0.6.3/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-20 23:47:01.000000 cfr-0.6.3/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.261764 cfr-0.6.4/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.4/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-21 18:27:14.261573 cfr-0.6.4/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.4/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.252684 cfr-0.6.4/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.4/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.257291 cfr-0.6.4/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-0.6.4/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.4/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.261235 cfr-0.6.4/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.4/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.4/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.4/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.4/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    64854 2023-06-21 18:25:07.000000 cfr-0.6.4/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.4/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-19 02:39:39.000000 cfr-0.6.4/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.4/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.4/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26722 2023-06-20 23:08:04.000000 cfr-0.6.4/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.4/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.260478 cfr-0.6.4/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.4/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-21 18:27:14.261824 cfr-0.6.4/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-21 18:25:41.000000 cfr-0.6.4/setup.py
```

### Comparing `cfr-0.6.3/LICENSE` & `cfr-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/PKG-INFO` & `cfr-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.3
+Version: 0.6.4
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.3/README.md` & `cfr-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/bin/cfr` & `cfr-0.6.4/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/climate.py` & `cfr-0.6.4/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/da/enkf.py` & `cfr-0.6.4/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/gcm.py` & `cfr-0.6.4/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/ml.py` & `cfr-0.6.4/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/proxy.py` & `cfr-0.6.4/cfr/proxy.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/psm.py` & `cfr-0.6.4/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/reconjob.py` & `cfr-0.6.4/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/reconres.py` & `cfr-0.6.4/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/ts.py` & `cfr-0.6.4/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/utils.py` & `cfr-0.6.4/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr/visual.py` & `cfr-0.6.4/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.3/cfr.egg-info/PKG-INFO` & `cfr-0.6.4/cfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.3
+Version: 0.6.4
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.3/setup.py` & `cfr-0.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.6.3',
+    version='0.6.4',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

