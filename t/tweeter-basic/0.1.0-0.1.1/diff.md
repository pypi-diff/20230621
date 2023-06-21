# Comparing `tmp/tweeter-basic-0.1.0.tar.gz` & `tmp/tweeter-basic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeter-basic-0.1.0.tar", last modified: Wed Jun 21 04:05:34 2023, max compression
+gzip compressed data, was "tweeter-basic-0.1.1.tar", last modified: Wed Jun 21 04:42:42 2023, max compression
```

## Comparing `tweeter-basic-0.1.0.tar` & `tweeter-basic-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:05:34.265365 tweeter-basic-0.1.0/
--rw-r--r--   0 mike      (1000) mike      (1000)     3672 2023-06-21 04:05:34.265365 tweeter-basic-0.1.0/PKG-INFO
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:05:34.255365 tweeter-basic-0.1.0/Tweet/
--rw-r--r--   0 mike      (1000) mike      (1000)     2431 2023-06-21 03:20:30.000000 tweeter-basic-0.1.0/Tweet/Tweet.py
--rw-r--r--   0 mike      (1000) mike      (1000)       21 2023-06-21 01:56:53.000000 tweeter-basic-0.1.0/Tweet/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)      218 2023-06-20 04:17:23.000000 tweeter-basic-0.1.0/Tweet/file.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3731 2023-06-21 03:25:18.000000 tweeter-basic-0.1.0/Tweet/upload.py
--rw-r--r--   0 mike      (1000) mike      (1000)       38 2023-06-21 04:05:34.265365 tweeter-basic-0.1.0/setup.cfg
--rw-r--r--   0 mike      (1000) mike      (1000)     1140 2023-06-21 04:05:29.000000 tweeter-basic-0.1.0/setup.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:05:34.255365 tweeter-basic-0.1.0/test/
--rw-r--r--   0 mike      (1000) mike      (1000)      373 2023-06-21 01:58:55.000000 tweeter-basic-0.1.0/test/test.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:05:34.265365 tweeter-basic-0.1.0/tweeter_basic.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     3672 2023-06-21 04:05:34.000000 tweeter-basic-0.1.0/tweeter_basic.egg-info/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)      268 2023-06-21 04:05:34.000000 tweeter-basic-0.1.0/tweeter_basic.egg-info/SOURCES.txt
--rw-r--r--   0 mike      (1000) mike      (1000)        1 2023-06-21 04:05:34.000000 tweeter-basic-0.1.0/tweeter_basic.egg-info/dependency_links.txt
--rw-r--r--   0 mike      (1000) mike      (1000)       33 2023-06-21 04:05:34.000000 tweeter-basic-0.1.0/tweeter_basic.egg-info/requires.txt
--rw-r--r--   0 mike      (1000) mike      (1000)        6 2023-06-21 04:05:34.000000 tweeter-basic-0.1.0/tweeter_basic.egg-info/top_level.txt
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:42:42.088356 tweeter-basic-0.1.1/
+-rw-r--r--   0 mike      (1000) mike      (1000)     3687 2023-06-21 04:42:42.088356 tweeter-basic-0.1.1/PKG-INFO
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:42:42.088356 tweeter-basic-0.1.1/Tweet/
+-rw-r--r--   0 mike      (1000) mike      (1000)     2433 2023-06-21 04:42:04.000000 tweeter-basic-0.1.1/Tweet/Tweet.py
+-rw-r--r--   0 mike      (1000) mike      (1000)       21 2023-06-21 01:56:53.000000 tweeter-basic-0.1.1/Tweet/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      218 2023-06-20 04:17:23.000000 tweeter-basic-0.1.1/Tweet/file.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3731 2023-06-21 03:25:18.000000 tweeter-basic-0.1.1/Tweet/upload.py
+-rw-r--r--   0 mike      (1000) mike      (1000)       38 2023-06-21 04:42:42.098357 tweeter-basic-0.1.1/setup.cfg
+-rw-r--r--   0 mike      (1000) mike      (1000)     1140 2023-06-21 04:42:34.000000 tweeter-basic-0.1.1/setup.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:42:42.088356 tweeter-basic-0.1.1/test/
+-rw-r--r--   0 mike      (1000) mike      (1000)      373 2023-06-21 01:58:55.000000 tweeter-basic-0.1.1/test/test.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-21 04:42:42.088356 tweeter-basic-0.1.1/tweeter_basic.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     3687 2023-06-21 04:42:41.000000 tweeter-basic-0.1.1/tweeter_basic.egg-info/PKG-INFO
+-rw-r--r--   0 mike      (1000) mike      (1000)      268 2023-06-21 04:42:42.000000 tweeter-basic-0.1.1/tweeter_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)        1 2023-06-21 04:42:41.000000 tweeter-basic-0.1.1/tweeter_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)       33 2023-06-21 04:42:41.000000 tweeter-basic-0.1.1/tweeter_basic.egg-info/requires.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)        6 2023-06-21 04:42:41.000000 tweeter-basic-0.1.1/tweeter_basic.egg-info/top_level.txt
```

### Comparing `tweeter-basic-0.1.0/PKG-INFO` & `tweeter-basic-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeter-basic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Send tweets (with optional images) through the Twitter v2 API (OAuth 2.0) - authentication included
 Home-page: https://mike.busuttil.ca/
 Author: Mike Busuttil
 Author-email: mike@busuttil.ca
 License: MIT
 Description: # Tweeter Basic
         
@@ -32,16 +32,16 @@
         - Docker engine
         - Twitter project with: 
           - v1.1 API read & write access
           - v2 API access
         
         ## 2do
         
-        - create PyPI entry
         - give a more verbose explanation of the steps
+        - write separate PyPI instructions
         
         ### future
         
         - add geolocation to tweets:
           - try posting with the v1 API instead of v2:
             - https://developer.twitter.com/en/docs/twitter-api/v1/tweets/post-and-engage/api-reference/post-statuses-update
             - using this format: https://en.wikipedia.org/wiki/GeoJSON
```

### Comparing `tweeter-basic-0.1.0/Tweet/Tweet.py` & `tweeter-basic-0.1.1/Tweet/Tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from requests_oauthlib import OAuth2Session
 import json
 from requests import post
-from upload import TwitterMedia
-from file import read, write
+from .upload import TwitterMedia
+from .file import read, write
 
 def print_response(r):
     if 'application/json' in r.headers.get('Content-Type', ''):
         return json.dumps(r.json(), indent=2)
     return r.text
 
 class Tweet:
```

### Comparing `tweeter-basic-0.1.0/Tweet/upload.py` & `tweeter-basic-0.1.1/Tweet/upload.py`

 * *Files identical despite different names*

### Comparing `tweeter-basic-0.1.0/setup.py` & `tweeter-basic-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'tweeter-basic',
     description = 'Send tweets (with optional images) through the Twitter v2 API (OAuth 2.0) - authentication included',
-    version = '0.1.0',
+    version = '0.1.1',
     license = 'MIT',
     url = 'https://mike.busuttil.ca/',
     install_requires =['flask', 'requests', 'requests-oauthlib'],
     packages = find_packages(),
     long_description = open('readme.md', encoding='utf-8').read(),
     long_description_content_type = 'text/markdown',
     author = 'Mike Busuttil',
```

### Comparing `tweeter-basic-0.1.0/tweeter_basic.egg-info/PKG-INFO` & `tweeter-basic-0.1.1/tweeter_basic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeter-basic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Send tweets (with optional images) through the Twitter v2 API (OAuth 2.0) - authentication included
 Home-page: https://mike.busuttil.ca/
 Author: Mike Busuttil
 Author-email: mike@busuttil.ca
 License: MIT
 Description: # Tweeter Basic
         
@@ -32,16 +32,16 @@
         - Docker engine
         - Twitter project with: 
           - v1.1 API read & write access
           - v2 API access
         
         ## 2do
         
-        - create PyPI entry
         - give a more verbose explanation of the steps
+        - write separate PyPI instructions
         
         ### future
         
         - add geolocation to tweets:
           - try posting with the v1 API instead of v2:
             - https://developer.twitter.com/en/docs/twitter-api/v1/tweets/post-and-engage/api-reference/post-statuses-update
             - using this format: https://en.wikipedia.org/wiki/GeoJSON
```

