# Comparing `tmp/autogluon.features-0.8.1b20230619.tar.gz` & `tmp/autogluon.features-0.8.1b20230620.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.features-0.8.1b20230619.tar", last modified: Mon Jun 19 09:04:08 2023, max compression
+gzip compressed data, was "autogluon.features-0.8.1b20230620.tar", last modified: Tue Jun 20 09:04:07 2023, max compression
```

## Comparing `autogluon.features-0.8.1b20230619.tar` & `autogluon.features-0.8.1b20230620.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:08.176340 autogluon.features-0.8.1b20230619/
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-19 09:04:08.176340 autogluon.features-0.8.1b20230619/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:04:08.176340 autogluon.features-0.8.1b20230619/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:08.172340 autogluon.features-0.8.1b20230619/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:08.172340 autogluon.features-0.8.1b20230619/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:08.176340 autogluon.features-0.8.1b20230619/src/autogluon/features/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:08.176340 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44073 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/auto_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/drop_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/drop_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/fillna.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/isnan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/memory_minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/text_ngram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/generators/text_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-19 09:03:45.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon/features/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:08.176340 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:04:08.000000 autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:07.440264 autogluon.features-0.8.1b20230620/
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-20 09:04:07.440264 autogluon.features-0.8.1b20230620/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:04:07.440264 autogluon.features-0.8.1b20230620/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:07.436264 autogluon.features-0.8.1b20230620/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:07.436264 autogluon.features-0.8.1b20230620/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:07.436264 autogluon.features-0.8.1b20230620/src/autogluon/features/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:07.440264 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44073 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/auto_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/drop_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/drop_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/fillna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/isnan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/memory_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/text_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/generators/text_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-20 09:03:44.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon/features/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:07.436264 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:04:07.000000 autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/zip-safe
```

### Comparing `autogluon.features-0.8.1b20230619/PKG-INFO` & `autogluon.features-0.8.1b20230620/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.8.1b20230619
+Version: 0.8.1b20230620
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.features-0.8.1b20230619/setup.py` & `autogluon.features-0.8.1b20230620/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/binning.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/binning.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/__init__.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/abstract.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/astype.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/astype.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/auto_ml_pipeline.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/auto_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/binned.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/binned.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/bulk.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/bulk.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/category.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/category.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/datetime.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/drop_duplicates.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/drop_duplicates.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/drop_unique.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/drop_unique.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/dummy.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/dummy.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/fillna.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/identity.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/identity.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/isnan.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/isnan.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/label_encoder.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/memory_minimize.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/memory_minimize.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/one_hot_encoder.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/pipeline.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/rename.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/rename.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/text_ngram.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/text_ngram.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/generators/text_special.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/generators/text_special.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/utils.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon/features/vectorizers.py` & `autogluon.features-0.8.1b20230620/src/autogluon/features/vectorizers.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/PKG-INFO` & `autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.8.1b20230619
+Version: 0.8.1b20230620
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.features-0.8.1b20230619/src/autogluon.features.egg-info/SOURCES.txt` & `autogluon.features-0.8.1b20230620/src/autogluon.features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

