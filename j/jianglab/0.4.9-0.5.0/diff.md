# Comparing `tmp/jianglab-0.4.9.tar.gz` & `tmp/jianglab-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.4.9.tar", last modified: Wed Jun 21 15:59:50 2023, max compression
+gzip compressed data, was "jianglab-0.5.0.tar", last modified: Wed Jun 21 16:07:13 2023, max compression
```

## Comparing `jianglab-0.4.9.tar` & `jianglab-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 15:59:50.786878 jianglab-0.4.9/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 15:59:50.786344 jianglab-0.4.9/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.9/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 15:59:50.781851 jianglab-0.4.9/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.9/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    22888 2023-06-21 15:59:47.000000 jianglab-0.4.9/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.9/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 15:59:50.785451 jianglab-0.4.9/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-21 15:59:50.000000 jianglab-0.4.9/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-21 15:59:50.787018 jianglab-0.4.9/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-21 15:59:45.000000 jianglab-0.4.9/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 16:07:13.825354 jianglab-0.5.0/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 16:07:13.825020 jianglab-0.5.0/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.0/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 16:07:13.822363 jianglab-0.5.0/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.0/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    22892 2023-06-21 16:06:57.000000 jianglab-0.5.0/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.0/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 16:07:13.824415 jianglab-0.5.0/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 16:07:13.000000 jianglab-0.5.0/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-21 16:07:13.000000 jianglab-0.5.0/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-21 16:07:13.000000 jianglab-0.5.0/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-21 16:07:13.000000 jianglab-0.5.0/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-21 16:07:13.000000 jianglab-0.5.0/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-21 16:07:13.825501 jianglab-0.5.0/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-21 16:07:08.000000 jianglab-0.5.0/setup.py
```

### Comparing `jianglab-0.4.9/PKG-INFO` & `jianglab-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.9
+Version: 0.5.0
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.9/README.md` & `jianglab-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.4.9/jianglab/common_functions.py` & `jianglab-0.5.0/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,16 +313,16 @@
     gsheet = import_gsheet()
     bad_lanes = cmcr_file_path.split("\\")[-1].replace("-",".").split(".")[:6]
     bad_lanes = ".".join(bad_lanes)
     bad_lanes = gsheet[gsheet.File_name.str.contains(bad_lanes)]["Bad_lanes"]
     if pd.isna(bad_lanes).any():
         bad_lanes = []
         print("No bad lanes found")
-    elif len(bad_lanes) == 1:
-        bad_lanes = bad_lanes
+    # elif len(bad_lanes) == 1:
+    #     bad_lanes = bad_lanes
     else:                      
         bad_lanes = [int(x) for x in list(bad_lanes)[0].split(",")]
     return bad_lanes
 
 def clean_centers_all_process(arr, neighbour_size = (6,6,6)):
     def find_3d_local_min_general(arr, neighbor_size = (6,6,6)):
         if arr.shape[0] != 0:
```

### Comparing `jianglab-0.4.9/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.0/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.9
+Version: 0.5.0
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.9/setup.py` & `jianglab-0.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.4.9',
+    version='0.5.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

