# Comparing `tmp/WrikePy-1.0.3.tar.gz` & `tmp/WrikePy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrikePy-1.0.3.tar", last modified: Wed Jun 21 00:19:29 2023, max compression
+gzip compressed data, was "WrikePy-1.0.4.tar", last modified: Wed Jun 21 00:23:06 2023, max compression
```

## Comparing `WrikePy-1.0.3.tar` & `WrikePy-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 00:19:29.971754 WrikePy-1.0.3/
--rw-rw-rw-   0        0        0        0 2023-06-20 16:22:43.000000 WrikePy-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2012 2023-06-21 00:19:29.973258 WrikePy-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-06-20 16:22:43.000000 WrikePy-1.0.3/README.md
--rw-rw-rw-   0        0        0      103 2023-06-20 16:22:43.000000 WrikePy-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      658 2023-06-21 00:19:29.976266 WrikePy-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-21 00:19:29.923125 WrikePy-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 00:19:29.949695 WrikePy-1.0.3/src/WrikePy/
--rw-rw-rw-   0        0        0       45 2023-06-21 00:13:53.000000 WrikePy-1.0.3/src/WrikePy/__init__.py
--rw-rw-rw-   0        0        0     1342 2023-06-20 16:22:43.000000 WrikePy-1.0.3/src/WrikePy/helpers.py
--rw-rw-rw-   0        0        0    84818 2023-06-21 00:19:01.000000 WrikePy-1.0.3/src/WrikePy/wrikepy.py
-drwxrwxrwx   0        0        0        0 2023-06-21 00:19:29.967743 WrikePy-1.0.3/src/WrikePy.egg-info/
--rw-rw-rw-   0        0        0     2012 2023-06-21 00:19:29.000000 WrikePy-1.0.3/src/WrikePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-06-21 00:19:29.000000 WrikePy-1.0.3/src/WrikePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 00:19:29.000000 WrikePy-1.0.3/src/WrikePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 00:19:29.000000 WrikePy-1.0.3/src/WrikePy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 00:23:06.781430 WrikePy-1.0.4/
+-rw-rw-rw-   0        0        0        0 2023-06-20 16:22:43.000000 WrikePy-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2012 2023-06-21 00:23:06.783437 WrikePy-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-06-21 00:22:15.000000 WrikePy-1.0.4/README.md
+-rw-rw-rw-   0        0        0      103 2023-06-20 16:22:43.000000 WrikePy-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      658 2023-06-21 00:23:06.785943 WrikePy-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 00:23:06.721269 WrikePy-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 00:23:06.759373 WrikePy-1.0.4/src/WrikePy/
+-rw-rw-rw-   0        0        0       45 2023-06-21 00:13:53.000000 WrikePy-1.0.4/src/WrikePy/__init__.py
+-rw-rw-rw-   0        0        0     1342 2023-06-20 16:22:43.000000 WrikePy-1.0.4/src/WrikePy/helpers.py
+-rw-rw-rw-   0        0        0    84818 2023-06-21 00:19:01.000000 WrikePy-1.0.4/src/WrikePy/wrikepy.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:23:06.777420 WrikePy-1.0.4/src/WrikePy.egg-info/
+-rw-rw-rw-   0        0        0     2012 2023-06-21 00:23:06.000000 WrikePy-1.0.4/src/WrikePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-06-21 00:23:06.000000 WrikePy-1.0.4/src/WrikePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 00:23:06.000000 WrikePy-1.0.4/src/WrikePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 00:23:06.000000 WrikePy-1.0.4/src/WrikePy.egg-info/top_level.txt
```

### Comparing `WrikePy-1.0.3/PKG-INFO` & `WrikePy-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrikePy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the Wrike API.
 Home-page: https://github.com/TGoers-FNSB/WrikePy
 Author: T. Goers
 Author-email: tristan.goers@fnsb.gov
 Project-URL: Bug Tracker, https://github.com/TGoers-FNSB/WrikePy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 
 # WrikePy
 WrikePy is a Python Wrapper for the [Wrike.com](https://www.wrike.com/) API.
 
 ## Getting Started
 ### Import WrikePy
 ```python
-from wrikepy import *
+from WrikePy import *
 ```
 ### Initialize API
 Every Wrike API call requires a Wrike object parameter in order to send a request.
 ```python
 wrike = Wrike(base_url, perm_access_token, ssl_verify)
 ```
  - The **base_url** parameter is the base URL for every Wrike API
```

### Comparing `WrikePy-1.0.3/README.md` & `WrikePy-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # WrikePy
 WrikePy is a Python Wrapper for the [Wrike.com](https://www.wrike.com/) API.
 
 ## Getting Started
 ### Import WrikePy
 ```python
-from wrikepy import *
+from WrikePy import *
 ```
 ### Initialize API
 Every Wrike API call requires a Wrike object parameter in order to send a request.
 ```python
 wrike = Wrike(base_url, perm_access_token, ssl_verify)
 ```
  - The **base_url** parameter is the base URL for every Wrike API
```

### Comparing `WrikePy-1.0.3/setup.cfg` & `WrikePy-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2057 7269 6b65 5079 0d0a 7665 7273   = WrikePy..vers
-00000020: 696f 6e20 3d20 312e 302e 330d 0a61 7574  ion = 1.0.3..aut
+00000020: 696f 6e20 3d20 312e 302e 340d 0a61 7574  ion = 1.0.4..aut
 00000030: 686f 7220 3d20 542e 2047 6f65 7273 0d0a  hor = T. Goers..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2074  author_email = t
 00000050: 7269 7374 616e 2e67 6f65 7273 4066 6e73  ristan.goers@fns
 00000060: 622e 676f 760d 0a64 6573 6372 6970 7469  b.gov..descripti
 00000070: 6f6e 203d 2041 2050 7974 686f 6e20 7772  on = A Python wr
 00000080: 6170 7065 7220 666f 7220 7468 6520 5772  apper for the Wr
 00000090: 696b 6520 4150 492e 0d0a 6c6f 6e67 5f64  ike API...long_d
```

### Comparing `WrikePy-1.0.3/src/WrikePy/helpers.py` & `WrikePy-1.0.4/src/WrikePy/helpers.py`

 * *Files identical despite different names*

### Comparing `WrikePy-1.0.3/src/WrikePy/wrikepy.py` & `WrikePy-1.0.4/src/WrikePy/wrikepy.py`

 * *Files identical despite different names*

### Comparing `WrikePy-1.0.3/src/WrikePy.egg-info/PKG-INFO` & `WrikePy-1.0.4/src/WrikePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrikePy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the Wrike API.
 Home-page: https://github.com/TGoers-FNSB/WrikePy
 Author: T. Goers
 Author-email: tristan.goers@fnsb.gov
 Project-URL: Bug Tracker, https://github.com/TGoers-FNSB/WrikePy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 
 # WrikePy
 WrikePy is a Python Wrapper for the [Wrike.com](https://www.wrike.com/) API.
 
 ## Getting Started
 ### Import WrikePy
 ```python
-from wrikepy import *
+from WrikePy import *
 ```
 ### Initialize API
 Every Wrike API call requires a Wrike object parameter in order to send a request.
 ```python
 wrike = Wrike(base_url, perm_access_token, ssl_verify)
 ```
  - The **base_url** parameter is the base URL for every Wrike API
```

