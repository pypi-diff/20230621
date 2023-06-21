# Comparing `tmp/isTrue-0.0.5.tar.gz` & `tmp/isTrue-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isTrue-0.0.5.tar", last modified: Sat Jun 17 20:03:16 2023, max compression
+gzip compressed data, was "isTrue-0.0.6.tar", last modified: Wed Jun 21 15:59:37 2023, max compression
```

## Comparing `isTrue-0.0.5.tar` & `isTrue-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 20:03:16.308078 isTrue-0.0.5/
--rw-rw-rw-   0        0        0      372 2023-06-17 20:03:16.307078 isTrue-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 20:03:16.298076 isTrue-0.0.5/isTrue/
--rw-rw-rw-   0        0        0       27 2023-06-17 19:49:19.000000 isTrue-0.0.5/isTrue/__init__.py
--rw-rw-rw-   0        0        0      129 2023-06-17 20:03:09.000000 isTrue-0.0.5/isTrue/isTrue.py
-drwxrwxrwx   0        0        0        0 2023-06-17 20:03:16.306075 isTrue-0.0.5/isTrue.egg-info/
--rw-rw-rw-   0        0        0      372 2023-06-17 20:03:16.000000 isTrue-0.0.5/isTrue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-06-17 20:03:16.000000 isTrue-0.0.5/isTrue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 20:03:16.000000 isTrue-0.0.5/isTrue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 20:03:16.000000 isTrue-0.0.5/isTrue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 20:03:16.308078 isTrue-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-06-17 20:03:09.000000 isTrue-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 15:59:37.230135 isTrue-0.0.6/
+-rw-rw-rw-   0        0        0      412 2023-06-21 15:59:37.230135 isTrue-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 15:59:37.215134 isTrue-0.0.6/isTrue/
+-rw-rw-rw-   0        0        0       27 2023-06-17 19:49:19.000000 isTrue-0.0.6/isTrue/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-06-17 20:03:09.000000 isTrue-0.0.6/isTrue/isTrue.py
+drwxrwxrwx   0        0        0        0 2023-06-21 15:59:37.229135 isTrue-0.0.6/isTrue.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-06-21 15:59:37.000000 isTrue-0.0.6/isTrue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-21 15:59:37.000000 isTrue-0.0.6/isTrue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 15:59:37.000000 isTrue-0.0.6/isTrue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      354 2023-06-21 15:59:37.000000 isTrue-0.0.6/isTrue.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-06-21 15:59:37.000000 isTrue-0.0.6/isTrue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 15:59:37.230135 isTrue-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-06-21 15:58:29.000000 isTrue-0.0.6/setup.py
```

