# Comparing `tmp/featurelayers-1.1.3.tar.gz` & `tmp/featurelayers-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.1.3.tar", last modified: Wed Jun 21 19:01:53 2023, max compression
+gzip compressed data, was "featurelayers-1.1.4.tar", last modified: Wed Jun 21 19:03:57 2023, max compression
```

## Comparing `featurelayers-1.1.3.tar` & `featurelayers-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:53.192434 featurelayers-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 19:01:53.192434 featurelayers-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 19:01:35.000000 featurelayers-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:53.192434 featurelayers-1.1.3/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 19:01:35.000000 featurelayers-1.1.3/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:01:35.000000 featurelayers-1.1.3/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 19:01:35.000000 featurelayers-1.1.3/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:53.192434 featurelayers-1.1.3/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 19:01:35.000000 featurelayers-1.1.3/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 19:01:35.000000 featurelayers-1.1.3/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:53.192434 featurelayers-1.1.3/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 19:01:53.000000 featurelayers-1.1.3/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 19:01:53.000000 featurelayers-1.1.3/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:01:53.000000 featurelayers-1.1.3/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 19:01:53.000000 featurelayers-1.1.3/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 19:01:53.000000 featurelayers-1.1.3/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:01:53.192434 featurelayers-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 19:01:35.000000 featurelayers-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:03:57.396601 featurelayers-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 19:03:57.396601 featurelayers-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 19:03:40.000000 featurelayers-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:03:57.396601 featurelayers-1.1.4/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 19:03:40.000000 featurelayers-1.1.4/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:03:40.000000 featurelayers-1.1.4/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 19:03:40.000000 featurelayers-1.1.4/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:03:57.396601 featurelayers-1.1.4/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 19:03:40.000000 featurelayers-1.1.4/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 19:03:40.000000 featurelayers-1.1.4/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:03:57.396601 featurelayers-1.1.4/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 19:03:57.000000 featurelayers-1.1.4/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 19:03:57.000000 featurelayers-1.1.4/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:03:57.000000 featurelayers-1.1.4/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 19:03:57.000000 featurelayers-1.1.4/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 19:03:57.000000 featurelayers-1.1.4/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:03:57.396601 featurelayers-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 19:03:40.000000 featurelayers-1.1.4/setup.py
```

### Comparing `featurelayers-1.1.3/featurelayers/layers/LBC.py` & `featurelayers-1.1.4/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.1.3/setup.py` & `featurelayers-1.1.4/setup.py`

 * *Files identical despite different names*

