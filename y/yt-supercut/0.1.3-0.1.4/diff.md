# Comparing `tmp/yt_supercut-0.1.3.tar.gz` & `tmp/yt_supercut-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_supercut-0.1.3.tar", max compression
+gzip compressed data, was "yt_supercut-0.1.4.tar", max compression
```

## Comparing `yt_supercut-0.1.3.tar` & `yt_supercut-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       14 2023-05-29 21:15:44.453273 yt_supercut-0.1.3/README.md
--rw-r--r--   0        0        0      702 2023-06-21 20:18:44.447684 yt_supercut-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6072 2023-06-19 02:56:18.515490 yt_supercut-0.1.3/yt_supercut/db.py
--rw-r--r--   0        0        0     3813 2023-06-21 19:47:48.838530 yt_supercut-0.1.3/yt_supercut/main.py
--rw-r--r--   0        0        0     4206 2023-06-21 20:10:07.117721 yt_supercut-0.1.3/yt_supercut/utils.py
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 yt_supercut-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-05-29 21:15:44.453273 yt_supercut-0.1.4/README.md
+-rw-r--r--   0        0        0      702 2023-06-21 20:26:25.920750 yt_supercut-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6072 2023-06-19 02:56:18.515490 yt_supercut-0.1.4/yt_supercut/db.py
+-rw-r--r--   0        0        0     3813 2023-06-21 19:47:48.838530 yt_supercut-0.1.4/yt_supercut/main.py
+-rw-r--r--   0        0        0     4202 2023-06-21 20:26:13.543789 yt_supercut-0.1.4/yt_supercut/utils.py
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 yt_supercut-0.1.4/PKG-INFO
```

### Comparing `yt_supercut-0.1.3/pyproject.toml` & `yt_supercut-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yt-supercut"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["redraw <redraw@sdf.org>"]
 readme = "README.md"
 packages = [{include = "yt_supercut"}]
 
 [tool.poetry.scripts]
 yt-supercut = "yt_supercut.main:cli"
```

### Comparing `yt_supercut-0.1.3/yt_supercut/db.py` & `yt_supercut-0.1.4/yt_supercut/db.py`

 * *Files identical despite different names*

### Comparing `yt_supercut-0.1.3/yt_supercut/main.py` & `yt_supercut-0.1.4/yt_supercut/main.py`

 * *Files identical despite different names*

### Comparing `yt_supercut-0.1.3/yt_supercut/utils.py` & `yt_supercut-0.1.4/yt_supercut/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import webvtt
 import appdirs
 from yt_dlp import YoutubeDL
 from yt_dlp.utils import download_range_func, ExistingVideoReached
 from . import db
 
 
-CONFIG_DIR = appdirs.user_config_dir("yt_supercut")
-Path(CONFIG_DIR).mkdir(parents=True, exist_ok=True)
+CACHE_DIR = appdirs.user_cache_dir("yt_supercut")
+Path(CACHE_DIR).mkdir(parents=True, exist_ok=True)
 
 
 def get_video_ids(url, cookies_from=None, lang=None, verbose=True):
     stripped_url = re.sub(r'[^\w]', '_', url)
-    archive_path = Path(CONFIG_DIR) / f"{stripped_url}.{lang}.txt"
+    archive_path = Path(CACHE_DIR) / f"{stripped_url}.{lang}.txt"
 
     opts = {
         "skipdownload": True,
         "no_warnings": True,
         "noprogress": True,
         "dumpjson": True,
         "quiet": not verbose,
```

### Comparing `yt_supercut-0.1.3/PKG-INFO` & `yt_supercut-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-supercut
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: redraw
 Author-email: redraw@sdf.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

