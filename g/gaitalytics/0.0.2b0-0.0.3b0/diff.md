# Comparing `tmp/gaitalytics-0.0.2b0.tar.gz` & `tmp/gaitalytics-0.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.0.2b0.tar", last modified: Wed Jun 21 06:53:56 2023, max compression
+gzip compressed data, was "gaitalytics-0.0.3b0.tar", last modified: Wed Jun 21 07:31:08 2023, max compression
```

## Comparing `gaitalytics-0.0.2b0.tar` & `gaitalytics-0.0.3b0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 06:53:56.026109 gaitalytics-0.0.2b0/
--rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.0.2b0/LICENSE
--rw-rw-rw-   0        0        0     1471 2023-06-21 06:53:56.025109 gaitalytics-0.0.2b0/PKG-INFO
--rw-rw-rw-   0        0        0      879 2023-06-21 04:53:15.000000 gaitalytics-0.0.2b0/README.md
--rw-rw-rw-   0        0        0      672 2023-06-21 06:53:34.000000 gaitalytics-0.0.2b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 06:53:56.026109 gaitalytics-0.0.2b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-21 06:53:56.004824 gaitalytics-0.0.2b0/src/
--rw-rw-rw-   0        0        0        0 2023-06-20 18:48:14.000000 gaitalytics-0.0.2b0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 06:53:56.018284 gaitalytics-0.0.2b0/src/gaitalytics/
--rw-rw-rw-   0        0        0        0 2023-05-09 08:54:38.000000 gaitalytics-0.0.2b0/src/gaitalytics/__init__.py
--rw-rw-rw-   0        0        0    19482 2023-06-20 16:36:53.000000 gaitalytics-0.0.2b0/src/gaitalytics/analysis.py
--rw-rw-rw-   0        0        0    10450 2023-06-21 06:41:27.000000 gaitalytics-0.0.2b0/src/gaitalytics/api.py
--rw-rw-rw-   0        0        0     4160 2023-06-20 15:51:04.000000 gaitalytics-0.0.2b0/src/gaitalytics/c3d.py
--rw-rw-rw-   0        0        0    18703 2023-06-20 15:51:04.000000 gaitalytics-0.0.2b0/src/gaitalytics/cycle.py
--rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.0.2b0/src/gaitalytics/emg.py
--rw-rw-rw-   0        0        0    15087 2023-06-20 18:48:37.000000 gaitalytics-0.0.2b0/src/gaitalytics/events.py
--rw-rw-rw-   0        0        0     9354 2023-06-20 15:51:04.000000 gaitalytics-0.0.2b0/src/gaitalytics/modelling.py
--rw-rw-rw-   0        0        0     6051 2023-06-20 15:51:04.000000 gaitalytics-0.0.2b0/src/gaitalytics/plot.py
--rw-rw-rw-   0        0        0     1505 2023-06-20 15:51:04.000000 gaitalytics-0.0.2b0/src/gaitalytics/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 06:53:56.024110 gaitalytics-0.0.2b0/src/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     1471 2023-06-21 06:53:55.000000 gaitalytics-0.0.2b0/src/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-06-21 06:53:55.000000 gaitalytics-0.0.2b0/src/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 06:53:55.000000 gaitalytics-0.0.2b0/src/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-21 06:53:55.000000 gaitalytics-0.0.2b0/src/gaitalytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 07:31:08.634400 gaitalytics-0.0.3b0/
+-rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.0.3b0/LICENSE
+-rw-rw-rw-   0        0        0     1471 2023-06-21 07:31:08.632876 gaitalytics-0.0.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2023-06-21 04:53:15.000000 gaitalytics-0.0.3b0/README.md
+-rw-rw-rw-   0        0        0      775 2023-06-21 07:30:48.000000 gaitalytics-0.0.3b0/pyproject.toml
+-rw-rw-rw-   0        0        0       75 2023-06-21 07:30:25.000000 gaitalytics-0.0.3b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 07:31:08.634400 gaitalytics-0.0.3b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 07:31:08.601812 gaitalytics-0.0.3b0/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 07:31:08.622964 gaitalytics-0.0.3b0/src/gaitalytics/
+-rw-rw-rw-   0        0        0        0 2023-05-09 08:54:38.000000 gaitalytics-0.0.3b0/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0    19482 2023-06-20 16:36:53.000000 gaitalytics-0.0.3b0/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    10450 2023-06-21 06:41:27.000000 gaitalytics-0.0.3b0/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0     4160 2023-06-20 15:51:04.000000 gaitalytics-0.0.3b0/src/gaitalytics/c3d.py
+-rw-rw-rw-   0        0        0    18703 2023-06-20 15:51:04.000000 gaitalytics-0.0.3b0/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.0.3b0/src/gaitalytics/emg.py
+-rw-rw-rw-   0        0        0    15087 2023-06-20 18:48:37.000000 gaitalytics-0.0.3b0/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0     9354 2023-06-20 15:51:04.000000 gaitalytics-0.0.3b0/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     6051 2023-06-20 15:51:04.000000 gaitalytics-0.0.3b0/src/gaitalytics/plot.py
+-rw-rw-rw-   0        0        0     1505 2023-06-20 15:51:04.000000 gaitalytics-0.0.3b0/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:31:08.631862 gaitalytics-0.0.3b0/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0     1471 2023-06-21 07:31:08.000000 gaitalytics-0.0.3b0/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-06-21 07:31:08.000000 gaitalytics-0.0.3b0/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 07:31:08.000000 gaitalytics-0.0.3b0/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-21 07:31:08.000000 gaitalytics-0.0.3b0/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 07:31:08.000000 gaitalytics-0.0.3b0/src/gaitalytics.egg-info/top_level.txt
```

### Comparing `gaitalytics-0.0.2b0/LICENSE` & `gaitalytics-0.0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/PKG-INFO` & `gaitalytics-0.0.3b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.0.2b0
+Version: 0.0.3b0
 Summary: Library to analyse gait data captured with a mocap system
 Author-email: André Böni <andre.boeni@cereneo.foundation>
 Project-URL: Homepage, https://github.com/cereneo-foundation/gait_analysis
 Project-URL: Bug Tracker, https://github.com/cereneo-foundation/gait_analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaitalytics-0.0.2b0/README.md` & `gaitalytics-0.0.3b0/README.md`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/analysis.py` & `gaitalytics-0.0.3b0/src/gaitalytics/analysis.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/api.py` & `gaitalytics-0.0.3b0/src/gaitalytics/api.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/c3d.py` & `gaitalytics-0.0.3b0/src/gaitalytics/c3d.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/cycle.py` & `gaitalytics-0.0.3b0/src/gaitalytics/cycle.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/emg.py` & `gaitalytics-0.0.3b0/src/gaitalytics/emg.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/events.py` & `gaitalytics-0.0.3b0/src/gaitalytics/events.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/modelling.py` & `gaitalytics-0.0.3b0/src/gaitalytics/modelling.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/plot.py` & `gaitalytics-0.0.3b0/src/gaitalytics/plot.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics/utils.py` & `gaitalytics-0.0.3b0/src/gaitalytics/utils.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.2b0/src/gaitalytics.egg-info/PKG-INFO` & `gaitalytics-0.0.3b0/src/gaitalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.0.2b0
+Version: 0.0.3b0
 Summary: Library to analyse gait data captured with a mocap system
 Author-email: André Böni <andre.boeni@cereneo.foundation>
 Project-URL: Homepage, https://github.com/cereneo-foundation/gait_analysis
 Project-URL: Bug Tracker, https://github.com/cereneo-foundation/gait_analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

