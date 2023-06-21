# Comparing `tmp/element-animal-0.1.5.tar.gz` & `tmp/element-animal-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-animal-0.1.5.tar", last modified: Fri Mar  3 15:45:55 2023, max compression
+gzip compressed data, was "element-animal-0.1.8.tar", last modified: Wed Jun 21 01:48:35 2023, max compression
```

## Comparing `element-animal-0.1.5.tar` & `element-animal-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:45:55.686898 element-animal-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-03 15:45:53.000000 element-animal-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-03 15:45:55.686898 element-animal-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-03 15:45:53.000000 element-animal-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:45:55.686898 element-animal-0.1.5/element_animal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 15:45:53.000000 element-animal-0.1.5/element_animal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:45:55.686898 element-animal-0.1.5/element_animal/export/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-03 15:45:53.000000 element-animal-0.1.5/element_animal/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-03 15:45:53.000000 element-animal-0.1.5/element_animal/export/nwb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-03-03 15:45:53.000000 element-animal-0.1.5/element_animal/genotyping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-03-03 15:45:53.000000 element-animal-0.1.5/element_animal/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-03-03 15:45:53.000000 element-animal-0.1.5/element_animal/surgery.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-03 15:45:53.000000 element-animal-0.1.5/element_animal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 15:45:55.686898 element-animal-0.1.5/element_animal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-03 15:45:55.000000 element-animal-0.1.5/element_animal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-03 15:45:55.000000 element-animal-0.1.5/element_animal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 15:45:55.000000 element-animal-0.1.5/element_animal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-03 15:45:55.000000 element-animal-0.1.5/element_animal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-03 15:45:55.000000 element-animal-0.1.5/element_animal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 15:45:55.686898 element-animal-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-03 15:45:53.000000 element-animal-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:48:35.598766 element-animal-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 01:48:29.000000 element-animal-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-21 01:48:35.598766 element-animal-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-21 01:48:29.000000 element-animal-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:48:35.594766 element-animal-0.1.8/element_animal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 01:48:29.000000 element-animal-0.1.8/element_animal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:48:35.594766 element-animal-0.1.8/element_animal/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 01:48:29.000000 element-animal-0.1.8/element_animal/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-21 01:48:29.000000 element-animal-0.1.8/element_animal/export/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-21 01:48:29.000000 element-animal-0.1.8/element_animal/genotyping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-21 01:48:29.000000 element-animal-0.1.8/element_animal/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-21 01:48:29.000000 element-animal-0.1.8/element_animal/surgery.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 01:48:29.000000 element-animal-0.1.8/element_animal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:48:35.594766 element-animal-0.1.8/element_animal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-21 01:48:35.000000 element-animal-0.1.8/element_animal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-21 01:48:35.000000 element-animal-0.1.8/element_animal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:48:35.000000 element-animal-0.1.8/element_animal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 01:48:35.000000 element-animal-0.1.8/element_animal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 01:48:35.000000 element-animal-0.1.8/element_animal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:48:35.598766 element-animal-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 01:48:29.000000 element-animal-0.1.8/setup.py
```

### Comparing `element-animal-0.1.5/LICENSE` & `element-animal-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `element-animal-0.1.5/PKG-INFO` & `element-animal-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: element-animal
-Version: 0.1.5
+Version: 0.1.8
 Summary: DataJoint Element for Animal Management
 Home-page: https://github.com/datajoint/element-animal
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience animal-management datajoint
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/element-animal.svg)](http://badge.fury.io/py/element-animal)
+
 # Element Animal
 
 DataJoint Element for storing animal meta data, genotype, and surgery information.
 DataJoint Elements collectively standardize and automate data collection and analysis
 for neuroscience experiments. Each Element is a modular pipeline for data storage and
 processing with corresponding database tables that can be combined with other Elements
 to assemble a fully functional pipeline.
```

### Comparing `element-animal-0.1.5/README.md` & `element-animal-0.1.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://badge.fury.io/py/element-animal.svg)](http://badge.fury.io/py/element-animal)
+
 # Element Animal
 
 DataJoint Element for storing animal meta data, genotype, and surgery information.
 DataJoint Elements collectively standardize and automate data collection and analysis
 for neuroscience experiments. Each Element is a modular pipeline for data storage and
 processing with corresponding database tables that can be combined with other Elements
 to assemble a fully functional pipeline.
```

### Comparing `element-animal-0.1.5/element_animal/export/nwb.py` & `element-animal-0.1.8/element_animal/export/nwb.py`

 * *Files identical despite different names*

### Comparing `element-animal-0.1.5/element_animal/genotyping.py` & `element-animal-0.1.8/element_animal/genotyping.py`

 * *Files identical despite different names*

### Comparing `element-animal-0.1.5/element_animal/subject.py` & `element-animal-0.1.8/element_animal/subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def activate(
     schema_name: str,
     *,
     create_schema: bool = True,
     create_tables: bool = True,
-    linking_module: bool = True
+    linking_module: bool = True,
 ):
     """Activate this schema.
 
     Args:
         schema_name (str): schema name on the database server to activate the
                         `subject` element
         create_schema (bool): when True (default), create schema in the
```

### Comparing `element-animal-0.1.5/element_animal/surgery.py` & `element-animal-0.1.8/element_animal/surgery.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def activate(
     surgery_schema_name: str,
     subject_schema_name: str = None,
     *,
     create_schema: bool = True,
     create_tables: bool = True,
-    linking_module: bool = True
+    linking_module: bool = True,
 ):
     """Activate this schema.
 
     Args:
         schema_name (str): schema name on the database server to activate the
                         `subject` element
         create_schema (bool): when True (default), create schema in the
@@ -127,29 +127,27 @@
     )
 
 
 @schema
 class Implantation(dj.Manual):
     """Implantation of a device
 
-    WRT: With Respect To
-
     Attributes:
         Session (foreign key): Session primary key
         location_id (int): ID of of brain location
         ap ( float ): In mm, Anterior/posterior; Anterior Positive
         ap_reference (projected attribute): Coordinate reference
         ml ( float ): In mm, medial axis; Right Positive
         ml_reference (projected attribute): Coordinate reference
         dv ( float ): In mm, dorso-ventral axis. Ventral negative
         dv_reference (projected attribute): Coordinate reference
         theta ( float, nullable ): Elevation in degrees.
-            Rotation about ml-axis [0, 180] WRT Z
+            Rotation about ml-axis [0, 180] relative to z-axis
         phi ( float, nullable ): Azimuth in degrees.
-            Rotations about dv-axis [0, 360] WRT X
+            Rotations about dv-axis [0, 360] relative to x-axis
         beta ( float, nullable ): Rotation about shank in degrees.
             Rotation about the shank [-180, 180]. Clockwise is increasing.
             0 is the probe-front facing anterior
     """
 
     definition = """
     -> subject.Subject
```

### Comparing `element-animal-0.1.5/element_animal.egg-info/PKG-INFO` & `element-animal-0.1.8/element_animal.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: element-animal
-Version: 0.1.5
+Version: 0.1.8
 Summary: DataJoint Element for Animal Management
 Home-page: https://github.com/datajoint/element-animal
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience animal-management datajoint
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/element-animal.svg)](http://badge.fury.io/py/element-animal)
+
 # Element Animal
 
 DataJoint Element for storing animal meta data, genotype, and surgery information.
 DataJoint Elements collectively standardize and automate data collection and analysis
 for neuroscience experiments. Each Element is a modular pipeline for data storage and
 processing with corresponding database tables that can be combined with other Elements
 to assemble a fully functional pipeline.
```

### Comparing `element-animal-0.1.5/setup.py` & `element-animal-0.1.8/setup.py`

 * *Files identical despite different names*

