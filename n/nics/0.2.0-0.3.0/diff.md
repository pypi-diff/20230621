# Comparing `tmp/nics-0.2.0.tar.gz` & `tmp/nics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nics-0.2.0.tar", last modified: Wed Jun 21 14:43:02 2023, max compression
+gzip compressed data, was "nics-0.3.0.tar", last modified: Wed Jun 21 16:02:42 2023, max compression
```

## Comparing `nics-0.2.0.tar` & `nics-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 14:43:02.026890 nics-0.2.0/
--rw-rw-rw-   0        0        0     1097 2023-06-21 04:57:10.000000 nics-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1351 2023-06-21 14:43:02.027888 nics-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-21 08:49:46.000000 nics-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 14:43:01.767575 nics-0.2.0/nics/
--rw-rw-rw-   0        0        0      805 2023-06-21 12:51:21.000000 nics-0.2.0/nics/__init__.py
--rw-rw-rw-   0        0        0       65 2023-06-21 12:48:52.000000 nics-0.2.0/nics/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:43:01.973881 nics-0.2.0/nics/compile/
--rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.2.0/nics/compile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:43:01.999885 nics-0.2.0/nics/wizard/
--rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.2.0/nics/wizard/step1.py
--rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.2.0/nics/wizard/step2.py
--rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.2.0/nics/wizard/step3.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:43:01.963892 nics-0.2.0/nics.egg-info/
--rw-rw-rw-   0        0        0     1351 2023-06-21 14:43:01.000000 nics-0.2.0/nics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-21 14:43:01.000000 nics-0.2.0/nics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 14:43:01.000000 nics-0.2.0/nics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-21 14:43:01.000000 nics-0.2.0/nics.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-21 14:43:01.000000 nics-0.2.0/nics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-21 14:43:01.000000 nics-0.2.0/nics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1257 2023-06-21 14:42:00.000000 nics-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      171 2023-06-21 14:43:02.077899 nics-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-21 04:57:10.000000 nics-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:02:42.092237 nics-0.3.0/
+-rw-rw-rw-   0        0        0     1097 2023-06-21 04:57:10.000000 nics-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1351 2023-06-21 16:02:42.094237 nics-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-21 08:49:46.000000 nics-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 16:02:41.701143 nics-0.3.0/nics/
+-rw-rw-rw-   0        0        0     2290 2023-06-21 15:56:17.000000 nics-0.3.0/nics/__init__.py
+-rw-rw-rw-   0        0        0       65 2023-06-21 12:48:52.000000 nics-0.3.0/nics/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:02:41.978207 nics-0.3.0/nics/compile/
+-rw-rw-rw-   0        0        0      383 2023-06-21 15:35:39.000000 nics-0.3.0/nics/compile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:02:42.087238 nics-0.3.0/nics/wizard/
+-rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.3.0/nics/wizard/step1.py
+-rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.3.0/nics/wizard/step2.py
+-rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.3.0/nics/wizard/step3.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:02:41.948200 nics-0.3.0/nics.egg-info/
+-rw-rw-rw-   0        0        0     1351 2023-06-21 16:02:40.000000 nics-0.3.0/nics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-21 16:02:41.000000 nics-0.3.0/nics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 16:02:40.000000 nics-0.3.0/nics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-21 16:02:40.000000 nics-0.3.0/nics.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 16:02:40.000000 nics-0.3.0/nics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-21 16:02:40.000000 nics-0.3.0/nics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1257 2023-06-21 16:00:12.000000 nics-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      171 2023-06-21 16:02:42.149526 nics-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-21 04:57:10.000000 nics-0.3.0/setup.py
```

### Comparing `nics-0.2.0/LICENSE` & `nics-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-0.2.0/PKG-INFO` & `nics-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 0.2.0
+Version: 0.3.0
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-0.2.0/nics.egg-info/PKG-INFO` & `nics-0.3.0/nics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 0.2.0
+Version: 0.3.0
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-0.2.0/pyproject.toml` & `nics-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "0.2.0"
+version = "0.3.0"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

