# Comparing `tmp/lm_datahandler-0.1.6.tar.gz` & `tmp/lm_datahandler-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_datahandler-0.1.6.tar", last modified: Tue Jun 20 08:03:26 2023, max compression
+gzip compressed data, was "lm_datahandler-0.1.7.tar", last modified: Wed Jun 21 02:56:46 2023, max compression
```

## Comparing `lm_datahandler-0.1.6.tar` & `lm_datahandler-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.884471 lm_datahandler-0.1.6/
--rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      325 2023-06-20 08:03:26.884009 lm_datahandler-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.819170 lm_datahandler-0.1.6/lm_datahandler/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.6/lm_datahandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.831112 lm_datahandler-0.1.6/lm_datahandler/data_download/
--rw-rw-rw-   0        0        0        0 2023-06-20 07:02:42.000000 lm_datahandler-0.1.6/lm_datahandler/data_download/__init__.py
--rw-rw-rw-   0        0        0     3008 2023-06-20 07:59:35.000000 lm_datahandler-0.1.6/lm_datahandler/data_download/data_download.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.836269 lm_datahandler-0.1.6/lm_datahandler/data_load/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.6/lm_datahandler/data_load/__init__.py
--rw-rw-rw-   0        0        0     2026 2023-06-20 07:11:38.000000 lm_datahandler-0.1.6/lm_datahandler/data_load/data_loader.py
--rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.6/lm_datahandler/data_load/loaders.py
--rw-rw-rw-   0        0        0    24249 2023-06-20 03:21:12.000000 lm_datahandler-0.1.6/lm_datahandler/datahandler.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.861121 lm_datahandler-0.1.6/lm_datahandler/functions/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.6/lm_datahandler/functions/__init__.py
--rw-rw-rw-   0        0        0    31179 2023-06-14 03:24:58.000000 lm_datahandler-0.1.6/lm_datahandler/functions/biomarker.py
--rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.6/lm_datahandler/functions/feature_extract.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.6/lm_datahandler/functions/os_detect.py
--rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.6/lm_datahandler/functions/posture_analyse.py
--rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.6/lm_datahandler/functions/sleep_staging.py
--rw-rw-rw-   0        0        0     3828 2023-06-19 09:29:10.000000 lm_datahandler-0.1.6/lm_datahandler/functions/sleep_variable_compute.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.6/lm_datahandler/functions/spindle_detect.py
--rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.6/lm_datahandler/functions/wear_detect.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.861974 lm_datahandler-0.1.6/lm_datahandler/models/
--rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.6/lm_datahandler/models/wear_detection_1s.txt
--rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.6/lm_datahandler/models/wholenight_sleep_staging.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.876018 lm_datahandler-0.1.6/lm_datahandler/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.6/lm_datahandler/plots/__init__.py
--rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.6/lm_datahandler/plots/biomarker_plot.py
--rw-rw-rw-   0        0        0     6763 2023-06-19 08:57:14.000000 lm_datahandler-0.1.6/lm_datahandler/plots/sleep_staging_plot.py
--rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.6/lm_datahandler/plots/stim_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.877422 lm_datahandler-0.1.6/lm_datahandler/postprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.6/lm_datahandler/postprocess/__init__.py
--rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.6/lm_datahandler/postprocess/label_smooth.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.881456 lm_datahandler-0.1.6/lm_datahandler/preprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.6/lm_datahandler/preprocess/__init__.py
--rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.6/lm_datahandler/preprocess/filter.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.6/lm_datahandler/preprocess/tailor.py
--rw-rw-rw-   0        0        0     2553 2023-06-20 08:01:37.000000 lm_datahandler-0.1.6/lm_datahandler/scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.881769 lm_datahandler-0.1.6/lm_datahandler/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.6/lm_datahandler/utils/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.6/lm_datahandler/utils/numba_func.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:03:26.829978 lm_datahandler-0.1.6/lm_datahandler.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-20 08:03:26.000000 lm_datahandler-0.1.6/lm_datahandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2023-06-20 08:03:26.000000 lm_datahandler-0.1.6/lm_datahandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:03:26.000000 lm_datahandler-0.1.6/lm_datahandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-20 08:03:26.000000 lm_datahandler-0.1.6/lm_datahandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-20 08:03:26.000000 lm_datahandler-0.1.6/lm_datahandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 08:03:26.884471 lm_datahandler-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-06-20 08:03:08.000000 lm_datahandler-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.165796 lm_datahandler-0.1.7/
+-rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      325 2023-06-21 02:56:46.165796 lm_datahandler-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.146782 lm_datahandler-0.1.7/lm_datahandler/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.7/lm_datahandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.154397 lm_datahandler-0.1.7/lm_datahandler/data_download/
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:02:42.000000 lm_datahandler-0.1.7/lm_datahandler/data_download/__init__.py
+-rw-rw-rw-   0        0        0     3008 2023-06-20 07:59:35.000000 lm_datahandler-0.1.7/lm_datahandler/data_download/data_download.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.155403 lm_datahandler-0.1.7/lm_datahandler/data_load/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.7/lm_datahandler/data_load/__init__.py
+-rw-rw-rw-   0        0        0     2026 2023-06-20 07:11:38.000000 lm_datahandler-0.1.7/lm_datahandler/data_load/data_loader.py
+-rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.7/lm_datahandler/data_load/loaders.py
+-rw-rw-rw-   0        0        0    24249 2023-06-20 03:21:12.000000 lm_datahandler-0.1.7/lm_datahandler/datahandler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.159363 lm_datahandler-0.1.7/lm_datahandler/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.7/lm_datahandler/functions/__init__.py
+-rw-rw-rw-   0        0        0    33356 2023-06-21 02:52:28.000000 lm_datahandler-0.1.7/lm_datahandler/functions/biomarker.py
+-rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.7/lm_datahandler/functions/feature_extract.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.7/lm_datahandler/functions/os_detect.py
+-rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.7/lm_datahandler/functions/posture_analyse.py
+-rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.7/lm_datahandler/functions/sleep_staging.py
+-rw-rw-rw-   0        0        0     3828 2023-06-19 09:29:10.000000 lm_datahandler-0.1.7/lm_datahandler/functions/sleep_variable_compute.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.7/lm_datahandler/functions/spindle_detect.py
+-rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.7/lm_datahandler/functions/wear_detect.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.159877 lm_datahandler-0.1.7/lm_datahandler/models/
+-rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.7/lm_datahandler/models/wear_detection_1s.txt
+-rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.7/lm_datahandler/models/wholenight_sleep_staging.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.162252 lm_datahandler-0.1.7/lm_datahandler/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.7/lm_datahandler/plots/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.7/lm_datahandler/plots/biomarker_plot.py
+-rw-rw-rw-   0        0        0     6763 2023-06-19 08:57:14.000000 lm_datahandler-0.1.7/lm_datahandler/plots/sleep_staging_plot.py
+-rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.7/lm_datahandler/plots/stim_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.163520 lm_datahandler-0.1.7/lm_datahandler/postprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.7/lm_datahandler/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.7/lm_datahandler/postprocess/label_smooth.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.164334 lm_datahandler-0.1.7/lm_datahandler/preprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.7/lm_datahandler/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.7/lm_datahandler/preprocess/filter.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.7/lm_datahandler/preprocess/tailor.py
+-rw-rw-rw-   0        0        0     4743 2023-06-21 02:56:05.000000 lm_datahandler-0.1.7/lm_datahandler/scripts.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.165232 lm_datahandler-0.1.7/lm_datahandler/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.7/lm_datahandler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.7/lm_datahandler/utils/numba_func.py
+drwxrwxrwx   0        0        0        0 2023-06-21 02:56:46.153507 lm_datahandler-0.1.7/lm_datahandler.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 02:56:46.000000 lm_datahandler-0.1.7/lm_datahandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 02:56:46.166457 lm_datahandler-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-06-21 02:56:42.000000 lm_datahandler-0.1.7/setup.py
```

### Comparing `lm_datahandler-0.1.6/LICENSE` & `lm_datahandler-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/data_download/data_download.py` & `lm_datahandler-0.1.7/lm_datahandler/data_download/data_download.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/data_load/data_loader.py` & `lm_datahandler-0.1.7/lm_datahandler/data_load/data_loader.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/data_load/loaders.py` & `lm_datahandler-0.1.7/lm_datahandler/data_load/loaders.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/datahandler.py` & `lm_datahandler-0.1.7/lm_datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/functions/biomarker.py` & `lm_datahandler-0.1.7/lm_datahandler/functions/biomarker.py`

 * *Files 6% similar despite different names*

```diff
@@ -505,14 +505,31 @@
     # where at least two out of the three treshold were crossed.
     n_thresh = 3
     where_sp = np.where(idx_sum > (n_thresh - 1))[0]
 
     # If no events are found, skip to next channel
     if not len(where_sp):
         logging.warning("No spindle were found.")
+        return pd.DataFrame({
+            "Start_Time": [],
+            "Peak_Time": [],
+            "End_Time": [],
+            "Start_Index": [],
+            "End_Index": [],
+
+            "Duration": [],
+            "Amplitude": [],
+            "RMS": [],
+            "AbsPower": [],
+            "RelPower": [],
+            "Frequency": [],
+            "Oscillations": [],
+            "Symmetry": [],
+            # 'SOPhase': sp_cou,
+        })
 
     # Merge events that are too close
     if min_distance is not None and min_distance > 0:
         where_sp = _merge_close(where_sp, min_distance, sf)
 
     # Extract start, end, and duration of each spindle
     sp = np.split(where_sp, np.where(np.diff(where_sp) != 1)[0] + 1)
@@ -523,14 +540,31 @@
 
     # Find events with bad duration
     good_dur = np.logical_and(sp_dur > duration[0], sp_dur < duration[1])
 
     # If no events of good duration are found, skip to next channel
     if all(~good_dur):
         logging.warning("No spindle were found.")
+        return pd.DataFrame({
+            "Start_Time": [],
+            "Peak_Time": [],
+            "End_Time": [],
+            "Start_Index": [],
+            "End_Index": [],
+
+            "Duration": [],
+            "Amplitude": [],
+            "RMS": [],
+            "AbsPower": [],
+            "RelPower": [],
+            "Frequency": [],
+            "Oscillations": [],
+            "Symmetry": [],
+            # 'SOPhase': sp_cou,
+        })
 
     # Initialize empty variables
     sp_amp = np.zeros(len(sp))
     sp_freq = np.zeros(len(sp))
     sp_rms = np.zeros(len(sp))
     sp_osc = np.zeros(len(sp))
     sp_sym = np.zeros(len(sp))
@@ -690,15 +724,14 @@
     #
     # # find every peak without setting limit
     # idx_neg_peaks, _ = signal.find_peaks(-1 * data_filt[:], height=(0, 500))
     # idx_pos_peaks, _ = signal.find_peaks(data_filt[:], height=(0, 500))
     # idx_neg_peaks = np.intersect1d(idx_neg_peaks, idx_mask, assume_unique=True)
     # idx_pos_peaks = np.intersect1d(idx_pos_peaks, idx_mask, assume_unique=True)
 
-
     # ##################################
 
     # ####################################################################
     # START SINGLE CHANNEL DETECTION
     # ####################################################################
 
     # todo: data_filt形状
@@ -710,14 +743,29 @@
     # Intersect with sleep stage vector
     idx_neg_peaks = np.intersect1d(idx_neg_peaks, idx_mask, assume_unique=True)
     idx_pos_peaks = np.intersect1d(idx_pos_peaks, idx_mask, assume_unique=True)
 
     # If no peaks are detected, return None
     if len(idx_neg_peaks) == 0 or len(idx_pos_peaks) == 0:
         logging.warning("No SW were found.")
+        return pd.DataFrame({
+            "Start_Time": [],
+            "NegPeak": [],
+            "MidCrossing": [],
+            "PosPeak": [],
+            "End_Time": [],
+            "Start_Index": [],
+            "End_Index": [],
+            "Duration": [],
+            "ValNegPeak": [],
+            "ValPosPeak": [],
+            "PTP": [],
+            "Slope": [],
+            "Frequency": [],
+        })
 
     # Make sure that the last detected peak is a positive one
     if idx_pos_peaks[-1] < idx_neg_peaks[-1]:
         # If not, append a fake positive peak one sample after the last neg
         idx_pos_peaks = np.append(idx_pos_peaks, idx_neg_peaks[-1] + 1)
 
     # For each negative peak, we find the closest following positive peak
@@ -729,14 +777,29 @@
     # Now we compute the PTP amplitude and keep only the good peaks
     sw_ptp = np.abs(data_filt[idx_neg_peaks]) + data_filt[idx_pos_peaks]
     good_ptp = np.logical_and(sw_ptp > amp_ptp[0], sw_ptp < amp_ptp[1])
 
     # If good_ptp is all False
     if all(~good_ptp):
         logging.warning("No SW were found.")
+        return pd.DataFrame({
+            "Start_Time": [],
+            "NegPeak": [],
+            "MidCrossing": [],
+            "PosPeak": [],
+            "End_Time": [],
+            "Start_Index": [],
+            "End_Index": [],
+            "Duration": [],
+            "ValNegPeak": [],
+            "ValPosPeak": [],
+            "PTP": [],
+            "Slope": [],
+            "Frequency": [],
+        })
 
     sw_ptp = sw_ptp[good_ptp]
     idx_neg_peaks = idx_neg_peaks[good_ptp]
     idx_pos_peaks = idx_pos_peaks[good_ptp]
 
     # Now we need to check the negative and positive phase duration
     # For that we need to compute the zero crossings of the filtered signal
@@ -797,14 +860,29 @@
             sw_midcrossing < sw_end,
             sw_slope > 0,
         )
     )
 
     if all(~good_sw):
         logging.warning("No SW were found.")
+        return pd.DataFrame({
+            "Start_Time": [],
+            "NegPeak": [],
+            "MidCrossing": [],
+            "PosPeak": [],
+            "End_Time": [],
+            "Start_Index": [],
+            "End_Index": [],
+            "Duration": [],
+            "ValNegPeak": [],
+            "ValPosPeak": [],
+            "PTP": [],
+            "Slope": [],
+            "Frequency": [],
+        })
 
     # Filter good events
     idx_neg_peaks = idx_neg_peaks[good_sw]
     idx_pos_peaks = idx_pos_peaks[good_sw]
     sw_start = sw_start[good_sw]
     sw_idx_neg = sw_idx_neg[good_sw]
     sw_midcrossing = sw_midcrossing[good_sw]
@@ -862,11 +940,10 @@
     # ####################################################################
 
     df = pd.concat([df, df_chan], axis=0, ignore_index=True)
 
     # If no SW were detected, return None
     if df.empty:
         logging.warning("No SW were found in data. Returning None.")
-        return None
 
     return df
     # return SWResults(events=df, data=data, sf=sf, ch_names=ch_names, hypno=hypno, data_filt=data_filt)
```

### Comparing `lm_datahandler-0.1.6/lm_datahandler/functions/feature_extract.py` & `lm_datahandler-0.1.7/lm_datahandler/functions/feature_extract.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/functions/posture_analyse.py` & `lm_datahandler-0.1.7/lm_datahandler/functions/posture_analyse.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/functions/sleep_staging.py` & `lm_datahandler-0.1.7/lm_datahandler/functions/sleep_staging.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/functions/sleep_variable_compute.py` & `lm_datahandler-0.1.7/lm_datahandler/functions/sleep_variable_compute.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/functions/wear_detect.py` & `lm_datahandler-0.1.7/lm_datahandler/functions/wear_detect.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/models/wear_detection_1s.txt` & `lm_datahandler-0.1.7/lm_datahandler/models/wear_detection_1s.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/models/wholenight_sleep_staging.txt` & `lm_datahandler-0.1.7/lm_datahandler/models/wholenight_sleep_staging.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/plots/biomarker_plot.py` & `lm_datahandler-0.1.7/lm_datahandler/plots/biomarker_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/plots/sleep_staging_plot.py` & `lm_datahandler-0.1.7/lm_datahandler/plots/sleep_staging_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/plots/stim_plot.py` & `lm_datahandler-0.1.7/lm_datahandler/plots/stim_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/postprocess/label_smooth.py` & `lm_datahandler-0.1.7/lm_datahandler/postprocess/label_smooth.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/preprocess/filter.py` & `lm_datahandler-0.1.7/lm_datahandler/preprocess/filter.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler/utils/numba_func.py` & `lm_datahandler-0.1.7/lm_datahandler/utils/numba_func.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/lm_datahandler.egg-info/SOURCES.txt` & `lm_datahandler-0.1.7/lm_datahandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.6/setup.py` & `lm_datahandler-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lm_datahandler',
-    version = '0.1.6',
+    version = '0.1.7',
     keywords='eeg sleep staging analysis',
     description = 'a python analyse tool for LM Data Recorder data',
     license = 'MIT License',
     url = 'https://github.com/zx950618/lm_datahandler',
     author = 'Eric Zheng',
     author_email = '1248471980@qq.com',
     packages = find_packages(),
```

