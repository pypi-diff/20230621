# Comparing `tmp/AdyanUtils-0.6.3.tar.gz` & `tmp/AdyanUtils-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdyanUtils-0.6.3.tar", last modified: Wed Jun 21 04:36:06 2023, max compression
+gzip compressed data, was "AdyanUtils-0.6.4.tar", last modified: Wed Jun 21 04:38:45 2023, max compression
```

## Comparing `AdyanUtils-0.6.3.tar` & `AdyanUtils-0.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 04:36:06.014901 AdyanUtils-0.6.3/
-drwxrwxrwx   0        0        0        0 2023-06-21 04:36:05.930302 AdyanUtils-0.6.3/AdyanUtils.egg-info/
--rw-rw-rw-   0        0        0     1831 2023-06-21 04:36:05.000000 AdyanUtils-0.6.3/AdyanUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-06-21 04:36:05.000000 AdyanUtils-0.6.3/AdyanUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 04:36:05.000000 AdyanUtils-0.6.3/AdyanUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2023-06-21 04:36:05.000000 AdyanUtils-0.6.3/AdyanUtils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-21 04:36:05.000000 AdyanUtils-0.6.3/AdyanUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-04-12 02:49:17.000000 AdyanUtils-0.6.3/LICENSE
--rw-rw-rw-   0        0        0     1831 2023-06-21 04:36:06.013895 AdyanUtils-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1410 2022-04-12 02:49:17.000000 AdyanUtils-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 04:36:05.931293 AdyanUtils-0.6.3/Utils/
--rw-rw-rw-   0        0        0      563 2022-04-27 01:17:08.000000 AdyanUtils-0.6.3/Utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 04:36:06.004897 AdyanUtils-0.6.3/Utils/connect/
--rw-rw-rw-   0        0        0      131 2022-04-27 01:21:59.000000 AdyanUtils-0.6.3/Utils/connect/__init__.py
--rw-rw-rw-   0        0        0     3920 2022-08-08 02:33:20.000000 AdyanUtils-0.6.3/Utils/connect/mongo_conn.py
--rw-rw-rw-   0        0        0     3806 2022-08-10 02:25:33.000000 AdyanUtils-0.6.3/Utils/connect/rabbit_conn.py
--rw-rw-rw-   0        0        0     4497 2022-09-22 08:56:08.000000 AdyanUtils-0.6.3/Utils/connect/redis_conn.py
-drwxrwxrwx   0        0        0        0 2023-06-21 04:36:06.012894 AdyanUtils-0.6.3/Utils/crawler/
--rw-rw-rw-   0        0        0     4687 2023-06-19 08:39:04.000000 AdyanUtils-0.6.3/Utils/crawler/Forge.py
--rw-rw-rw-   0        0        0      131 2022-04-27 01:17:08.000000 AdyanUtils-0.6.3/Utils/crawler/__init__.py
--rw-rw-rw-   0        0        0     4696 2022-09-07 06:52:36.000000 AdyanUtils-0.6.3/Utils/crawler/function.py
--rw-rw-rw-   0        0        0     2749 2022-06-25 01:26:17.000000 AdyanUtils-0.6.3/Utils/crawler/init.py
--rw-rw-rw-   0        0        0     4269 2022-07-29 05:02:05.000000 AdyanUtils-0.6.3/Utils/crawler/middleware.py
--rw-rw-rw-   0        0        0     5260 2022-04-12 02:49:17.000000 AdyanUtils-0.6.3/Utils/crawler/proxy.py
--rw-rw-rw-   0        0        0     1510 2022-04-27 01:08:27.000000 AdyanUtils-0.6.3/Utils/crawler/save_xls.py
--rw-rw-rw-   0        0        0     1641 2022-04-27 01:08:33.000000 AdyanUtils-0.6.3/Utils/crawler/scheduler.py
--rw-rw-rw-   0        0        0      108 2022-04-12 02:49:17.000000 AdyanUtils-0.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 04:36:06.014901 AdyanUtils-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-19 08:39:48.000000 AdyanUtils-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:38:45.872756 AdyanUtils-0.6.4/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:38:45.855753 AdyanUtils-0.6.4/AdyanUtils.egg-info/
+-rw-rw-rw-   0        0        0     1831 2023-06-21 04:38:45.000000 AdyanUtils-0.6.4/AdyanUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-06-21 04:38:45.000000 AdyanUtils-0.6.4/AdyanUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 04:38:45.000000 AdyanUtils-0.6.4/AdyanUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2023-06-21 04:38:45.000000 AdyanUtils-0.6.4/AdyanUtils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-21 04:38:45.000000 AdyanUtils-0.6.4/AdyanUtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-04-12 02:49:17.000000 AdyanUtils-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0     1831 2023-06-21 04:38:45.871756 AdyanUtils-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1410 2022-04-12 02:49:17.000000 AdyanUtils-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 04:38:45.856752 AdyanUtils-0.6.4/Utils/
+-rw-rw-rw-   0        0        0      563 2022-04-27 01:17:08.000000 AdyanUtils-0.6.4/Utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:38:45.860753 AdyanUtils-0.6.4/Utils/connect/
+-rw-rw-rw-   0        0        0      131 2022-04-27 01:21:59.000000 AdyanUtils-0.6.4/Utils/connect/__init__.py
+-rw-rw-rw-   0        0        0     3978 2023-06-21 04:37:58.000000 AdyanUtils-0.6.4/Utils/connect/mongo_conn.py
+-rw-rw-rw-   0        0        0     3806 2022-08-10 02:25:33.000000 AdyanUtils-0.6.4/Utils/connect/rabbit_conn.py
+-rw-rw-rw-   0        0        0     4497 2022-09-22 08:56:08.000000 AdyanUtils-0.6.4/Utils/connect/redis_conn.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:38:45.870754 AdyanUtils-0.6.4/Utils/crawler/
+-rw-rw-rw-   0        0        0     4687 2023-06-19 08:39:04.000000 AdyanUtils-0.6.4/Utils/crawler/Forge.py
+-rw-rw-rw-   0        0        0      131 2022-04-27 01:17:08.000000 AdyanUtils-0.6.4/Utils/crawler/__init__.py
+-rw-rw-rw-   0        0        0     4696 2022-09-07 06:52:36.000000 AdyanUtils-0.6.4/Utils/crawler/function.py
+-rw-rw-rw-   0        0        0     2749 2022-06-25 01:26:17.000000 AdyanUtils-0.6.4/Utils/crawler/init.py
+-rw-rw-rw-   0        0        0     4269 2022-07-29 05:02:05.000000 AdyanUtils-0.6.4/Utils/crawler/middleware.py
+-rw-rw-rw-   0        0        0     5260 2022-04-12 02:49:17.000000 AdyanUtils-0.6.4/Utils/crawler/proxy.py
+-rw-rw-rw-   0        0        0     1510 2022-04-27 01:08:27.000000 AdyanUtils-0.6.4/Utils/crawler/save_xls.py
+-rw-rw-rw-   0        0        0     1641 2022-04-27 01:08:33.000000 AdyanUtils-0.6.4/Utils/crawler/scheduler.py
+-rw-rw-rw-   0        0        0      108 2022-04-12 02:49:17.000000 AdyanUtils-0.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 04:38:45.872756 AdyanUtils-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-21 04:38:05.000000 AdyanUtils-0.6.4/setup.py
```

### Comparing `AdyanUtils-0.6.3/AdyanUtils.egg-info/PKG-INFO` & `AdyanUtils-0.6.4/AdyanUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdyanUtils
-Version: 0.6.3
+Version: 0.6.4
 Summary: Special package
 Home-page: https://gitee.com/liujiang99/AdyanUtils
 Author: Adyan
 Author-email: 228923910@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AdyanUtils-0.6.3/AdyanUtils.egg-info/SOURCES.txt` & `AdyanUtils-0.6.4/AdyanUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/LICENSE` & `AdyanUtils-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/PKG-INFO` & `AdyanUtils-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdyanUtils
-Version: 0.6.3
+Version: 0.6.4
 Summary: Special package
 Home-page: https://gitee.com/liujiang99/AdyanUtils
 Author: Adyan
 Author-email: 228923910@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AdyanUtils-0.6.3/README.md` & `AdyanUtils-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/__init__.py` & `AdyanUtils-0.6.4/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/connect/mongo_conn.py` & `AdyanUtils-0.6.4/Utils/connect/mongo_conn.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,15 +69,18 @@
             self.collection.update(dic, {"$set": item}, upsert=True)
 
     def insert_one(self, param):
         """
         :param param: 多条list 或者 单条dict
         :return:
         """
-        self.collection.insert(param)
+        try:
+            self.collection.insert_many(param)
+        except:
+            pass
 
     def find_len(self, dic=None):
         if dic:
             return self.collection.find(dic).count()
         return self.collection.find().count()
 
     def find_one(self):
```

### Comparing `AdyanUtils-0.6.3/Utils/connect/rabbit_conn.py` & `AdyanUtils-0.6.4/Utils/connect/rabbit_conn.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/connect/redis_conn.py` & `AdyanUtils-0.6.4/Utils/connect/redis_conn.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/crawler/Forge.py` & `AdyanUtils-0.6.4/Utils/crawler/Forge.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/crawler/function.py` & `AdyanUtils-0.6.4/Utils/crawler/function.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/crawler/init.py` & `AdyanUtils-0.6.4/Utils/crawler/init.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/crawler/middleware.py` & `AdyanUtils-0.6.4/Utils/crawler/middleware.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/crawler/proxy.py` & `AdyanUtils-0.6.4/Utils/crawler/proxy.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/crawler/save_xls.py` & `AdyanUtils-0.6.4/Utils/crawler/save_xls.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/Utils/crawler/scheduler.py` & `AdyanUtils-0.6.4/Utils/crawler/scheduler.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.3/setup.py` & `AdyanUtils-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AdyanUtils",
-    version="0.6.3",
+    version="0.6.4",
     author="Adyan",
     author_email="228923910@qq.com",
     description="Special package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/liujiang99/AdyanUtils",
     packages=setuptools.find_packages(),
```

