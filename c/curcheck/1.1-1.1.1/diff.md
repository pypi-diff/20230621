# Comparing `tmp/curcheck-1.1.tar.gz` & `tmp/curcheck-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curcheck-1.1.tar", last modified: Wed Jun 21 20:05:13 2023, max compression
+gzip compressed data, was "curcheck-1.1.1.tar", last modified: Wed Jun 21 20:08:39 2023, max compression
```

## Comparing `curcheck-1.1.tar` & `curcheck-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:05:13.949033 curcheck-1.1/
--rw-rw-rw-   0        0        0     1086 2023-01-06 12:52:22.000000 curcheck-1.1/LICENSE.md
--rw-rw-rw-   0        0        0      222 2023-06-21 20:05:13.949033 curcheck-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 20:05:13.921096 curcheck-1.1/curcheck/
--rw-rw-rw-   0        0        0      473 2023-06-07 10:59:42.000000 curcheck-1.1/curcheck/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-20 20:06:51.000000 curcheck-1.1/curcheck/config.py
--rw-rw-rw-   0        0        0     1061 2023-06-21 19:55:22.000000 curcheck-1.1/curcheck/dispatcher.py
--rw-rw-rw-   0        0        0     6731 2023-06-20 20:06:31.000000 curcheck-1.1/curcheck/events.py
--rw-rw-rw-   0        0        0      766 2023-06-21 19:56:05.000000 curcheck-1.1/curcheck/gui.py
--rw-rw-rw-   0        0        0     3072 2023-06-20 18:54:15.000000 curcheck-1.1/curcheck/router.py
--rw-rw-rw-   0        0        0       73 2023-06-20 20:06:13.000000 curcheck-1.1/curcheck/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:05:13.947049 curcheck-1.1/curcheck.egg-info/
--rw-rw-rw-   0        0        0      222 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 20:05:13.951034 curcheck-1.1/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-21 20:02:53.000000 curcheck-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:08:39.161022 curcheck-1.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-01-06 12:52:22.000000 curcheck-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      244 2023-06-21 20:08:39.162022 curcheck-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 20:08:39.145020 curcheck-1.1.1/curcheck/
+-rw-rw-rw-   0        0        0      473 2023-06-07 10:59:42.000000 curcheck-1.1.1/curcheck/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-20 20:06:51.000000 curcheck-1.1.1/curcheck/config.py
+-rw-rw-rw-   0        0        0     1061 2023-06-21 19:55:22.000000 curcheck-1.1.1/curcheck/dispatcher.py
+-rw-rw-rw-   0        0        0     6731 2023-06-20 20:06:31.000000 curcheck-1.1.1/curcheck/events.py
+-rw-rw-rw-   0        0        0      766 2023-06-21 19:56:05.000000 curcheck-1.1.1/curcheck/gui.py
+-rw-rw-rw-   0        0        0     3072 2023-06-20 18:54:15.000000 curcheck-1.1.1/curcheck/router.py
+-rw-rw-rw-   0        0        0       73 2023-06-20 20:06:13.000000 curcheck-1.1.1/curcheck/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:08:39.161022 curcheck-1.1.1/curcheck.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-21 20:08:39.000000 curcheck-1.1.1/curcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-21 20:08:39.000000 curcheck-1.1.1/curcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 20:08:39.000000 curcheck-1.1.1/curcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 20:08:39.000000 curcheck-1.1.1/curcheck.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2023-06-21 20:08:39.000000 curcheck-1.1.1/curcheck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 20:08:39.000000 curcheck-1.1.1/curcheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 20:08:39.164016 curcheck-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-06-21 20:08:34.000000 curcheck-1.1.1/setup.py
```

### Comparing `curcheck-1.1/LICENSE.md` & `curcheck-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curcheck-1.1/curcheck/dispatcher.py` & `curcheck-1.1.1/curcheck/dispatcher.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1/curcheck/events.py` & `curcheck-1.1.1/curcheck/events.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1/curcheck/gui.py` & `curcheck-1.1.1/curcheck/gui.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1/curcheck/router.py` & `curcheck-1.1.1/curcheck/router.py`

 * *Files identical despite different names*

