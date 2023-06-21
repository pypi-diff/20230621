# Comparing `tmp/ShapeYModular-2.0.0.tar.gz` & `tmp/ShapeYModular-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShapeYModular-2.0.0.tar", last modified: Wed Jun 21 20:37:11 2023, max compression
+gzip compressed data, was "ShapeYModular-2.0.1.tar", last modified: Wed Jun 21 20:54:35 2023, max compression
```

## Comparing `ShapeYModular-2.0.0.tar` & `ShapeYModular-2.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.645437 ShapeYModular-2.0.0/
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1062 2023-06-21 20:35:32.000000 ShapeYModular-2.0.0/LICENSE
--rw-r--r--   0 namj      (1007) dcuser    (1001)      461 2023-06-21 20:37:11.645437 ShapeYModular-2.0.0/PKG-INFO
--rw-r--r--   0 namj      (1007) dcuser    (1001)       37 2023-04-04 21:05:58.000000 ShapeYModular-2.0.0/README.md
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.637437 ShapeYModular-2.0.0/ShapeYModular.egg-info/
--rw-r--r--   0 namj      (1007) dcuser    (1001)      461 2023-06-21 20:37:11.000000 ShapeYModular-2.0.0/ShapeYModular.egg-info/PKG-INFO
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1556 2023-06-21 20:37:11.000000 ShapeYModular-2.0.0/ShapeYModular.egg-info/SOURCES.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-06-21 20:37:11.000000 ShapeYModular-2.0.0/ShapeYModular.egg-info/dependency_links.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)      151 2023-06-21 20:37:11.000000 ShapeYModular-2.0.0/ShapeYModular.egg-info/requires.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)       14 2023-06-21 20:37:11.000000 ShapeYModular-2.0.0/ShapeYModular.egg-info/top_level.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)       38 2023-06-21 20:37:11.645437 ShapeYModular-2.0.0/setup.cfg
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1144 2023-06-21 20:35:16.000000 ShapeYModular-2.0.0/setup.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.637437 ShapeYModular-2.0.0/shapeymodular/
--rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-05-23 22:20:02.000000 ShapeYModular-2.0.0/shapeymodular/__init__.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.637437 ShapeYModular-2.0.0/shapeymodular/analysis/
--rw-r--r--   0 namj      (1007) dcuser    (1001)       80 2023-06-09 17:43:22.000000 ShapeYModular-2.0.0/shapeymodular/analysis/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    26181 2023-06-13 18:09:42.000000 ShapeYModular-2.0.0/shapeymodular/analysis/nn_analysis.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    41776 2023-06-21 17:19:46.000000 ShapeYModular-2.0.0/shapeymodular/analysis/postprocess.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      723 2023-06-05 17:13:26.000000 ShapeYModular-2.0.0/shapeymodular/analysis/preprocess.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.641437 ShapeYModular-2.0.0/shapeymodular/data_classes/
--rw-r--r--   0 namj      (1007) dcuser    (1001)      116 2023-06-06 15:58:15.000000 ShapeYModular-2.0.0/shapeymodular/data_classes/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4190 2023-05-26 18:10:32.000000 ShapeYModular-2.0.0/shapeymodular/data_classes/axis_description.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1840 2023-05-26 18:09:35.000000 ShapeYModular-2.0.0/shapeymodular/data_classes/corrmat.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4573 2023-06-20 00:51:00.000000 ShapeYModular-2.0.0/shapeymodular/data_classes/graph_data.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1630 2023-05-26 18:20:11.000000 ShapeYModular-2.0.0/shapeymodular/data_classes/nn_analysis_configs.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.641437 ShapeYModular-2.0.0/shapeymodular/data_loader/
--rw-r--r--   0 namj      (1007) dcuser    (1001)       69 2023-05-26 18:05:58.000000 ShapeYModular-2.0.0/shapeymodular/data_loader/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      976 2023-06-02 17:07:40.000000 ShapeYModular-2.0.0/shapeymodular/data_loader/data_loader.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4804 2023-05-26 18:11:03.000000 ShapeYModular-2.0.0/shapeymodular/data_loader/dir_mat.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     7236 2023-06-06 18:12:07.000000 ShapeYModular-2.0.0/shapeymodular/data_loader/hdf.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.641437 ShapeYModular-2.0.0/shapeymodular/macros/
--rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-25 19:17:00.000000 ShapeYModular-2.0.0/shapeymodular/macros/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1615 2023-06-19 23:27:33.000000 ShapeYModular-2.0.0/shapeymodular/macros/compute_distance.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2307 2023-05-26 17:31:55.000000 ShapeYModular-2.0.0/shapeymodular/macros/compute_threshold.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    14772 2023-06-21 20:07:14.000000 ShapeYModular-2.0.0/shapeymodular/macros/graphing.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     9393 2023-06-21 19:56:24.000000 ShapeYModular-2.0.0/shapeymodular/macros/nn_batch.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.641437 ShapeYModular-2.0.0/shapeymodular/test/
--rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-23 22:19:39.000000 ShapeYModular-2.0.0/shapeymodular/test/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      230 2023-06-08 19:49:41.000000 ShapeYModular-2.0.0/shapeymodular/test/conftest.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.641437 ShapeYModular-2.0.0/shapeymodular/utils/
--rw-r--r--   0 namj      (1007) dcuser    (1001)      113 2023-06-07 19:38:27.000000 ShapeYModular-2.0.0/shapeymodular/utils/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      501 2023-05-25 21:00:16.000000 ShapeYModular-2.0.0/shapeymodular/utils/cmdtools.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2735 2023-06-21 19:30:05.000000 ShapeYModular-2.0.0/shapeymodular/utils/constants.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     3443 2023-06-13 15:27:47.000000 ShapeYModular-2.0.0/shapeymodular/utils/image_name_helper.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     3407 2023-06-09 19:12:08.000000 ShapeYModular-2.0.0/shapeymodular/utils/indexing_helper.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:37:11.645437 ShapeYModular-2.0.0/shapeymodular/visualization/
--rw-r--r--   0 namj      (1007) dcuser    (1001)      130 2023-06-20 20:45:00.000000 ShapeYModular-2.0.0/shapeymodular/visualization/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     5456 2023-05-26 16:58:09.000000 ShapeYModular-2.0.0/shapeymodular/visualization/correlation_fall_off.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1385 2023-06-20 18:39:52.000000 ShapeYModular-2.0.0/shapeymodular/visualization/exclusion_distance.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2987 2023-06-20 16:43:06.000000 ShapeYModular-2.0.0/shapeymodular/visualization/histogram.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4167 2023-06-21 15:24:06.000000 ShapeYModular-2.0.0/shapeymodular/visualization/image.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    38608 2023-05-26 16:58:09.000000 ShapeYModular-2.0.0/shapeymodular/visualization/image_panel.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2843 2023-06-20 16:41:54.000000 ShapeYModular-2.0.0/shapeymodular/visualization/line_graph.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1074 2023-06-21 02:34:42.000000 ShapeYModular-2.0.0/shapeymodular/visualization/styles.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1226 2023-06-20 18:51:46.000000 ShapeYModular-2.0.0/shapeymodular/visualization/tuning_curve.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1062 2023-06-21 20:35:32.000000 ShapeYModular-2.0.1/LICENSE
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2018 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/PKG-INFO
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1595 2023-06-21 20:54:22.000000 ShapeYModular-2.0.1/README.md
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.183731 ShapeYModular-2.0.1/ShapeYModular.egg-info/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2018 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/PKG-INFO
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1556 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/SOURCES.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/dependency_links.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      151 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/requires.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       14 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/top_level.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       38 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/setup.cfg
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1144 2023-06-21 20:54:29.000000 ShapeYModular-2.0.1/setup.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-05-23 22:20:02.000000 ShapeYModular-2.0.1/shapeymodular/__init__.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/analysis/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       80 2023-06-09 17:43:22.000000 ShapeYModular-2.0.1/shapeymodular/analysis/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)    26181 2023-06-13 18:09:42.000000 ShapeYModular-2.0.1/shapeymodular/analysis/nn_analysis.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)    41776 2023-06-21 17:19:46.000000 ShapeYModular-2.0.1/shapeymodular/analysis/postprocess.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      723 2023-06-05 17:13:26.000000 ShapeYModular-2.0.1/shapeymodular/analysis/preprocess.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/data_classes/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      116 2023-06-06 15:58:15.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4190 2023-05-26 18:10:32.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/axis_description.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1840 2023-05-26 18:09:35.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/corrmat.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4573 2023-06-20 00:51:00.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/graph_data.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1630 2023-05-26 18:20:11.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/nn_analysis_configs.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/data_loader/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       69 2023-05-26 18:05:58.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      976 2023-06-02 17:07:40.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/data_loader.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4804 2023-05-26 18:11:03.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/dir_mat.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     7236 2023-06-06 18:12:07.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/hdf.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/macros/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-25 19:17:00.000000 ShapeYModular-2.0.1/shapeymodular/macros/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1615 2023-06-19 23:27:33.000000 ShapeYModular-2.0.1/shapeymodular/macros/compute_distance.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2307 2023-05-26 17:31:55.000000 ShapeYModular-2.0.1/shapeymodular/macros/compute_threshold.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)    14772 2023-06-21 20:07:14.000000 ShapeYModular-2.0.1/shapeymodular/macros/graphing.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     9393 2023-06-21 19:56:24.000000 ShapeYModular-2.0.1/shapeymodular/macros/nn_batch.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/test/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-23 22:19:39.000000 ShapeYModular-2.0.1/shapeymodular/test/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      230 2023-06-08 19:49:41.000000 ShapeYModular-2.0.1/shapeymodular/test/conftest.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/utils/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      113 2023-06-07 19:38:27.000000 ShapeYModular-2.0.1/shapeymodular/utils/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      501 2023-05-25 21:00:16.000000 ShapeYModular-2.0.1/shapeymodular/utils/cmdtools.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2735 2023-06-21 19:30:05.000000 ShapeYModular-2.0.1/shapeymodular/utils/constants.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     3443 2023-06-13 15:27:47.000000 ShapeYModular-2.0.1/shapeymodular/utils/image_name_helper.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     3407 2023-06-09 19:12:08.000000 ShapeYModular-2.0.1/shapeymodular/utils/indexing_helper.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/shapeymodular/visualization/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      130 2023-06-20 20:45:00.000000 ShapeYModular-2.0.1/shapeymodular/visualization/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     5456 2023-05-26 16:58:09.000000 ShapeYModular-2.0.1/shapeymodular/visualization/correlation_fall_off.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1385 2023-06-20 18:39:52.000000 ShapeYModular-2.0.1/shapeymodular/visualization/exclusion_distance.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2987 2023-06-20 16:43:06.000000 ShapeYModular-2.0.1/shapeymodular/visualization/histogram.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4167 2023-06-21 20:42:03.000000 ShapeYModular-2.0.1/shapeymodular/visualization/image.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)    38608 2023-05-26 16:58:09.000000 ShapeYModular-2.0.1/shapeymodular/visualization/image_panel.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2843 2023-06-20 16:41:54.000000 ShapeYModular-2.0.1/shapeymodular/visualization/line_graph.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1076 2023-06-21 20:49:59.000000 ShapeYModular-2.0.1/shapeymodular/visualization/styles.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1226 2023-06-20 18:51:46.000000 ShapeYModular-2.0.1/shapeymodular/visualization/tuning_curve.py
```

### Comparing `ShapeYModular-2.0.0/LICENSE` & `ShapeYModular-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/ShapeYModular.egg-info/SOURCES.txt` & `ShapeYModular-2.0.1/ShapeYModular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/setup.py` & `ShapeYModular-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Development Status :: 4 - Beta",
 ]
 
 # calling the setup function
 # TODO: separate dev / test / deploy setup with options
 setuptools.setup(
     name="ShapeYModular",
-    version="2.0.0",
+    version="2.0.1",
     description="Benchmark that tests shape recognition",
     long_description=long_description,
     url="https://github.com/njw0709/ShapeYV2",
     author="Jong Woo Nam",
     author_email="namj@usc.edu",
     license="MIT",
     packages=setuptools.find_packages(),
```

### Comparing `ShapeYModular-2.0.0/shapeymodular/analysis/nn_analysis.py` & `ShapeYModular-2.0.1/shapeymodular/analysis/nn_analysis.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/analysis/postprocess.py` & `ShapeYModular-2.0.1/shapeymodular/analysis/postprocess.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/analysis/preprocess.py` & `ShapeYModular-2.0.1/shapeymodular/analysis/preprocess.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/data_classes/axis_description.py` & `ShapeYModular-2.0.1/shapeymodular/data_classes/axis_description.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/data_classes/corrmat.py` & `ShapeYModular-2.0.1/shapeymodular/data_classes/corrmat.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/data_classes/graph_data.py` & `ShapeYModular-2.0.1/shapeymodular/data_classes/graph_data.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/data_classes/nn_analysis_configs.py` & `ShapeYModular-2.0.1/shapeymodular/data_classes/nn_analysis_configs.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/data_loader/data_loader.py` & `ShapeYModular-2.0.1/shapeymodular/data_loader/data_loader.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/data_loader/dir_mat.py` & `ShapeYModular-2.0.1/shapeymodular/data_loader/dir_mat.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/data_loader/hdf.py` & `ShapeYModular-2.0.1/shapeymodular/data_loader/hdf.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/macros/compute_distance.py` & `ShapeYModular-2.0.1/shapeymodular/macros/compute_distance.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/macros/compute_threshold.py` & `ShapeYModular-2.0.1/shapeymodular/macros/compute_threshold.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/macros/graphing.py` & `ShapeYModular-2.0.1/shapeymodular/macros/graphing.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/macros/nn_batch.py` & `ShapeYModular-2.0.1/shapeymodular/macros/nn_batch.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/utils/constants.py` & `ShapeYModular-2.0.1/shapeymodular/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/utils/image_name_helper.py` & `ShapeYModular-2.0.1/shapeymodular/utils/image_name_helper.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/utils/indexing_helper.py` & `ShapeYModular-2.0.1/shapeymodular/utils/indexing_helper.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/correlation_fall_off.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/correlation_fall_off.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/exclusion_distance.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/exclusion_distance.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/histogram.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/histogram.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/image.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/image.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/image_panel.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/image_panel.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/line_graph.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/line_graph.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/styles.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/styles.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 BLANK_IMG = os.path.join(os.path.dirname(__file__), "blank.png")
 MARKER_STYLES = [m for m in markers.MarkerStyle.markers if m not in ["None", "none"]]
 COLORS = cm.get_cmap("tab20", 20)
 LINE_STYLES = ["-", "--", "-.", ":"]
 LABEL_FONT_SIZE = 15
 TITLE_FONT_SIZE = 17
 TICK_FONT_SIZE = 15
-SHAPEY_IMG_DIR = "/home/namj/projects/ShapeYAnalysis/data/ShapeY200/dataset/"
+SHAPEY_IMG_DIR = os.environ.get("SHAPEY_IMG_DIR", "../data/ShapeY200/dataset/")
 ANNOTATION_FONT_SIZE = 7
 CORRECT_MATCH_COLOR = "blue"
 CORRECT_MATCH_BORDER_WIDTH = 4
 
 
 def format_xdist_graph(
     fig: mplfig.Figure, ax: mplax.Axes
```

### Comparing `ShapeYModular-2.0.0/shapeymodular/visualization/tuning_curve.py` & `ShapeYModular-2.0.1/shapeymodular/visualization/tuning_curve.py`

 * *Files identical despite different names*

