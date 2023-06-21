# Comparing `tmp/agsi-2.6.tar.gz` & `tmp/agsi-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-2.6.tar", last modified: Tue Jun 20 13:27:45 2023, max compression
+gzip compressed data, was "agsi-2.7.tar", last modified: Wed Jun 21 05:12:29 2023, max compression
```

## Comparing `agsi-2.6.tar` & `agsi-2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 13:27:45.584137 agsi-2.6/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.6/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-20 13:27:45.584137 agsi-2.6/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.6/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 13:27:45.584137 agsi-2.6/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.6/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 13:27:45.584137 agsi-2.6/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    16773 2023-06-20 10:51:50.000000 agsi-2.6/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.6/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     9612 2023-06-20 13:27:08.000000 agsi-2.6/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075510 2023-06-15 07:22:38.000000 agsi-2.6/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.6/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.6/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 13:27:45.584137 agsi-2.6/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-20 13:27:45.000000 agsi-2.6/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-20 13:27:45.000000 agsi-2.6/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-20 13:27:45.000000 agsi-2.6/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-20 13:27:45.000000 agsi-2.6/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-20 13:27:45.000000 agsi-2.6/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-20 13:27:45.584137 agsi-2.6/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-20 13:27:38.000000 agsi-2.6/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-21 05:12:29.708181 agsi-2.7/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.7/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-21 05:12:29.708181 agsi-2.7/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.7/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-21 05:12:29.708181 agsi-2.7/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.7/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-21 05:12:29.708181 agsi-2.7/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    16773 2023-06-20 10:51:50.000000 agsi-2.7/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.7/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     9612 2023-06-21 05:12:21.000000 agsi-2.7/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075510 2023-06-15 07:22:38.000000 agsi-2.7/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.7/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.7/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-21 05:12:29.708181 agsi-2.7/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-21 05:12:29.000000 agsi-2.7/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-21 05:12:29.000000 agsi-2.7/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-21 05:12:29.000000 agsi-2.7/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-21 05:12:29.000000 agsi-2.7/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-21 05:12:29.000000 agsi-2.7/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-21 05:12:29.708181 agsi-2.7/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-21 05:12:24.000000 agsi-2.7/setup.py
```

### Comparing `agsi-2.6/agsi/data/FarmData.py` & `agsi-2.7/agsi/data/FarmData.py`

 * *Files identical despite different names*

### Comparing `agsi-2.6/agsi/data/utils.py` & `agsi-2.7/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-2.6/agsi/demo_V2.ipynb` & `agsi-2.7/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

