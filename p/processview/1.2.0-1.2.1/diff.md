# Comparing `tmp/processview-1.2.0.tar.gz` & `tmp/processview-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processview-1.2.0.tar", last modified: Wed May 31 14:37:04 2023, max compression
+gzip compressed data, was "processview-1.2.1.tar", last modified: Wed Jun 21 09:48:11 2023, max compression
```

## Comparing `processview-1.2.0.tar` & `processview-1.2.1.tar`

### file list

```diff
@@ -1,53 +1,47 @@
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.2.0/LICENSE
--rw-r--r--   0 payno    (81067) soft      (3401)     1043 2023-05-31 14:37:04.312884 processview-1.2.0/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)      767 2023-02-02 10:20:46.000000 processview-1.2.0/README.md
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/
--rw-r--r--   0 payno    (81067) soft      (3401)       91 2023-05-31 13:34:50.000000 processview-1.2.0/processview/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3289 2023-05-31 13:32:57.000000 processview-1.2.0/processview/core/dataset.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2350 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/helpers.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/manager/
--rw-r--r--   0 payno    (81067) soft      (3401)       23 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/manager/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    13677 2023-05-25 09:34:28.000000 processview-1.2.0/processview/core/manager/manager.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/manager/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1534 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/manager/test/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4823 2023-05-31 13:34:50.000000 processview-1.2.0/processview/core/manager/test/test_manager.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1745 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/setup.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1067 2023-05-31 12:17:21.000000 processview-1.2.0/processview/core/sorting.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5128 2021-11-10 14:06:33.000000 processview-1.2.0/processview/core/superviseprocess.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1561 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/test/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/gui/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.2.0/processview/gui/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    12926 2023-03-30 07:14:30.000000 processview-1.2.0/processview/gui/icons.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2296 2021-10-26 07:14:42.000000 processview-1.2.0/processview/gui/messagebox.py
--rw-r--r--   0 payno    (81067) soft      (3401)    25054 2023-05-31 14:28:04.000000 processview-1.2.0/processview/gui/processmanager.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/gui/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1584 2021-10-26 07:14:42.000000 processview-1.2.0/processview/gui/test/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3666 2023-05-31 13:36:47.000000 processview-1.2.0/processview/gui/test/test_process_manager.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/resources/
--rw-r--r--   0 payno    (81067) soft      (3401)    10757 2022-08-22 08:58:53.000000 processview-1.2.0/processview/resources/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/resources/gui/
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/resources/gui/icons/
--rw-r--r--   0 payno    (81067) soft      (3401)      729 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/advancement.png
--rw-r--r--   0 payno    (81067) soft      (3401)     5781 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/advancement.svg
--rw-r--r--   0 payno    (81067) soft      (3401)      926 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/magnifying_glass.png
--rw-r--r--   0 payno    (81067) soft      (3401)     4631 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/magnifying_glass.svg
--rw-r--r--   0 payno    (81067) soft      (3401)     1822 2021-10-26 07:14:42.000000 processview-1.2.0/processview/setup.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1695 2021-10-26 07:14:42.000000 processview-1.2.0/processview/test/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/utils/
--rw-r--r--   0 payno    (81067) soft      (3401)     2565 2021-10-26 07:14:42.000000 processview-1.2.0/processview/utils/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1559 2021-10-26 07:14:42.000000 processview-1.2.0/processview/utils/singleton.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4411 2023-05-31 13:34:50.000000 processview-1.2.0/processview/version.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview.egg-info/
--rw-r--r--   0 payno    (81067) soft      (3401)     1043 2023-05-31 14:37:03.000000 processview-1.2.0/processview.egg-info/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)     1200 2023-05-31 14:37:04.000000 processview-1.2.0/processview.egg-info/SOURCES.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-05-31 14:37:03.000000 processview-1.2.0/processview.egg-info/dependency_links.txt
--rw-r--r--   0 payno    (81067) soft      (3401)       73 2023-05-31 14:37:03.000000 processview-1.2.0/processview.egg-info/requires.txt
--rw-r--r--   0 payno    (81067) soft      (3401)       12 2023-05-31 14:37:04.000000 processview-1.2.0/processview.egg-info/top_level.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-05-31 12:44:26.000000 processview-1.2.0/processview.egg-info/zip-safe
--rw-r--r--   0 payno    (81067) soft      (3401)     1089 2023-05-31 14:37:04.312884 processview-1.2.0/setup.cfg
--rw-r--r--   0 payno    (81067) soft      (3401)       69 2023-05-31 13:34:50.000000 processview-1.2.0/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.381427 processview-1.2.1/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.1/LICENSE
+-rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 09:48:11.381427 processview-1.2.1/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      767 2023-06-21 09:33:50.000000 processview-1.2.1/README.md
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.373427 processview-1.2.1/processview/
+-rw-r--r--   0 payno     (1001) payno     (1001)       91 2023-06-21 09:33:50.000000 processview-1.2.1/processview/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3289 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/dataset.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2350 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/helpers.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/manager/
+-rw-r--r--   0 payno     (1001) payno     (1001)       23 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    13677 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/manager/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1534 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4823 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/test/test_manager.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1745 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/setup.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1067 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/sorting.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5128 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/superviseprocess.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1561 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/gui/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    12926 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/icons.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2296 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/messagebox.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    25061 2023-06-21 09:36:58.000000 processview-1.2.1/processview/gui/processmanager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/gui/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1584 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3666 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/test/test_process_manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/resources/
+-rw-r--r--   0 payno     (1001) payno     (1001)    10757 2023-06-21 09:33:50.000000 processview-1.2.1/processview/resources/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1822 2023-06-21 09:33:50.000000 processview-1.2.1/processview/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.381427 processview-1.2.1/processview/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1695 2023-06-21 09:33:50.000000 processview-1.2.1/processview/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.381427 processview-1.2.1/processview/utils/
+-rw-r--r--   0 payno     (1001) payno     (1001)     2565 2023-06-21 09:33:50.000000 processview-1.2.1/processview/utils/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1559 2023-06-21 09:33:50.000000 processview-1.2.1/processview/utils/singleton.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4411 2023-06-21 09:47:52.000000 processview-1.2.1/processview/version.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview.egg-info/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      998 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       94 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/requires.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       12 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/zip-safe
+-rw-r--r--   0 payno     (1001) payno     (1001)     1113 2023-06-21 09:48:11.381427 processview-1.2.1/setup.cfg
+-rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-21 09:33:50.000000 processview-1.2.1/setup.py
```

### Comparing `processview-1.2.0/PKG-INFO` & `processview-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
@@ -19,9 +19,10 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: test
+Provides-Extra: doc
 Provides-Extra: full
 License-File: LICENSE
```

### Comparing `processview-1.2.0/README.md` & `processview-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/dataset.py` & `processview-1.2.1/processview/core/dataset.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/helpers.py` & `processview-1.2.1/processview/core/helpers.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/manager/manager.py` & `processview-1.2.1/processview/core/manager/manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/manager/test/__init__.py` & `processview-1.2.1/processview/core/manager/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/manager/test/test_manager.py` & `processview-1.2.1/processview/core/manager/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/setup.py` & `processview-1.2.1/processview/core/setup.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/sorting.py` & `processview-1.2.1/processview/core/sorting.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/superviseprocess.py` & `processview-1.2.1/processview/core/superviseprocess.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/core/test/__init__.py` & `processview-1.2.1/processview/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/gui/icons.py` & `processview-1.2.1/processview/gui/icons.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/gui/messagebox.py` & `processview-1.2.1/processview/gui/messagebox.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/gui/processmanager.py` & `processview-1.2.1/processview/gui/processmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             process_idx = column - 1
             if process_idx < len(processes):
                 return processes[list(processes.keys())[process_idx]]
 
     def _datasetAt(self, y_pos):
         row = self.rowAt(y_pos)
         if row >= 0:
-            datasets = self.model()._datasets
+            datasets = self.model()._sorted_datasets
             if row < len(datasets):
                 return datasets[list(datasets.keys())[row]]
 
     def contextMenuEvent(self, event):
         row = self.columnAt(event.pos().x())
         dataset = self._datasetAt(event.pos().y())
         if row == 0:
```

### Comparing `processview-1.2.0/processview/gui/test/__init__.py` & `processview-1.2.1/processview/gui/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/gui/test/test_process_manager.py` & `processview-1.2.1/processview/gui/test/test_process_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/resources/__init__.py` & `processview-1.2.1/processview/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/setup.py` & `processview-1.2.1/processview/setup.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/test/__init__.py` & `processview-1.2.1/processview/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/utils/__init__.py` & `processview-1.2.1/processview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/utils/singleton.py` & `processview-1.2.1/processview/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.0/processview/version.py` & `processview-1.2.1/processview/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     "gamma": 11,
     "rc": 12,
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 2
-MICRO = 0
+MICRO = 1
 RELEV = "final"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 from collections import namedtuple
```

### Comparing `processview-1.2.0/processview.egg-info/PKG-INFO` & `processview-1.2.1/processview.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
@@ -19,9 +19,10 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: test
+Provides-Extra: doc
 Provides-Extra: full
 License-File: LICENSE
```

### Comparing `processview-1.2.0/setup.cfg` & `processview-1.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 	packaging
 	wheel
 	silx>=1.0
 
 [options.extras_require]
 test = 
 	pytest
+doc = 
+	Sphinx
 full = 
+	%(doc)s
 	%(test)s
 	PyQt5
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

