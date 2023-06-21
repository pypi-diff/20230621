# Comparing `tmp/element-event-0.2.0.tar.gz` & `tmp/element-event-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-event-0.2.0.tar", last modified: Thu Apr  6 20:47:00 2023, max compression
+gzip compressed data, was "element-event-0.2.3.tar", last modified: Wed Jun 21 01:54:31 2023, max compression
```

## Comparing `element-event-0.2.0.tar` & `element-event-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:47:00.769889 element-event-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-06 20:46:58.000000 element-event-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-06 20:47:00.769889 element-event-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-06 20:46:58.000000 element-event-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:47:00.765890 element-event-0.2.0/element_event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:46:58.000000 element-event-0.2.0/element_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-04-06 20:46:58.000000 element-event-0.2.0/element_event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-04-06 20:46:58.000000 element-event-0.2.0/element_event/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-06 20:46:58.000000 element-event-0.2.0/element_event/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:47:00.769889 element-event-0.2.0/element_event.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-06 20:47:00.000000 element-event-0.2.0/element_event.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-06 20:47:00.000000 element-event-0.2.0/element_event.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 20:47:00.000000 element-event-0.2.0/element_event.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 20:47:00.000000 element-event-0.2.0/element_event.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 20:47:00.000000 element-event-0.2.0/element_event.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 20:47:00.769889 element-event-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-06 20:46:58.000000 element-event-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:54:31.932147 element-event-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 01:54:28.000000 element-event-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-21 01:54:31.932147 element-event-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-21 01:54:28.000000 element-event-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:54:31.932147 element-event-0.2.3/element_event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 01:54:28.000000 element-event-0.2.3/element_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-21 01:54:28.000000 element-event-0.2.3/element_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-06-21 01:54:28.000000 element-event-0.2.3/element_event/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 01:54:28.000000 element-event-0.2.3/element_event/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:54:31.932147 element-event-0.2.3/element_event.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-21 01:54:31.000000 element-event-0.2.3/element_event.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-21 01:54:31.000000 element-event-0.2.3/element_event.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:54:31.000000 element-event-0.2.3/element_event.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 01:54:31.000000 element-event-0.2.3/element_event.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 01:54:31.000000 element-event-0.2.3/element_event.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:54:31.932147 element-event-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-21 01:54:28.000000 element-event-0.2.3/setup.py
```

### Comparing `element-event-0.2.0/LICENSE` & `element-event-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `element-event-0.2.0/PKG-INFO` & `element-event-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: element-event
-Version: 0.2.0
+Version: 0.2.3
 Summary: DataJoint Elements for Trialized Experiments
 Home-page: https://github.com/datajoint/element-event
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience behavior bpod trials datajoint
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/element-event.svg)](http://badge.fury.io/py/element-event)
+
 # DataJoint Element - Experimental trials
 
 + `element-event` features a DataJoint pipeline design for event, trial, and block management. 
 
 + `element-event` is not a complete workflow by itself, but rather a modular design of tables and dependencies. 
 
 + `element-event` can be flexibly attached to any DataJoint workflow.
```

### Comparing `element-event-0.2.0/README.md` & `element-event-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://badge.fury.io/py/element-event.svg)](http://badge.fury.io/py/element-event)
+
 # DataJoint Element - Experimental trials
 
 + `element-event` features a DataJoint pipeline design for event, trial, and block management. 
 
 + `element-event` is not a complete workflow by itself, but rather a modular design of tables and dependencies. 
 
 + `element-event` can be flexibly attached to any DataJoint workflow.
```

### Comparing `element-event-0.2.0/element_event/event.py` & `element-event-0.2.3/element_event/event.py`

 * *Files identical despite different names*

### Comparing `element-event-0.2.0/element_event/trial.py` & `element-event-0.2.3/element_event/trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     block_stop_time        : float     # (s) relative to recording stop
     """
 
     class Attribute(dj.Part):
         """Extra Block attributes to fully describe a block
 
         Attributes:
-             Block (foreign key): Block table primary key. 
+             Block (foreign key): Block table primary key.
              attribute_name ( varchar(32) ): Name of block attribute
              attribute_value ( varchar(2000) ): Optional. Block attribute value
              attribute_blob (longblob): Optional. Block attribute numerical numerical data
         """
 
         definition = """  # Additional block attributes to fully describe a block
         -> master
```

### Comparing `element-event-0.2.0/element_event.egg-info/PKG-INFO` & `element-event-0.2.3/element_event.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: element-event
-Version: 0.2.0
+Version: 0.2.3
 Summary: DataJoint Elements for Trialized Experiments
 Home-page: https://github.com/datajoint/element-event
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience behavior bpod trials datajoint
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/element-event.svg)](http://badge.fury.io/py/element-event)
+
 # DataJoint Element - Experimental trials
 
 + `element-event` features a DataJoint pipeline design for event, trial, and block management. 
 
 + `element-event` is not a complete workflow by itself, but rather a modular design of tables and dependencies. 
 
 + `element-event` can be flexibly attached to any DataJoint workflow.
```

### Comparing `element-event-0.2.0/setup.py` & `element-event-0.2.3/setup.py`

 * *Files identical despite different names*

