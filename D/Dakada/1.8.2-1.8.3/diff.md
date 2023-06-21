# Comparing `tmp/Dakada-1.8.2.tar.gz` & `tmp/Dakada-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Dakada-1.8.2.tar", last modified: Wed Jun 21 13:34:04 2023, max compression
+gzip compressed data, was "dist\Dakada-1.8.3.tar", last modified: Wed Jun 21 13:36:55 2023, max compression
```

## Comparing `Dakada-1.8.2.tar` & `Dakada-1.8.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:34:04.000000 Dakada-1.8.2/
-drwxrwxrwx   0        0        0        0 2023-06-21 13:34:04.000000 Dakada-1.8.2/Dakada.egg-info/
--rw-rw-rw-   0        0        0      666 2023-06-21 13:34:04.000000 Dakada-1.8.2/Dakada.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-21 13:34:04.000000 Dakada-1.8.2/Dakada.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:34:04.000000 Dakada-1.8.2/Dakada.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-21 13:34:04.000000 Dakada-1.8.2/Dakada.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-21 13:34:04.000000 Dakada-1.8.2/Dakada.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2023-06-21 13:34:04.000000 Dakada-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-06-21 13:15:08.000000 Dakada-1.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 13:34:04.000000 Dakada-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     3734 2023-06-21 13:33:44.000000 Dakada-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:36:55.000000 Dakada-1.8.3/
+drwxrwxrwx   0        0        0        0 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      666 2023-06-21 13:36:55.000000 Dakada-1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-06-21 13:15:08.000000 Dakada-1.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:36:55.000000 Dakada-1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     3734 2023-06-21 13:36:36.000000 Dakada-1.8.3/setup.py
```

### Comparing `Dakada-1.8.2/Dakada.egg-info/PKG-INFO` & `Dakada-1.8.3/Dakada.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.8.2
+Version: 1.8.3
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Description: 
         114514
```

### Comparing `Dakada-1.8.2/PKG-INFO` & `Dakada-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.8.2
+Version: 1.8.3
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Description: 
         114514
```

### Comparing `Dakada-1.8.2/setup.py` & `Dakada-1.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'Dakada'
 DESCRIPTION = 'A web framework by Dakada CN'
 URL = 'https://github.com/dakadayyds/dakadaWeb'
 EMAIL = 's75uy1e@dingtalk.com'
 AUTHOR = 'dakada'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.8.2'
+VERSION = '1.8.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'jinja2'
 ]
 
 # What packages are optional?
```

