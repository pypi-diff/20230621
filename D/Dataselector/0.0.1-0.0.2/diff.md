# Comparing `tmp/Dataselector-0.0.1.tar.gz` & `tmp/Dataselector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dataselector-0.0.1.tar", last modified: Tue Jun 20 13:19:35 2023, max compression
+gzip compressed data, was "Dataselector-0.0.2.tar", last modified: Wed Jun 21 05:50:36 2023, max compression
```

## Comparing `Dataselector-0.0.1.tar` & `Dataselector-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:19:35.604920 Dataselector-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-20 13:19:35.604920 Dataselector-0.0.1/Dataselector.egg-info/
--rw-rw-rw-   0        0        0      786 2023-06-20 13:19:35.000000 Dataselector-0.0.1/Dataselector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-06-20 13:19:35.000000 Dataselector-0.0.1/Dataselector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:19:35.000000 Dataselector-0.0.1/Dataselector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:19:35.000000 Dataselector-0.0.1/Dataselector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-06-20 12:22:56.000000 Dataselector-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      786 2023-06-20 13:19:35.604920 Dataselector-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      123 2023-06-20 12:15:51.000000 Dataselector-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 13:19:35.604920 Dataselector-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-06-20 12:58:56.000000 Dataselector-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:50:36.137707 Dataselector-0.0.2/
+-rw-rw-rw-   0        0        0      150 2023-06-21 04:18:10.000000 Dataselector-0.0.2/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 05:50:36.123824 Dataselector-0.0.2/Dataselector/
+-rw-rw-rw-   0        0        0     3337 2023-06-21 04:29:11.000000 Dataselector-0.0.2/Dataselector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:50:36.130403 Dataselector-0.0.2/Dataselector.egg-info/
+-rw-rw-rw-   0        0        0      854 2023-06-21 05:50:36.000000 Dataselector-0.0.2/Dataselector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-21 05:50:36.000000 Dataselector-0.0.2/Dataselector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:50:36.000000 Dataselector-0.0.2/Dataselector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-21 05:50:36.000000 Dataselector-0.0.2/Dataselector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 05:50:36.000000 Dataselector-0.0.2/Dataselector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-06-20 12:22:56.000000 Dataselector-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-21 04:11:24.000000 Dataselector-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      854 2023-06-21 05:50:36.137707 Dataselector-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2023-06-20 12:15:51.000000 Dataselector-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:50:36.137707 Dataselector-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      873 2023-06-21 05:50:29.000000 Dataselector-0.0.2/setup.py
```

### Comparing `Dataselector-0.0.1/Dataselector.egg-info/PKG-INFO` & `Dataselector-0.0.2/Dataselector.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dataselector
-Version: 0.0.1
+Version: 0.0.2
 Summary: A handy library to import dataset from various excel file types and URls
 Home-page: 
 Author: Siddharth Mishra
 Author-email: Siddharth.mishra@ganitinc.co.in
 License: MIT
 Keywords: Dataset,Import,URl,CSV
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,7 +18,11 @@
 
 Change Log
 ==========
 
 0.0.1 (20/06/2023)
 -------------------
 - First Release
+
+0.0.2 (21/06/2023)
+-------------------
+- Beta test release two
```

### Comparing `Dataselector-0.0.1/LICENSE.txt` & `Dataselector-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Dataselector-0.0.1/PKG-INFO` & `Dataselector-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dataselector
-Version: 0.0.1
+Version: 0.0.2
 Summary: A handy library to import dataset from various excel file types and URls
 Home-page: 
 Author: Siddharth Mishra
 Author-email: Siddharth.mishra@ganitinc.co.in
 License: MIT
 Keywords: Dataset,Import,URl,CSV
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,7 +18,11 @@
 
 Change Log
 ==========
 
 0.0.1 (20/06/2023)
 -------------------
 - First Release
+
+0.0.2 (21/06/2023)
+-------------------
+- Beta test release two
```

### Comparing `Dataselector-0.0.1/setup.py` & `Dataselector-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='Dataselector',
-  version='0.0.1',
+  version='0.0.2',
   description='A handy library to import dataset from various excel file types and URls',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Siddharth Mishra',
   author_email='Siddharth.mishra@ganitinc.co.in',
   license='MIT', 
   classifiers=classifiers,
   keywords='Dataset, Import, URl, CSV', 
   packages=find_packages(),
-  install_requires=[''] 
+  install_requires=['sys','os','pandas','pathlib','ipydatagrid','IPython.display','requests','termcolor','ipyfilechooser'] 
 )
```

