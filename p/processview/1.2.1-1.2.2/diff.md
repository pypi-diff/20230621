# Comparing `tmp/processview-1.2.1.tar.gz` & `tmp/processview-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processview-1.2.1.tar", last modified: Wed Jun 21 09:48:11 2023, max compression
+gzip compressed data, was "processview-1.2.2.tar", last modified: Wed Jun 21 11:54:30 2023, max compression
```

## Comparing `processview-1.2.1.tar` & `processview-1.2.2.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.381427 processview-1.2.1/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.1/LICENSE
--rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 09:48:11.381427 processview-1.2.1/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)      767 2023-06-21 09:33:50.000000 processview-1.2.1/README.md
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.373427 processview-1.2.1/processview/
--rw-r--r--   0 payno     (1001) payno     (1001)       91 2023-06-21 09:33:50.000000 processview-1.2.1/processview/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3289 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/dataset.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2350 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/helpers.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/manager/
--rw-r--r--   0 payno     (1001) payno     (1001)       23 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    13677 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/manager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/manager/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1534 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/test/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4823 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/manager/test/test_manager.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1745 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/setup.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1067 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/sorting.py
--rw-r--r--   0 payno     (1001) payno     (1001)     5128 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/superviseprocess.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/core/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1561 2023-06-21 09:33:50.000000 processview-1.2.1/processview/core/test/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/gui/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    12926 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/icons.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2296 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/messagebox.py
--rw-r--r--   0 payno     (1001) payno     (1001)    25061 2023-06-21 09:36:58.000000 processview-1.2.1/processview/gui/processmanager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/gui/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1584 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/test/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3666 2023-06-21 09:33:50.000000 processview-1.2.1/processview/gui/test/test_process_manager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview/resources/
--rw-r--r--   0 payno     (1001) payno     (1001)    10757 2023-06-21 09:33:50.000000 processview-1.2.1/processview/resources/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1822 2023-06-21 09:33:50.000000 processview-1.2.1/processview/setup.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.381427 processview-1.2.1/processview/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1695 2023-06-21 09:33:50.000000 processview-1.2.1/processview/test/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.381427 processview-1.2.1/processview/utils/
--rw-r--r--   0 payno     (1001) payno     (1001)     2565 2023-06-21 09:33:50.000000 processview-1.2.1/processview/utils/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1559 2023-06-21 09:33:50.000000 processview-1.2.1/processview/utils/singleton.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4411 2023-06-21 09:47:52.000000 processview-1.2.1/processview/version.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 09:48:11.377427 processview-1.2.1/processview.egg-info/
--rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)      998 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1001) payno     (1001)       94 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/requires.txt
--rw-r--r--   0 payno     (1001) payno     (1001)       12 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/top_level.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.2.1/processview.egg-info/zip-safe
--rw-r--r--   0 payno     (1001) payno     (1001)     1113 2023-06-21 09:48:11.381427 processview-1.2.1/setup.cfg
--rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-21 09:33:50.000000 processview-1.2.1/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.2/LICENSE
+-rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 11:54:30.218018 processview-1.2.2/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      767 2023-06-21 09:33:50.000000 processview-1.2.2/README.md
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.210018 processview-1.2.2/processview/
+-rw-r--r--   0 payno     (1001) payno     (1001)       91 2023-06-21 09:33:50.000000 processview-1.2.2/processview/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3289 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/dataset.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2350 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/helpers.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/manager/
+-rw-r--r--   0 payno     (1001) payno     (1001)       23 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    13677 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/manager/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1534 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4823 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/test/test_manager.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1745 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/setup.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1067 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/sorting.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5128 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/superviseprocess.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1561 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/gui/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    12926 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/icons.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2296 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/messagebox.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    25061 2023-06-21 09:36:58.000000 processview-1.2.2/processview/gui/processmanager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/gui/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1584 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3666 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/test/test_process_manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/resources/
+-rw-r--r--   0 payno     (1001) payno     (1001)    10757 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.210018 processview-1.2.2/processview/resources/gui/
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/resources/gui/icons/
+-rw-r--r--   0 payno     (1001) payno     (1001)      729 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/advancement.png
+-rw-r--r--   0 payno     (1001) payno     (1001)     5781 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/advancement.svg
+-rw-r--r--   0 payno     (1001) payno     (1001)      926 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/magnifying_glass.png
+-rw-r--r--   0 payno     (1001) payno     (1001)     4631 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/magnifying_glass.svg
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1695 2023-06-21 09:33:50.000000 processview-1.2.2/processview/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/utils/
+-rw-r--r--   0 payno     (1001) payno     (1001)     2565 2023-06-21 09:33:50.000000 processview-1.2.2/processview/utils/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1559 2023-06-21 09:33:50.000000 processview-1.2.2/processview/utils/singleton.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4411 2023-06-21 11:53:53.000000 processview-1.2.2/processview/version.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview.egg-info/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)     1179 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       94 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/requires.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       12 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.2.2/processview.egg-info/zip-safe
+-rw-r--r--   0 payno     (1001) payno     (1001)     1196 2023-06-21 11:54:30.218018 processview-1.2.2/setup.cfg
+-rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-21 09:33:50.000000 processview-1.2.2/setup.py
```

### Comparing `processview-1.2.1/PKG-INFO` & `processview-1.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

### Comparing `processview-1.2.1/README.md` & `processview-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/dataset.py` & `processview-1.2.2/processview/core/dataset.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/helpers.py` & `processview-1.2.2/processview/core/helpers.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/manager/manager.py` & `processview-1.2.2/processview/core/manager/manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/manager/test/__init__.py` & `processview-1.2.2/processview/core/manager/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/manager/test/test_manager.py` & `processview-1.2.2/processview/core/manager/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/setup.py` & `processview-1.2.2/processview/core/setup.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/sorting.py` & `processview-1.2.2/processview/core/sorting.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/superviseprocess.py` & `processview-1.2.2/processview/core/superviseprocess.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/core/test/__init__.py` & `processview-1.2.2/processview/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/gui/icons.py` & `processview-1.2.2/processview/gui/icons.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/gui/messagebox.py` & `processview-1.2.2/processview/gui/messagebox.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/gui/processmanager.py` & `processview-1.2.2/processview/gui/processmanager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/gui/test/__init__.py` & `processview-1.2.2/processview/gui/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/gui/test/test_process_manager.py` & `processview-1.2.2/processview/gui/test/test_process_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/resources/__init__.py` & `processview-1.2.2/processview/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/test/__init__.py` & `processview-1.2.2/processview/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/utils/__init__.py` & `processview-1.2.2/processview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/utils/singleton.py` & `processview-1.2.2/processview/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.1/processview/version.py` & `processview-1.2.2/processview/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     "gamma": 11,
     "rc": 12,
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 2
-MICRO = 1
+MICRO = 2
 RELEV = "final"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 from collections import namedtuple
```

### Comparing `processview-1.2.1/processview.egg-info/PKG-INFO` & `processview-1.2.2/processview.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

### Comparing `processview-1.2.1/setup.cfg` & `processview-1.2.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 packages = find:
 install_requires = 
 	setuptools
 	packaging
 	wheel
 	silx>=1.0
 
+[options.package_data]
+processview.resources = 
+	gui/icons/*.png
+	gui/icons/*.svg
+
 [options.extras_require]
 test = 
 	pytest
 doc = 
 	Sphinx
 full = 
 	%(doc)s
```

