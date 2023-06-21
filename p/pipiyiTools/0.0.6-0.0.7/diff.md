# Comparing `tmp/pipiyiTools-0.0.6.tar.gz` & `tmp/pipiyiTools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipiyiTools-0.0.6.tar", last modified: Wed Jun 21 14:36:41 2023, max compression
+gzip compressed data, was "dist/pipiyiTools-0.0.7.tar", last modified: Wed Jun 21 15:04:35 2023, max compression
```

## Comparing `pipiyiTools-0.0.6.tar` & `pipiyiTools-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      314 2023-06-06 08:59:34.000000 pipiyiTools-0.0.6/README.md
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/pipiyiTools/
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyiTools-0.0.6/pipiyiTools/EpubSpliter.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyiTools-0.0.6/pipiyiTools/FileOperation.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1385 2023-06-06 09:02:18.000000 pipiyiTools-0.0.6/pipiyiTools/ListQueue.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1918 2023-06-12 14:17:44.000000 pipiyiTools-0.0.6/pipiyiTools/Log.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2142 2023-06-21 14:36:05.000000 pipiyiTools-0.0.6/pipiyiTools/MyRequest.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyiTools-0.0.6/pipiyiTools/PooledBase.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyiTools-0.0.6/pipiyiTools/Storage.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:06:54.000000 pipiyiTools-0.0.6/pipiyiTools/__init__.py
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/pipiyiTools.egg-info/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/pipiyiTools.egg-info/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      390 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/pipiyiTools.egg-info/SOURCES.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/pipiyiTools.egg-info/dependency_links.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/pipiyiTools.egg-info/requires.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       12 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/pipiyiTools.egg-info/top_level.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-06-21 14:36:41.000000 pipiyiTools-0.0.6/setup.cfg
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1005 2023-06-21 14:36:22.000000 pipiyiTools-0.0.6/setup.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      314 2023-06-06 08:59:34.000000 pipiyiTools-0.0.7/README.md
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/pipiyiTools/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyiTools-0.0.7/pipiyiTools/EpubSpliter.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyiTools-0.0.7/pipiyiTools/FileOperation.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1385 2023-06-06 09:02:18.000000 pipiyiTools-0.0.7/pipiyiTools/ListQueue.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1918 2023-06-12 14:17:44.000000 pipiyiTools-0.0.7/pipiyiTools/Log.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2140 2023-06-21 15:04:08.000000 pipiyiTools-0.0.7/pipiyiTools/MyRequest.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyiTools-0.0.7/pipiyiTools/PooledBase.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyiTools-0.0.7/pipiyiTools/Storage.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:06:54.000000 pipiyiTools-0.0.7/pipiyiTools/__init__.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/pipiyiTools.egg-info/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/pipiyiTools.egg-info/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      390 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/pipiyiTools.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/pipiyiTools.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/pipiyiTools.egg-info/requires.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       12 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/pipiyiTools.egg-info/top_level.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-06-21 15:04:35.000000 pipiyiTools-0.0.7/setup.cfg
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1005 2023-06-21 15:04:18.000000 pipiyiTools-0.0.7/setup.py
```

### Comparing `pipiyiTools-0.0.6/PKG-INFO` & `pipiyiTools-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipiyiTools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
```

### Comparing `pipiyiTools-0.0.6/pipiyiTools/EpubSpliter.py` & `pipiyiTools-0.0.7/pipiyiTools/EpubSpliter.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.6/pipiyiTools/FileOperation.py` & `pipiyiTools-0.0.7/pipiyiTools/FileOperation.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.6/pipiyiTools/ListQueue.py` & `pipiyiTools-0.0.7/pipiyiTools/ListQueue.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.6/pipiyiTools/Log.py` & `pipiyiTools-0.0.7/pipiyiTools/Log.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.6/pipiyiTools/MyRequest.py` & `pipiyiTools-0.0.7/pipiyiTools/MyRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,12 +44,12 @@
         except requests.RequestException as e:
             self.log.error(f"{method} request error: {e}, URL:{url}")
             return False
         except Exception as e:
             self.log.error(f"{method} request Exception Error: {e}, URL:{url}")
             return False
 
-    def get(self, url, params=None, headers=None, timeout=5, verify=False):
+    def get(self, url, params=None, headers=None, timeout=5, verify=True):
         return self.request("GET", url, params=params, headers=headers, timeout=timeout)
 
-    def post(self, url, data=None, headers=None, timeout=5, verify=False):
+    def post(self, url, data=None, headers=None, timeout=5, verify=True):
         return self.request("POST", url, data=data, headers=headers, timeout=timeout)
```

### Comparing `pipiyiTools-0.0.6/pipiyiTools/PooledBase.py` & `pipiyiTools-0.0.7/pipiyiTools/PooledBase.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.6/pipiyiTools/Storage.py` & `pipiyiTools-0.0.7/pipiyiTools/Storage.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.6/pipiyiTools.egg-info/PKG-INFO` & `pipiyiTools-0.0.7/pipiyiTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipiyiTools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
```

### Comparing `pipiyiTools-0.0.6/setup.py` & `pipiyiTools-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "Personal tool library"
 
 # Setting up
 setup(
     name="pipiyiTools",
     version=VERSION,
     author="pipiyi",
```

