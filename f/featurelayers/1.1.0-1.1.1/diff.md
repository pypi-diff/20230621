# Comparing `tmp/featurelayers-1.1.0.tar.gz` & `tmp/featurelayers-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.1.0.tar", last modified: Wed Jun 21 18:51:49 2023, max compression
+gzip compressed data, was "featurelayers-1.1.1.tar", last modified: Wed Jun 21 18:53:35 2023, max compression
```

## Comparing `featurelayers-1.1.0.tar` & `featurelayers-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:51:49.509365 featurelayers-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 18:51:49.509365 featurelayers-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 18:51:32.000000 featurelayers-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:51:49.505365 featurelayers-1.1.0/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 18:51:32.000000 featurelayers-1.1.0/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 18:51:32.000000 featurelayers-1.1.0/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 18:51:32.000000 featurelayers-1.1.0/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:51:49.509365 featurelayers-1.1.0/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 18:51:32.000000 featurelayers-1.1.0/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 18:51:32.000000 featurelayers-1.1.0/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:51:49.509365 featurelayers-1.1.0/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 18:51:49.000000 featurelayers-1.1.0/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 18:51:49.000000 featurelayers-1.1.0/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:51:49.000000 featurelayers-1.1.0/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 18:51:49.000000 featurelayers-1.1.0/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 18:51:49.000000 featurelayers-1.1.0/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:51:49.509365 featurelayers-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 18:51:32.000000 featurelayers-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:53:35.893275 featurelayers-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 18:53:35.893275 featurelayers-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 18:53:19.000000 featurelayers-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:53:35.893275 featurelayers-1.1.1/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 18:53:19.000000 featurelayers-1.1.1/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 18:53:19.000000 featurelayers-1.1.1/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 18:53:19.000000 featurelayers-1.1.1/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:53:35.893275 featurelayers-1.1.1/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 18:53:19.000000 featurelayers-1.1.1/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 18:53:19.000000 featurelayers-1.1.1/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:53:35.893275 featurelayers-1.1.1/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 18:53:35.000000 featurelayers-1.1.1/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 18:53:35.000000 featurelayers-1.1.1/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:53:35.000000 featurelayers-1.1.1/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 18:53:35.000000 featurelayers-1.1.1/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 18:53:35.000000 featurelayers-1.1.1/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:53:35.893275 featurelayers-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 18:53:19.000000 featurelayers-1.1.1/setup.py
```

### Comparing `featurelayers-1.1.0/featurelayers/layers/LBC.py` & `featurelayers-1.1.1/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.1.0/setup.py` & `featurelayers-1.1.1/setup.py`

 * *Files identical despite different names*

