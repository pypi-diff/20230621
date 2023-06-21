# Comparing `tmp/kineticstoolkit-0.9.1.tar.gz` & `tmp/kineticstoolkit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kineticstoolkit-0.9.1.tar", last modified: Thu Sep 15 13:53:21 2022, max compression
+gzip compressed data, was "kineticstoolkit-0.9.2.tar", last modified: Thu Sep 15 14:54:01 2022, max compression
```

## Comparing `kineticstoolkit-0.9.1.tar` & `kineticstoolkit-0.9.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 13:53:21.816870 kineticstoolkit-0.9.1/
--rwxr-xr-x   0 felix      (502) staff       (20)    10173 2021-03-29 01:48:21.000000 kineticstoolkit-0.9.1/LICENSE.txt
--rwxr-xr-x   0 felix      (502) staff       (20)      336 2020-10-25 00:25:29.000000 kineticstoolkit-0.9.1/NOTICE.txt
--rw-r--r--   0 felix      (502) staff       (20)     1215 2022-09-15 13:53:21.816513 kineticstoolkit-0.9.1/PKG-INFO
--rwxr-xr-x   0 felix      (502) staff       (20)      263 2022-07-14 08:27:53.000000 kineticstoolkit-0.9.1/README.md
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 13:53:21.812448 kineticstoolkit-0.9.1/kineticstoolkit/
--rw-r--r--   0 felix      (502) staff       (20)        5 2022-09-15 13:47:34.000000 kineticstoolkit-0.9.1/kineticstoolkit/VERSION
--rw-r--r--   0 felix      (502) staff       (20)     2949 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.1/kineticstoolkit/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     4393 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.1/kineticstoolkit/_repr.py
--rwxr-xr-x   0 felix      (502) staff       (20)     2458 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.1/kineticstoolkit/config.py
--rwxr-xr-x   0 felix      (502) staff       (20)    20063 2022-08-24 20:29:26.000000 kineticstoolkit-0.9.1/kineticstoolkit/cycles.py
--rwxr-xr-x   0 felix      (502) staff       (20)     3338 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.1/kineticstoolkit/decorators.py
--rwxr-xr-x   0 felix      (502) staff       (20)     4538 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.1/kineticstoolkit/dev.py
--rw-r--r--   0 felix      (502) staff       (20)     2940 2022-08-24 20:29:25.000000 kineticstoolkit-0.9.1/kineticstoolkit/doc.py
--rw-r--r--   0 felix      (502) staff       (20)     2716 2022-08-24 20:29:25.000000 kineticstoolkit-0.9.1/kineticstoolkit/ext.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 13:53:21.815468 kineticstoolkit-0.9.1/kineticstoolkit/external/
--rw-r--r--   0 felix      (502) staff       (20)        0 2020-12-10 15:37:16.000000 kineticstoolkit-0.9.1/kineticstoolkit/external/__init__.py
--rwxr-xr-x   0 felix      (502) staff       (20)     4452 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.1/kineticstoolkit/external/icp.py
--rw-r--r--   0 felix      (502) staff       (20)    20280 2022-08-31 19:02:20.000000 kineticstoolkit-0.9.1/kineticstoolkit/files.py
--rwxr-xr-x   0 felix      (502) staff       (20)     9899 2022-08-24 20:29:26.000000 kineticstoolkit-0.9.1/kineticstoolkit/filters.py
--rwxr-xr-x   0 felix      (502) staff       (20)    18352 2022-09-15 12:27:54.000000 kineticstoolkit-0.9.1/kineticstoolkit/geometry.py
--rwxr-xr-x   0 felix      (502) staff       (20)     5559 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.1/kineticstoolkit/gui.py
--rwxr-xr-x   0 felix      (502) staff       (20)    23856 2022-09-15 12:27:54.000000 kineticstoolkit-0.9.1/kineticstoolkit/kinematics.py
--rwxr-xr-x   0 felix      (502) staff       (20)     1233 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.1/kineticstoolkit/lab.py
--rwxr-xr-x   0 felix      (502) staff       (20)     2428 2021-06-03 17:14:03.000000 kineticstoolkit-0.9.1/kineticstoolkit/logo.png
--rwxr-xr-x   0 felix      (502) staff       (20)    12244 2021-06-03 17:14:03.000000 kineticstoolkit-0.9.1/kineticstoolkit/logo_hires.png
--rw-r--r--   0 felix      (502) staff       (20)    39647 2022-09-15 12:32:01.000000 kineticstoolkit-0.9.1/kineticstoolkit/player.py
--rwxr-xr-x   0 felix      (502) staff       (20)    20891 2022-08-06 13:13:40.000000 kineticstoolkit-0.9.1/kineticstoolkit/pushrimkinetics.py
--rw-r--r--   0 felix      (502) staff       (20)    99611 2022-09-15 12:22:24.000000 kineticstoolkit-0.9.1/kineticstoolkit/timeseries.py
--rw-r--r--   0 felix      (502) staff       (20)     4454 2022-08-24 20:29:25.000000 kineticstoolkit-0.9.1/kineticstoolkit/tools.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 13:53:21.814791 kineticstoolkit-0.9.1/kineticstoolkit.egg-info/
--rw-r--r--   0 felix      (502) staff       (20)     1215 2022-09-15 13:53:21.000000 kineticstoolkit-0.9.1/kineticstoolkit.egg-info/PKG-INFO
--rw-r--r--   0 felix      (502) staff       (20)      875 2022-09-15 13:53:21.000000 kineticstoolkit-0.9.1/kineticstoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 felix      (502) staff       (20)        1 2022-09-15 13:53:21.000000 kineticstoolkit-0.9.1/kineticstoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 felix      (502) staff       (20)       91 2022-09-15 13:53:21.000000 kineticstoolkit-0.9.1/kineticstoolkit.egg-info/requires.txt
--rw-r--r--   0 felix      (502) staff       (20)       16 2022-09-15 13:53:21.000000 kineticstoolkit-0.9.1/kineticstoolkit.egg-info/top_level.txt
--rw-r--r--   0 felix      (502) staff       (20)     1533 2022-08-05 13:14:18.000000 kineticstoolkit-0.9.1/pyproject.toml
--rw-r--r--   0 felix      (502) staff       (20)       38 2022-09-15 13:53:21.817033 kineticstoolkit-0.9.1/setup.cfg
--rw-r--r--   0 felix      (502) staff       (20)     1765 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.1/setup.py
+drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 14:54:01.296542 kineticstoolkit-0.9.2/
+-rwxr-xr-x   0 felix      (502) staff       (20)    10173 2021-03-29 01:48:21.000000 kineticstoolkit-0.9.2/LICENSE.txt
+-rwxr-xr-x   0 felix      (502) staff       (20)      336 2020-10-25 00:25:29.000000 kineticstoolkit-0.9.2/NOTICE.txt
+-rw-r--r--   0 felix      (502) staff       (20)     1215 2022-09-15 14:54:01.296244 kineticstoolkit-0.9.2/PKG-INFO
+-rwxr-xr-x   0 felix      (502) staff       (20)      263 2022-07-14 08:27:53.000000 kineticstoolkit-0.9.2/README.md
+drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 14:54:01.292286 kineticstoolkit-0.9.2/kineticstoolkit/
+-rw-r--r--   0 felix      (502) staff       (20)        5 2022-09-15 14:53:19.000000 kineticstoolkit-0.9.2/kineticstoolkit/VERSION
+-rw-r--r--   0 felix      (502) staff       (20)     2949 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.2/kineticstoolkit/__init__.py
+-rw-r--r--   0 felix      (502) staff       (20)     4393 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.2/kineticstoolkit/_repr.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     2458 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.2/kineticstoolkit/config.py
+-rwxr-xr-x   0 felix      (502) staff       (20)    20063 2022-08-24 20:29:26.000000 kineticstoolkit-0.9.2/kineticstoolkit/cycles.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     3338 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.2/kineticstoolkit/decorators.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     4538 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.2/kineticstoolkit/dev.py
+-rw-r--r--   0 felix      (502) staff       (20)     2940 2022-08-24 20:29:25.000000 kineticstoolkit-0.9.2/kineticstoolkit/doc.py
+-rw-r--r--   0 felix      (502) staff       (20)     2716 2022-08-24 20:29:25.000000 kineticstoolkit-0.9.2/kineticstoolkit/ext.py
+drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 14:54:01.295112 kineticstoolkit-0.9.2/kineticstoolkit/external/
+-rw-r--r--   0 felix      (502) staff       (20)        0 2020-12-10 15:37:16.000000 kineticstoolkit-0.9.2/kineticstoolkit/external/__init__.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     4452 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.2/kineticstoolkit/external/icp.py
+-rw-r--r--   0 felix      (502) staff       (20)    20260 2022-09-15 14:51:23.000000 kineticstoolkit-0.9.2/kineticstoolkit/files.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     9899 2022-08-24 20:29:26.000000 kineticstoolkit-0.9.2/kineticstoolkit/filters.py
+-rwxr-xr-x   0 felix      (502) staff       (20)    18352 2022-09-15 12:27:54.000000 kineticstoolkit-0.9.2/kineticstoolkit/geometry.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     5559 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.2/kineticstoolkit/gui.py
+-rwxr-xr-x   0 felix      (502) staff       (20)    23856 2022-09-15 12:27:54.000000 kineticstoolkit-0.9.2/kineticstoolkit/kinematics.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     1233 2022-08-05 00:13:08.000000 kineticstoolkit-0.9.2/kineticstoolkit/lab.py
+-rwxr-xr-x   0 felix      (502) staff       (20)     2428 2021-06-03 17:14:03.000000 kineticstoolkit-0.9.2/kineticstoolkit/logo.png
+-rwxr-xr-x   0 felix      (502) staff       (20)    12244 2021-06-03 17:14:03.000000 kineticstoolkit-0.9.2/kineticstoolkit/logo_hires.png
+-rw-r--r--   0 felix      (502) staff       (20)    39647 2022-09-15 12:32:01.000000 kineticstoolkit-0.9.2/kineticstoolkit/player.py
+-rwxr-xr-x   0 felix      (502) staff       (20)    20891 2022-08-06 13:13:40.000000 kineticstoolkit-0.9.2/kineticstoolkit/pushrimkinetics.py
+-rw-r--r--   0 felix      (502) staff       (20)    99611 2022-09-15 12:22:24.000000 kineticstoolkit-0.9.2/kineticstoolkit/timeseries.py
+-rw-r--r--   0 felix      (502) staff       (20)     4454 2022-08-24 20:29:25.000000 kineticstoolkit-0.9.2/kineticstoolkit/tools.py
+drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-09-15 14:54:01.294127 kineticstoolkit-0.9.2/kineticstoolkit.egg-info/
+-rw-r--r--   0 felix      (502) staff       (20)     1215 2022-09-15 14:54:01.000000 kineticstoolkit-0.9.2/kineticstoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 felix      (502) staff       (20)      875 2022-09-15 14:54:01.000000 kineticstoolkit-0.9.2/kineticstoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 felix      (502) staff       (20)        1 2022-09-15 14:54:01.000000 kineticstoolkit-0.9.2/kineticstoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 felix      (502) staff       (20)       91 2022-09-15 14:54:01.000000 kineticstoolkit-0.9.2/kineticstoolkit.egg-info/requires.txt
+-rw-r--r--   0 felix      (502) staff       (20)       16 2022-09-15 14:54:01.000000 kineticstoolkit-0.9.2/kineticstoolkit.egg-info/top_level.txt
+-rw-r--r--   0 felix      (502) staff       (20)     1533 2022-08-05 13:14:18.000000 kineticstoolkit-0.9.2/pyproject.toml
+-rw-r--r--   0 felix      (502) staff       (20)       38 2022-09-15 14:54:01.296681 kineticstoolkit-0.9.2/setup.cfg
+-rw-r--r--   0 felix      (502) staff       (20)     1765 2022-07-14 08:27:54.000000 kineticstoolkit-0.9.2/setup.py
```

### Comparing `kineticstoolkit-0.9.1/LICENSE.txt` & `kineticstoolkit-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/PKG-INFO` & `kineticstoolkit-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kineticstoolkit
-Version: 0.9.1
+Version: 0.9.2
 Summary: An Open-Source Python Package to Facilitate Research in Biomechanics.
 Home-page: https://kineticstoolkit.uqam.ca
 Author: Félix Chénier
 Author-email: chenier.felix@uqam.ca
 License: Apache
 Project-URL: Documentation, https://kineticstoolkit.uqam.ca
 Project-URL: Source, https://github.com/felixchenier/kineticstoolkit/
```

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/__init__.py` & `kineticstoolkit-0.9.2/kineticstoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/_repr.py` & `kineticstoolkit-0.9.2/kineticstoolkit/_repr.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/config.py` & `kineticstoolkit-0.9.2/kineticstoolkit/config.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/cycles.py` & `kineticstoolkit-0.9.2/kineticstoolkit/cycles.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/decorators.py` & `kineticstoolkit-0.9.2/kineticstoolkit/decorators.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/dev.py` & `kineticstoolkit-0.9.2/kineticstoolkit/dev.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/doc.py` & `kineticstoolkit-0.9.2/kineticstoolkit/doc.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/ext.py` & `kineticstoolkit-0.9.2/kineticstoolkit/ext.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/external/icp.py` & `kineticstoolkit-0.9.2/kineticstoolkit/external/icp.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/files.py` & `kineticstoolkit-0.9.2/kineticstoolkit/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,19 +406,19 @@
             os.remove(tempfile)
 
     else:
         raise FileNotFoundError(f"File {filename} was not found.")
 
     # ---------------------------------
     # List the events
-    if "EVENT" in reader["parameters"]:
+    try:
         event_names = reader["parameters"]["EVENT"]["LABELS"]["value"]
         event_times = reader["parameters"]["EVENT"]["TIMES"]["value"].T
         event_times = event_times[:, 0] * 60 + event_times[:, 1]
-    else:
+    except KeyError:
         event_names = []
         event_times = []
 
     # ---------------------------------
     # Create the points TimeSeries
     points = TimeSeries()
```

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/filters.py` & `kineticstoolkit-0.9.2/kineticstoolkit/filters.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/geometry.py` & `kineticstoolkit-0.9.2/kineticstoolkit/geometry.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/gui.py` & `kineticstoolkit-0.9.2/kineticstoolkit/gui.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/kinematics.py` & `kineticstoolkit-0.9.2/kineticstoolkit/kinematics.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/lab.py` & `kineticstoolkit-0.9.2/kineticstoolkit/lab.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/logo.png` & `kineticstoolkit-0.9.2/kineticstoolkit/logo.png`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/logo_hires.png` & `kineticstoolkit-0.9.2/kineticstoolkit/logo_hires.png`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/player.py` & `kineticstoolkit-0.9.2/kineticstoolkit/player.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/pushrimkinetics.py` & `kineticstoolkit-0.9.2/kineticstoolkit/pushrimkinetics.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/timeseries.py` & `kineticstoolkit-0.9.2/kineticstoolkit/timeseries.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit/tools.py` & `kineticstoolkit-0.9.2/kineticstoolkit/tools.py`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit.egg-info/PKG-INFO` & `kineticstoolkit-0.9.2/kineticstoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kineticstoolkit
-Version: 0.9.1
+Version: 0.9.2
 Summary: An Open-Source Python Package to Facilitate Research in Biomechanics.
 Home-page: https://kineticstoolkit.uqam.ca
 Author: Félix Chénier
 Author-email: chenier.felix@uqam.ca
 License: Apache
 Project-URL: Documentation, https://kineticstoolkit.uqam.ca
 Project-URL: Source, https://github.com/felixchenier/kineticstoolkit/
```

### Comparing `kineticstoolkit-0.9.1/kineticstoolkit.egg-info/SOURCES.txt` & `kineticstoolkit-0.9.2/kineticstoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/pyproject.toml` & `kineticstoolkit-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kineticstoolkit-0.9.1/setup.py` & `kineticstoolkit-0.9.2/setup.py`

 * *Files identical despite different names*

