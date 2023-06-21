# Comparing `tmp/yt_idefix-2.2.0.tar.gz` & `tmp/yt_idefix-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-2.2.0.tar", last modified: Sat Jun  3 16:23:07 2023, max compression
+gzip compressed data, was "yt_idefix-2.2.1.tar", last modified: Wed Jun 21 06:41:50 2023, max compression
```

## Comparing `yt_idefix-2.2.0.tar` & `yt_idefix-2.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.484503 yt_idefix-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.488503 yt_idefix-2.2.0/src/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/src/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34740 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/src/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.592519 yt_idefix-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.592519 yt_idefix-2.2.1/src/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/src/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34740 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.592519 yt_idefix-2.2.1/src/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_xdmf.py
```

### Comparing `yt_idefix-2.2.0/LICENSE` & `yt_idefix-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/PKG-INFO` & `yt_idefix-2.2.1/src/yt_idefix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yt_idefix
-Version: 2.2.0
+Name: yt-idefix
+Version: 2.2.1
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
@@ -67,28 +67,32 @@
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
 Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
 
 ```python
 # Examples
-ds = yt.load("data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini")
-ds = yt.load("data.0010.vtk", geometry='spherical")
+ds = yt.load(
+    "data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini"
+)
+ds = yt.load("data.0010.vtk", geometry="spherical")
 ```
 
 The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. This frontend can convert data from code units into `cgs` properly, based on the unit definitions from metadata.
 
 Users are able to choose the unit displayed in two ways, through `unit_system` ("code", "mks" and "cgs") and `units_override`(only valid for Pluto).
 
 ```python
 # Examples on units
-ds = yt.load("data.0010.vtk", unit_system='mks")
+ds = yt.load("data.0010.vtk", unit_system="mks")
 
 units_override = dict(length_unit=(100.0, "au"), mass_unit=yt.units.mass_sun)
-ds = yt.load("data.0010.vtk", unit_override=unit_override) # Caution that other units will also be changed for consistency!!
+
+# Caution that other units will also be changed for consistency!
+ds = yt.load("data.0010.vtk", unit_override=unit_override)
 ```
 With Pluto data, the rest of the system will be derived consistently with given units, within the following rules:
 1. Temperature unit cannot be overridden (always set to Kelvin)
 2. No more than three units can be overridden at once (overconstrained systems are never validated for simplicity)
 3. When given less than three overrides, base units in Pluto (ordered: velocity_unit, density_unit, length_unit) are assumed
 4. The following combinations are not allowed
```

### Comparing `yt_idefix-2.2.0/README.md` & `yt_idefix-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,32 @@
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
 Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
 
 ```python
 # Examples
-ds = yt.load("data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini")
-ds = yt.load("data.0010.vtk", geometry='spherical")
+ds = yt.load(
+    "data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini"
+)
+ds = yt.load("data.0010.vtk", geometry="spherical")
 ```
 
 The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. This frontend can convert data from code units into `cgs` properly, based on the unit definitions from metadata.
 
 Users are able to choose the unit displayed in two ways, through `unit_system` ("code", "mks" and "cgs") and `units_override`(only valid for Pluto).
 
 ```python
 # Examples on units
-ds = yt.load("data.0010.vtk", unit_system='mks")
+ds = yt.load("data.0010.vtk", unit_system="mks")
 
 units_override = dict(length_unit=(100.0, "au"), mass_unit=yt.units.mass_sun)
-ds = yt.load("data.0010.vtk", unit_override=unit_override) # Caution that other units will also be changed for consistency!!
+
+# Caution that other units will also be changed for consistency!
+ds = yt.load("data.0010.vtk", unit_override=unit_override)
 ```
 With Pluto data, the rest of the system will be derived consistently with given units, within the following rules:
 1. Temperature unit cannot be overridden (always set to Kelvin)
 2. No more than three units can be overridden at once (overconstrained systems are never validated for simplicity)
 3. When given less than three overrides, base units in Pluto (ordered: velocity_unit, density_unit, length_unit) are assumed
 4. The following combinations are not allowed
```

### Comparing `yt_idefix-2.2.0/pyproject.toml` & `yt_idefix-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/_backports.py` & `yt_idefix-2.2.1/src/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/_io/commons.py` & `yt_idefix-2.2.1/src/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.2.1/src/yt_idefix/_io/dmp_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     is_scalar=False,
 ):
     # NOTE: ret type is only dependent on skip_data...
     # this could be better expressed in the type annotations but it would make
     # more sense to just refactor this function to avoid the boolean trap, so I'll keep wonky
     # type hints for now
     assert ndim == len(dim)
-    count = np.product(dim)
+    count = np.prod(dim)
     size = count * np.dtype(dtype).itemsize
     if skip_data:
         fh.seek(size, 1)
         return None
 
     # note: this reversal may not be desirable in general
     if is_scalar:
```

### Comparing `yt_idefix-2.2.0/src/yt_idefix/_io/h5_io.py` & `yt_idefix-2.2.1/src/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.2.1/src/yt_idefix/_io/vtk_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/data_structures.py` & `yt_idefix-2.2.1/src/yt_idefix/data_structures.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/definitions.py` & `yt_idefix-2.2.1/src/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/fields.py` & `yt_idefix-2.2.1/src/yt_idefix/fields.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix/io.py` & `yt_idefix-2.2.1/src/yt_idefix/io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/src/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yt-idefix
-Version: 2.2.0
+Name: yt_idefix
+Version: 2.2.1
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
@@ -67,28 +67,32 @@
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
 Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
 
 ```python
 # Examples
-ds = yt.load("data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini")
-ds = yt.load("data.0010.vtk", geometry='spherical")
+ds = yt.load(
+    "data.0010.vtk", definitions_header="../definitions.h", inifile="example.ini"
+)
+ds = yt.load("data.0010.vtk", geometry="spherical")
 ```
 
 The data are loaded as physical quantities with units. The default unit system is `cgs` in yt. This frontend can convert data from code units into `cgs` properly, based on the unit definitions from metadata.
 
 Users are able to choose the unit displayed in two ways, through `unit_system` ("code", "mks" and "cgs") and `units_override`(only valid for Pluto).
 
 ```python
 # Examples on units
-ds = yt.load("data.0010.vtk", unit_system='mks")
+ds = yt.load("data.0010.vtk", unit_system="mks")
 
 units_override = dict(length_unit=(100.0, "au"), mass_unit=yt.units.mass_sun)
-ds = yt.load("data.0010.vtk", unit_override=unit_override) # Caution that other units will also be changed for consistency!!
+
+# Caution that other units will also be changed for consistency!
+ds = yt.load("data.0010.vtk", unit_override=unit_override)
 ```
 With Pluto data, the rest of the system will be derived consistently with given units, within the following rules:
 1. Temperature unit cannot be overridden (always set to Kelvin)
 2. No more than three units can be overridden at once (overconstrained systems are never validated for simplicity)
 3. When given less than three overrides, base units in Pluto (ordered: velocity_unit, density_unit, length_unit) are assumed
 4. The following combinations are not allowed
```

### Comparing `yt_idefix-2.2.0/src/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-2.2.1/src/yt_idefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/tests/test_C_io.py` & `yt_idefix-2.2.1/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/tests/test_dmp.py` & `yt_idefix-2.2.1/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/tests/test_loading.py` & `yt_idefix-2.2.1/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/tests/test_vtk.py` & `yt_idefix-2.2.1/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.0/tests/test_xdmf.py` & `yt_idefix-2.2.1/tests/test_xdmf.py`

 * *Files identical despite different names*

