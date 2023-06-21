# Comparing `tmp/pypubmed-1.1.0.tar.gz` & `tmp/pypubmed-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypubmed-1.1.0.tar", last modified: Fri Apr 28 02:41:26 2023, max compression
+gzip compressed data, was "pypubmed-1.1.1.tar", last modified: Wed Jun 21 02:41:20 2023, max compression
```

## Comparing `pypubmed-1.1.0.tar` & `pypubmed-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.140064 pypubmed-1.1.0/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       63 2020-12-08 08:44:31.000000 pypubmed-1.1.0/MANIFEST.in
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1894 2023-04-28 02:41:26.133464 pypubmed-1.1.0/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      733 2023-04-28 02:41:07.000000 pypubmed-1.1.0/README.md
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:25.771367 pypubmed-1.1.0/pypubmed/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      197 2020-12-10 07:10:17.000000 pypubmed-1.1.0/pypubmed/__init__.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:25.955008 pypubmed-1.1.0/pypubmed/bin/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-08-11 08:30:01.000000 pypubmed-1.1.0/pypubmed/bin/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1705 2020-12-11 02:19:16.000000 pypubmed-1.1.0/pypubmed/bin/_citations.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     5348 2021-03-01 06:29:04.000000 pypubmed-1.1.0/pypubmed/bin/_search.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1586 2023-04-28 02:21:02.000000 pypubmed-1.1.0/pypubmed/bin/cli.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.050610 pypubmed-1.1.0/pypubmed/core/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-09-11 05:55:10.000000 pypubmed-1.1.0/pypubmed/core/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      616 2020-09-15 08:44:09.000000 pypubmed-1.1.0/pypubmed/core/article.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2917 2020-12-08 07:47:09.000000 pypubmed-1.1.0/pypubmed/core/citations.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)    10160 2023-04-28 02:27:59.000000 pypubmed-1.1.0/pypubmed/core/eutils.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     6381 2021-02-23 03:53:38.000000 pypubmed-1.1.0/pypubmed/core/export.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.090122 pypubmed-1.1.0/pypubmed/util/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      336 2020-12-09 03:34:07.000000 pypubmed-1.1.0/pypubmed/util/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     5631 2021-08-11 05:51:51.000000 pypubmed-1.1.0/pypubmed/util/xml_parser.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.111284 pypubmed-1.1.0/pypubmed/version/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      167 2023-04-28 02:28:48.000000 pypubmed-1.1.0/pypubmed/version/version.json
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:25.883358 pypubmed-1.1.0/pypubmed.egg-info/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1894 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      568 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/SOURCES.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/dependency_links.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       83 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/entry_points.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      118 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/requires.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        9 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/top_level.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      118 2023-04-28 02:39:17.000000 pypubmed-1.1.0/requirements.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-04-28 02:41:26.144073 pypubmed-1.1.0/setup.cfg
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1540 2020-12-11 03:36:41.000000 pypubmed-1.1.0/setup.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-06-21 02:41:20.689585 pypubmed-1.1.1/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       63 2020-12-08 08:44:31.000000 pypubmed-1.1.1/MANIFEST.in
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1894 2023-06-21 02:41:20.682225 pypubmed-1.1.1/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      733 2023-04-28 02:41:07.000000 pypubmed-1.1.1/README.md
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-06-21 02:41:20.088814 pypubmed-1.1.1/pypubmed/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      197 2020-12-10 07:10:17.000000 pypubmed-1.1.1/pypubmed/__init__.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-06-21 02:41:20.334496 pypubmed-1.1.1/pypubmed/bin/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-08-11 08:30:01.000000 pypubmed-1.1.1/pypubmed/bin/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1705 2020-12-11 02:19:16.000000 pypubmed-1.1.1/pypubmed/bin/_citations.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     5348 2021-03-01 06:29:04.000000 pypubmed-1.1.1/pypubmed/bin/_search.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1586 2023-04-28 02:21:02.000000 pypubmed-1.1.1/pypubmed/bin/cli.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-06-21 02:41:20.476257 pypubmed-1.1.1/pypubmed/core/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-09-11 05:55:10.000000 pypubmed-1.1.1/pypubmed/core/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      616 2020-09-15 08:44:09.000000 pypubmed-1.1.1/pypubmed/core/article.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2917 2020-12-08 07:47:09.000000 pypubmed-1.1.1/pypubmed/core/citations.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)    10294 2023-06-21 02:38:09.000000 pypubmed-1.1.1/pypubmed/core/eutils.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     6381 2021-02-23 03:53:38.000000 pypubmed-1.1.1/pypubmed/core/export.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-06-21 02:41:20.573383 pypubmed-1.1.1/pypubmed/util/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      336 2020-12-09 03:34:07.000000 pypubmed-1.1.1/pypubmed/util/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     5631 2021-08-11 05:51:51.000000 pypubmed-1.1.1/pypubmed/util/xml_parser.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-06-21 02:41:20.659457 pypubmed-1.1.1/pypubmed/version/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      167 2023-06-21 02:40:29.000000 pypubmed-1.1.1/pypubmed/version/version.json
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-06-21 02:41:20.226350 pypubmed-1.1.1/pypubmed.egg-info/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1894 2023-06-21 02:41:19.000000 pypubmed-1.1.1/pypubmed.egg-info/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      568 2023-06-21 02:41:19.000000 pypubmed-1.1.1/pypubmed.egg-info/SOURCES.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-06-21 02:41:19.000000 pypubmed-1.1.1/pypubmed.egg-info/dependency_links.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       83 2023-06-21 02:41:19.000000 pypubmed-1.1.1/pypubmed.egg-info/entry_points.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      118 2023-06-21 02:41:19.000000 pypubmed-1.1.1/pypubmed.egg-info/requires.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        9 2023-06-21 02:41:19.000000 pypubmed-1.1.1/pypubmed.egg-info/top_level.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      118 2023-04-28 02:39:17.000000 pypubmed-1.1.1/requirements.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-06-21 02:41:20.696507 pypubmed-1.1.1/setup.cfg
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1540 2020-12-11 03:36:41.000000 pypubmed-1.1.1/setup.py
```

### Comparing `pypubmed-1.1.0/PKG-INFO` & `pypubmed-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypubmed
-Version: 1.1.0
+Version: 1.1.1
 Summary: Toolkits for NCBI Pubmed
 Home-page: https://github.com/suqingdong/pypubmed
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: BSD License
 Project-URL: Documentation, https://pypubmed.readthedocs.io
 Project-URL: Tracker, https://github.com/suqingdong/pypubmed/issues
```

### Comparing `pypubmed-1.1.0/README.md` & `pypubmed-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed/bin/_citations.py` & `pypubmed-1.1.1/pypubmed/bin/_citations.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed/bin/_search.py` & `pypubmed-1.1.1/pypubmed/bin/_search.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed/bin/cli.py` & `pypubmed-1.1.1/pypubmed/bin/cli.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed/core/article.py` & `pypubmed-1.1.1/pypubmed/core/article.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed/core/citations.py` & `pypubmed-1.1.1/pypubmed/core/citations.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed/core/eutils.py` & `pypubmed-1.1.1/pypubmed/core/eutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,19 @@
             idlist = term.split(',')
         else:
             idlist = self.esearch(term, **kwargs)
 
         articles = self.efetch(idlist, **kwargs)
         for article in articles:
             if impact_factor:
-                res = self.IF.search(article.issn) or self.IF.search(article.e_issn)
+                res = None
+                if article.issn:
+                    res = self.IF.search(article.issn)
+                if not res and article.e_issn:
+                    res = self.IF.search(article.e_issn)
                 article.impact_factor = res[0]['factor'] if res else '.'
 
             if cited:
                 article.cited = self.get_cited(article.pmid)
 
             if translate and self.TR_OK:
                 if translate_cache and translate_cache.get(article.pmid):
```

### Comparing `pypubmed-1.1.0/pypubmed/core/export.py` & `pypubmed-1.1.1/pypubmed/core/export.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed/util/xml_parser.py` & `pypubmed-1.1.1/pypubmed/util/xml_parser.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/pypubmed.egg-info/PKG-INFO` & `pypubmed-1.1.1/pypubmed.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypubmed
-Version: 1.1.0
+Version: 1.1.1
 Summary: Toolkits for NCBI Pubmed
 Home-page: https://github.com/suqingdong/pypubmed
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: BSD License
 Project-URL: Documentation, https://pypubmed.readthedocs.io
 Project-URL: Tracker, https://github.com/suqingdong/pypubmed/issues
```

### Comparing `pypubmed-1.1.0/pypubmed.egg-info/SOURCES.txt` & `pypubmed-1.1.1/pypubmed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypubmed-1.1.0/setup.py` & `pypubmed-1.1.1/setup.py`

 * *Files identical despite different names*

