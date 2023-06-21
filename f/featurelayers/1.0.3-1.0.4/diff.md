# Comparing `tmp/featurelayers-1.0.3.tar.gz` & `tmp/featurelayers-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.0.3.tar", last modified: Wed Jun 21 11:58:47 2023, max compression
+gzip compressed data, was "featurelayers-1.0.4.tar", last modified: Wed Jun 21 12:04:47 2023, max compression
```

## Comparing `featurelayers-1.0.3.tar` & `featurelayers-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 11:58:47.603378 featurelayers-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-21 11:58:47.594842 featurelayers-1.0.3/FeatureLayers/
--rw-rw-rw-   0        0        0        0 2023-06-21 11:37:38.000000 featurelayers-1.0.3/FeatureLayers/__init__.py
--rw-rw-rw-   0        0        0      391 2023-06-21 11:58:47.602375 featurelayers-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-21 10:03:40.000000 featurelayers-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 11:58:47.601375 featurelayers-1.0.3/featurelayers.egg-info/
--rw-rw-rw-   0        0        0      391 2023-06-21 11:58:47.000000 featurelayers-1.0.3/featurelayers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-21 11:58:47.000000 featurelayers-1.0.3/featurelayers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 11:58:47.000000 featurelayers-1.0.3/featurelayers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-21 11:58:47.000000 featurelayers-1.0.3/featurelayers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-21 11:58:47.000000 featurelayers-1.0.3/featurelayers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 11:58:47.603378 featurelayers-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-21 11:58:46.000000 featurelayers-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:04:47.084690 featurelayers-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-21 12:04:47.076691 featurelayers-1.0.4/FeatureLayers/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:37:38.000000 featurelayers-1.0.4/FeatureLayers/__init__.py
+-rw-rw-rw-   0        0        0      391 2023-06-21 12:04:47.084690 featurelayers-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-21 10:03:40.000000 featurelayers-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 12:04:47.082689 featurelayers-1.0.4/featurelayers.egg-info/
+-rw-rw-rw-   0        0        0      391 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-21 12:04:46.000000 featurelayers-1.0.4/featurelayers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 12:04:47.085689 featurelayers-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-06-21 11:59:57.000000 featurelayers-1.0.4/setup.py
```

### Comparing `featurelayers-1.0.3/setup.py` & `featurelayers-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='featurelayers',
-    version='1.0.3',
+    version='1.0.4',
     description='FeatureLayers Package',
     author='khengyun',
     author_email='khaangnguyeen@email.com',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
```

