# Comparing `tmp/getpaper-0.0.3.tar.gz` & `tmp/getpaper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.0.3.tar", last modified: Tue Jun 20 21:41:15 2023, max compression
+gzip compressed data, was "getpaper-0.0.4.tar", last modified: Tue Jun 20 23:35:35 2023, max compression
```

## Comparing `getpaper-0.0.3.tar` & `getpaper-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:41:15.589508 getpaper-0.0.3/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.3/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      642 2023-06-20 21:41:15.589508 getpaper-0.0.3/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       28 2023-06-20 19:48:29.000000 getpaper-0.0.3/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:41:15.589508 getpaper-0.0.3/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.3/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3543 2023-06-20 21:23:26.000000 getpaper-0.0.3/getpaper/download.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:41:15.589508 getpaper-0.0.3/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      642 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      262 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       51 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      132 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-20 21:41:15.589508 getpaper-0.0.3/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1378 2023-06-20 21:41:14.000000 getpaper-0.0.3/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 23:35:35.530794 getpaper-0.0.4/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.4/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-20 23:35:35.530794 getpaper-0.0.4/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1344 2023-06-20 23:35:34.000000 getpaper-0.0.4/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 23:35:35.530794 getpaper-0.0.4/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.4/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3544 2023-06-20 22:10:24.000000 getpaper-0.0.4/getpaper/download.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3162 2023-06-20 23:27:35.000000 getpaper-0.0.4/getpaper/parse.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 23:35:35.530794 getpaper-0.0.4/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1959 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      280 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      142 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-20 23:35:35.000000 getpaper-0.0.4/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-20 23:35:35.530794 getpaper-0.0.4/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1472 2023-06-20 23:35:34.000000 getpaper-0.0.4/setup.py
```

### Comparing `getpaper-0.0.3/LICENSE` & `getpaper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.3/getpaper/download.py` & `getpaper-0.0.4/getpaper/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from click import Context
 from pycomfort.files import with_ext
 from pynction import Try
 from scidownl import scihub_download
 
 def doi_from_pubmed(pubmed_id: str):
     """
-    resolves doi by pubmedid
+    resolves doi by pubmed id
     :param pubmed_id:
     :return:
     """
     base_url = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi"
     params = {
         "db": "pubmed",
         "id": pubmed_id,
```

### Comparing `getpaper-0.0.3/setup.py` & `getpaper-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
     author="antonkulaga (Anton Kulaga)",
     author_email="<antonkulaga@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pyfunctional', 'more-itertools', 'click', 'unstructured', 'unstructured-inference', 'unstructured[local-inference]', 'unstructured.PaddleOCR', 'scidownl'],
+    install_requires=['pyfunctional', 'more-itertools', 'click',
+                      'unstructured', 'unstructured-inference', 'unstructured[local-inference]', 'unstructured.PaddleOCR',
+                      'scidownl', 'langchain'],
     keywords=['python', 'utils', 'files', 'papers', 'download'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     entry_points={
      "console_scripts": [
-         "download=getpaper.download:app"
+         "download=getpaper.download:app",
+         "parse=getpaper.parse:app"
      ]
     }
 )
```

