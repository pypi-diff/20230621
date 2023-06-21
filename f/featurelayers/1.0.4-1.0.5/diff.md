# Comparing `tmp/featurelayers-1.0.4.tar.gz` & `tmp/featurelayers-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.0.4.tar", last modified: Wed Jun 21 12:04:47 2023, max compression
+gzip compressed data, was "featurelayers-1.0.5.tar", last modified: Wed Jun 21 12:11:30 2023, max compression
```

## Comparing `featurelayers-1.0.4.tar` & `featurelayers-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 12:04:47.084690 featurelayers-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-21 12:04:47.076691 featurelayers-1.0.4/FeatureLayers/
--rw-rw-rw-   0        0        0        0 2023-06-21 11:37:38.000000 featurelayers-1.0.4/FeatureLayers/__init__.py
--rw-rw-rw-   0        0        0      391 2023-06-21 12:04:47.084690 featurelayers-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-21 10:03:40.000000 featurelayers-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 12:04:47.082689 featurelayers-1.0.4/featurelayers.egg-info/
--rw-rw-rw-   0        0        0      391 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 12:04:47.085689 featurelayers-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-21 11:59:57.000000 featurelayers-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.708572 featurelayers-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.698014 featurelayers-1.0.5/FeatureLayers/
+drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.700557 featurelayers-1.0.5/FeatureLayers/Layers/
+-rw-rw-rw-   0        0        0     3131 2023-06-21 10:29:31.000000 featurelayers-1.0.5/FeatureLayers/Layers/LBC.py
+-rw-rw-rw-   0        0        0        0 2023-06-21 12:11:05.000000 featurelayers-1.0.5/FeatureLayers/Layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:37:38.000000 featurelayers-1.0.5/FeatureLayers/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-06-21 12:11:20.000000 featurelayers-1.0.5/FeatureLayers/example.py
+-rw-rw-rw-   0        0        0      391 2023-06-21 12:11:30.708572 featurelayers-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-21 10:03:40.000000 featurelayers-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.706560 featurelayers-1.0.5/featurelayers.egg-info/
+-rw-rw-rw-   0        0        0      391 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 12:11:30.709574 featurelayers-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-06-21 12:11:29.000000 featurelayers-1.0.5/setup.py
```

### Comparing `featurelayers-1.0.4/setup.py` & `featurelayers-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='featurelayers',
-    version='1.0.4',
+    version='1.0.5',
     description='FeatureLayers Package',
     author='khengyun',
     author_email='khaangnguyeen@email.com',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
```

