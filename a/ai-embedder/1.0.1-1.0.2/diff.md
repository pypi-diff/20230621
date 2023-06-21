# Comparing `tmp/ai_embedder-1.0.1.tar.gz` & `tmp/ai_embedder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_embedder-1.0.1.tar", last modified: Wed Jun 21 17:48:54 2023, max compression
+gzip compressed data, was "ai_embedder-1.0.2.tar", last modified: Wed Jun 21 17:56:16 2023, max compression
```

## Comparing `ai_embedder-1.0.1.tar` & `ai_embedder-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:54.847630 ai_embedder-1.0.1/ai_embedder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/ai_embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/ai_embedder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/ai_embedder/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/ai_embedder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 17:48:54.000000 ai_embedder-1.0.1/ai_embedder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:48:54.851630 ai_embedder-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 17:48:44.000000 ai_embedder-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:56:16.147563 ai_embedder-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 17:56:06.000000 ai_embedder-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-21 17:56:16.147563 ai_embedder-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-21 17:56:06.000000 ai_embedder-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:56:16.147563 ai_embedder-1.0.2/ai_embedder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:56:06.000000 ai_embedder-1.0.2/ai_embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 17:56:06.000000 ai_embedder-1.0.2/ai_embedder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 17:56:06.000000 ai_embedder-1.0.2/ai_embedder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:56:16.147563 ai_embedder-1.0.2/ai_embedder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-21 17:56:16.000000 ai_embedder-1.0.2/ai_embedder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 17:56:16.000000 ai_embedder-1.0.2/ai_embedder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:56:16.000000 ai_embedder-1.0.2/ai_embedder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 17:56:16.000000 ai_embedder-1.0.2/ai_embedder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 17:56:16.000000 ai_embedder-1.0.2/ai_embedder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:56:16.147563 ai_embedder-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-21 17:56:06.000000 ai_embedder-1.0.2/setup.py
```

### Comparing `ai_embedder-1.0.1/LICENSE` & `ai_embedder-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_embedder-1.0.1/PKG-INFO` & `ai_embedder-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_embedder
-Version: 1.0.1
+Version: 1.0.2
 Summary: This script takes .ai files and save them with linked files embedded.
 Author: mdobosz
 Author-email: doboszsite@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AI Link Embedder #
```

### Comparing `ai_embedder-1.0.1/README.md` & `ai_embedder-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ai_embedder-1.0.1/ai_embedder/main.py` & `ai_embedder-1.0.2/ai_embedder/main.py`

 * *Files identical despite different names*

### Comparing `ai_embedder-1.0.1/ai_embedder.egg-info/PKG-INFO` & `ai_embedder-1.0.2/ai_embedder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-embedder
-Version: 1.0.1
+Version: 1.0.2
 Summary: This script takes .ai files and save them with linked files embedded.
 Author: mdobosz
 Author-email: doboszsite@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AI Link Embedder #
```

### Comparing `ai_embedder-1.0.1/setup.py` & `ai_embedder-1.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,13 +19,11 @@
       description='This script takes .ai files and save them with linked files embedded.',
       author='mdobosz',
       author_email='doboszsite@gmail.com',
       packages=find_packages(),
       long_description_content_type="text/markdown",
       long_description=README,
       install_requires=[
-            "altgraph==0.17.3",
-           " pefile==2023.2.7",
             "pywin32==306",
             "pywin32-ctypes==0.2.1"
       ]
       )
```

