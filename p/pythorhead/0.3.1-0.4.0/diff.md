# Comparing `tmp/pythorhead-0.3.1.tar.gz` & `tmp/pythorhead-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.3.1.tar", last modified: Tue Jun 20 14:13:22 2023, max compression
+gzip compressed data, was "pythorhead-0.4.0.tar", last modified: Wed Jun 21 00:05:55 2023, max compression
```

## Comparing `pythorhead-0.3.1.tar` & `pythorhead-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:13:22.795829 pythorhead-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:13:22.791829 pythorhead-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:13:22.791829 pythorhead-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-20 14:13:03.000000 pythorhead-0.3.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-20 14:13:03.000000 pythorhead-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-20 14:13:10.000000 pythorhead-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 14:13:03.000000 pythorhead-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-20 14:13:22.795829 pythorhead-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-20 14:13:03.000000 pythorhead-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-20 14:13:03.000000 pythorhead-0.3.1/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-20 14:13:10.000000 pythorhead-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:13:22.791829 pythorhead-0.3.1/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:13:22.795829 pythorhead-0.3.1/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 14:13:03.000000 pythorhead-0.3.1/pythorhead/types/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:13:22.795829 pythorhead-0.3.1/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-20 14:13:22.000000 pythorhead-0.3.1/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 14:13:22.000000 pythorhead-0.3.1/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:13:22.000000 pythorhead-0.3.1/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 14:13:22.000000 pythorhead-0.3.1/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:13:03.000000 pythorhead-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:13:22.795829 pythorhead-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:05:55.586688 pythorhead-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:05:55.582688 pythorhead-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:05:55.586688 pythorhead-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-21 00:05:36.000000 pythorhead-0.4.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-21 00:05:36.000000 pythorhead-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-21 00:05:43.000000 pythorhead-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-21 00:05:36.000000 pythorhead-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-21 00:05:55.586688 pythorhead-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-21 00:05:36.000000 pythorhead-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-21 00:05:36.000000 pythorhead-0.4.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-21 00:05:43.000000 pythorhead-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:05:55.586688 pythorhead-0.4.0/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:05:55.586688 pythorhead-0.4.0/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 00:05:36.000000 pythorhead-0.4.0/pythorhead/types/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:05:55.586688 pythorhead-0.4.0/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-21 00:05:55.000000 pythorhead-0.4.0/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 00:05:55.000000 pythorhead-0.4.0/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:05:55.000000 pythorhead-0.4.0/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 00:05:55.000000 pythorhead-0.4.0/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:05:36.000000 pythorhead-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:05:55.586688 pythorhead-0.4.0/setup.cfg
```

### Comparing `pythorhead-0.3.1/.github/workflows/pypi.yml` & `pythorhead-0.4.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/.gitignore` & `pythorhead-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/CHANGELOG.md` & `pythorhead-0.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [v0.4.0](https://github.com/db0/pythorhead/tree/v0.4.0) (2023-06-21)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.3.1...v0.4.0)
+
+**Merged pull requests:**
+
+- feat: Added site [\#13](https://github.com/db0/pythorhead/pull/13) ([db0](https://github.com/db0))
+
 ## [v0.3.1](https://github.com/db0/pythorhead/tree/v0.3.1) (2023-06-20)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.3.0...v0.3.1)
 
 **Merged pull requests:**
 
 - Moderator remove and fix error in comments list [\#12](https://github.com/db0/pythorhead/pull/12) ([NicKoehler](https://github.com/NicKoehler))
```

### Comparing `pythorhead-0.3.1/LICENSE` & `pythorhead-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/PKG-INFO` & `pythorhead-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.3.1
+Version: 0.4.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.3.1/README.md` & `pythorhead-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/logo.png` & `pythorhead-0.4.0/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/pyproject.toml` & `pythorhead-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.3.1"
+version = "v0.4.0"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.3.1/pythorhead/auth.py` & `pythorhead-0.4.0/pythorhead/auth.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/pythorhead/comment.py` & `pythorhead-0.4.0/pythorhead/comment.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/pythorhead/lemmy.py` & `pythorhead-0.4.0/pythorhead/lemmy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import Optional
 
 from pythorhead.comment import Comment
 from pythorhead.post import Post
+from pythorhead.site import Site
 from pythorhead.requestor import Request, Requestor
 
 logging.basicConfig(format="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
 
 class Lemmy:
     post: Post
@@ -15,14 +16,15 @@
     _requestor: Requestor
 
     def __init__(self, api_base_url: str) -> None:
         self._requestor = Requestor()
         self._requestor.set_api_base_url(f"{api_base_url}/api/v3")
         self.post = Post()
         self.comment = Comment()
+        self.site = Site()
 
     def log_in(self, username_or_email: str, password: str) -> bool:
         return self._requestor.log_in(username_or_email, password)
 
     def discover_community(self, community_name: str) -> Optional[int]:
         if community_name in self._known_communities:
             return self._known_communities[community_name]
```

### Comparing `pythorhead-0.3.1/pythorhead/post.py` & `pythorhead-0.4.0/pythorhead/post.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/pythorhead/requestor.py` & `pythorhead-0.4.0/pythorhead/requestor.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.3.1/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.4.0/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.3.1
+Version: 0.4.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

