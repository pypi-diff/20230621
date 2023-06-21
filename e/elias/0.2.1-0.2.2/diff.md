# Comparing `tmp/elias-0.2.1.tar.gz` & `tmp/elias-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-elv4s3hw/elias-0.2.1.tar", last modified: Thu Jun  1 16:31:17 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-hueguy6a/elias-0.2.2.tar", last modified: Wed Jun 21 14:23:45 2023, max compression
```

## Comparing `elias-0.2.1.tar` & `elias-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:17.686972 elias-0.2.1/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.1/LICENSE
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-01 16:31:17.686972 elias-0.2.1/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.1/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.1/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-06-01 16:31:17.697341 elias-0.2.1/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.1/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:15.931860 elias-0.2.1/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.137287 elias-0.2.1/src/elias/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22222 2023-04-24 08:29:27.000000 elias-0.2.1/src/elias/config.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.581947 elias-0.2.1/src/elias/data/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/combined.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/loader.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/sampling.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/stop_criterion.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.896908 elias-0.2.1/src/elias/folder/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/folder/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/folder/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.1/src/elias/folder/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.1/src/elias/folder/folder.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.1/src/elias/folder/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.1/src/elias/folder/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:17.267704 elias-0.2.1/src/elias/manager/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/artifact.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/buffered.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.1/src/elias/manager/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.1/src/elias/manager/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.1/src/elias/manager/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:17.645622 elias-0.2.1/src/elias/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.1/src/elias/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.1/src/elias/util/fs.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.1/src/elias/util/io.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.1/src/elias/util/range.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.1/src/elias/util/timing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      390 2023-05-26 09:28:39.000000 elias-0.2.1/src/elias/util/typing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.1/src/elias/util/version.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.321601 elias-0.2.1/src/elias.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      923 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.829326 elias-0.2.2/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.2/LICENSE
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 14:23:45.829326 elias-0.2.2/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.2/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.2/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-06-21 14:23:45.829326 elias-0.2.2/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.2/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.118004 elias-0.2.2/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.307908 elias-0.2.2/src/elias/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22222 2023-04-24 08:29:27.000000 elias-0.2.2/src/elias/config.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.724000 elias-0.2.2/src/elias/data/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/combined.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/loader.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/sampling.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/stop_criterion.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.027385 elias-0.2.2/src/elias/folder/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/folder/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/folder/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.2/src/elias/folder/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.2/src/elias/folder/folder.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.2/src/elias/folder/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.2/src/elias/folder/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.387624 elias-0.2.2/src/elias/manager/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/artifact.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/buffered.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.2/src/elias/manager/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.2/src/elias/manager/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.2/src/elias/manager/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.785415 elias-0.2.2/src/elias/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.2/src/elias/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.2/src/elias/util/fs.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.2/src/elias/util/io.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.2/src/elias/util/random.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.2/src/elias/util/range.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.2/src/elias/util/timing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      390 2023-05-26 09:28:39.000000 elias-0.2.2/src/elias/util/typing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.2/src/elias/util/version.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.482925 elias-0.2.2/src/elias.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-06-21 14:23:44.000000 elias-0.2.2/src/elias.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/top_level.txt
```

### Comparing `elias-0.2.1/PKG-INFO` & `elias-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.1
+Version: 0.2.2
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.1/README.md` & `elias-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/setup.cfg` & `elias-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elias
-version = 0.2.1
+version = 0.2.2
 author = Tobias Kirschstein
 author_email = tobias.kirschstein@gmail.com
 description = ELIAS experiment library for facilitating machine learning projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tobias-kirschstein/elias
 project_urls =
```

### Comparing `elias-0.2.1/src/elias/config.py` & `elias-0.2.2/src/elias/config.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/data/combined.py` & `elias-0.2.2/src/elias/data/combined.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/data/loader.py` & `elias-0.2.2/src/elias/data/loader.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/data/sampling.py` & `elias-0.2.2/src/elias/data/sampling.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/data/stop_criterion.py` & `elias-0.2.2/src/elias/data/stop_criterion.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/folder/analysis.py` & `elias-0.2.2/src/elias/folder/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/folder/data.py` & `elias-0.2.2/src/elias/folder/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/folder/folder.py` & `elias-0.2.2/src/elias/folder/folder.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/folder/model.py` & `elias-0.2.2/src/elias/folder/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/folder/run.py` & `elias-0.2.2/src/elias/folder/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/manager/analysis.py` & `elias-0.2.2/src/elias/manager/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/manager/artifact.py` & `elias-0.2.2/src/elias/manager/artifact.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/manager/buffered.py` & `elias-0.2.2/src/elias/manager/buffered.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/manager/data.py` & `elias-0.2.2/src/elias/manager/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/manager/model.py` & `elias-0.2.2/src/elias/manager/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/manager/run.py` & `elias-0.2.2/src/elias/manager/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/util/fs.py` & `elias-0.2.2/src/elias/util/fs.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/util/io.py` & `elias-0.2.2/src/elias/util/io.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/util/range.py` & `elias-0.2.2/src/elias/util/range.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/util/timing.py` & `elias-0.2.2/src/elias/util/timing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias/util/version.py` & `elias-0.2.2/src/elias/util/version.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.1/src/elias.egg-info/PKG-INFO` & `elias-0.2.2/src/elias.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.1
+Version: 0.2.2
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.1/src/elias.egg-info/SOURCES.txt` & `elias-0.2.2/src/elias.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,11 +27,12 @@
 src/elias/manager/buffered.py
 src/elias/manager/data.py
 src/elias/manager/model.py
 src/elias/manager/run.py
 src/elias/util/__init__.py
 src/elias/util/fs.py
 src/elias/util/io.py
+src/elias/util/random.py
 src/elias/util/range.py
 src/elias/util/timing.py
 src/elias/util/typing.py
 src/elias/util/version.py
```

