# Comparing `tmp/AqEquil-0.9.2.tar.gz` & `tmp/AqEquil-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AqEquil-0.9.2.tar", last modified: Sat Oct  2 15:44:52 2021, max compression
+gzip compressed data, was "dist\AqEquil-0.9.3.tar", last modified: Sun Oct  3 14:06:22 2021, max compression
```

## Comparing `AqEquil-0.9.2.tar` & `AqEquil-0.9.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-10-02 15:44:52.000000 AqEquil-0.9.2/
-drwxrwxrwx   0        0        0        0 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil/
--rw-rw-rw-   0        0        0   116553 2021-10-02 15:43:30.000000 AqEquil-0.9.2/AqEquil/AqSpeciation.py
--rw-rw-rw-   0        0        0       39 2021-10-02 15:43:28.000000 AqEquil-0.9.2/AqEquil/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil.egg-info/
--rw-rw-rw-   0        0        0     3275 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-10-02 15:44:52.000000 AqEquil-0.9.2/AqEquil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3275 2021-10-02 15:44:52.000000 AqEquil-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     2417 2021-10-02 15:40:52.000000 AqEquil-0.9.2/README.md
--rw-rw-rw-   0        0        0       42 2021-10-02 15:44:52.000000 AqEquil-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      805 2021-10-02 15:43:56.000000 AqEquil-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-03 14:06:22.000000 AqEquil-0.9.3/
+drwxrwxrwx   0        0        0        0 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil/
+-rw-rw-rw-   0        0        0   116546 2021-10-03 14:05:54.000000 AqEquil-0.9.3/AqEquil/AqSpeciation.py
+-rw-rw-rw-   0        0        0       39 2021-10-03 14:05:54.000000 AqEquil-0.9.3/AqEquil/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil.egg-info/
+-rw-rw-rw-   0        0        0     3275 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-10-03 14:06:22.000000 AqEquil-0.9.3/AqEquil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3275 2021-10-03 14:06:22.000000 AqEquil-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2021-10-03 14:04:47.000000 AqEquil-0.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2021-10-03 14:06:22.000000 AqEquil-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      805 2021-10-03 14:05:32.000000 AqEquil-0.9.3/setup.py
```

### Comparing `AqEquil-0.9.2/AqEquil/AqSpeciation.py` & `AqEquil-0.9.3/AqEquil/AqSpeciation.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,15 +745,15 @@
         config = {'displaylogo': False,
                   'modeBarButtonsToRemove': ['zoom2d', 'pan2d', 'select2d',
                                              'lasso2d', 'zoomIn2d', 'zoomOut2d',
                                              'autoScale2d', 'resetScale2d',
                                              'toggleSpikelines'],
                   'toImageButtonOptions': {
                                              'format': save_format,
-                                             'filename': save_as+'.png',
+                                             'filename': save_as,
                                              'height': plot_height*ppi,
                                              'width': plot_width*ppi,
                                              'scale': save_scale,
                                            },
                   }
         if not interactive:
             config['staticPlot'] = True
```

### Comparing `AqEquil-0.9.2/AqEquil.egg-info/PKG-INFO` & `AqEquil-0.9.3/AqEquil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AqEquil
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python tools for aqueous chemical speciation.
 Home-page: UNKNOWN
 Author: Grayson Boyer
 Author-email: gmboyer@asu.edu
 License: UNKNOWN
 Description: # AqEquil
```

### Comparing `AqEquil-0.9.2/PKG-INFO` & `AqEquil-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AqEquil
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python tools for aqueous chemical speciation.
 Home-page: UNKNOWN
 Author: Grayson Boyer
 Author-email: gmboyer@asu.edu
 License: UNKNOWN
 Description: # AqEquil
```

### Comparing `AqEquil-0.9.2/README.md` & `AqEquil-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `AqEquil-0.9.2/setup.py` & `AqEquil-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AqEquil",
-    version="0.9.2",
+    version="0.9.3",
     author="Grayson Boyer",
     author_email="gmboyer@asu.edu",
     description="Python tools for aqueous chemical speciation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={},
     packages=['AqEquil'],
```

