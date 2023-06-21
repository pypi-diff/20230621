# Comparing `tmp/newport-motors-py-0.1.0.tar.gz` & `tmp/newport-motors-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newport-motors-py-0.1.0.tar", last modified: Wed Jun 21 03:25:22 2023, max compression
+gzip compressed data, was "newport-motors-py-0.1.1.tar", last modified: Wed Jun 21 03:49:03 2023, max compression
```

## Comparing `newport-motors-py-0.1.0.tar` & `newport-motors-py-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1067 2023-06-18 08:47:09.000000 newport-motors-py-0.1.0/LICENSE
--rw-rw-r--   0 adam      (1000) adam      (1000)     4659 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/PKG-INFO
--rw-rw-r--   0 adam      (1000) adam      (1000)     4199 2023-06-21 03:22:07.000000 newport-motors-py-0.1.0/README.md
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/GUI/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1612 2023-05-15 00:20:57.000000 newport-motors-py-0.1.0/newport_motors/GUI/CustomNumeric.py
--rw-rw-r--   0 adam      (1000) adam      (1000)      141 2023-05-15 01:50:46.000000 newport-motors-py-0.1.0/newport_motors/GUI/InstrumentGUI.py
--rw-rw-r--   0 adam      (1000) adam      (1000)      982 2023-06-05 00:14:07.000000 newport-motors-py-0.1.0/newport_motors/GUI/LinearUI.py
--rw-rw-r--   0 adam      (1000) adam      (1000)     2206 2023-06-07 05:22:30.000000 newport-motors-py-0.1.0/newport_motors/GUI/TipTiltUI.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/Mocks/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1637 2023-05-11 05:05:38.000000 newport-motors-py-0.1.0/newport_motors/Mocks/motor.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/Motors/
--rw-rw-r--   0 adam      (1000) adam      (1000)     7395 2023-06-10 00:24:39.000000 newport-motors-py-0.1.0/newport_motors/Motors/instrument.py
--rw-rw-r--   0 adam      (1000) adam      (1000)    11499 2023-06-10 00:27:37.000000 newport-motors-py-0.1.0/newport_motors/Motors/motor.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/USBs/
--rw-rw-r--   0 adam      (1000) adam      (1000)     3779 2023-06-10 00:28:40.000000 newport-motors-py-0.1.0/newport_motors/USBs/USBs.py
--rw-rw-r--   0 adam      (1000) adam      (1000)      211 2023-06-19 13:13:53.000000 newport-motors-py-0.1.0/newport_motors/__init__.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors_py.egg-info/
--rw-rw-r--   0 adam      (1000) adam      (1000)     4659 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1000) adam      (1000)      586 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)        1 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)       60 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/requires.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)      109 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/top_level.txt
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/pyvisa_mock/
--rw-rw-r--   0 adam      (1000) adam      (1000)       87 2023-06-21 03:15:09.000000 newport-motors-py-0.1.0/pyvisa_mock/__init__.py
--rw-rw-r--   0 adam      (1000) adam      (1000)       38 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/setup.cfg
--rw-rw-r--   0 adam      (1000) adam      (1000)     1893 2023-06-21 03:15:37.000000 newport-motors-py-0.1.0/setup.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/tests/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1125 2023-06-19 12:49:39.000000 newport-motors-py-0.1.0/tests/test_motor.py
--rw-rw-r--   0 adam      (1000) adam      (1000)     1178 2023-06-19 13:05:28.000000 newport-motors-py-0.1.0/tests/test_motor_mock.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1067 2023-06-18 08:47:09.000000 newport-motors-py-0.1.1/LICENSE
+-rw-rw-r--   0 adam      (1000) adam      (1000)     4659 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/PKG-INFO
+-rw-rw-r--   0 adam      (1000) adam      (1000)     4199 2023-06-21 03:22:07.000000 newport-motors-py-0.1.1/README.md
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/newport_motors/
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/newport_motors/GUI/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1612 2023-05-15 00:20:57.000000 newport-motors-py-0.1.1/newport_motors/GUI/CustomNumeric.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)      141 2023-05-15 01:50:46.000000 newport-motors-py-0.1.1/newport_motors/GUI/InstrumentGUI.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)      982 2023-06-05 00:14:07.000000 newport-motors-py-0.1.1/newport_motors/GUI/LinearUI.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)     2206 2023-06-07 05:22:30.000000 newport-motors-py-0.1.1/newport_motors/GUI/TipTiltUI.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/newport_motors/Mocks/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1637 2023-05-11 05:05:38.000000 newport-motors-py-0.1.1/newport_motors/Mocks/motor.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/newport_motors/Motors/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     7395 2023-06-10 00:24:39.000000 newport-motors-py-0.1.1/newport_motors/Motors/instrument.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)    11499 2023-06-10 00:27:37.000000 newport-motors-py-0.1.1/newport_motors/Motors/motor.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/newport_motors/USBs/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     3779 2023-06-10 00:28:40.000000 newport-motors-py-0.1.1/newport_motors/USBs/USBs.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)      211 2023-06-21 03:49:01.000000 newport-motors-py-0.1.1/newport_motors/__init__.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/newport_motors_py.egg-info/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     4659 2023-06-21 03:49:03.000000 newport-motors-py-0.1.1/newport_motors_py.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1000) adam      (1000)      586 2023-06-21 03:49:03.000000 newport-motors-py-0.1.1/newport_motors_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1000) adam      (1000)        1 2023-06-21 03:49:03.000000 newport-motors-py-0.1.1/newport_motors_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1000) adam      (1000)       60 2023-06-21 03:49:03.000000 newport-motors-py-0.1.1/newport_motors_py.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1000) adam      (1000)      109 2023-06-21 03:49:03.000000 newport-motors-py-0.1.1/newport_motors_py.egg-info/top_level.txt
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/pyvisa_mock/
+-rw-rw-r--   0 adam      (1000) adam      (1000)       87 2023-06-21 03:15:09.000000 newport-motors-py-0.1.1/pyvisa_mock/__init__.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)       38 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/setup.cfg
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1893 2023-06-21 03:41:24.000000 newport-motors-py-0.1.1/setup.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:49:03.321325 newport-motors-py-0.1.1/tests/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1125 2023-06-19 12:49:39.000000 newport-motors-py-0.1.1/tests/test_motor.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1178 2023-06-19 13:05:28.000000 newport-motors-py-0.1.1/tests/test_motor_mock.py
```

### Comparing `newport-motors-py-0.1.0/LICENSE` & `newport-motors-py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/PKG-INFO` & `newport-motors-py-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newport-motors-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package for operating newport motors
 Home-page: https://github.com/ataras2/newport_motors
 Author: Adam Taras
 Author-email: adam.taras@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/ataras2/newport_motors/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `newport-motors-py-0.1.0/README.md` & `newport-motors-py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors/GUI/CustomNumeric.py` & `newport-motors-py-0.1.1/newport_motors/GUI/CustomNumeric.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors/GUI/LinearUI.py` & `newport-motors-py-0.1.1/newport_motors/GUI/LinearUI.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors/GUI/TipTiltUI.py` & `newport-motors-py-0.1.1/newport_motors/GUI/TipTiltUI.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors/Mocks/motor.py` & `newport-motors-py-0.1.1/newport_motors/Mocks/motor.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors/Motors/instrument.py` & `newport-motors-py-0.1.1/newport_motors/Motors/instrument.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors/Motors/motor.py` & `newport-motors-py-0.1.1/newport_motors/Motors/motor.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors/USBs/USBs.py` & `newport-motors-py-0.1.1/newport_motors/USBs/USBs.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/newport_motors_py.egg-info/PKG-INFO` & `newport-motors-py-0.1.1/newport_motors_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newport-motors-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package for operating newport motors
 Home-page: https://github.com/ataras2/newport_motors
 Author: Adam Taras
 Author-email: adam.taras@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/ataras2/newport_motors/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `newport-motors-py-0.1.0/newport_motors_py.egg-info/SOURCES.txt` & `newport-motors-py-0.1.1/newport_motors_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/setup.py` & `newport-motors-py-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/tests/test_motor.py` & `newport-motors-py-0.1.1/tests/test_motor.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.1.0/tests/test_motor_mock.py` & `newport-motors-py-0.1.1/tests/test_motor_mock.py`

 * *Files identical despite different names*

