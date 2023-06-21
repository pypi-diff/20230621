# Comparing `tmp/bantam-2.4.3.tar.gz` & `tmp/bantam-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.4.3.tar", last modified: Wed Jun 21 04:42:10 2023, max compression
+gzip compressed data, was "bantam-2.4.4.tar", last modified: Wed Jun 21 04:49:35 2023, max compression
```

## Comparing `bantam-2.4.3.tar` & `bantam-2.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:42:10.512422 bantam-2.4.3/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.3/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.3/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-21 04:42:10.512422 bantam-2.4.3/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-21 04:41:13.000000 bantam-2.4.3/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.508422 bantam-2.4.3/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.3/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.3/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.3/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.3/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22873 2023-06-21 04:39:45.000000 bantam-2.4.3/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.3/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.3/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    50578 2023-06-21 03:43:56.000000 bantam-2.4.3/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.3/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.3/src/bantam/js_async.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     5623 2023-06-21 04:28:06.000000 bantam-2.4.3/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.3/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.3/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.3/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.3/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.3/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.3/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.3/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.310540 bantam-2.4.4/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:49:35.310540 bantam-2.4.4/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.4/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.4/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-21 04:49:35.310540 bantam-2.4.4/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-21 04:49:13.000000 bantam-2.4.4/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.4/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.4/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.4/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.4/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22978 2023-06-21 04:48:21.000000 bantam-2.4.4/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.4/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.4/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    50578 2023-06-21 03:43:56.000000 bantam-2.4.4/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.4/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.4/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.310540 bantam-2.4.4/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5623 2023-06-21 04:28:06.000000 bantam-2.4.4/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.4/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.4/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.4/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.4/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.4/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.4/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.4/test/test_js_async.py
```

### Comparing `bantam-2.4.3/PKG-INFO` & `bantam-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.3
+Version: 2.4.4
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.3
+Download-URL: https://github.com/bantam/dist/2.4.4
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.3/setup.py` & `bantam-2.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.4.3"
+VERSION = "2.4.4"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.4.3/src/bantam/__init__.py` & `bantam-2.4.4/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam/api.py` & `bantam-2.4.4/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam/autogen/main.py` & `bantam-2.4.4/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam/client.py` & `bantam-2.4.4/src/bantam/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,20 @@
 C = TypeVar('C', bound="WebInterface")
 
 
 class InvocationError(Exception):
     def __init__(self, message: str):
         self.message = message
 
+    def __str__(self):
+        return self.message
+
+    def __repr__(self):
+        return self.message
+
 
 # noinspection PyProtectedMember
 class WebInterface(ABC):
 
     _clients: Dict[str, Any] = {}
 
     @classmethod
```

### Comparing `bantam-2.4.3/src/bantam/conversions.py` & `bantam-2.4.4/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam/decorators.py` & `bantam-2.4.4/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam/http.py` & `bantam-2.4.4/src/bantam/http.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam/js.py` & `bantam-2.4.4/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam/js_async.py` & `bantam-2.4.4/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.4/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.3
+Version: 2.4.4
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.3
+Download-URL: https://github.com/bantam/dist/2.4.4
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.3/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.4/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/test/test_client_get.py` & `bantam-2.4.4/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/test/test_client_post.py` & `bantam-2.4.4/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/test/test_client_post_inherited_apis.py` & `bantam-2.4.4/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/test/test_conversions.py` & `bantam-2.4.4/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/test/test_decorators.py` & `bantam-2.4.4/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/test/test_js.py` & `bantam-2.4.4/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.3/test/test_js_async.py` & `bantam-2.4.4/test/test_js_async.py`

 * *Files identical despite different names*

