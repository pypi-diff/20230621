# Comparing `tmp/maxgradient-0.1.2.tar.gz` & `tmp/maxgradient-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxgradient-0.1.2.tar", last modified: Wed Jun 21 02:00:36 2023, max compression
+gzip compressed data, was "maxgradient-0.1.3.tar", last modified: Wed Jun 21 02:05:14 2023, max compression
```

## Comparing `maxgradient-0.1.2.tar` & `maxgradient-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-05-20 01:18:06.237490 maxgradient-0.1.2/LICENSE
--rw-r--r--   0        0        0     4749 2023-06-21 02:00:13.184953 maxgradient-0.1.2/README.md
--rw-r--r--   0        0        0      735 2023-06-19 17:15:40.456613 maxgradient-0.1.2/maxgradient/__init__.py
--rw-r--r--   0        0        0    10879 2023-06-18 19:16:19.295760 maxgradient-0.1.2/maxgradient/_gradient_substring.py
--rw-r--r--   0        0        0     1886 2023-06-14 20:46:22.513323 maxgradient-0.1.2/maxgradient/_mode.py
--rw-r--r--   0        0        0    16154 2023-06-16 21:20:44.170100 maxgradient-0.1.2/maxgradient/_rich.py
--rw-r--r--   0        0        0    12225 2023-06-16 21:17:22.440850 maxgradient-0.1.2/maxgradient/_x11.py
--rw-r--r--   0        0        0     2395 2023-06-20 03:47:24.996801 maxgradient-0.1.2/maxgradient/cli.py
--rw-r--r--   0        0        0    19133 2023-06-19 01:34:58.510343 maxgradient-0.1.2/maxgradient/color.py
--rw-r--r--   0        0        0     3294 2023-06-16 21:20:58.780049 maxgradient-0.1.2/maxgradient/color_list.py
--rw-r--r--   0        0        0    10462 2023-06-19 00:24:10.378696 maxgradient-0.1.2/maxgradient/console.py
--rw-r--r--   0        0        0    30263 2023-06-16 16:09:50.267902 maxgradient-0.1.2/maxgradient/default_styles.py
--rw-r--r--   0        0        0    20228 2023-06-19 03:17:18.349630 maxgradient-0.1.2/maxgradient/gradient.py
--rw-r--r--   0        0        0    13231 2023-06-18 15:30:08.337049 maxgradient-0.1.2/maxgradient/log.py
--rw-r--r--   0        0        0     1473 2023-06-19 17:26:36.354259 maxgradient-0.1.2/maxgradient/logs/debug.log
--rw-r--r--   0        0        0       87 2023-06-19 17:26:36.354163 maxgradient-0.1.2/maxgradient/logs/info.log
--rw-r--r--   0        0        0     2649 2023-06-18 18:22:16.438034 maxgradient-0.1.2/maxgradient/theme.py
--rw-r--r--   0        0        0      876 2023-06-21 02:00:36.489638 maxgradient-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2284 2023-06-20 04:32:57.158944 maxgradient-0.1.2/tests/test_color.py
--rw-r--r--   0        0        0      658 2023-06-20 04:22:37.208149 maxgradient-0.1.2/tests/test_rich_colors.py
--rw-r--r--   0        0        0      654 2023-06-20 04:18:31.642710 maxgradient-0.1.2/tests/test_x11_colors.py
--rw-r--r--   0        0        0     5301 1970-01-01 00:00:00.000000 maxgradient-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-20 01:18:06.237490 maxgradient-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4614 2023-06-21 02:04:51.054299 maxgradient-0.1.3/README.md
+-rw-r--r--   0        0        0      735 2023-06-19 17:15:40.456613 maxgradient-0.1.3/maxgradient/__init__.py
+-rw-r--r--   0        0        0    10879 2023-06-18 19:16:19.295760 maxgradient-0.1.3/maxgradient/_gradient_substring.py
+-rw-r--r--   0        0        0     1886 2023-06-14 20:46:22.513323 maxgradient-0.1.3/maxgradient/_mode.py
+-rw-r--r--   0        0        0    16154 2023-06-16 21:20:44.170100 maxgradient-0.1.3/maxgradient/_rich.py
+-rw-r--r--   0        0        0    12225 2023-06-16 21:17:22.440850 maxgradient-0.1.3/maxgradient/_x11.py
+-rw-r--r--   0        0        0     2395 2023-06-20 03:47:24.996801 maxgradient-0.1.3/maxgradient/cli.py
+-rw-r--r--   0        0        0    19133 2023-06-19 01:34:58.510343 maxgradient-0.1.3/maxgradient/color.py
+-rw-r--r--   0        0        0     3294 2023-06-16 21:20:58.780049 maxgradient-0.1.3/maxgradient/color_list.py
+-rw-r--r--   0        0        0    10462 2023-06-19 00:24:10.378696 maxgradient-0.1.3/maxgradient/console.py
+-rw-r--r--   0        0        0    30263 2023-06-16 16:09:50.267902 maxgradient-0.1.3/maxgradient/default_styles.py
+-rw-r--r--   0        0        0    20228 2023-06-19 03:17:18.349630 maxgradient-0.1.3/maxgradient/gradient.py
+-rw-r--r--   0        0        0    13231 2023-06-18 15:30:08.337049 maxgradient-0.1.3/maxgradient/log.py
+-rw-r--r--   0        0        0     1473 2023-06-19 17:26:36.354259 maxgradient-0.1.3/maxgradient/logs/debug.log
+-rw-r--r--   0        0        0       87 2023-06-19 17:26:36.354163 maxgradient-0.1.3/maxgradient/logs/info.log
+-rw-r--r--   0        0        0     2649 2023-06-18 18:22:16.438034 maxgradient-0.1.3/maxgradient/theme.py
+-rw-r--r--   0        0        0      876 2023-06-21 02:05:14.429199 maxgradient-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2284 2023-06-20 04:32:57.158944 maxgradient-0.1.3/tests/test_color.py
+-rw-r--r--   0        0        0      658 2023-06-20 04:22:37.208149 maxgradient-0.1.3/tests/test_rich_colors.py
+-rw-r--r--   0        0        0      654 2023-06-20 04:18:31.642710 maxgradient-0.1.3/tests/test_x11_colors.py
+-rw-r--r--   0        0        0     5166 1970-01-01 00:00:00.000000 maxgradient-0.1.3/PKG-INFO
```

### Comparing `maxgradient-0.1.2/LICENSE` & `maxgradient-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/README.md` & `maxgradient-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-
-<html>
-<head>
-<meta charset="UTF-8"><meta name="viewport" content="width=device-width initial-scale=1">
-<title>README</title>
-</head>
 <body>
     <head>
         <link href="styles/gradient.css" rel="stylesheet">
         <!--<link href="styles/link.css" rel="stylesheet">-->
     </head>
     <body>
         <img src="Images/MaxGradient_banner.gif" alt="MaxGradient" width="100%" height="auto">
@@ -15,15 +9,15 @@
             <a href="https://GitHub.com/maxludden/maxgradient">
                 <img  class="badge" src="https://img.shields.io/badge/Python-3.9 | 3.10 | 3.11-blue?logo=python" alt="PyPI - MaxGradient">
             </a>
             <a href="https://GitHub.com/maxludden/maxgradient">
                 <img  class="badge" src="https://img.shields.io/badge/PyPI-MaxGradient-blue?" alt="PyPI - MaxGradient">
             </a>
             <a href="https://GitHub.com/maxludden/maxgradient">
-                <img  class="badge" src="https://img.shields.io/badge/Version-0.1.2-bbbbbb" alt="Version - 0.1.2">
+                <img  class="badge" src="https://img.shields.io/badge/Version-0.1.2-bbbbbb" alt="Version - 0.1.3">
             </a>
             <a href="https://pdm.fming.dev/">
                 <img class="badge" src="https://camo.githubusercontent.com/acf0526fc1f541f9d980d7983ff5ab8e540cf2136206c2b5dc740f658a37fac0/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f70646d2d6d616e616765642d626c756576696f6c6574">
             </a>
         </div>
         <h1 class="rainbow-wipefont">MaxGradient</h1>
             <div class="summary">MaxGradient automating printing gradient colored text to the console. It's built upon the great <a href="https://rich.readthedocs.io/en/latest/introduction.html">rich library.</a></div>
```

### Comparing `maxgradient-0.1.2/maxgradient/__init__.py` & `maxgradient-0.1.3/maxgradient/__init__.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/_gradient_substring.py` & `maxgradient-0.1.3/maxgradient/_gradient_substring.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/_mode.py` & `maxgradient-0.1.3/maxgradient/_mode.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/_rich.py` & `maxgradient-0.1.3/maxgradient/_rich.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/_x11.py` & `maxgradient-0.1.3/maxgradient/_x11.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/cli.py` & `maxgradient-0.1.3/maxgradient/cli.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/color.py` & `maxgradient-0.1.3/maxgradient/color.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/color_list.py` & `maxgradient-0.1.3/maxgradient/color_list.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/console.py` & `maxgradient-0.1.3/maxgradient/console.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/default_styles.py` & `maxgradient-0.1.3/maxgradient/default_styles.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/gradient.py` & `maxgradient-0.1.3/maxgradient/gradient.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/log.py` & `maxgradient-0.1.3/maxgradient/log.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/logs/debug.log` & `maxgradient-0.1.3/maxgradient/logs/debug.log`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/maxgradient/theme.py` & `maxgradient-0.1.3/maxgradient/theme.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/pyproject.toml` & `maxgradient-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "MaxGradient"
-version = "0.1.2"
+version = "0.1.3"
 description = "A library to make printing gradient color to the terminal a lot easier. Think `lolcat` but utilizing python's `rich` library so you can use it anywhere."
 authors = [
     { name = "maxludden", email = "dev@maxludden.com" },
 ]
 dependencies = [
     "rich>=13.3.5",
     "lorem-text>=2.1",
```

### Comparing `maxgradient-0.1.2/tests/test_color.py` & `maxgradient-0.1.3/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/tests/test_rich_colors.py` & `maxgradient-0.1.3/tests/test_rich_colors.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/tests/test_x11_colors.py` & `maxgradient-0.1.3/tests/test_x11_colors.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.2/PKG-INFO` & `maxgradient-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 Metadata-Version: 2.1
 Name: maxgradient
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library to make printing gradient color to the terminal a lot easier. Think `lolcat` but utilizing python's `rich` library so you can use it anywhere.
 Author-Email: maxludden <dev@maxludden.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: rich>=13.3.5
 Requires-Dist: lorem-text>=2.1
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: loguru>=0.7.0
 Requires-Dist: typer>=0.9.0
 Requires-Dist: typer[all]>=0.9.0; extra == "cli"
 Provides-Extra: cli
 Description-Content-Type: text/markdown
 
-
-<html>
-<head>
-<meta charset="UTF-8"><meta name="viewport" content="width=device-width initial-scale=1">
-<title>README</title>
-</head>
 <body>
     <head>
         <link href="styles/gradient.css" rel="stylesheet">
         <!--<link href="styles/link.css" rel="stylesheet">-->
     </head>
     <body>
         <img src="Images/MaxGradient_banner.gif" alt="MaxGradient" width="100%" height="auto">
@@ -31,15 +25,15 @@
             <a href="https://GitHub.com/maxludden/maxgradient">
                 <img  class="badge" src="https://img.shields.io/badge/Python-3.9 | 3.10 | 3.11-blue?logo=python" alt="PyPI - MaxGradient">
             </a>
             <a href="https://GitHub.com/maxludden/maxgradient">
                 <img  class="badge" src="https://img.shields.io/badge/PyPI-MaxGradient-blue?" alt="PyPI - MaxGradient">
             </a>
             <a href="https://GitHub.com/maxludden/maxgradient">
-                <img  class="badge" src="https://img.shields.io/badge/Version-0.1.2-bbbbbb" alt="Version - 0.1.2">
+                <img  class="badge" src="https://img.shields.io/badge/Version-0.1.2-bbbbbb" alt="Version - 0.1.3">
             </a>
             <a href="https://pdm.fming.dev/">
                 <img class="badge" src="https://camo.githubusercontent.com/acf0526fc1f541f9d980d7983ff5ab8e540cf2136206c2b5dc740f658a37fac0/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f70646d2d6d616e616765642d626c756576696f6c6574">
             </a>
         </div>
         <h1 class="rainbow-wipefont">MaxGradient</h1>
             <div class="summary">MaxGradient automating printing gradient colored text to the console. It's built upon the great <a href="https://rich.readthedocs.io/en/latest/introduction.html">rich library.</a></div>
```

