# Comparing `tmp/curcheck-0.0.tar.gz` & `tmp/curcheck-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curcheck-0.0.tar", last modified: Thu Jan  5 20:36:36 2023, max compression
+gzip compressed data, was "curcheck-1.1.tar", last modified: Wed Jun 21 20:05:13 2023, max compression
```

## Comparing `curcheck-0.0.tar` & `curcheck-1.1.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-05 20:36:36.685717 curcheck-0.0/
--rw-rw-rw-   0        0        0      137 2023-01-05 20:36:36.689715 curcheck-0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-05 20:36:36.637703 curcheck-0.0/curcheck/
--rw-rw-rw-   0        0        0     1139 2023-01-05 17:37:21.000000 curcheck-0.0/curcheck/__init__.py
--rw-rw-rw-   0        0        0      994 2023-01-04 11:57:26.000000 curcheck-0.0/curcheck/base.py
-drwxrwxrwx   0        0        0        0 2023-01-05 20:36:36.685717 curcheck-0.0/curcheck.egg-info/
--rw-rw-rw-   0        0        0      137 2023-01-05 20:36:36.000000 curcheck-0.0/curcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-01-05 20:36:36.000000 curcheck-0.0/curcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-05 20:36:36.000000 curcheck-0.0/curcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-05 20:36:36.000000 curcheck-0.0/curcheck.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-01-05 20:36:36.000000 curcheck-0.0/curcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-05 20:36:36.693731 curcheck-0.0/setup.cfg
--rw-rw-rw-   0        0        0      231 2023-01-05 20:33:22.000000 curcheck-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:05:13.949033 curcheck-1.1/
+-rw-rw-rw-   0        0        0     1086 2023-01-06 12:52:22.000000 curcheck-1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      222 2023-06-21 20:05:13.949033 curcheck-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 20:05:13.921096 curcheck-1.1/curcheck/
+-rw-rw-rw-   0        0        0      473 2023-06-07 10:59:42.000000 curcheck-1.1/curcheck/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-20 20:06:51.000000 curcheck-1.1/curcheck/config.py
+-rw-rw-rw-   0        0        0     1061 2023-06-21 19:55:22.000000 curcheck-1.1/curcheck/dispatcher.py
+-rw-rw-rw-   0        0        0     6731 2023-06-20 20:06:31.000000 curcheck-1.1/curcheck/events.py
+-rw-rw-rw-   0        0        0      766 2023-06-21 19:56:05.000000 curcheck-1.1/curcheck/gui.py
+-rw-rw-rw-   0        0        0     3072 2023-06-20 18:54:15.000000 curcheck-1.1/curcheck/router.py
+-rw-rw-rw-   0        0        0       73 2023-06-20 20:06:13.000000 curcheck-1.1/curcheck/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:05:13.947049 curcheck-1.1/curcheck.egg-info/
+-rw-rw-rw-   0        0        0      222 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 20:05:13.000000 curcheck-1.1/curcheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 20:05:13.951034 curcheck-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-21 20:02:53.000000 curcheck-1.1/setup.py
```

