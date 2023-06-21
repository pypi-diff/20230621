# Comparing `tmp/Telexy.MARS-1.23.621.tar.gz` & `tmp/Telexy.MARS-1.23.622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telexy.MARS-1.23.621.tar", last modified: Wed Jun 21 00:27:09 2023, max compression
+gzip compressed data, was "Telexy.MARS-1.23.622.tar", last modified: Wed Jun 21 00:33:49 2023, max compression
```

## Comparing `Telexy.MARS-1.23.621.tar` & `Telexy.MARS-1.23.622.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 00:27:09.669989 Telexy.MARS-1.23.621/
--rw-rw-rw-   0        0        0     1076 2023-03-15 22:01:12.000000 Telexy.MARS-1.23.621/LICENSE.txt
--rw-rw-rw-   0        0        0     1010 2023-06-21 00:21:13.000000 Telexy.MARS-1.23.621/MARS.py
--rw-rw-rw-   0        0        0     1859 2023-06-20 23:59:15.000000 Telexy.MARS-1.23.621/MARSRegistry.py
--rw-rw-rw-   0        0        0      478 2023-06-21 00:27:09.668990 Telexy.MARS-1.23.621/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 00:27:09.666992 Telexy.MARS-1.23.621/Telexy.MARS.egg-info/
--rw-rw-rw-   0        0        0      478 2023-06-21 00:27:09.000000 Telexy.MARS-1.23.621/Telexy.MARS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-06-21 00:27:09.000000 Telexy.MARS-1.23.621/Telexy.MARS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 00:27:09.000000 Telexy.MARS-1.23.621/Telexy.MARS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-21 00:27:09.000000 Telexy.MARS-1.23.621/Telexy.MARS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-21 00:27:09.000000 Telexy.MARS-1.23.621/Telexy.MARS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 00:27:09.669989 Telexy.MARS-1.23.621/setup.cfg
--rw-rw-rw-   0        0        0     1445 2023-06-21 00:26:13.000000 Telexy.MARS-1.23.621/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:33:49.655982 Telexy.MARS-1.23.622/
+-rw-rw-rw-   0        0        0     1076 2023-03-15 22:01:12.000000 Telexy.MARS-1.23.622/LICENSE.txt
+-rw-rw-rw-   0        0        0      478 2023-06-21 00:33:49.653981 Telexy.MARS-1.23.622/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 00:33:49.652980 Telexy.MARS-1.23.622/Telexy.MARS.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-06-21 00:33:49.000000 Telexy.MARS-1.23.622/Telexy.MARS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-06-21 00:33:49.000000 Telexy.MARS-1.23.622/Telexy.MARS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 00:33:49.000000 Telexy.MARS-1.23.622/Telexy.MARS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-21 00:33:49.000000 Telexy.MARS-1.23.622/Telexy.MARS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-21 00:33:49.000000 Telexy.MARS-1.23.622/Telexy.MARS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 00:33:49.655982 Telexy.MARS-1.23.622/setup.cfg
+-rw-rw-rw-   0        0        0     1445 2023-06-21 00:33:35.000000 Telexy.MARS-1.23.622/setup.py
```

### Comparing `Telexy.MARS-1.23.621/LICENSE.txt` & `Telexy.MARS-1.23.622/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Telexy.MARS-1.23.621/setup.py` & `Telexy.MARS-1.23.622/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Telexy.MARS",                     # This is the name of the package
-    version="1.23.621",                        # The initial release version
+    version="1.23.622",                        # The initial release version
     author="Telexy",                     # Full name of the author
     author_email="support@telexy.com", # Full email of author
     description="MARS Inference server",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
```

