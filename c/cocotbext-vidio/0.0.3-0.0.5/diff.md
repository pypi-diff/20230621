# Comparing `tmp/cocotbext-vidio-0.0.3.tar.gz` & `tmp/cocotbext-vidio-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocotbext-vidio-0.0.3.tar", last modified: Sun Apr 30 22:25:47 2023, max compression
+gzip compressed data, was "cocotbext-vidio-0.0.5.tar", last modified: Wed Jun 21 21:30:05 2023, max compression
```

## Comparing `cocotbext-vidio-0.0.3.tar` & `cocotbext-vidio-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1075 2023-04-30 22:02:02.000000 cocotbext-vidio-0.0.3/LICENSE
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1634 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/PKG-INFO
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      727 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/README.md
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/cocotbext/
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/cocotbext/vidio/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       87 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/__init__.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)    10699 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/colorconv.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      295 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/constants.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      609 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/csc.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     2054 2023-04-30 22:03:53.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/tpg.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     2034 2023-04-30 22:05:53.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/utils.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       21 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/version.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1895 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/vidio.py
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1634 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/PKG-INFO
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      457 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/SOURCES.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)        1 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/dependency_links.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       72 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/requires.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       10 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/top_level.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1133 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/setup.cfg
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       78 2023-04-30 22:04:31.000000 cocotbext-vidio-0.0.3/setup.py
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/tests/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      396 2023-04-30 22:05:46.000000 cocotbext-vidio-0.0.3/tests/test_tpg.py
+drwxrwxr-x   0 nitheesh  (1000) nitheesh  (1000)        0 2023-06-21 21:30:05.871653 cocotbext-vidio-0.0.5/
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)     1075 2023-06-21 21:25:02.000000 cocotbext-vidio-0.0.5/LICENSE
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)     1729 2023-06-21 21:30:05.871653 cocotbext-vidio-0.0.5/PKG-INFO
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)      822 2023-06-21 21:26:04.000000 cocotbext-vidio-0.0.5/README.md
+drwxrwxr-x   0 nitheesh  (1000) nitheesh  (1000)        0 2023-06-21 21:30:05.867653 cocotbext-vidio-0.0.5/cocotbext/
+drwxrwxr-x   0 nitheesh  (1000) nitheesh  (1000)        0 2023-06-21 21:30:05.867653 cocotbext-vidio-0.0.5/cocotbext/vidio/
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)       84 2023-06-21 21:25:33.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/__init__.py
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)    10699 2023-06-21 21:25:02.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/colorconv.py
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)      250 2023-06-21 21:25:37.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/constants.py
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)      609 2023-06-21 21:25:02.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/csc.py
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)     2054 2023-06-21 21:25:02.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/tpg.py
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)     5270 2023-06-21 21:26:48.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/utils.py
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)       21 2023-06-21 21:25:49.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/version.py
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)     2604 2023-06-21 21:25:53.000000 cocotbext-vidio-0.0.5/cocotbext/vidio/vidio.py
+drwxrwxr-x   0 nitheesh  (1000) nitheesh  (1000)        0 2023-06-21 21:30:05.871653 cocotbext-vidio-0.0.5/cocotbext_vidio.egg-info/
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)     1729 2023-06-21 21:30:05.000000 cocotbext-vidio-0.0.5/cocotbext_vidio.egg-info/PKG-INFO
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)      459 2023-06-21 21:30:05.000000 cocotbext-vidio-0.0.5/cocotbext_vidio.egg-info/SOURCES.txt
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)        1 2023-06-21 21:30:05.000000 cocotbext-vidio-0.0.5/cocotbext_vidio.egg-info/dependency_links.txt
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)       72 2023-06-21 21:30:05.000000 cocotbext-vidio-0.0.5/cocotbext_vidio.egg-info/requires.txt
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)       10 2023-06-21 21:30:05.000000 cocotbext-vidio-0.0.5/cocotbext_vidio.egg-info/top_level.txt
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)     1133 2023-06-21 21:30:05.871653 cocotbext-vidio-0.0.5/setup.cfg
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)       78 2023-06-21 21:25:02.000000 cocotbext-vidio-0.0.5/setup.py
+drwxrwxr-x   0 nitheesh  (1000) nitheesh  (1000)        0 2023-06-21 21:30:05.871653 cocotbext-vidio-0.0.5/tests/
+-rw-rw-r--   0 nitheesh  (1000) nitheesh  (1000)      515 2023-06-21 21:25:13.000000 cocotbext-vidio-0.0.5/tests/test_vidio.py
```

### Comparing `cocotbext-vidio-0.0.3/LICENSE` & `cocotbext-vidio-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cocotbext-vidio-0.0.3/PKG-INFO` & `cocotbext-vidio-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotbext-vidio
-Version: 0.0.3
+Version: 0.0.5
 Summary: AXIS video subsystem for cocotb
 Home-page: https://github.com/nitheeshkm/cocotbext-vidio
 Download-URL: https://github.com/nitheeshkm/cocotbext-vidio/tarball/main
 Author: Nitheesh Manjunath
 Author-email: nitheesh2013@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nitheeshkm/cocotbext-vidio/issues
@@ -21,22 +21,23 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # vidio (video io)
 
 This generates the AXIStream frame for video subsystems to be used with cocotb.  
+This generates the AXIStream frame for video subsystems to be used with cocotb.  
 
 Functions:
-- GenRGBAXIStream: Generates an AXIS frame
+- GenAXIStream: Generates an AXIS frame
 - ConvertAXIStreamCS: Converts color space RGB to YUV [In development] 
 
 Roadmap:
-- AXIS to matrix
-- Matrix to AXIS
+- AXIS to matrix [Add 422, 420]
+- Matrix to AXIS 
 - Generate color bars AXIS/matrix, supporting ITU-R BT.601-7, ITU-R BT.709-5
 - Color convertion
 - Chroma convertion
 - Video to SMPTE-2110 packet
 
 References:
 - [Xilinx TPG](https://www.xilinx.com/content/dam/xilinx/support/documents/ip_documentation/v_tpg/v8_1/pg103-v-tpg.pdf)
```

### Comparing `cocotbext-vidio-0.0.3/README.md` & `cocotbext-vidio-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # vidio (video io)
 
 This generates the AXIStream frame for video subsystems to be used with cocotb.  
+This generates the AXIStream frame for video subsystems to be used with cocotb.  
 
 Functions:
-- GenRGBAXIStream: Generates an AXIS frame
+- GenAXIStream: Generates an AXIS frame
 - ConvertAXIStreamCS: Converts color space RGB to YUV [In development] 
 
 Roadmap:
-- AXIS to matrix
-- Matrix to AXIS
+- AXIS to matrix [Add 422, 420]
+- Matrix to AXIS 
 - Generate color bars AXIS/matrix, supporting ITU-R BT.601-7, ITU-R BT.709-5
 - Color convertion
 - Chroma convertion
 - Video to SMPTE-2110 packet
 
 References:
 - [Xilinx TPG](https://www.xilinx.com/content/dam/xilinx/support/documents/ip_documentation/v_tpg/v8_1/pg103-v-tpg.pdf)
```

### Comparing `cocotbext-vidio-0.0.3/cocotbext/vidio/colorconv.py` & `cocotbext-vidio-0.0.5/cocotbext/vidio/colorconv.py`

 * *Files identical despite different names*

### Comparing `cocotbext-vidio-0.0.3/cocotbext/vidio/csc.py` & `cocotbext-vidio-0.0.5/cocotbext/vidio/csc.py`

 * *Files identical despite different names*

### Comparing `cocotbext-vidio-0.0.3/cocotbext/vidio/tpg.py` & `cocotbext-vidio-0.0.5/cocotbext/vidio/tpg.py`

 * *Files identical despite different names*

### Comparing `cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/PKG-INFO` & `cocotbext-vidio-0.0.5/cocotbext_vidio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotbext-vidio
-Version: 0.0.3
+Version: 0.0.5
 Summary: AXIS video subsystem for cocotb
 Home-page: https://github.com/nitheeshkm/cocotbext-vidio
 Download-URL: https://github.com/nitheeshkm/cocotbext-vidio/tarball/main
 Author: Nitheesh Manjunath
 Author-email: nitheesh2013@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nitheeshkm/cocotbext-vidio/issues
@@ -21,22 +21,23 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # vidio (video io)
 
 This generates the AXIStream frame for video subsystems to be used with cocotb.  
+This generates the AXIStream frame for video subsystems to be used with cocotb.  
 
 Functions:
-- GenRGBAXIStream: Generates an AXIS frame
+- GenAXIStream: Generates an AXIS frame
 - ConvertAXIStreamCS: Converts color space RGB to YUV [In development] 
 
 Roadmap:
-- AXIS to matrix
-- Matrix to AXIS
+- AXIS to matrix [Add 422, 420]
+- Matrix to AXIS 
 - Generate color bars AXIS/matrix, supporting ITU-R BT.601-7, ITU-R BT.709-5
 - Color convertion
 - Chroma convertion
 - Video to SMPTE-2110 packet
 
 References:
 - [Xilinx TPG](https://www.xilinx.com/content/dam/xilinx/support/documents/ip_documentation/v_tpg/v8_1/pg103-v-tpg.pdf)
```

### Comparing `cocotbext-vidio-0.0.3/setup.cfg` & `cocotbext-vidio-0.0.5/setup.cfg`

 * *Files identical despite different names*

