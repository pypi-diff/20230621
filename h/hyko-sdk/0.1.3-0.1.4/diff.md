# Comparing `tmp/hyko_sdk-0.1.3.tar.gz` & `tmp/hyko_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.1.3.tar", last modified: Wed Jun 21 08:26:30 2023, max compression
+gzip compressed data, was "hyko_sdk-0.1.4.tar", last modified: Wed Jun 21 08:40:21 2023, max compression
```

## Comparing `hyko_sdk-0.1.3.tar` & `hyko_sdk-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:26:30.785402 hyko_sdk-0.1.3/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      161 2023-06-21 08:26:30.788736 hyko_sdk-0.1.3/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.1.3/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:26:30.785402 hyko_sdk-0.1.3/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       42 2023-06-21 08:26:13.000000 hyko_sdk-0.1.3/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2734 2023-06-21 07:53:26.000000 hyko_sdk-0.1.3/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1767 2023-06-21 07:53:27.000000 hyko_sdk-0.1.3/hyko_sdk/metadata.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:26:30.785402 hyko_sdk-0.1.3/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      161 2023-06-21 08:26:30.000000 hyko_sdk-0.1.3/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      250 2023-06-21 08:26:30.000000 hyko_sdk-0.1.3/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-06-21 08:26:30.000000 hyko_sdk-0.1.3/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-06-21 08:26:30.000000 hyko_sdk-0.1.3/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-06-21 08:26:30.000000 hyko_sdk-0.1.3/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.1.3/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      296 2023-06-21 08:26:30.788736 hyko_sdk-0.1.3/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:40:21.349930 hyko_sdk-0.1.4/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      161 2023-06-21 08:40:21.349930 hyko_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.1.4/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:40:21.349930 hyko_sdk-0.1.4/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       40 2023-06-21 08:40:10.000000 hyko_sdk-0.1.4/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2734 2023-06-21 07:53:26.000000 hyko_sdk-0.1.4/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1767 2023-06-21 07:53:27.000000 hyko_sdk-0.1.4/hyko_sdk/metadata.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:40:21.349930 hyko_sdk-0.1.4/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      161 2023-06-21 08:40:21.000000 hyko_sdk-0.1.4/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      250 2023-06-21 08:40:21.000000 hyko_sdk-0.1.4/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-06-21 08:40:21.000000 hyko_sdk-0.1.4/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-06-21 08:40:21.000000 hyko_sdk-0.1.4/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-06-21 08:40:21.000000 hyko_sdk-0.1.4/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      296 2023-06-21 08:40:21.349930 hyko_sdk-0.1.4/setup.cfg
```

### Comparing `hyko_sdk-0.1.3/hyko_sdk/io.py` & `hyko_sdk-0.1.4/hyko_sdk/io.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.1.3/hyko_sdk/metadata.py` & `hyko_sdk-0.1.4/hyko_sdk/metadata.py`

 * *Files identical despite different names*

