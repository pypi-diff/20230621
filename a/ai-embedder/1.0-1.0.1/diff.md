# Comparing `tmp/ai_embedder-1.0.tar.gz` & `tmp/ai_embedder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_embedder-1.0.tar", last modified: Wed Jun 21 17:07:33 2023, max compression
+gzip compressed data, was "ai_embedder-1.0.1.tar", last modified: Wed Jun 21 17:48:54 2023, max compression
```

## Comparing `ai_embedder-1.0.tar` & `ai_embedder-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:33.161582 ai_embedder-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 17:07:21.000000 ai_embedder-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-21 17:07:33.161582 ai_embedder-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 17:07:21.000000 ai_embedder-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:33.161582 ai_embedder-1.0/ai_embedder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:21.000000 ai_embedder-1.0/ai_embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 17:07:21.000000 ai_embedder-1.0/ai_embedder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 17:07:21.000000 ai_embedder-1.0/ai_embedder/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:33.161582 ai_embedder-1.0/ai_embedder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-21 17:07:33.000000 ai_embedder-1.0/ai_embedder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 17:07:33.000000 ai_embedder-1.0/ai_embedder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:07:33.000000 ai_embedder-1.0/ai_embedder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 17:07:33.000000 ai_embedder-1.0/ai_embedder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 17:07:33.000000 ai_embedder-1.0/ai_embedder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:07:33.161582 ai_embedder-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-21 17:07:21.000000 ai_embedder-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:54.847630 ai_embedder-1.0.1/ai_embedder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/ai_embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/ai_embedder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/ai_embedder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/ai_embedder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/setup.py
```

### Comparing `ai_embedder-1.0/LICENSE` & `ai_embedder-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_embedder-1.0/README.md` & `ai_embedder-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 # AI Link Embedder #
 ## Introduction ##
 This abomination of a code was created to solve my fiancé issue with migrating Adobe Illustrator files to different machine. It comes with absolutely no guarantee, but it seems to work. Good luck.
-
 ## Requirements ##
 Running this script requires:
 - Windows OS (macOS is not supported for now)
 - Adobe Illustrator installed
-## Setup ##
-To install necessary dependency you need to run:
-```shell
-pip install -r requirement.txt
-```
 ## Run ##
 Usage:
 ```
 usage: AI Link Embedder [-h] [-r] [-o] [-d DEST] [-p PREFIX] [-s SUFFIX]
                         dictionary
 
 This script takes .ai files and save them with linked files embedded
@@ -27,10 +21,10 @@
   -r, --recursive       Scan for .ai files recursively
   -o, --override        Override resulting .ai is it exists
   -d DEST, --dest DEST  Directory where resulting .ai files will be saved to
   -p PREFIX, --prefix PREFIX
   -s SUFFIX, --suffix SUFFIX
 ```
 Example:
-```shell
-python3 main.py -o -d C:\Users\Username\Documents\ai_embedded -r C:\Users\Username\Documents\
+```
+python -m ai_embedder
 ```
```

### Comparing `ai_embedder-1.0/ai_embedder/main.py` & `ai_embedder-1.0.1/ai_embedder/main.py`

 * *Files identical despite different names*

### Comparing `ai_embedder-1.0/setup.py` & `ai_embedder-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 #!/usr/bin/env python
+import os
 
 from setuptools import find_packages, setup
 
+with open("README.md", "r") as readme_file:
+    README = readme_file.read()
+
+
+def _get_version():
+    version = os.getenv("RELEASE_VERSION", default="1.0")
+    if version.startswith("v"):
+        version = version[1:]
+    return version
+
+
 setup(name='ai_embedder',
-      version='1.0',
+      version=_get_version(),
       description='This script takes .ai files and save them with linked files embedded.',
       author='mdobosz',
       author_email='doboszsite@gmail.com',
       packages=find_packages(),
-      long_description="This script takes .ai files and save them with linked files embedded.",
+      long_description_content_type="text/markdown",
+      long_description=README,
       install_requires=[
             "altgraph==0.17.3",
            " pefile==2023.2.7",
             "pywin32==306",
             "pywin32-ctypes==0.2.1"
       ]
       )
```

