# Comparing `tmp/curcheck-1.1.2b0.tar.gz` & `tmp/curcheck-1.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curcheck-1.1.2b0.tar", last modified: Wed Jun 21 20:18:55 2023, max compression
+gzip compressed data, was "curcheck-1.1.3b0.tar", last modified: Wed Jun 21 20:23:20 2023, max compression
```

## Comparing `curcheck-1.1.2b0.tar` & `curcheck-1.1.3b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:18:55.812509 curcheck-1.1.2b0/
--rw-rw-rw-   0        0        0     1086 2023-01-06 12:52:22.000000 curcheck-1.1.2b0/LICENSE.md
--rw-rw-rw-   0        0        0      246 2023-06-21 20:18:55.813510 curcheck-1.1.2b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 20:18:55.796505 curcheck-1.1.2b0/curcheck/
--rw-rw-rw-   0        0        0      473 2023-06-07 10:59:42.000000 curcheck-1.1.2b0/curcheck/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-20 20:06:51.000000 curcheck-1.1.2b0/curcheck/config.py
--rw-rw-rw-   0        0        0     1061 2023-06-21 19:55:22.000000 curcheck-1.1.2b0/curcheck/dispatcher.py
--rw-rw-rw-   0        0        0     6731 2023-06-20 20:06:31.000000 curcheck-1.1.2b0/curcheck/events.py
--rw-rw-rw-   0        0        0      766 2023-06-21 19:56:05.000000 curcheck-1.1.2b0/curcheck/gui.py
--rw-rw-rw-   0        0        0     3028 2023-06-21 20:17:55.000000 curcheck-1.1.2b0/curcheck/router.py
--rw-rw-rw-   0        0        0       73 2023-06-20 20:06:13.000000 curcheck-1.1.2b0/curcheck/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:18:55.811509 curcheck-1.1.2b0/curcheck.egg-info/
--rw-rw-rw-   0        0        0      246 2023-06-21 20:18:55.000000 curcheck-1.1.2b0/curcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-06-21 20:18:55.000000 curcheck-1.1.2b0/curcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:18:55.000000 curcheck-1.1.2b0/curcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 20:18:55.000000 curcheck-1.1.2b0/curcheck.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2023-06-21 20:18:55.000000 curcheck-1.1.2b0/curcheck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 20:18:55.000000 curcheck-1.1.2b0/curcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 20:18:55.814511 curcheck-1.1.2b0/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-06-21 20:18:52.000000 curcheck-1.1.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:23:20.350671 curcheck-1.1.3b0/
+-rw-rw-rw-   0        0        0     1086 2023-01-06 12:52:22.000000 curcheck-1.1.3b0/LICENSE.md
+-rw-rw-rw-   0        0        0      248 2023-06-21 20:23:20.350671 curcheck-1.1.3b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 20:23:20.334666 curcheck-1.1.3b0/curcheck/
+-rw-rw-rw-   0        0        0      473 2023-06-07 10:59:42.000000 curcheck-1.1.3b0/curcheck/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-20 20:06:51.000000 curcheck-1.1.3b0/curcheck/config.py
+-rw-rw-rw-   0        0        0     1061 2023-06-21 19:55:22.000000 curcheck-1.1.3b0/curcheck/dispatcher.py
+-rw-rw-rw-   0        0        0     6731 2023-06-20 20:06:31.000000 curcheck-1.1.3b0/curcheck/events.py
+-rw-rw-rw-   0        0        0      766 2023-06-21 19:56:05.000000 curcheck-1.1.3b0/curcheck/gui.py
+-rw-rw-rw-   0        0        0     3028 2023-06-21 20:20:54.000000 curcheck-1.1.3b0/curcheck/router.py
+-rw-rw-rw-   0        0        0       73 2023-06-20 20:06:13.000000 curcheck-1.1.3b0/curcheck/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:23:20.349670 curcheck-1.1.3b0/curcheck.egg-info/
+-rw-rw-rw-   0        0        0      248 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 20:23:20.352671 curcheck-1.1.3b0/setup.cfg
+-rw-rw-rw-   0        0        0      529 2023-06-21 20:23:15.000000 curcheck-1.1.3b0/setup.py
```

### Comparing `curcheck-1.1.2b0/LICENSE.md` & `curcheck-1.1.3b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.2b0/curcheck/dispatcher.py` & `curcheck-1.1.3b0/curcheck/dispatcher.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.2b0/curcheck/events.py` & `curcheck-1.1.3b0/curcheck/events.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.2b0/curcheck/gui.py` & `curcheck-1.1.3b0/curcheck/gui.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.2b0/curcheck/router.py` & `curcheck-1.1.3b0/curcheck/router.py`

 * *Files identical despite different names*

