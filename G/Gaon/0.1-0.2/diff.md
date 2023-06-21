# Comparing `tmp/Gaon-0.1.tar.gz` & `tmp/Gaon-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gaon-0.1.tar", last modified: Wed Jun 21 15:56:01 2023, max compression
+gzip compressed data, was "Gaon-0.2.tar", last modified: Wed Jun 21 16:04:31 2023, max compression
```

## Comparing `Gaon-0.1.tar` & `Gaon-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 15:56:01.563746 Gaon-0.1/
-drwxrwxrwx   0        0        0        0 2023-06-21 15:56:01.554659 Gaon-0.1/Gaon.egg-info/
--rw-rw-rw-   0        0        0      186 2023-06-21 15:56:01.000000 Gaon-0.1/Gaon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-06-21 15:56:01.000000 Gaon-0.1/Gaon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 15:56:01.000000 Gaon-0.1/Gaon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-21 15:56:01.000000 Gaon-0.1/Gaon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-21 15:56:01.000000 Gaon-0.1/Gaon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 15:56:01.557642 Gaon-0.1/GaonSidedrawer/
--rw-rw-rw-   0        0        0       37 2023-06-21 15:47:55.000000 Gaon-0.1/GaonSidedrawer/__init__.py
--rw-rw-rw-   0        0        0     1937 2023-06-21 15:52:58.000000 Gaon-0.1/GaonSidedrawer/main.py
--rw-rw-rw-   0        0        0     7601 2023-06-21 15:50:30.000000 Gaon-0.1/GaonSidedrawer/utils.py
--rw-rw-rw-   0        0        0     1090 2023-06-21 15:41:09.000000 Gaon-0.1/LICENSE
--rw-rw-rw-   0        0        0      186 2023-06-21 15:56:01.562745 Gaon-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-21 15:41:09.000000 Gaon-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 15:56:01.563746 Gaon-0.1/setup.cfg
--rw-rw-rw-   0        0        0      434 2023-06-21 15:53:35.000000 Gaon-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 15:56:01.560644 Gaon-0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-21 15:41:09.000000 Gaon-0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-06-21 15:41:09.000000 Gaon-0.1/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:04:31.254599 Gaon-0.2/
+drwxrwxrwx   0        0        0        0 2023-06-21 16:04:31.237439 Gaon-0.2/Gaon.egg-info/
+-rw-rw-rw-   0        0        0      186 2023-06-21 16:04:30.000000 Gaon-0.2/Gaon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-06-21 16:04:31.000000 Gaon-0.2/Gaon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 16:04:30.000000 Gaon-0.2/Gaon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-21 16:04:30.000000 Gaon-0.2/Gaon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-21 16:04:30.000000 Gaon-0.2/Gaon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 16:04:31.244437 Gaon-0.2/GaonSidedrawer/
+-rw-rw-rw-   0        0        0       51 2023-06-21 16:04:21.000000 Gaon-0.2/GaonSidedrawer/__init__.py
+-rw-rw-rw-   0        0        0     1937 2023-06-21 16:04:19.000000 Gaon-0.2/GaonSidedrawer/main.py
+-rw-rw-rw-   0        0        0     7601 2023-06-21 15:50:30.000000 Gaon-0.2/GaonSidedrawer/utils.py
+-rw-rw-rw-   0        0        0     1090 2023-06-21 15:41:09.000000 Gaon-0.2/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-06-21 16:04:31.252608 Gaon-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-21 15:41:09.000000 Gaon-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 16:04:31.254599 Gaon-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      434 2023-06-21 16:04:16.000000 Gaon-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:04:31.249662 Gaon-0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:41:09.000000 Gaon-0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-06-21 15:41:09.000000 Gaon-0.2/tests/test_main.py
```

### Comparing `Gaon-0.1/GaonSidedrawer/main.py` & `Gaon-0.2/GaonSidedrawer/main.py`

 * *Files identical despite different names*

### Comparing `Gaon-0.1/GaonSidedrawer/utils.py` & `Gaon-0.2/GaonSidedrawer/utils.py`

 * *Files identical despite different names*

### Comparing `Gaon-0.1/LICENSE` & `Gaon-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Gaon-0.1/tests/test_main.py` & `Gaon-0.2/tests/test_main.py`

 * *Files identical despite different names*

