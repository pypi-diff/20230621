# Comparing `tmp/dreamcoat-0.0.1.tar.gz` & `tmp/dreamcoat-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamcoat-0.0.1.tar", last modified: Sat Nov 12 15:31:48 2022, max compression
+gzip compressed data, was "dreamcoat-0.1.tar", last modified: Wed Jun 21 07:45:19 2023, max compression
```

## Comparing `dreamcoat-0.0.1.tar` & `dreamcoat-0.1.tar`

### file list

```diff
@@ -1,13 +1,25 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-11-12 15:31:48.772834 dreamcoat-0.0.1/
--rw-r--r--   0 matthew    (501) staff       (20)    35149 2022-10-24 13:12:40.000000 dreamcoat-0.0.1/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)       75 2022-11-12 15:31:48.772708 dreamcoat-0.0.1/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)       12 2022-11-12 15:25:36.000000 dreamcoat-0.0.1/README.md
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-11-12 15:31:48.772014 dreamcoat-0.0.1/dreamcoat/
--rw-r--r--   0 matthew    (501) staff       (20)      532 2022-11-12 15:28:41.000000 dreamcoat-0.0.1/dreamcoat/__init__.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-11-12 15:31:48.772563 dreamcoat-0.0.1/dreamcoat.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)       75 2022-11-12 15:31:48.000000 dreamcoat-0.0.1/dreamcoat.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      186 2022-11-12 15:31:48.000000 dreamcoat-0.0.1/dreamcoat.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2022-11-12 15:31:48.000000 dreamcoat-0.0.1/dreamcoat.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)       10 2022-11-12 15:31:48.000000 dreamcoat-0.0.1/dreamcoat.egg-info/top_level.txt
--rw-r--r--   0 matthew    (501) staff       (20)      135 2022-11-12 15:30:02.000000 dreamcoat-0.0.1/pyproject.toml
--rw-r--r--   0 matthew    (501) staff       (20)       38 2022-11-12 15:31:48.772880 dreamcoat-0.0.1/setup.cfg
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-21 07:45:19.646492 dreamcoat-0.1/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    35149 2022-12-05 14:15:10.000000 dreamcoat-0.1/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      258 2023-06-21 07:45:19.646492 dreamcoat-0.1/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       74 2022-12-05 14:15:10.000000 dreamcoat-0.1/README.md
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-21 07:45:19.646492 dreamcoat-0.1/dreamcoat/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     2070 2023-06-21 07:18:54.000000 dreamcoat-0.1/dreamcoat/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    35118 2023-05-19 12:05:42.000000 dreamcoat-0.1/dreamcoat/cmems.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     4102 2023-03-07 08:56:55.000000 dreamcoat-0.1/dreamcoat/convert.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     5449 2023-06-21 07:18:54.000000 dreamcoat-0.1/dreamcoat/ctd.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-21 07:45:19.646492 dreamcoat-0.1/dreamcoat/mapping/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    18312 2023-06-21 07:18:54.000000 dreamcoat-0.1/dreamcoat/mapping/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3459 2023-03-07 08:56:55.000000 dreamcoat-0.1/dreamcoat/mapping/degrees_decimal_minutes.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1824 2023-06-21 07:24:00.000000 dreamcoat-0.1/dreamcoat/meta.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     9378 2023-02-01 09:21:09.000000 dreamcoat-0.1/dreamcoat/modis.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    32148 2023-03-07 08:56:55.000000 dreamcoat-0.1/dreamcoat/plot.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     4818 2023-01-10 08:30:13.000000 dreamcoat-0.1/dreamcoat/send.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     5774 2023-03-07 08:56:55.000000 dreamcoat-0.1/dreamcoat/style.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-21 07:45:19.646492 dreamcoat-0.1/dreamcoat.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      258 2023-06-21 07:45:19.000000 dreamcoat-0.1/dreamcoat.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      442 2023-06-21 07:45:19.000000 dreamcoat-0.1/dreamcoat.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-06-21 07:45:19.000000 dreamcoat-0.1/dreamcoat.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      139 2023-06-21 07:45:19.000000 dreamcoat-0.1/dreamcoat.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       10 2023-06-21 07:45:19.000000 dreamcoat-0.1/dreamcoat.egg-info/top_level.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      838 2023-06-21 07:44:40.000000 dreamcoat-0.1/pyproject.toml
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-06-21 07:45:19.646492 dreamcoat-0.1/setup.cfg
```

### Comparing `dreamcoat-0.0.1/LICENSE` & `dreamcoat-0.1/LICENSE`

 * *Files identical despite different names*

