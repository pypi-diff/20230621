# Comparing `tmp/gwdali-0.0.5.tar.gz` & `tmp/gwdali-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdali-0.0.5.tar", last modified: Mon Jun 12 18:18:33 2023, max compression
+gzip compressed data, was "gwdali-0.0.6.tar", last modified: Wed Jun 21 17:19:34 2023, max compression
```

## Comparing `gwdali-0.0.5.tar` & `gwdali-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 18:18:33.381553 gwdali-0.0.5/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 18:18:33.377553 gwdali-0.0.5/GWDALI/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 18:18:33.377553 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/
--rw-r--r--   0 josiel    (1000) josiel    (1000)    78018 2022-08-02 22:07:44.000000 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_CE.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    78021 2022-12-22 19:03:32.000000 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_ET.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    83058 2021-03-30 20:13:46.000000 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_K.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    56323 2022-05-06 19:34:28.000000 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_L.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    84000 2020-01-20 12:10:56.000000 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_V.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)       14 2022-11-09 20:10:14.000000 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      921 2023-02-28 14:51:14.000000 gwdali-0.0.5/GWDALI/Detectors_Sensitivity/plot_Sn.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     9246 2023-06-12 01:59:52.000000 gwdali-0.0.5/GWDALI/GWDALI.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.5/GWDALI/__init__.py
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 18:18:33.381553 gwdali-0.0.5/GWDALI/lib/
--rw-r--r--   0 josiel    (1000) josiel    (1000)     2945 2022-08-02 22:07:40.000000 gwdali-0.0.5/GWDALI/lib/Angles_lib.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     8601 2023-05-16 02:02:47.000000 gwdali-0.0.5/GWDALI/lib/Compute_Tensors.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5858 2023-02-16 19:29:30.000000 gwdali-0.0.5/GWDALI/lib/Corner_Plots.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5713 2023-06-12 02:03:46.000000 gwdali-0.0.5/GWDALI/lib/Derivatives_Tensors.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     3172 2023-05-16 01:56:05.000000 gwdali-0.0.5/GWDALI/lib/Dictionaries.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     8121 2023-06-09 16:38:20.000000 gwdali-0.0.5/GWDALI/lib/Likelihood.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     3274 2023-01-20 00:22:18.000000 gwdali-0.0.5/GWDALI/lib/Symmetric_Indexies.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4650 2023-06-12 18:15:33.000000 gwdali-0.0.5/GWDALI/lib/Waveforms.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      145 2023-01-12 19:30:22.000000 gwdali-0.0.5/GWDALI/lib/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.5/LICENSE
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-12 18:18:33.381553 gwdali-0.0.5/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4709 2023-04-14 13:50:04.000000 gwdali-0.0.5/README.md
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 18:18:33.381553 gwdali-0.0.5/gwdali.egg-info/
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-12 18:18:33.000000 gwdali-0.0.5/gwdali.egg-info/PKG-INFO
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      703 2023-06-12 18:18:33.000000 gwdali-0.0.5/gwdali.egg-info/SOURCES.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)        1 2023-06-12 18:18:33.000000 gwdali-0.0.5/gwdali.egg-info/dependency_links.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)        7 2023-06-12 18:18:33.000000 gwdali-0.0.5/gwdali.egg-info/top_level.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-06-12 18:18:33.381553 gwdali-0.0.5/setup.cfg
--rw-r--r--   0 josiel    (1000) josiel    (1000)      760 2023-06-12 18:04:40.000000 gwdali-0.0.5/setup.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.940870 gwdali-0.0.6/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.928870 gwdali-0.0.6/GWDALI/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.936870 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)    78018 2022-08-02 22:07:44.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_CE.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)    78021 2022-12-22 19:03:32.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_ET.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)    83058 2021-03-30 20:13:46.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_K.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)    56323 2022-05-06 19:34:28.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_L.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)    84000 2020-01-20 12:10:56.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_V.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)       14 2022-11-09 20:10:14.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      921 2023-02-28 14:51:14.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/plot_Sn.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     9246 2023-06-12 01:59:52.000000 gwdali-0.0.6/GWDALI/GWDALI.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.6/GWDALI/__init__.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.940870 gwdali-0.0.6/GWDALI/lib/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     2945 2022-08-02 22:07:40.000000 gwdali-0.0.6/GWDALI/lib/Angles_lib.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4176 2023-06-21 16:21:27.000000 gwdali-0.0.6/GWDALI/lib/Compute_Tensors.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5858 2023-02-16 19:29:30.000000 gwdali-0.0.6/GWDALI/lib/Corner_Plots.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5713 2023-06-12 02:03:46.000000 gwdali-0.0.6/GWDALI/lib/Derivatives_Tensors.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     3172 2023-05-16 01:56:05.000000 gwdali-0.0.6/GWDALI/lib/Dictionaries.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     8121 2023-06-09 16:38:20.000000 gwdali-0.0.6/GWDALI/lib/Likelihood.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     1714 2023-06-21 16:06:21.000000 gwdali-0.0.6/GWDALI/lib/Symmetric_Indexies.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4650 2023-06-12 18:15:33.000000 gwdali-0.0.6/GWDALI/lib/Waveforms.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      145 2023-01-12 19:30:22.000000 gwdali-0.0.6/GWDALI/lib/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.6/LICENSE
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-21 17:19:34.940870 gwdali-0.0.6/PKG-INFO
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4709 2023-04-14 13:50:04.000000 gwdali-0.0.6/README.md
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.940870 gwdali-0.0.6/gwdali.egg-info/
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/PKG-INFO
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      703 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/SOURCES.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)        1 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/dependency_links.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)        7 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/top_level.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-06-21 17:19:34.940870 gwdali-0.0.6/setup.cfg
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      760 2023-06-21 17:18:53.000000 gwdali-0.0.6/setup.py
```

### Comparing `gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_CE.txt` & `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_CE.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_ET.txt` & `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_ET.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_K.txt` & `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_K.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_L.txt` & `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_L.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/Detectors_Sensitivity/Sn_V.txt` & `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_V.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/Detectors_Sensitivity/plot_Sn.py` & `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/plot_Sn.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/GWDALI.py` & `gwdali-0.0.6/GWDALI/GWDALI.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/lib/Angles_lib.py` & `gwdali-0.0.6/GWDALI/lib/Angles_lib.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/lib/Corner_Plots.py` & `gwdali-0.0.6/GWDALI/lib/Corner_Plots.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/lib/Derivatives_Tensors.py` & `gwdali-0.0.6/GWDALI/lib/Derivatives_Tensors.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/lib/Dictionaries.py` & `gwdali-0.0.6/GWDALI/lib/Dictionaries.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/lib/Likelihood.py` & `gwdali-0.0.6/GWDALI/lib/Likelihood.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/GWDALI/lib/Waveforms.py` & `gwdali-0.0.6/GWDALI/lib/Waveforms.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/LICENSE` & `gwdali-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/PKG-INFO` & `gwdali-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: jmsdsouza.phd@gmail.com
 License: MIT License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.0.5/README.md` & `gwdali-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/gwdali.egg-info/PKG-INFO` & `gwdali-0.0.6/gwdali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: jmsdsouza.phd@gmail.com
 License: MIT License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.0.5/gwdali.egg-info/SOURCES.txt` & `gwdali-0.0.6/gwdali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.5/setup.py` & `gwdali-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md",'r') as arq:
 	readme = arq.read()
 
 setup(
 	name = 'gwdali',
-	version = '0.0.5',
+	version = '0.0.6',
 	license = 'MIT License',
 	author  = 'Josiel Mendonça Soares de Souza',
 	long_description = readme,
 	long_description_content_type = "text/markdown",
 	author_email = 'jmsdsouza.phd@gmail.com',
 	keywords = 'fisher matrix, gravitational waves, gw, dali',
 	description = 'A Fisher-Based Software for Parameter Estimation from Gravitational Waves',
```

