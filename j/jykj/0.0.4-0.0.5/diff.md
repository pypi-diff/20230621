# Comparing `tmp/jykj-0.0.4.tar.gz` & `tmp/jykj-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jykj-0.0.4.tar", last modified: Fri Jun 16 10:13:50 2023, max compression
+gzip compressed data, was "jykj-0.0.5.tar", last modified: Wed Jun 21 08:39:41 2023, max compression
```

## Comparing `jykj-0.0.4.tar` & `jykj-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 10:13:50.429427 jykj-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      348 2023-06-16 10:13:50.429427 jykj-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 10:13:50.405427 jykj-0.0.4/jykj/
--rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.4/jykj/__init__.py
--rw-rw-rw-   0        0        0    61712 2023-06-16 06:11:58.000000 jykj-0.0.4/jykj/business_model.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:13:50.428427 jykj-0.0.4/jykj.egg-info/
--rw-rw-rw-   0        0        0      348 2023-06-16 10:13:50.000000 jykj-0.0.4/jykj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-16 10:13:50.000000 jykj-0.0.4/jykj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 10:13:50.000000 jykj-0.0.4/jykj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 10:13:50.000000 jykj-0.0.4/jykj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-16 10:13:50.000000 jykj-0.0.4/jykj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 10:13:50.429427 jykj-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      548 2023-06-16 10:13:36.000000 jykj-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.213119 jykj-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      348 2023-06-21 08:39:41.212118 jykj-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.185112 jykj-0.0.5/jykj/
+-rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.5/jykj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.211139 jykj-0.0.5/jykj/business_model/
+-rw-rw-rw-   0        0        0    17263 2023-06-20 02:59:17.000000 jykj-0.0.5/jykj/business_model/SHE.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.5/jykj/business_model/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.5/jykj/business_model/prevention.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.5/jykj/business_model/production.py
+-rw-rw-rw-   0        0        0    14682 2023-06-20 02:56:19.000000 jykj-0.0.5/jykj/business_model/security.py
+-rw-rw-rw-   0        0        0    29712 2023-06-21 08:39:19.000000 jykj-0.0.5/jykj/business_model/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.200118 jykj-0.0.5/jykj.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 08:39:41.213119 jykj-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-21 08:20:45.000000 jykj-0.0.5/setup.py
```

### Comparing `jykj-0.0.4/LICENSE` & `jykj-0.0.5/LICENSE`

 * *Files identical despite different names*

