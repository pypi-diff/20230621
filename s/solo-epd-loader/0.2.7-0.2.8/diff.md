# Comparing `tmp/solo_epd_loader-0.2.7.tar.gz` & `tmp/solo_epd_loader-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-lwq7isme/solo_epd_loader-0.2.7.tar", last modified: Tue Jun 20 12:50:57 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-htd_kfzz/solo_epd_loader-0.2.8.tar", last modified: Wed Jun 21 10:41:23 2023, max compression
```

## Comparing `solo_epd_loader-0.2.7.tar` & `solo_epd_loader-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.7/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.7/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.7/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.7/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.905557 solo_epd_loader-0.2.7/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.7/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.905557 solo_epd_loader-0.2.7/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.7/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.7/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.7/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.7/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.905557 solo_epd_loader-0.2.7/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.7/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.7/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.7/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    55969 2023-06-20 12:40:19.000000 solo_epd_loader-0.2.7/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.7/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.8/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.8/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.8/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.8/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.813713 solo_epd_loader-0.2.8/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.8/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.813713 solo_epd_loader-0.2.8/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.8/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.8/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.8/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.8/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.8/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.8/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-21 10:41:23.821713 solo_epd_loader-0.2.8/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.8/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    55919 2023-06-21 10:39:08.000000 solo_epd_loader-0.2.8/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.8/tox.ini
```

### Comparing `solo_epd_loader-0.2.7/LICENSE.rst` & `solo_epd_loader-0.2.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/PKG-INFO` & `solo_epd_loader-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.7
+Version: 0.2.8
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.7/README.rst` & `solo_epd_loader-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/code_of_conduct.md` & `solo_epd_loader-0.2.8/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/docs/Makefile` & `solo_epd_loader-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/docs/conf.py` & `solo_epd_loader-0.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/docs/make.bat` & `solo_epd_loader-0.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.8/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.8/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/gh2021_fig_2.png` & `solo_epd_loader-0.2.8/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/gh2021_fig_2a.png` & `solo_epd_loader-0.2.8/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/licenses/LICENSE.rst` & `solo_epd_loader-0.2.8/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.8/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/setup.cfg` & `solo_epd_loader-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/setup.py` & `solo_epd_loader-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.8/solo_epd_loader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,15 +536,15 @@
     for d in [startdate, enddate]:
         if isinstance(d, int):
             if len(str(d)) != 8:
                 raise SystemExit(f"startdate & enddate must be (datetime objects or) integers of the form YYYYMMDD, not {d}!")
 
     if sensor.lower() == 'step':
         datadf, energies_dict = \
-            _read_step_cdf(level, startdate, enddate, path, autodownload, only_averages, contamination_threshold)
+            _read_step_cdf(level, startdate, enddate, path, autodownload, only_averages)
         return datadf, energies_dict
     if sensor.lower() == 'ept' or sensor.lower() == 'het':
         if viewing is None:
             raise Exception("EPT and HET need a telescope 'viewing' " +
                             "direction! No data read!")
             df_epd_p = []
             df_epd_e = []
@@ -951,15 +951,15 @@
 
             datadf.index.names = ['Time']
 
             # if type(contamination_threshold) == int:
             #     print("'contamination_threshold' not yet included for old STEP data (before Oct 22, 2021)!")
 
         elif product == 'main':
-            datadf, energies_dict = _read_new_step_cdf(filelist, only_averages, contamination_threshold)
+            datadf, energies_dict = _read_new_step_cdf(filelist, only_averages)
 
     '''
     Careful if adding more species - they might have different EPOCH
     dependencies and cannot easily be put in the same dataframe!
     '''
 
     return datadf, energies_dict
```

### Comparing `solo_epd_loader-0.2.7/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.8/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.7
+Version: 0.2.8
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.7/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.8/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.7/tox.ini` & `solo_epd_loader-0.2.8/tox.ini`

 * *Files identical despite different names*

