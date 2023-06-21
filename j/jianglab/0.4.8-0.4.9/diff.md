# Comparing `tmp/jianglab-0.4.8.tar.gz` & `tmp/jianglab-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.4.8.tar", last modified: Tue Jun 20 20:36:44 2023, max compression
+gzip compressed data, was "jianglab-0.4.9.tar", last modified: Wed Jun 21 15:59:50 2023, max compression
```

## Comparing `jianglab-0.4.8.tar` & `jianglab-0.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 20:36:44.426046 jianglab-0.4.8/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 20:36:44.425680 jianglab-0.4.8/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.8/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 20:36:44.422157 jianglab-0.4.8/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.8/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    22884 2023-06-20 20:35:52.000000 jianglab-0.4.8/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.8/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 20:36:44.424830 jianglab-0.4.8/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-20 20:36:44.000000 jianglab-0.4.8/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-20 20:36:44.426195 jianglab-0.4.8/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-20 20:36:05.000000 jianglab-0.4.8/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 15:59:50.786878 jianglab-0.4.9/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 15:59:50.786344 jianglab-0.4.9/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.9/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 15:59:50.781851 jianglab-0.4.9/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.9/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    22888 2023-06-21 15:59:47.000000 jianglab-0.4.9/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.9/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 15:59:50.785451 jianglab-0.4.9/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-21 15:59:50.787018 jianglab-0.4.9/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-21 15:59:45.000000 jianglab-0.4.9/setup.py
```

### Comparing `jianglab-0.4.8/PKG-INFO` & `jianglab-0.4.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.8
+Version: 0.4.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.8/README.md` & `jianglab-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.4.8/jianglab/common_functions.py` & `jianglab-0.4.9/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     np_array = raw_cmcr_data.Acquisition.Sensor_Data.SensorData_1_1
     images = np_array[::pre_resample_rate]
     images = resample_med(images, kernel_size= kernel_size, resample_rate = post_resample_rate) 
     return images
 
 
 def remove_bad_lanes(data, bad_lanes): # for low pass filtered data
-    if bad_lanes != []:
+    if len(bad_lanes) != 0:
         data = np.delete(data, [int(lane)-1 for lane in bad_lanes], axis= 2)
     else:
         pass
     return data
 
 def save_instance(filename, instance):
     with open(filename, "wb") as file_:
```

### Comparing `jianglab-0.4.8/jianglab.egg-info/PKG-INFO` & `jianglab-0.4.9/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.8
+Version: 0.4.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.8/setup.py` & `jianglab-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.4.8',
+    version='0.4.9',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

