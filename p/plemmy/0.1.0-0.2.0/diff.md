# Comparing `tmp/plemmy-0.1.0.tar.gz` & `tmp/plemmy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.1.0.tar", last modified: Tue Jun 20 01:00:20 2023, max compression
+gzip compressed data, was "plemmy-0.2.0.tar", last modified: Tue Jun 20 22:26:54 2023, max compression
```

## Comparing `plemmy-0.1.0.tar` & `plemmy-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 01:00:20.350299 plemmy-0.1.0/
--rw-rw-rw-   0        0        0    11367 2023-06-20 00:43:37.000000 plemmy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      337 2023-06-20 01:00:20.350299 plemmy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-06-19 02:46:04.000000 plemmy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 01:00:20.330295 plemmy-0.1.0/plemmy/
--rw-rw-rw-   0        0        0      140 2023-06-20 00:36:09.000000 plemmy-0.1.0/plemmy/__init__.py
--rw-rw-rw-   0        0        0     6405 2023-06-20 00:37:01.000000 plemmy-0.1.0/plemmy/lemmyhttp.py
--rw-rw-rw-   0        0        0     1395 2023-06-20 00:34:27.000000 plemmy-0.1.0/plemmy/utils.py
--rw-rw-rw-   0        0        0      121 2023-06-20 00:35:51.000000 plemmy-0.1.0/plemmy/version.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:00:20.349299 plemmy-0.1.0/plemmy.egg-info/
--rw-rw-rw-   0        0        0      337 2023-06-20 01:00:20.000000 plemmy-0.1.0/plemmy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-20 01:00:20.000000 plemmy-0.1.0/plemmy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:00:20.000000 plemmy-0.1.0/plemmy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 01:00:20.000000 plemmy-0.1.0/plemmy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-06-20 01:00:20.000000 plemmy-0.1.0/plemmy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 01:00:20.000000 plemmy-0.1.0/plemmy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 01:00:20.351299 plemmy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-06-20 00:48:06.000000 plemmy-0.1.0/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-20 22:26:54.350271 plemmy-0.2.0/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.0/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-20 22:26:54.350098 plemmy-0.2.0/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.0/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-20 22:26:54.348959 plemmy-0.2.0/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.0/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    42043 2023-06-20 22:25:52.000000 plemmy-0.2.0/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1395 2023-06-20 19:47:16.000000 plemmy-0.2.0/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-20 22:25:52.000000 plemmy-0.2.0/plemmy/version.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-20 22:26:54.349872 plemmy-0.2.0/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-20 22:26:54.350320 plemmy-0.2.0/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.0/setup.py
```

### Comparing `plemmy-0.1.0/LICENSE` & `plemmy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.1.0/plemmy/utils.py` & `plemmy-0.2.0/plemmy/utils.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.1.0/setup.py` & `plemmy-0.2.0/setup.py`

 * *Files identical despite different names*

