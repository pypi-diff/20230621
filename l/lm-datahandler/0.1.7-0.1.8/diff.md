# Comparing `tmp/lm_datahandler-0.1.7.tar.gz` & `tmp/lm_datahandler-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_datahandler-0.1.7.tar", last modified: Wed Jun 21 02:56:46 2023, max compression
+gzip compressed data, was "lm_datahandler-0.1.8.tar", last modified: Wed Jun 21 03:05:37 2023, max compression
```

## Comparing `lm_datahandler-0.1.7.tar` & `lm_datahandler-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.165796 lm_datahandler-0.1.7/
--rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      325 2023-06-21 02:56:46.165796 lm_datahandler-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.146782 lm_datahandler-0.1.7/lm_datahandler/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.7/lm_datahandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.154397 lm_datahandler-0.1.7/lm_datahandler/data_download/
--rw-rw-rw-   0        0        0        0 2023-06-20 07:02:42.000000 lm_datahandler-0.1.7/lm_datahandler/data_download/__init__.py
--rw-rw-rw-   0        0        0     3008 2023-06-20 07:59:35.000000 lm_datahandler-0.1.7/lm_datahandler/data_download/data_download.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.155403 lm_datahandler-0.1.7/lm_datahandler/data_load/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.7/lm_datahandler/data_load/__init__.py
--rw-rw-rw-   0        0        0     2026 2023-06-20 07:11:38.000000 lm_datahandler-0.1.7/lm_datahandler/data_load/data_loader.py
--rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.7/lm_datahandler/data_load/loaders.py
--rw-rw-rw-   0        0        0    24249 2023-06-20 03:21:12.000000 lm_datahandler-0.1.7/lm_datahandler/datahandler.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.159363 lm_datahandler-0.1.7/lm_datahandler/functions/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.7/lm_datahandler/functions/__init__.py
--rw-rw-rw-   0        0        0    33356 2023-06-21 02:52:28.000000 lm_datahandler-0.1.7/lm_datahandler/functions/biomarker.py
--rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.7/lm_datahandler/functions/feature_extract.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.7/lm_datahandler/functions/os_detect.py
--rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.7/lm_datahandler/functions/posture_analyse.py
--rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.7/lm_datahandler/functions/sleep_staging.py
--rw-rw-rw-   0        0        0     3828 2023-06-19 09:29:10.000000 lm_datahandler-0.1.7/lm_datahandler/functions/sleep_variable_compute.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.7/lm_datahandler/functions/spindle_detect.py
--rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.7/lm_datahandler/functions/wear_detect.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.159877 lm_datahandler-0.1.7/lm_datahandler/models/
--rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.7/lm_datahandler/models/wear_detection_1s.txt
--rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.7/lm_datahandler/models/wholenight_sleep_staging.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.162252 lm_datahandler-0.1.7/lm_datahandler/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.7/lm_datahandler/plots/__init__.py
--rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.7/lm_datahandler/plots/biomarker_plot.py
--rw-rw-rw-   0        0        0     6763 2023-06-19 08:57:14.000000 lm_datahandler-0.1.7/lm_datahandler/plots/sleep_staging_plot.py
--rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.7/lm_datahandler/plots/stim_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.163520 lm_datahandler-0.1.7/lm_datahandler/postprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.7/lm_datahandler/postprocess/__init__.py
--rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.7/lm_datahandler/postprocess/label_smooth.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.164334 lm_datahandler-0.1.7/lm_datahandler/preprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.7/lm_datahandler/preprocess/__init__.py
--rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.7/lm_datahandler/preprocess/filter.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.7/lm_datahandler/preprocess/tailor.py
--rw-rw-rw-   0        0        0     4743 2023-06-21 02:56:05.000000 lm_datahandler-0.1.7/lm_datahandler/scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.165232 lm_datahandler-0.1.7/lm_datahandler/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.7/lm_datahandler/utils/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.7/lm_datahandler/utils/numba_func.py
-drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.153507 lm_datahandler-0.1.7/lm_datahandler.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 02:56:46.166457 lm_datahandler-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-06-21 02:56:42.000000 lm_datahandler-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.648739 lm_datahandler-0.1.8/
+-rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      325 2023-06-21 03:05:37.648739 lm_datahandler-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.626570 lm_datahandler-0.1.8/lm_datahandler/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.8/lm_datahandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.635918 lm_datahandler-0.1.8/lm_datahandler/data_download/
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:02:42.000000 lm_datahandler-0.1.8/lm_datahandler/data_download/__init__.py
+-rw-rw-rw-   0        0        0     3008 2023-06-20 07:59:35.000000 lm_datahandler-0.1.8/lm_datahandler/data_download/data_download.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.639001 lm_datahandler-0.1.8/lm_datahandler/data_load/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.8/lm_datahandler/data_load/__init__.py
+-rw-rw-rw-   0        0        0     2026 2023-06-20 07:11:38.000000 lm_datahandler-0.1.8/lm_datahandler/data_load/data_loader.py
+-rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.8/lm_datahandler/data_load/loaders.py
+-rw-rw-rw-   0        0        0    24249 2023-06-20 03:21:12.000000 lm_datahandler-0.1.8/lm_datahandler/datahandler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.642013 lm_datahandler-0.1.8/lm_datahandler/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.8/lm_datahandler/functions/__init__.py
+-rw-rw-rw-   0        0        0    33356 2023-06-21 02:52:28.000000 lm_datahandler-0.1.8/lm_datahandler/functions/biomarker.py
+-rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.8/lm_datahandler/functions/feature_extract.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.8/lm_datahandler/functions/os_detect.py
+-rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.8/lm_datahandler/functions/posture_analyse.py
+-rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.8/lm_datahandler/functions/sleep_staging.py
+-rw-rw-rw-   0        0        0     3828 2023-06-19 09:29:10.000000 lm_datahandler-0.1.8/lm_datahandler/functions/sleep_variable_compute.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.8/lm_datahandler/functions/spindle_detect.py
+-rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.8/lm_datahandler/functions/wear_detect.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.643052 lm_datahandler-0.1.8/lm_datahandler/models/
+-rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.8/lm_datahandler/models/wear_detection_1s.txt
+-rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.8/lm_datahandler/models/wholenight_sleep_staging.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.644792 lm_datahandler-0.1.8/lm_datahandler/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.8/lm_datahandler/plots/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.8/lm_datahandler/plots/biomarker_plot.py
+-rw-rw-rw-   0        0        0     6763 2023-06-19 08:57:14.000000 lm_datahandler-0.1.8/lm_datahandler/plots/sleep_staging_plot.py
+-rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.8/lm_datahandler/plots/stim_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.645798 lm_datahandler-0.1.8/lm_datahandler/postprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.8/lm_datahandler/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.8/lm_datahandler/postprocess/label_smooth.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.647519 lm_datahandler-0.1.8/lm_datahandler/preprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.8/lm_datahandler/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.8/lm_datahandler/preprocess/filter.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.8/lm_datahandler/preprocess/tailor.py
+-rw-rw-rw-   0        0        0     4843 2023-06-21 03:05:18.000000 lm_datahandler-0.1.8/lm_datahandler/scripts.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.648201 lm_datahandler-0.1.8/lm_datahandler/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.8/lm_datahandler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.8/lm_datahandler/utils/numba_func.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.634953 lm_datahandler-0.1.8/lm_datahandler.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:05:37.648739 lm_datahandler-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-06-21 03:05:22.000000 lm_datahandler-0.1.8/setup.py
```

### Comparing `lm_datahandler-0.1.7/LICENSE` & `lm_datahandler-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/data_download/data_download.py` & `lm_datahandler-0.1.8/lm_datahandler/data_download/data_download.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/data_load/data_loader.py` & `lm_datahandler-0.1.8/lm_datahandler/data_load/data_loader.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/data_load/loaders.py` & `lm_datahandler-0.1.8/lm_datahandler/data_load/loaders.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/datahandler.py` & `lm_datahandler-0.1.8/lm_datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/functions/biomarker.py` & `lm_datahandler-0.1.8/lm_datahandler/functions/biomarker.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/functions/feature_extract.py` & `lm_datahandler-0.1.8/lm_datahandler/functions/feature_extract.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/functions/posture_analyse.py` & `lm_datahandler-0.1.8/lm_datahandler/functions/posture_analyse.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/functions/sleep_staging.py` & `lm_datahandler-0.1.8/lm_datahandler/functions/sleep_staging.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/functions/sleep_variable_compute.py` & `lm_datahandler-0.1.8/lm_datahandler/functions/sleep_variable_compute.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/functions/wear_detect.py` & `lm_datahandler-0.1.8/lm_datahandler/functions/wear_detect.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/models/wear_detection_1s.txt` & `lm_datahandler-0.1.8/lm_datahandler/models/wear_detection_1s.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/models/wholenight_sleep_staging.txt` & `lm_datahandler-0.1.8/lm_datahandler/models/wholenight_sleep_staging.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/plots/biomarker_plot.py` & `lm_datahandler-0.1.8/lm_datahandler/plots/biomarker_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/plots/sleep_staging_plot.py` & `lm_datahandler-0.1.8/lm_datahandler/plots/sleep_staging_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/plots/stim_plot.py` & `lm_datahandler-0.1.8/lm_datahandler/plots/stim_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/postprocess/label_smooth.py` & `lm_datahandler-0.1.8/lm_datahandler/postprocess/label_smooth.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/preprocess/filter.py` & `lm_datahandler-0.1.8/lm_datahandler/preprocess/filter.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler/scripts.py` & `lm_datahandler-0.1.8/lm_datahandler/scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
             print("data: \"{}\" not found, skipped.")
             continue
         data_handler = DataHandler()
 
         data_path = os.path.join(dir_path, data_name)
 
         data_analysis_save_path = os.path.join(analysis_save_path, data_name)
+        if os.path.exists(data_analysis_save_path):
+            os.mkdir(data_analysis_save_path)
         sleep_fig_save_path = os.path.join(data_analysis_save_path, "sleep_fig.png")
         slow_wave_stim_sham_plot = os.path.join(data_analysis_save_path, "sw_stim_sham_fig.png")
 
         slow_wave_excel_save_path = os.path.join(data_analysis_save_path, "sw.csv")
         spindle_excel_save_path = os.path.join(data_analysis_save_path, "sp.csv")
 
         # 数据加载
```

### Comparing `lm_datahandler-0.1.7/lm_datahandler/utils/numba_func.py` & `lm_datahandler-0.1.8/lm_datahandler/utils/numba_func.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/lm_datahandler.egg-info/SOURCES.txt` & `lm_datahandler-0.1.8/lm_datahandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.7/setup.py` & `lm_datahandler-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lm_datahandler',
-    version = '0.1.7',
+    version = '0.1.8',
     keywords='eeg sleep staging analysis',
     description = 'a python analyse tool for LM Data Recorder data',
     license = 'MIT License',
     url = 'https://github.com/zx950618/lm_datahandler',
     author = 'Eric Zheng',
     author_email = '1248471980@qq.com',
     packages = find_packages(),
```

