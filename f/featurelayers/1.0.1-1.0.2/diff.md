# Comparing `tmp/featurelayers-1.0.1.tar.gz` & `tmp/featurelayers-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.0.1.tar", last modified: Wed Jun 21 11:27:57 2023, max compression
+gzip compressed data, was "featurelayers-1.0.2.tar", last modified: Wed Jun 21 11:40:59 2023, max compression
```

## Comparing `featurelayers-1.0.1.tar` & `featurelayers-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 11:27:57.471151 featurelayers-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-21 11:27:57.462639 featurelayers-1.0.1/FeatureLayers/
--rw-rw-rw-   0        0        0       24 2023-06-21 10:37:34.000000 featurelayers-1.0.1/FeatureLayers/__init__.py
--rw-rw-rw-   0        0        0      391 2023-06-21 11:27:57.471151 featurelayers-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-21 10:03:40.000000 featurelayers-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 11:27:57.469151 featurelayers-1.0.1/featurelayers.egg-info/
--rw-rw-rw-   0        0        0      391 2023-06-21 11:27:57.000000 featurelayers-1.0.1/featurelayers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-21 11:27:57.000000 featurelayers-1.0.1/featurelayers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 11:27:57.000000 featurelayers-1.0.1/featurelayers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-21 11:27:57.000000 featurelayers-1.0.1/featurelayers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-21 11:27:57.000000 featurelayers-1.0.1/featurelayers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 11:27:57.472151 featurelayers-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-21 11:27:12.000000 featurelayers-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:40:59.253674 featurelayers-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-21 11:40:59.245162 featurelayers-1.0.2/FeatureLayers/
+-rw-rw-rw-   0        0        0        0 2023-06-21 11:37:38.000000 featurelayers-1.0.2/FeatureLayers/__init__.py
+-rw-rw-rw-   0        0        0      391 2023-06-21 11:40:59.253674 featurelayers-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-21 10:03:40.000000 featurelayers-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 11:40:59.251674 featurelayers-1.0.2/featurelayers.egg-info/
+-rw-rw-rw-   0        0        0      391 2023-06-21 11:40:59.000000 featurelayers-1.0.2/featurelayers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-06-21 11:40:59.000000 featurelayers-1.0.2/featurelayers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 11:40:59.000000 featurelayers-1.0.2/featurelayers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-21 11:40:59.000000 featurelayers-1.0.2/featurelayers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-21 11:40:59.000000 featurelayers-1.0.2/featurelayers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 11:40:59.254673 featurelayers-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-06-21 11:40:23.000000 featurelayers-1.0.2/setup.py
```

### Comparing `featurelayers-1.0.1/setup.py` & `featurelayers-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='featurelayers',
-    version='1.0.1',
+    version='1.0.2',
     description='FeatureLayers Package',
     author='khengyun',
     author_email='khaangnguyeen@email.com',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
```

