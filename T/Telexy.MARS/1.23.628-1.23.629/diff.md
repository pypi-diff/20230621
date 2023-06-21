# Comparing `tmp/Telexy.MARS-1.23.628.tar.gz` & `tmp/Telexy.MARS-1.23.629.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telexy.MARS-1.23.628.tar", last modified: Wed Jun 21 03:51:45 2023, max compression
+gzip compressed data, was "Telexy.MARS-1.23.629.tar", last modified: Wed Jun 21 03:59:09 2023, max compression
```

## Comparing `Telexy.MARS-1.23.628.tar` & `Telexy.MARS-1.23.629.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 03:51:45.530932 Telexy.MARS-1.23.628/
--rw-rw-rw-   0        0        0     1076 2023-03-15 22:01:12.000000 Telexy.MARS-1.23.628/LICENSE.txt
--rw-rw-rw-   0        0        0      478 2023-06-21 03:51:45.529931 Telexy.MARS-1.23.628/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 03:51:45.528932 Telexy.MARS-1.23.628/Telexy.MARS.egg-info/
--rw-rw-rw-   0        0        0      478 2023-06-21 03:51:45.000000 Telexy.MARS-1.23.628/Telexy.MARS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-21 03:51:45.000000 Telexy.MARS-1.23.628/Telexy.MARS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 03:51:45.000000 Telexy.MARS-1.23.628/Telexy.MARS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-21 03:51:45.000000 Telexy.MARS-1.23.628/Telexy.MARS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-21 03:51:45.000000 Telexy.MARS-1.23.628/Telexy.MARS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 03:51:45.530932 Telexy.MARS-1.23.628/setup.cfg
--rw-rw-rw-   0        0        0     1429 2023-06-21 03:51:25.000000 Telexy.MARS-1.23.628/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:59:09.973970 Telexy.MARS-1.23.629/
+-rw-rw-rw-   0        0        0     1076 2023-06-21 03:48:56.000000 Telexy.MARS-1.23.629/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 03:59:09.966970 Telexy.MARS-1.23.629/MARS/
+-rw-rw-rw-   0        0        0       23 2023-06-21 03:48:57.000000 Telexy.MARS-1.23.629/MARS/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-06-21 03:48:56.000000 Telexy.MARS-1.23.629/MARS/__main__.py
+-rw-rw-rw-   0        0        0     1859 2023-06-21 03:48:56.000000 Telexy.MARS-1.23.629/MARS/registry.py
+-rw-rw-rw-   0        0        0      478 2023-06-21 03:59:09.972970 Telexy.MARS-1.23.629/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 03:59:09.971969 Telexy.MARS-1.23.629/Telexy.MARS.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-06-21 03:59:09.000000 Telexy.MARS-1.23.629/Telexy.MARS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-21 03:59:09.000000 Telexy.MARS-1.23.629/Telexy.MARS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:59:09.000000 Telexy.MARS-1.23.629/Telexy.MARS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-21 03:59:09.000000 Telexy.MARS-1.23.629/Telexy.MARS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-21 03:59:09.000000 Telexy.MARS-1.23.629/Telexy.MARS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:59:09.973970 Telexy.MARS-1.23.629/setup.cfg
+-rw-rw-rw-   0        0        0     1345 2023-06-21 03:59:07.000000 Telexy.MARS-1.23.629/setup.py
```

### Comparing `Telexy.MARS-1.23.628/LICENSE.txt` & `Telexy.MARS-1.23.629/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Telexy.MARS-1.23.628/setup.py` & `Telexy.MARS-1.23.629/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Telexy.MARS",                     # This is the name of the package
-    version="1.23.628",                        # The initial release version
+    version="1.23.629",                        # The initial release version
     author="Telexy",                     # Full name of the author
     author_email="support@telexy.com", # Full email of author
     description="MARS Inference server",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.10',                # Minimum version requirement of the package
     py_modules=["MARS"],             # Name of the python package
-    #package_dir={'':'/Telexy'},     # Directory of the source code of the package
     install_requires=['jsonpickle', "cherrypy"]                     # Install other dependencies if any
 )
```

