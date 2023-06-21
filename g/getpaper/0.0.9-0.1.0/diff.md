# Comparing `tmp/getpaper-0.0.9.tar.gz` & `tmp/getpaper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.0.9.tar", last modified: Wed Jun 21 14:23:02 2023, max compression
+gzip compressed data, was "getpaper-0.1.0.tar", last modified: Wed Jun 21 21:10:24 2023, max compression
```

## Comparing `getpaper-0.0.9.tar` & `getpaper-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 14:23:02.415236 getpaper-0.0.9/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.9/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 14:23:02.415236 getpaper-0.0.9/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1976 2023-06-21 14:08:28.000000 getpaper-0.0.9/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 14:23:02.415236 getpaper-0.0.9/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.9/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3997 2023-06-21 14:18:41.000000 getpaper-0.0.9/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4443 2023-06-21 14:18:52.000000 getpaper-0.0.9/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5437 2023-06-21 13:54:57.000000 getpaper-0.0.9/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1068 2023-06-21 10:50:13.000000 getpaper-0.0.9/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 14:23:02.415236 getpaper-0.0.9/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 14:23:02.000000 getpaper-0.0.9/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 14:23:02.000000 getpaper-0.0.9/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 14:23:02.000000 getpaper-0.0.9/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-21 14:23:02.000000 getpaper-0.0.9/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 14:23:02.000000 getpaper-0.0.9/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 14:23:02.000000 getpaper-0.0.9/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 14:23:02.415236 getpaper-0.0.9/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-21 14:22:59.000000 getpaper-0.0.9/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 21:10:24.403582 getpaper-0.1.0/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.0/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 21:10:24.403582 getpaper-0.1.0/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1976 2023-06-21 14:08:28.000000 getpaper-0.1.0/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 21:10:24.403582 getpaper-0.1.0/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.0/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3997 2023-06-21 14:18:41.000000 getpaper-0.1.0/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.0/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5437 2023-06-21 13:54:57.000000 getpaper-0.1.0/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.0/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 21:10:24.403582 getpaper-0.1.0/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 21:10:24.000000 getpaper-0.1.0/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 21:10:24.000000 getpaper-0.1.0/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 21:10:24.000000 getpaper-0.1.0/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-21 21:10:24.000000 getpaper-0.1.0/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 21:10:24.000000 getpaper-0.1.0/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 21:10:24.000000 getpaper-0.1.0/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 21:10:24.403582 getpaper-0.1.0/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-21 21:07:35.000000 getpaper-0.1.0/setup.py
```

### Comparing `getpaper-0.0.9/LICENSE` & `getpaper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.9/PKG-INFO` & `getpaper-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.9
+Version: 0.1.0
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.0.9/README.md` & `getpaper-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.9/getpaper/download.py` & `getpaper-0.1.0/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.9/getpaper/index.py` & `getpaper-0.1.0/getpaper/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from langchain.embeddings.base import Embeddings
 from langchain.schema import Document
 from langchain.text_splitter import TextSplitter
 from langchain.vectorstores import Chroma
 from pycomfort.files import *
 
 from getpaper.parse import papers_to_documents
-from splitter import RecursiveSplitterWithSource
+from getpaper.splitter import RecursiveSplitterWithSource
 
 
 def load_environment_keys(debug: bool = True):
     e = dotenv.find_dotenv()
     if debug:
         print(f"environment found at {e}")
     has_env: bool = load_dotenv(e, verbose=True, override=True)
```

### Comparing `getpaper-0.0.9/getpaper/parse.py` & `getpaper-0.1.0/getpaper/parse.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.9/getpaper/splitter.py` & `getpaper-0.1.0/getpaper/splitter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List
 
 from langchain.schema import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from pycomfort.files import *
 from copy import deepcopy
 
+
 class RecursiveSplitterWithSource(RecursiveCharacterTextSplitter):
     """
     Splitter that also modifies metadata
     """
     def create_documents(
             self, texts: List[str], metadatas: Optional[List[dict]] = None
     ) -> List[Document]:
```

### Comparing `getpaper-0.0.9/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.0/getpaper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.9
+Version: 0.1.0
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.0.9/setup.py` & `getpaper-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

