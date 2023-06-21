# Comparing `tmp/simply_nwb-0.2.2.tar.gz` & `tmp/simply_nwb-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.2.2.tar", last modified: Wed Jun 21 18:20:51 2023, max compression
+gzip compressed data, was "simply_nwb-0.2.3.tar", last modified: Wed Jun 21 18:27:22 2023, max compression
```

## Comparing `simply_nwb-0.2.2.tar` & `simply_nwb-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.122476 simply_nwb-0.2.2/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      566 2023-06-21 18:20:51.122476 simply_nwb-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-21 18:20:51.122476 simply_nwb-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-06-21 18:20:41.000000 simply_nwb-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.109470 simply_nwb-0.2.2/simply_nwb/
--rw-rw-rw-   0        0        0       87 2023-06-02 16:40:09.000000 simply_nwb-0.2.2/simply_nwb/__init__.py
--rw-rw-rw-   0        0        0    31384 2023-06-12 18:15:13.000000 simply_nwb-0.2.2/simply_nwb/simple_nwb.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.114182 simply_nwb-0.2.2/simply_nwb/transferring/
--rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.2.2/simply_nwb/transferring/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.115502 simply_nwb-0.2.2/simply_nwb/transferring/filesync/
--rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.2.2/simply_nwb/transferring/filesync/__init__.py
--rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.2.2/simply_nwb/transferring/filesync/oneway.py
--rw-rw-rw-   0        0        0     7354 2023-06-02 16:03:22.000000 simply_nwb-0.2.2/simply_nwb/transferring/nwb_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.121472 simply_nwb-0.2.2/simply_nwb/transforms/
--rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.2.2/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/simply_nwb/transforms/blackrock.py
--rw-rw-rw-   0        0        0     1028 2023-06-12 16:22:14.000000 simply_nwb-0.2.2/simply_nwb/transforms/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.2.2/simply_nwb/transforms/labjack.py
--rw-rw-rw-   0        0        0     2111 2023-06-09 18:02:07.000000 simply_nwb-0.2.2/simply_nwb/transforms/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/simply_nwb/transforms/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/simply_nwb/transforms/plaintext.py
--rw-rw-rw-   0        0        0     4970 2023-06-21 18:12:56.000000 simply_nwb-0.2.2/simply_nwb/transforms/tif.py
--rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.2.2/simply_nwb/transforms/yaml.py
--rw-rw-rw-   0        0        0     7875 2023-06-08 18:59:36.000000 simply_nwb-0.2.2/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.112983 simply_nwb-0.2.2/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 18:27:22.338190 simply_nwb-0.2.3/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-06-21 18:27:22.337189 simply_nwb-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.2.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-21 18:27:22.338190 simply_nwb-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-06-21 18:27:21.000000 simply_nwb-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:27:22.324143 simply_nwb-0.2.3/simply_nwb/
+-rw-rw-rw-   0        0        0       87 2023-06-02 16:40:09.000000 simply_nwb-0.2.3/simply_nwb/__init__.py
+-rw-rw-rw-   0        0        0    31384 2023-06-12 18:15:13.000000 simply_nwb-0.2.3/simply_nwb/simple_nwb.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:27:22.329149 simply_nwb-0.2.3/simply_nwb/transferring/
+-rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.2.3/simply_nwb/transferring/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:27:22.330143 simply_nwb-0.2.3/simply_nwb/transferring/filesync/
+-rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.2.3/simply_nwb/transferring/filesync/__init__.py
+-rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.2.3/simply_nwb/transferring/filesync/oneway.py
+-rw-rw-rw-   0        0        0     7354 2023-06-02 16:03:22.000000 simply_nwb-0.2.3/simply_nwb/transferring/nwb_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:27:22.336199 simply_nwb-0.2.3/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.2.3/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.2.3/simply_nwb/transforms/blackrock.py
+-rw-rw-rw-   0        0        0     1028 2023-06-12 16:22:14.000000 simply_nwb-0.2.3/simply_nwb/transforms/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.2.3/simply_nwb/transforms/labjack.py
+-rw-rw-rw-   0        0        0     2111 2023-06-09 18:02:07.000000 simply_nwb-0.2.3/simply_nwb/transforms/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.2.3/simply_nwb/transforms/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.2.3/simply_nwb/transforms/plaintext.py
+-rw-rw-rw-   0        0        0     4970 2023-06-21 18:12:56.000000 simply_nwb-0.2.3/simply_nwb/transforms/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.2.3/simply_nwb/transforms/yaml.py
+-rw-rw-rw-   0        0        0     7875 2023-06-08 18:59:36.000000 simply_nwb-0.2.3/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:27:22.328142 simply_nwb-0.2.3/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-06-21 18:27:22.000000 simply_nwb-0.2.3/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-06-21 18:27:22.000000 simply_nwb-0.2.3/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 18:27:22.000000 simply_nwb-0.2.3/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-21 18:27:22.000000 simply_nwb-0.2.3/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 18:27:22.000000 simply_nwb-0.2.3/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.2.2/LICENSE` & `simply_nwb-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/PKG-INFO` & `simply_nwb-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply_nwb
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.2.2/setup.py` & `simply_nwb-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.2.2/simply_nwb/simple_nwb.py` & `simply_nwb-0.2.3/simply_nwb/simple_nwb.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transferring/__init__.py` & `simply_nwb-0.2.3/simply_nwb/transferring/__init__.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transferring/filesync/oneway.py` & `simply_nwb-0.2.3/simply_nwb/transferring/filesync/oneway.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transferring/nwb_transfer.py` & `simply_nwb-0.2.3/simply_nwb/transferring/nwb_transfer.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transforms/blackrock.py` & `simply_nwb-0.2.3/simply_nwb/transforms/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transforms/csv.py` & `simply_nwb-0.2.3/simply_nwb/transforms/csv.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transforms/labjack.py` & `simply_nwb-0.2.3/simply_nwb/transforms/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transforms/mp4.py` & `simply_nwb-0.2.3/simply_nwb/transforms/mp4.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transforms/p_erg.py` & `simply_nwb-0.2.3/simply_nwb/transforms/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transforms/plaintext.py` & `simply_nwb-0.2.3/simply_nwb/transforms/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/transforms/tif.py` & `simply_nwb-0.2.3/simply_nwb/transforms/tif.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb/util.py` & `simply_nwb-0.2.3/simply_nwb/util.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.2/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.2.3/simply_nwb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-nwb
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.2.2/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.2.3/simply_nwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

