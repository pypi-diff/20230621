# Comparing `tmp/featurelayers-1.0.7.tar.gz` & `tmp/featurelayers-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.0.7.tar", last modified: Wed Jun 21 17:21:00 2023, max compression
+gzip compressed data, was "featurelayers-1.0.8.tar", last modified: Wed Jun 21 17:35:12 2023, max compression
```

## Comparing `featurelayers-1.0.7.tar` & `featurelayers-1.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.155017 featurelayers-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.151017 featurelayers-1.0.7/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.idea/FeatureLayers.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.151017 featurelayers-1.0.7/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.idea/modules.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.151017 featurelayers-1.0.7/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.idea/runConfigurations/run.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 17:20:38.000000 featurelayers-1.0.7/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 17:21:00.155017 featurelayers-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 17:20:38.000000 featurelayers-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 17:20:38.000000 featurelayers-1.0.7/beforebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.151017 featurelayers-1.0.7/example/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:20:38.000000 featurelayers-1.0.7/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.151017 featurelayers-1.0.7/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 17:20:38.000000 featurelayers-1.0.7/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:20:38.000000 featurelayers-1.0.7/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.155017 featurelayers-1.0.7/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 17:20:38.000000 featurelayers-1.0.7/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 17:20:38.000000 featurelayers-1.0.7/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:21:00.151017 featurelayers-1.0.7/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 17:21:00.000000 featurelayers-1.0.7/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-21 17:21:00.000000 featurelayers-1.0.7/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:21:00.000000 featurelayers-1.0.7/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 17:21:00.000000 featurelayers-1.0.7/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 17:21:00.000000 featurelayers-1.0.7/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:21:00.155017 featurelayers-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-21 17:20:38.000000 featurelayers-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.368566 featurelayers-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.364566 featurelayers-1.0.8/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.idea/FeatureLayers.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.364566 featurelayers-1.0.8/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.idea/modules.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.364566 featurelayers-1.0.8/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.idea/runConfigurations/run.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 17:34:55.000000 featurelayers-1.0.8/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 17:35:12.368566 featurelayers-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 17:34:55.000000 featurelayers-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 17:34:55.000000 featurelayers-1.0.8/beforebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.364566 featurelayers-1.0.8/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:34:55.000000 featurelayers-1.0.8/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.364566 featurelayers-1.0.8/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 17:34:55.000000 featurelayers-1.0.8/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:34:55.000000 featurelayers-1.0.8/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.368566 featurelayers-1.0.8/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 17:34:55.000000 featurelayers-1.0.8/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 17:34:55.000000 featurelayers-1.0.8/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:35:12.368566 featurelayers-1.0.8/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 17:35:12.000000 featurelayers-1.0.8/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-21 17:35:12.000000 featurelayers-1.0.8/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:35:12.000000 featurelayers-1.0.8/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 17:35:12.000000 featurelayers-1.0.8/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 17:35:12.000000 featurelayers-1.0.8/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:35:12.368566 featurelayers-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-21 17:34:55.000000 featurelayers-1.0.8/setup.py
```

### Comparing `featurelayers-1.0.7/featurelayers/layers/LBC.py` & `featurelayers-1.0.8/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.0.7/featurelayers.egg-info/SOURCES.txt` & `featurelayers-1.0.8/featurelayers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featurelayers-1.0.7/setup.py` & `featurelayers-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='featurelayers',
-    version="1.0.7",
+    version="1.0.8",
     description='featurelayers Package',
     author='khengyun',
     author_email='khaangnguyeen@email.com',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
```

