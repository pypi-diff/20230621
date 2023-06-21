# Comparing `tmp/simply_nwb-0.2.1.tar.gz` & `tmp/simply_nwb-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.2.1.tar", last modified: Fri Jun 16 18:57:33 2023, max compression
+gzip compressed data, was "simply_nwb-0.2.2.tar", last modified: Wed Jun 21 18:20:51 2023, max compression
```

## Comparing `simply_nwb-0.2.1.tar` & `simply_nwb-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.059299 simply_nwb-0.2.1/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      566 2023-06-16 18:57:33.059299 simply_nwb-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-16 18:57:33.059299 simply_nwb-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-06-16 18:57:24.000000 simply_nwb-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.046501 simply_nwb-0.2.1/simply_nwb/
--rw-rw-rw-   0        0        0       87 2023-06-02 16:40:09.000000 simply_nwb-0.2.1/simply_nwb/__init__.py
--rw-rw-rw-   0        0        0    31384 2023-06-12 18:15:13.000000 simply_nwb-0.2.1/simply_nwb/simple_nwb.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.051668 simply_nwb-0.2.1/simply_nwb/transferring/
--rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.2.1/simply_nwb/transferring/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.052677 simply_nwb-0.2.1/simply_nwb/transferring/filesync/
--rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.2.1/simply_nwb/transferring/filesync/__init__.py
--rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.2.1/simply_nwb/transferring/filesync/oneway.py
--rw-rw-rw-   0        0        0     7354 2023-06-02 16:03:22.000000 simply_nwb-0.2.1/simply_nwb/transferring/nwb_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.058797 simply_nwb-0.2.1/simply_nwb/transforms/
--rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.2.1/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/simply_nwb/transforms/blackrock.py
--rw-rw-rw-   0        0        0     1028 2023-06-12 16:22:14.000000 simply_nwb-0.2.1/simply_nwb/transforms/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.2.1/simply_nwb/transforms/labjack.py
--rw-rw-rw-   0        0        0     2111 2023-06-09 18:02:07.000000 simply_nwb-0.2.1/simply_nwb/transforms/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/simply_nwb/transforms/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.2.1/simply_nwb/transforms/plaintext.py
--rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.2.1/simply_nwb/transforms/tif.py
--rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.2.1/simply_nwb/transforms/yaml.py
--rw-rw-rw-   0        0        0     7875 2023-06-08 18:59:36.000000 simply_nwb-0.2.1/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:57:33.049505 simply_nwb-0.2.1/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 18:57:32.000000 simply_nwb-0.2.1/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.122476 simply_nwb-0.2.2/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-06-21 18:20:51.122476 simply_nwb-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-21 18:20:51.122476 simply_nwb-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-06-21 18:20:41.000000 simply_nwb-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.109470 simply_nwb-0.2.2/simply_nwb/
+-rw-rw-rw-   0        0        0       87 2023-06-02 16:40:09.000000 simply_nwb-0.2.2/simply_nwb/__init__.py
+-rw-rw-rw-   0        0        0    31384 2023-06-12 18:15:13.000000 simply_nwb-0.2.2/simply_nwb/simple_nwb.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.114182 simply_nwb-0.2.2/simply_nwb/transferring/
+-rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.2.2/simply_nwb/transferring/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.115502 simply_nwb-0.2.2/simply_nwb/transferring/filesync/
+-rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.2.2/simply_nwb/transferring/filesync/__init__.py
+-rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.2.2/simply_nwb/transferring/filesync/oneway.py
+-rw-rw-rw-   0        0        0     7354 2023-06-02 16:03:22.000000 simply_nwb-0.2.2/simply_nwb/transferring/nwb_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.121472 simply_nwb-0.2.2/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.2.2/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/simply_nwb/transforms/blackrock.py
+-rw-rw-rw-   0        0        0     1028 2023-06-12 16:22:14.000000 simply_nwb-0.2.2/simply_nwb/transforms/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.2.2/simply_nwb/transforms/labjack.py
+-rw-rw-rw-   0        0        0     2111 2023-06-09 18:02:07.000000 simply_nwb-0.2.2/simply_nwb/transforms/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/simply_nwb/transforms/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.2.2/simply_nwb/transforms/plaintext.py
+-rw-rw-rw-   0        0        0     4970 2023-06-21 18:12:56.000000 simply_nwb-0.2.2/simply_nwb/transforms/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.2.2/simply_nwb/transforms/yaml.py
+-rw-rw-rw-   0        0        0     7875 2023-06-08 18:59:36.000000 simply_nwb-0.2.2/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:20:51.112983 simply_nwb-0.2.2/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 18:20:51.000000 simply_nwb-0.2.2/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.2.1/LICENSE` & `simply_nwb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/PKG-INFO` & `simply_nwb-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply_nwb
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.2.1/setup.py` & `simply_nwb-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.2.1/simply_nwb/simple_nwb.py` & `simply_nwb-0.2.2/simply_nwb/simple_nwb.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transferring/__init__.py` & `simply_nwb-0.2.2/simply_nwb/transferring/__init__.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transferring/filesync/oneway.py` & `simply_nwb-0.2.2/simply_nwb/transferring/filesync/oneway.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transferring/nwb_transfer.py` & `simply_nwb-0.2.2/simply_nwb/transferring/nwb_transfer.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transforms/blackrock.py` & `simply_nwb-0.2.2/simply_nwb/transforms/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transforms/csv.py` & `simply_nwb-0.2.2/simply_nwb/transforms/csv.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transforms/labjack.py` & `simply_nwb-0.2.2/simply_nwb/transforms/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transforms/mp4.py` & `simply_nwb-0.2.2/simply_nwb/transforms/mp4.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transforms/p_erg.py` & `simply_nwb-0.2.2/simply_nwb/transforms/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transforms/plaintext.py` & `simply_nwb-0.2.2/simply_nwb/transforms/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb/transforms/tif.py` & `simply_nwb-0.2.2/simply_nwb/transforms/tif.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,101 @@
 import os
 from PIL import Image
 import numpy as np
 import glob
 
 
-def tif_read_image(filename=None):
+class ImageLoadError(Exception):
+    pass
+
+
+def tif_read_image(filename=None, show_error=True):
     """
     Read TIF Image into a numpy array
 
     :param filename: TIF file to read
+    :param show_error: Print out errors or not, defaults to true
     :return: numpy array
     """
 
     if filename is None:
         raise ValueError("Must supply filename argument!")
     if not os.path.exists(filename):
         raise ValueError(f"Filename '{filename}' not found!")
     print(f"Reading TIF: '{filename}'")
 
     try:
         img = Image.open(filename)
         arr = np.array(img)
         img.close()
     except Exception as e:
-        print("ERROR! Failed reading image! (Is the file corrupted?)")
-        raise e
+        if show_error:
+            print("ERROR! Failed reading image! (Is the file corrupted?)")
+            print(f"Error {str(e)}")
+        raise ImageLoadError()
+
     return arr
 
 
-def tif_read_directory(foldername=None, filename_glob="*.tif"):
+def read_filelist(filelist, skip_on_error=False, show_error=True):
+    """
+    Load a list of files and return them
+
+    :param filelist: list of str filenames
+    :param skip_on_error: skip any images that fail
+    :param show_error: show an error when images fail to load
+    :return: list of loaded file data
+    """
+    data = []
+    for file in filelist:
+        try:
+            data.append(tif_read_image(file, show_error=show_error))
+        except ImageLoadError as e:
+            if skip_on_error:
+                print(f"Error reading file '{file}', skipping..")
+                continue
+            raise e
+    return data
+
+
+def tif_read_directory(foldername=None, filename_glob="*.tif", skip_on_error=False):
     """
     Read a directory of TIF files, giving a filename glob for specific TIFs to grab
 
     :param foldername: Folder that contains the TIF images, directly inside
+    :param skip_on_error: Skip any files that fail to load
     :param filename_glob: naming scheme for the TIF files to be collected. e.g. 'image_*.tif'
     :return: numpy array
     """
     if foldername is None:
         raise ValueError("Must provide folder name argument!")
     if not os.path.exists(foldername):
         raise ValueError(f"Folder '{foldername}' not found!")
 
     files = glob.glob(os.path.join(foldername, filename_glob))
     if files is None:
         raise ValueError(f"No files found with glob '{filename_glob}' in folder {foldername}!")
     if any([os.path.isdir(ff) for ff in files]):
         raise ValueError(f"Filename Glob '{filename_glob}' includes a directory!")
 
-    data = []
     print(f"Reading folder of TIFs: '{foldername}'")
-    for file in files:
-        data.append(tif_read_image(file))
+    data = read_filelist(files, skip_on_error=skip_on_error, show_error=not skip_on_error)
+
     return np.array(data)  # Convert our list into a numpy array
 
 
-def tif_read_subfolder_directory(parent_folder=None, subfolder_glob=None, subfolder_glob_fail_on_file_found=False, file_glob=None):
+def tif_read_subfolder_directory(parent_folder=None, subfolder_glob=None, subfolder_glob_fail_on_file_found=False, file_glob=None, skip_on_error=False):
     """
     Read a directory that contains folders that contain TIFs, and read each TIF from each subfolder into memory
 
     :param parent_folder: main folder containing more folders
     :param subfolder_glob: glob to specify which subfolders to look into e.g. 'folder_num_*'
     :param subfolder_glob_fail_on_file_found: If the subfolder glob returns a file, fail the operation. Defaults to True and if a file is matched, it will ignore it
     :param file_glob: TIF file glob to specify which TIFs from the subfolders to read, e.g. 'image0*.tif'
+    :param skip_on_error: Skip any files that fail to load
     :return: numpy array
     """
     if parent_folder is None:
         raise ValueError("Must provide parent_folder argument!")
     if subfolder_glob is None:
         raise ValueError("Must provide subfolder_glob argument!")
     if file_glob is None:
@@ -87,11 +117,11 @@
         print(f"Reading Subfolder of TIFs: '{subfolder}'")
         files = glob.glob(os.path.join(subfolder, file_glob))
         if any([os.path.isdir(f) for f in files]):
             raise ValueError(f"File glob '{file_glob}' returned a directory!")
         filenames.extend(files)
     if not filenames:
         raise ValueError(f"No files found using subfolder glob '{subfolder_glob}' and file glob '{file_glob}'")
-    imgs = []
-    for fn in filenames:
-        imgs.append(tif_read_image(fn))
+
+    print("Reading all files..")
+    imgs = read_filelist(filenames, skip_on_error=skip_on_error, show_error=not skip_on_error)
     return np.array(imgs)
```

### Comparing `simply_nwb-0.2.1/simply_nwb/util.py` & `simply_nwb-0.2.2/simply_nwb/util.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.2.1/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.2.2/simply_nwb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-nwb
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.2.1/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.2.2/simply_nwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

