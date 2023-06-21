# Comparing `tmp/clld_corpus_plugin-0.0.7.tar.gz` & `tmp/clld_corpus_plugin-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clld_corpus_plugin-0.0.7.tar", last modified: Mon Nov 28 00:53:09 2022, max compression
+gzip compressed data, was "dist/clld_corpus_plugin-0.0.8.tar", last modified: Wed Jun 21 09:12:59 2023, max compression
```

## Comparing `clld_corpus_plugin-0.0.7.tar` & `clld_corpus_plugin-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      424 2022-11-28 00:53:05.000000 clld_corpus_plugin-0.0.7/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-05-03 08:26:17.000000 clld_corpus_plugin-0.0.7/LICENSE
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       64 2022-11-28 00:52:30.000000 clld_corpus_plugin-0.0.7/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1236 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/PKG-INFO
--rw-r--r--   0 florianm  (1000) florianm  (1000)      326 2022-05-03 11:46:27.000000 clld_corpus_plugin-0.0.7/README.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      517 2022-11-04 22:00:40.000000 clld_corpus_plugin-0.0.7/pyproject.toml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1689 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-05-03 08:26:17.000000 clld_corpus_plugin-0.0.7/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1542 2022-11-28 00:52:59.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/__init__.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/cldf/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      603 2022-07-21 21:36:10.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/cldf/SpeakerTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1591 2022-07-21 21:20:48.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/cldf/TextTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      386 2022-07-21 21:34:19.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/cldf/__init__.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)      772 2022-11-04 21:51:25.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/datatables.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)      356 2022-11-04 21:51:25.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/interfaces.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)     4342 2022-11-16 04:42:38.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/models.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/static/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      136 2022-11-04 22:21:44.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/static/clld-corpus.css
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      219 2022-05-27 17:47:07.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/static/clld-corpus.js
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/meaning/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1114 2022-05-27 16:41:41.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/meaning/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      247 2022-05-10 08:02:33.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/meaning/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/sentence/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1650 2022-11-08 02:03:59.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/sentence/detail_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/speaker/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      764 2022-07-21 22:02:41.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/speaker/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      247 2022-07-21 21:52:58.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/speaker/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/tag/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      690 2022-06-01 00:03:23.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/tag/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      279 2022-06-01 00:00:49.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/tag/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/text/
--rwxrwxr-x   0 florianm  (1000) florianm  (1000)     1390 2022-11-16 04:54:29.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/text/detail_html.mako
--rwxr--r--   0 florianm  (1000) florianm  (1000)      281 2022-05-06 12:28:27.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/text/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/wordform/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1472 2022-05-27 16:22:25.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/wordform/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      245 2022-04-25 06:19:12.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/wordform/index_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)     5901 2022-11-16 04:46:44.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/util.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1236 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1383 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      183 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       19 2022-11-28 00:53:09.000000 clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      424 2023-06-21 09:12:50.000000 clld_corpus_plugin-0.0.8/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-05-03 08:26:17.000000 clld_corpus_plugin-0.0.8/LICENSE
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       64 2022-11-28 00:52:30.000000 clld_corpus_plugin-0.0.8/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1236 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/PKG-INFO
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      326 2022-05-03 11:46:27.000000 clld_corpus_plugin-0.0.8/README.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      517 2022-11-04 22:00:40.000000 clld_corpus_plugin-0.0.8/pyproject.toml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1689 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-05-03 08:26:17.000000 clld_corpus_plugin-0.0.8/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1571 2023-06-21 09:12:36.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/__init__.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/cldf/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      603 2022-07-21 21:36:10.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/cldf/SpeakerTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1591 2022-07-21 21:20:48.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/cldf/TextTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      386 2022-07-21 21:34:19.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/cldf/__init__.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1520 2023-06-21 05:18:42.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/datatables.py
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      356 2023-06-21 05:14:06.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/interfaces.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     4746 2023-06-21 05:18:19.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/models.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/static/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      136 2022-11-04 22:21:44.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/static/clld-corpus.css
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      219 2022-05-27 17:47:07.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/static/clld-corpus.js
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/meaning/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1114 2022-05-27 16:41:41.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/meaning/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      247 2022-05-10 08:02:33.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/meaning/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/sentence/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1849 2023-03-05 17:54:04.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/sentence/detail_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/speaker/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      764 2023-03-07 07:25:30.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/speaker/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      247 2022-07-21 21:52:58.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/speaker/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/tag/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      690 2022-06-01 00:03:23.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/tag/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      279 2022-06-01 00:00:49.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/tag/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/text/
+-rwxrwxr-x   0 florianm  (1000) florianm  (1000)     1390 2023-03-06 02:26:34.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/text/detail_html.mako
+-rwxr--r--   0 florianm  (1000) florianm  (1000)      281 2022-05-06 12:28:27.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/text/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/wordform/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1472 2022-05-27 16:22:25.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/wordform/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      245 2022-04-25 06:19:12.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/wordform/index_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5901 2023-03-05 21:54:23.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/util.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1236 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1383 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      183 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       19 2023-06-21 09:12:59.000000 clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/top_level.txt
```

### Comparing `clld_corpus_plugin-0.0.7/LICENSE` & `clld_corpus_plugin-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/PKG-INFO` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: clld_corpus_plugin
-Version: 0.0.7
+Name: clld-corpus-plugin
+Version: 0.0.8
 Summary: A plugin providing text functionality in CLLD.
 Home-page: https://github.com/fmatter/clld-corpus-plugin
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/clld-corpus-plugin/issues
 Keywords: clld,corpus linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `clld_corpus_plugin-0.0.7/pyproject.toml` & `clld_corpus_plugin-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/setup.cfg` & `clld_corpus_plugin-0.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	corpus linguistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = clld_corpus_plugin
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/clld-corpus-plugin/issues
 url = https://github.com/fmatter/clld-corpus-plugin
-version = 0.0.7
+version = 0.0.8
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/__init__.py` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Top-level package for clld-corpus-plugin."""
+import logging
+from pyramid.response import FileResponse
+from pyramid.response import Response
+from clld_corpus_plugin import datatables
 from clld_corpus_plugin import interfaces
 from clld_corpus_plugin import models
-from clld_corpus_plugin import datatables
-from pyramid.response import Response, FileResponse
-import logging
+
 
 log = logging.getLogger(__name__)
 
 __author__ = "Florian Matter"
 __email__ = "florianmatter@gmail.com"
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 audio_suffixes = [".mp3", ".wav"]
 
 
 def audio_view(request):
     audio_id = request.matchdict["audio_id"]
     log.debug(f"Audio {audio_id} requested")
@@ -32,12 +34,12 @@
     )
     config.add_static_view("clld-corpus-plugin-static", "clld_corpus_plugin:static")
     config.register_resource("text", models.Text, interfaces.IText, with_index=True)
     config.register_resource(
         "speaker", models.Speaker, interfaces.ISpeaker, with_index=True
     )
     config.register_resource("tag", models.Tag, interfaces.ITag, with_index=True)
-
     config.add_route("audio_route", "/audio/{audio_id}")
     config.add_view(audio_view, route_name="audio_route")
-    config.register_datatable("texts", datatables.Texts)
+
     config.register_datatable("sentences", datatables.SentencesWithAudio)
+    config.register_datatable("texts", datatables.Texts)
```

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/cldf/SpeakerTable-metadata.json` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/cldf/SpeakerTable-metadata.json`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/cldf/TextTable-metadata.json` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/cldf/TextTable-metadata.json`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/models.py` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,59 @@
+from clld import interfaces
 from clld.db.meta import Base
+from clld.db.meta import CustomModelMixin
 from clld.db.meta import PolymorphicBaseMixin
 from clld.db.models import IdNameDescriptionMixin
 from clld.db.models import Sentence
 from clld.db.models.common import Contribution
 from clld.db.models.common import HasSourceMixin
 from clld.db.models.common import Language
+from clld.interfaces import ISentence
 from sqlalchemy import JSON
 from sqlalchemy import Column
 from sqlalchemy import ForeignKey
 from sqlalchemy import Integer
 from sqlalchemy import String
 from sqlalchemy import Unicode
 from sqlalchemy import UniqueConstraint
+from sqlalchemy import text
 from sqlalchemy.orm import relationship
 from zope.interface import implementer
-from clld_corpus_plugin.interfaces import IText, ITag, ISpeaker
-from clld_corpus_plugin.interfaces import IWordform, IMeaning
+from clld_corpus_plugin.interfaces import IMeaning
+from clld_corpus_plugin.interfaces import ISpeaker
+from clld_corpus_plugin.interfaces import ITag
+from clld_corpus_plugin.interfaces import IText
+from clld_corpus_plugin.interfaces import IWordform
 
 
 @implementer(ITag)
 class Tag(Base, IdNameDescriptionMixin):
     pass
 
 
 @implementer(ISpeaker)
 class Speaker(Base, IdNameDescriptionMixin):
     pass
 
 
+@implementer(interfaces.ISentence)
+class Record(CustomModelMixin, Sentence):
+    pk = Column(Integer, ForeignKey("sentence.pk"), primary_key=True)
+
+    contribution_pk = Column(Integer, ForeignKey("contribution.pk"))
+    contribution = relationship(Contribution, backref="sentences")
+
+
 class SpeakerSentence(Base, PolymorphicBaseMixin):
     __table_args__ = (UniqueConstraint("speaker_pk", "sentence_pk"),)
 
     sentence_pk = Column(Integer, ForeignKey("sentence.pk"), nullable=False)
     speaker_pk = Column(Integer, ForeignKey("speaker.pk"), nullable=False)
     speaker = relationship(Speaker, innerjoin=True, backref="sentences")
-    sentence = relationship(Sentence, innerjoin=True, backref="speaker")
+    sentence = relationship(Record, innerjoin=True, backref="speaker")
 
 
 @implementer(IText)
 class Text(Base, IdNameDescriptionMixin, HasSourceMixin):
     text_type = Column(Unicode())
     text_metadata = Column(JSON)
 
@@ -57,20 +72,20 @@
 
 
 class SentenceTag(Base, PolymorphicBaseMixin):
     __table_args__ = (UniqueConstraint("sentence_pk", "tag_pk"),)
 
     sentence_pk = Column(Integer, ForeignKey("sentence.pk"), nullable=False)
     tag_pk = Column(Integer, ForeignKey("tag.pk"), nullable=False)
-    sentence = relationship(Sentence, innerjoin=True, backref="tags")
+    sentence = relationship(Record, innerjoin=True, backref="tags")
     tag = relationship(Tag, innerjoin=True, backref="sentences")
 
 
 try:
-    from clld_morphology_plugin.models import Wordform, Meaning, FormMeaning
+    from clld_morphology_plugin.models import Wordform
 except ImportError:
 
     @implementer(IWordform)
     class Wordform(Base, PolymorphicBaseMixin, IdNameDescriptionMixin, HasSourceMixin):
         __table_args__ = (UniqueConstraint("language_pk", "id"),)
 
         language_pk = Column(Integer, ForeignKey("language.pk"), nullable=False)
@@ -96,20 +111,21 @@
 
     text_pk = Column(Integer, ForeignKey("text.pk"), nullable=False)
     sentence_pk = Column(Integer, ForeignKey("sentence.pk"), nullable=False)
     record_number = Column(Integer, nullable=False)
     phrase_number = Column(Integer, nullable=True)
 
     text = relationship(
-        Text, innerjoin=True, backref="sentences", order_by="desc(TextSentence.record_number)"
+        Text,
+        innerjoin=True,
+        backref="sentences",
+        order_by="desc(TextSentence.record_number)",
     )
-    sentence = relationship(Sentence, innerjoin=True, backref="text_assocs")
+    sentence = relationship(Record, innerjoin=True, backref="text_assocs")
 
 
-class SentenceSlice(Base):
+class SentencePart(Base):
     form_pk = Column(Integer, ForeignKey("wordform.pk"))
     sentence_pk = Column(Integer, ForeignKey("sentence.pk"))
-    formmeaning_pk = Column(Integer, ForeignKey("formmeaning.pk"))
     form = relationship(Wordform, backref="sentence_assocs")
-    sentence = relationship(Sentence, backref="forms")
-    form_meaning = relationship(FormMeaning, backref="form_tokens")
+    sentence = relationship(Record, backref="forms")
     index = Column(Integer)
```

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/meaning/detail_html.mako` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/meaning/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/sentence/detail_html.mako` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/sentence/detail_html.mako`

 * *Files 20% similar despite different names*

```diff
@@ -13,48 +13,47 @@
             % endif
         % endfor
         </ul>
     </%util:well>
     % endif
 </%def>
 
-<h2>${_('Sentence')} ${ctx.id}</h2>
+<h3>${_('Sentence')} ${ctx.id}</h3>
+
+${cutil.rendered_sentence(request, ctx, in_context=False, text_link=False)|n}
+
+
 <dl>
     <dt>${_('Language')}:</dt>
     <dd>${h.link(request, ctx.language)}</dd>
     % if ctx.tags:
         <dt>Tags</dt> <dd>
         % for tag in ctx.tags:
             ${h.link(request, tag.tag)}
         % endfor
         </dd>
     % endif
-</dl>
-
-${cutil.rendered_sentence(request, ctx, in_context=False, text_link=False)|n}
-
-<dl>
-% if ctx.comment:
-<dt>${_('Comment')}:</dt>
-<dd>${ctx.markup_comment or ctx.comment|n}</dd>
-% endif
-% if ctx.source:
-<dt>${_('Type')}:</dt>
-<dd>${ctx.type}</dd>
-% endif
-% if ctx.speaker:
-<dt>${_('Speaker')}:</dt>
-<dd>${h.link(request, ctx.speaker[0].speaker)}</dd>
-% endif
-% if ctx.references or ctx.source or ctx.text_assocs:
-<dt>${_('Source')}:</dt>
-% if ctx.source:
-<dd>${ctx.source}</dd>
-% endif
-% if ctx.references:
-<dd>${h.linked_references(request, ctx)|n}</dd>
-% endif
-% if ctx.text_assocs:
-<dd>${h.link(request, ctx.text_assocs[0].text, url_kw={"_anchor":ctx.id})}</dd>
-% endif
-% endif
+    % if ctx.comment:
+        <dt>${_('Comment')}:</dt>
+        <dd>${ctx.markup_comment or ctx.comment|n}</dd>
+    % endif
+    % if ctx.source:
+        <dt>${_('Type')}:</dt>
+        <dd>${ctx.type}</dd>
+    % endif
+    % if ctx.speaker:
+        <dt>${_('Speaker')}:</dt>
+        <dd>${h.link(request, ctx.speaker[0].speaker)}</dd>
+    % endif
+    % if ctx.references or ctx.source or ctx.text_assocs:
+        <dt>${_('Source')}:</dt>
+        % if ctx.source:
+            <dd>${ctx.source}</dd>
+        % endif
+        % if ctx.references:
+            <dd>${h.linked_references(request, ctx)|n}</dd>
+        % endif
+        % if ctx.text_assocs:
+            <dd>${h.link(request, ctx.text_assocs[0].text, url_kw={"_anchor":ctx.id})}: ${ctx.text_assocs[0].record_number}</dd>
+        % endif
+    % endif
 </dl>
```

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/speaker/detail_html.mako` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/speaker/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/tag/detail_html.mako` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/tag/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/text/detail_html.mako` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/text/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/templates/wordform/detail_html.mako` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/templates/wordform/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin/util.py` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin/util.py`

 * *Files identical despite different names*

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/PKG-INFO` & `clld_corpus_plugin-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: clld-corpus-plugin
-Version: 0.0.7
+Name: clld_corpus_plugin
+Version: 0.0.8
 Summary: A plugin providing text functionality in CLLD.
 Home-page: https://github.com/fmatter/clld-corpus-plugin
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/clld-corpus-plugin/issues
 Keywords: clld,corpus linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `clld_corpus_plugin-0.0.7/src/clld_corpus_plugin.egg-info/SOURCES.txt` & `clld_corpus_plugin-0.0.8/src/clld_corpus_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

