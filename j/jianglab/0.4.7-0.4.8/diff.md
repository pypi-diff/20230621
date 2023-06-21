# Comparing `tmp/jianglab-0.4.7.tar.gz` & `tmp/jianglab-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.4.7.tar", last modified: Tue Jun 20 00:55:13 2023, max compression
+gzip compressed data, was "jianglab-0.4.8.tar", last modified: Tue Jun 20 20:36:44 2023, max compression
```

## Comparing `jianglab-0.4.7.tar` & `jianglab-0.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 00:55:13.293694 jianglab-0.4.7/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 00:55:13.293345 jianglab-0.4.7/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.7/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 00:55:13.290531 jianglab-0.4.7/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.7/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    22812 2023-06-20 00:54:58.000000 jianglab-0.4.7/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.7/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 00:55:13.292777 jianglab-0.4.7/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-20 00:55:13.293818 jianglab-0.4.7/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-20 00:55:07.000000 jianglab-0.4.7/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 20:36:44.426046 jianglab-0.4.8/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 20:36:44.425680 jianglab-0.4.8/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.8/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 20:36:44.422157 jianglab-0.4.8/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.8/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    22884 2023-06-20 20:35:52.000000 jianglab-0.4.8/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.8/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 20:36:44.424830 jianglab-0.4.8/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-20 20:36:44.426195 jianglab-0.4.8/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-20 20:36:05.000000 jianglab-0.4.8/setup.py
```

### Comparing `jianglab-0.4.7/PKG-INFO` & `jianglab-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.7
+Version: 0.4.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.7/README.md` & `jianglab-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.4.7/jianglab/common_functions.py` & `jianglab-0.4.8/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,19 @@
     filepath: path to the .cmcr or .cmtr file
     sampling_rate: sampling rate of the light reference
     '''
     raw_data = McsCMOSMEA.McsData(filepath)
     light_ref = raw_data.Acquisition.Analog_Data.ChannelData_1[:,::sampling_rate]
     return light_ref
 
+def hill(x, L, x0, k, b):
+    return L * (x**k) / (x0**k + x**k) + b
+
+
+
 def get_on_times_off_times_of_steps(light_ref, height = 5e4, distance = 400, verbose = True):
     on_times, _ = find_peaks(np.diff(light_ref), height = 5e4, distance = 400)
     if verbose:
         print(on_times.shape)
         print(np.diff(on_times))
     off_times, _ = find_peaks(-np.diff(light_ref), height = 5e4, distance = 400)
     if verbose:
```

### Comparing `jianglab-0.4.7/jianglab.egg-info/PKG-INFO` & `jianglab-0.4.8/jianglab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.7
+Version: 0.4.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.7/setup.py` & `jianglab-0.4.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.4.7',
+    version='0.4.8',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

