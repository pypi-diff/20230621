# Comparing `tmp/fluidCube-0.1.2.tar.gz` & `tmp/fluidCube-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidCube-0.1.2.tar", last modified: Wed Jun 21 06:48:30 2023, max compression
+gzip compressed data, was "fluidCube-0.1.3.tar", last modified: Wed Jun 21 06:53:00 2023, max compression
```

## Comparing `fluidCube-0.1.2.tar` & `fluidCube-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 06:48:30.809724 fluidCube-0.1.2/
--rw-rw-rw-   0        0        0      232 2023-06-21 06:48:30.809724 fluidCube-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 06:48:30.794113 fluidCube-0.1.2/fluidCube/
--rw-rw-rw-   0        0        0      174 2023-06-21 06:38:33.000000 fluidCube-0.1.2/fluidCube/__init__.py
--rw-rw-rw-   0        0        0     5164 2023-06-21 06:20:27.000000 fluidCube-0.1.2/fluidCube/fluidCube.py
--rw-rw-rw-   0        0        0     1045 2023-06-21 06:38:26.000000 fluidCube-0.1.2/fluidCube/main.py
-drwxrwxrwx   0        0        0        0 2023-06-21 06:48:30.809724 fluidCube-0.1.2/fluidCube.egg-info/
--rw-rw-rw-   0        0        0      232 2023-06-21 06:48:30.000000 fluidCube-0.1.2/fluidCube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-21 06:48:30.000000 fluidCube-0.1.2/fluidCube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 06:48:30.000000 fluidCube-0.1.2/fluidCube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-21 06:48:30.000000 fluidCube-0.1.2/fluidCube.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-21 06:48:30.000000 fluidCube-0.1.2/fluidCube.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 06:48:30.825372 fluidCube-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-06-21 06:48:00.000000 fluidCube-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:53:00.952888 fluidCube-0.1.3/
+-rw-rw-rw-   0        0        0      232 2023-06-21 06:53:00.952888 fluidCube-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 06:53:00.937259 fluidCube-0.1.3/fluidCube/
+-rw-rw-rw-   0        0        0      174 2023-06-21 06:38:33.000000 fluidCube-0.1.3/fluidCube/__init__.py
+-rw-rw-rw-   0        0        0     5164 2023-06-21 06:20:27.000000 fluidCube-0.1.3/fluidCube/fluidCube.py
+-rw-rw-rw-   0        0        0     1045 2023-06-21 06:38:26.000000 fluidCube-0.1.3/fluidCube/main.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:53:00.952888 fluidCube-0.1.3/fluidCube.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-06-21 06:53:00.000000 fluidCube-0.1.3/fluidCube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-21 06:53:00.000000 fluidCube-0.1.3/fluidCube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 06:53:00.000000 fluidCube-0.1.3/fluidCube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 06:53:00.000000 fluidCube-0.1.3/fluidCube.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-21 06:53:00.000000 fluidCube-0.1.3/fluidCube.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 06:53:00.968514 fluidCube-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      480 2023-06-21 06:52:26.000000 fluidCube-0.1.3/setup.py
```

### Comparing `fluidCube-0.1.2/fluidCube/fluidCube.py` & `fluidCube-0.1.3/fluidCube/fluidCube.py`

 * *Files identical despite different names*

### Comparing `fluidCube-0.1.2/fluidCube/main.py` & `fluidCube-0.1.3/fluidCube/main.py`

 * *Files identical despite different names*

