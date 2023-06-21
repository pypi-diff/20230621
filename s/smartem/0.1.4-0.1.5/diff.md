# Comparing `tmp/smartem-0.1.4.tar.gz` & `tmp/smartem-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartem-0.1.4.tar", last modified: Tue Jun 20 14:05:38 2023, max compression
+gzip compressed data, was "smartem-0.1.5.tar", last modified: Wed Jun 21 12:57:07 2023, max compression
```

## Comparing `smartem-0.1.4.tar` & `smartem-0.1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.868933 smartem-0.1.4/
--rw-r--r--   0 kif41228   (504) staff       (20)     1486 2022-12-08 11:26:40.000000 smartem-0.1.4/LICENSE
--rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-20 14:05:38.869018 smartem-0.1.4/PKG-INFO
--rw-r--r--   0 kif41228   (504) staff       (20)     1046 2022-12-08 11:26:40.000000 smartem-0.1.4/README.rst
--rw-r--r--   0 kif41228   (504) staff       (20)      130 2022-12-08 11:26:40.000000 smartem-0.1.4/pyproject.toml
--rw-r--r--   0 kif41228   (504) staff       (20)     1224 2023-06-20 14:05:38.869428 smartem-0.1.4/setup.cfg
--rw-r--r--   0 kif41228   (504) staff       (20)      154 2022-12-08 11:26:40.000000 smartem-0.1.4/setup.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.859585 smartem-0.1.4/src/
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.861520 smartem-0.1.4/src/smartem/
--rw-r--r--   0 kif41228   (504) staff       (20)      212 2023-06-20 14:04:04.000000 smartem-0.1.4/src/smartem/__init__.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.864482 smartem-0.1.4/src/smartem/cli/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)      808 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/change_epu_directory.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1143 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/export.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2864 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/initialise.py
--rw-r--r--   0 kif41228   (504) staff       (20)      158 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/launch.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2105 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/missing.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1136 2023-06-15 15:34:04.000000 smartem-0.1.4/src/smartem/cli/quick_epu_viewer.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1253 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/start.py
--rw-r--r--   0 kif41228   (504) staff       (20)      883 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/stop.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.865413 smartem-0.1.4/src/smartem/data_model/
--rw-r--r--   0 kif41228   (504) staff       (20)     7130 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2375 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/construct.py
--rw-r--r--   0 kif41228   (504) staff       (20)    35995 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/extract.py
--rw-r--r--   0 kif41228   (504) staff       (20)    11757 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/structure.py
--rw-r--r--   0 kif41228   (504) staff       (20)    14708 2023-06-15 09:29:29.000000 smartem-0.1.4/src/smartem/data_model/torch.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.865676 smartem-0.1.4/src/smartem/gui/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/__init__.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.867248 smartem-0.1.4/src/smartem/gui/qt/
--rw-r--r--   0 kif41228   (504) staff       (20)    10881 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2164 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/component_tab.py
--rw-r--r--   0 kif41228   (504) staff       (20)    38827 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/display.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12229 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/image_utils.py
--rw-r--r--   0 kif41228   (504) staff       (20)    24920 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/loader.py
--rw-r--r--   0 kif41228   (504) staff       (20)     5086 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/loader_csv.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1419 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/plotting_utils.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1289 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/qt_style.css
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.868486 smartem-0.1.4/src/smartem/parsing/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/parsing/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)    19542 2023-06-15 09:29:29.000000 smartem-0.1.4/src/smartem/parsing/epu.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12550 2023-06-20 14:03:27.000000 smartem-0.1.4/src/smartem/parsing/epu_vis.py
--rw-r--r--   0 kif41228   (504) staff       (20)    13637 2023-05-15 12:06:59.000000 smartem-0.1.4/src/smartem/parsing/export.py
--rw-r--r--   0 kif41228   (504) staff       (20)     5608 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/parsing/relion_default.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12683 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/parsing/star.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2434 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/stage_model.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.862825 smartem-0.1.4/src/smartem.egg-info/
--rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/PKG-INFO
--rw-r--r--   0 kif41228   (504) staff       (20)     1286 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/SOURCES.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/dependency_links.txt
--rw-r--r--   0 kif41228   (504) staff       (20)      372 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/entry_points.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-05-15 12:40:38.000000 smartem-0.1.4/src/smartem.egg-info/not-zip-safe
--rw-r--r--   0 kif41228   (504) staff       (20)       95 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/requires.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        8 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/top_level.txt
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.868706 smartem-0.1.4/tests/
--rw-r--r--   0 kif41228   (504) staff       (20)     1958 2023-06-15 09:29:29.000000 smartem-0.1.4/tests/test_stage_model.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.762328 smartem-0.1.5/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1486 2022-12-08 11:26:40.000000 smartem-0.1.5/LICENSE
+-rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-21 12:57:07.762408 smartem-0.1.5/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1046 2022-12-08 11:26:40.000000 smartem-0.1.5/README.rst
+-rw-r--r--   0 kif41228   (504) staff       (20)      130 2022-12-08 11:26:40.000000 smartem-0.1.5/pyproject.toml
+-rw-r--r--   0 kif41228   (504) staff       (20)     1224 2023-06-21 12:57:07.762816 smartem-0.1.5/setup.cfg
+-rw-r--r--   0 kif41228   (504) staff       (20)      154 2022-12-08 11:26:40.000000 smartem-0.1.5/setup.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.753837 smartem-0.1.5/src/
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.755176 smartem-0.1.5/src/smartem/
+-rw-r--r--   0 kif41228   (504) staff       (20)      212 2023-06-21 12:56:21.000000 smartem-0.1.5/src/smartem/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.757963 smartem-0.1.5/src/smartem/cli/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      808 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/change_epu_directory.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1143 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2864 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/initialise.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      158 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/launch.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2105 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/missing.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1136 2023-06-15 15:34:04.000000 smartem-0.1.5/src/smartem/cli/quick_epu_viewer.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1253 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/start.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      883 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/cli/stop.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.758841 smartem-0.1.5/src/smartem/data_model/
+-rw-r--r--   0 kif41228   (504) staff       (20)     7130 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/data_model/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2375 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/data_model/construct.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    35995 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/data_model/extract.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    11757 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/data_model/structure.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    14708 2023-06-15 09:29:29.000000 smartem-0.1.5/src/smartem/data_model/torch.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.759119 smartem-0.1.5/src/smartem/gui/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.760675 smartem-0.1.5/src/smartem/gui/qt/
+-rw-r--r--   0 kif41228   (504) staff       (20)    10881 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2164 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/component_tab.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    38827 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/display.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12229 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/image_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    24920 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/loader.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     5086 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/loader_csv.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1419 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/plotting_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1289 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/gui/qt/qt_style.css
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.761924 smartem-0.1.5/src/smartem/parsing/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/parsing/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    19542 2023-06-15 09:29:29.000000 smartem-0.1.5/src/smartem/parsing/epu.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12552 2023-06-21 12:54:44.000000 smartem-0.1.5/src/smartem/parsing/epu_vis.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    13637 2023-05-15 12:06:59.000000 smartem-0.1.5/src/smartem/parsing/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     5608 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/parsing/relion_default.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12683 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/parsing/star.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2434 2022-12-08 11:26:40.000000 smartem-0.1.5/src/smartem/stage_model.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.756276 smartem-0.1.5/src/smartem.egg-info/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-21 12:57:07.000000 smartem-0.1.5/src/smartem.egg-info/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1286 2023-06-21 12:57:07.000000 smartem-0.1.5/src/smartem.egg-info/SOURCES.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-06-21 12:57:07.000000 smartem-0.1.5/src/smartem.egg-info/dependency_links.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)      372 2023-06-21 12:57:07.000000 smartem-0.1.5/src/smartem.egg-info/entry_points.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-05-15 12:40:38.000000 smartem-0.1.5/src/smartem.egg-info/not-zip-safe
+-rw-r--r--   0 kif41228   (504) staff       (20)       95 2023-06-21 12:57:07.000000 smartem-0.1.5/src/smartem.egg-info/requires.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        8 2023-06-21 12:57:07.000000 smartem-0.1.5/src/smartem.egg-info/top_level.txt
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 12:57:07.762097 smartem-0.1.5/tests/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1958 2023-06-15 09:29:29.000000 smartem-0.1.5/tests/test_stage_model.py
```

### Comparing `smartem-0.1.4/LICENSE` & `smartem-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/PKG-INFO` & `smartem-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
```

### Comparing `smartem-0.1.4/README.rst` & `smartem-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/setup.cfg` & `smartem-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartem
-version = 0.1.4
+version = 0.1.5
 description = Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 long_description = file: README.rst
 license_file = LICENSE
 
 [options]
 include_package_data = True
 install_requires =
```

### Comparing `smartem-0.1.4/src/smartem/cli/change_epu_directory.py` & `smartem-0.1.5/src/smartem/cli/change_epu_directory.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/cli/export.py` & `smartem-0.1.5/src/smartem/cli/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/cli/initialise.py` & `smartem-0.1.5/src/smartem/cli/initialise.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/cli/missing.py` & `smartem-0.1.5/src/smartem/cli/missing.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/cli/quick_epu_viewer.py` & `smartem-0.1.5/src/smartem/cli/quick_epu_viewer.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/cli/start.py` & `smartem-0.1.5/src/smartem/cli/start.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/cli/stop.py` & `smartem-0.1.5/src/smartem/cli/stop.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/data_model/__init__.py` & `smartem-0.1.5/src/smartem/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/data_model/construct.py` & `smartem-0.1.5/src/smartem/data_model/construct.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/data_model/extract.py` & `smartem-0.1.5/src/smartem/data_model/extract.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/data_model/structure.py` & `smartem-0.1.5/src/smartem/data_model/structure.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/data_model/torch.py` & `smartem-0.1.5/src/smartem/data_model/torch.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/__init__.py` & `smartem-0.1.5/src/smartem/gui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/component_tab.py` & `smartem-0.1.5/src/smartem/gui/qt/component_tab.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/display.py` & `smartem-0.1.5/src/smartem/gui/qt/display.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/image_utils.py` & `smartem-0.1.5/src/smartem/gui/qt/image_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/loader.py` & `smartem-0.1.5/src/smartem/gui/qt/loader.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/loader_csv.py` & `smartem-0.1.5/src/smartem/gui/qt/loader_csv.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/plotting_utils.py` & `smartem-0.1.5/src/smartem/gui/qt/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/gui/qt/qt_style.css` & `smartem-0.1.5/src/smartem/gui/qt/qt_style.css`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/parsing/epu.py` & `smartem-0.1.5/src/smartem/parsing/epu.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/parsing/epu_vis.py` & `smartem-0.1.5/src/smartem/parsing/epu_vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,21 +131,21 @@
 
         if show_stage_positions:
             stage_data = self._grid_square_stage_locations
             keys = list(stage_data.keys())
             gs = keys[0]
             stage_sc = ax.scatter(
                 [
-                    int((-p[0]) / self._pixel_size)
+                    int((-p[1]) / self._pixel_size)
                     - corrected_center[0][0]
                     + self._readout_area[1] // 2
                     for p in stage_data.values()
                 ],
                 [
-                    int(p[1] / self._pixel_size)
+                    int(-p[0] / self._pixel_size)
                     + corrected_center[1][0]
                     + self._readout_area[0] // 2
                     for p in stage_data.values()
                 ],
                 marker="x",
                 color="red",
                 label="Stage from atlas mag",
@@ -156,21 +156,21 @@
         if self._epu_data_dir:
             grid_squares = []
             for gs in self._grid_square_positions.keys():
                 if GridSquare.found(self._epu_data_dir, int(gs)):
                     grid_squares.append(GridSquare(self._epu_data_dir, int(gs)))
             gs_sc = ax.scatter(
                 [
-                    int((-p._stage_position[0]) / self._pixel_size)
+                    int((-p._stage_position[1]) / self._pixel_size)
                     - corrected_center[0][0]
                     + self._readout_area[1] // 2
                     for p in grid_squares
                 ],
                 [
-                    int((p._stage_position[1]) / self._pixel_size)
+                    int((-p._stage_position[0]) / self._pixel_size)
                     + corrected_center[1][0]
                     + self._readout_area[0] // 2
                     for p in grid_squares
                 ],
                 marker="x",
                 color="blue",
                 label="Stage from grid square mag",
```

### Comparing `smartem-0.1.4/src/smartem/parsing/export.py` & `smartem-0.1.5/src/smartem/parsing/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/parsing/relion_default.py` & `smartem-0.1.5/src/smartem/parsing/relion_default.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/parsing/star.py` & `smartem-0.1.5/src/smartem/parsing/star.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem/stage_model.py` & `smartem-0.1.5/src/smartem/stage_model.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/src/smartem.egg-info/PKG-INFO` & `smartem-0.1.5/src/smartem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
```

### Comparing `smartem-0.1.4/src/smartem.egg-info/SOURCES.txt` & `smartem-0.1.5/src/smartem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartem-0.1.4/tests/test_stage_model.py` & `smartem-0.1.5/tests/test_stage_model.py`

 * *Files identical despite different names*

