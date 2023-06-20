# Comparing `tmp/coinpaprika_async-3.0.1.tar.gz` & `tmp/coinpaprika_async-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinpaprika_async-3.0.1.tar", last modified: Tue Jun 20 21:40:33 2023, max compression
+gzip compressed data, was "coinpaprika_async-3.0.2.tar", last modified: Tue Jun 20 23:41:22 2023, max compression
```

## Comparing `coinpaprika_async-3.0.1.tar` & `coinpaprika_async-3.0.2.tar`

### file list

```diff
@@ -1,22 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.905603 coinpaprika_async-3.0.1/
--rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.1/LICENSE
--rw-rw-rw-   0        0        0     2169 2023-06-20 21:40:33.905603 coinpaprika_async-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.861601 coinpaprika_async-3.0.1/coinpaprika_async/
--rw-rw-rw-   0        0        0      449 2023-06-20 21:32:25.000000 coinpaprika_async-3.0.1/coinpaprika_async/__init__.py
--rw-rw-rw-   0        0        0      125 2023-06-20 21:38:00.000000 coinpaprika_async-3.0.1/coinpaprika_async/_version__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.893603 coinpaprika_async-3.0.1/coinpaprika_async/api/
--rw-rw-rw-   0        0        0      245 2023-06-20 18:10:10.000000 coinpaprika_async-3.0.1/coinpaprika_async/api/__init__.py
--rw-rw-rw-   0        0        0      235 2023-06-18 16:35:59.000000 coinpaprika_async-3.0.1/coinpaprika_async/api/coinpaprika_api.py
--rw-rw-rw-   0        0        0     1314 2023-06-20 21:30:06.000000 coinpaprika_async-3.0.1/coinpaprika_async/coinpaprika_async_client.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.888602 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/
--rw-rw-rw-   0        0        0     2169 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      139 2023-06-20 21:40:33.907609 coinpaprika_async-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      899 2023-06-20 21:37:54.000000 coinpaprika_async-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.902600 coinpaprika_async-3.0.1/tests/
--rw-rw-rw-   0        0        0     1893 2023-06-20 18:16:17.000000 coinpaprika_async-3.0.1/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:22.070850 coinpaprika_async-3.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2169 2023-06-20 23:41:22.070850 coinpaprika_async-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.2/README.md
+-rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-3.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      139 2023-06-20 23:41:22.072852 coinpaprika_async-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-06-20 23:40:59.000000 coinpaprika_async-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.697865 coinpaprika_async-3.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.775852 coinpaprika_async-3.0.2/src/coinpaprika_async/
+-rw-rw-rw-   0        0        0      481 2023-06-20 23:37:28.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/__init__.py
+-rw-rw-rw-   0        0        0      125 2023-06-20 21:46:00.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/_version__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.843851 coinpaprika_async-3.0.2/src/coinpaprika_async/api/
+-rw-rw-rw-   0        0        0      245 2023-06-20 18:10:10.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-18 16:35:59.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coinpaprika_api.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.849850 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/__init__.py
+-rw-rw-rw-   0        0        0     3882 2023-06-20 19:23:07.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/api.py
+-rw-rw-rw-   0        0        0     3033 2023-06-20 18:29:31.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.859854 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:33:51.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/__init__.py
+-rw-rw-rw-   0        0        0      612 2023-06-18 16:34:24.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/api.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 16:34:04.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.869916 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:50.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-06-20 20:00:00.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/api.py
+-rw-rw-rw-   0        0        0      351 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.903852 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:39.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/__init__.py
+-rw-rw-rw-   0        0        0      307 2023-06-18 14:55:02.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/api.py
+-rw-rw-rw-   0        0        0      408 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.914851 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/__init__.py
+-rw-rw-rw-   0        0        0     3198 2023-06-20 20:00:40.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/api.py
+-rw-rw-rw-   0        0        0     1457 2023-06-20 17:52:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.924852 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/
+-rw-rw-rw-   0        0        0       62 2023-06-18 14:49:03.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/__init__.py
+-rw-rw-rw-   0        0        0     2683 2023-06-20 17:03:43.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/http_async_client.py
+-rw-rw-rw-   0        0        0      217 2023-06-20 17:03:37.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/http_models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.951878 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-06-20 20:01:10.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/api.py
+-rw-rw-rw-   0        0        0      569 2023-06-20 18:13:19.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.987853 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:37:29.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-06-20 20:05:47.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/api.py
+-rw-rw-rw-   0        0        0      241 2023-06-20 20:03:04.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:22.016854 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/__init__.py
+-rw-rw-rw-   0        0        0     2482 2023-06-20 18:32:49.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/api.py
+-rw-rw-rw-   0        0        0     1056 2023-06-20 17:15:14.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/models.py
+-rw-rw-rw-   0        0        0     1314 2023-06-20 21:30:06.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/coinpaprika_async_client.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.834850 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/
+-rw-rw-rw-   0        0        0     2169 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1688 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 23:41:22.025854 coinpaprika_async-3.0.2/tests/
+-rw-rw-rw-   0        0        0     1893 2023-06-20 18:16:17.000000 coinpaprika_async-3.0.2/tests/test_client.py
```

### Comparing `coinpaprika_async-3.0.1/LICENSE` & `coinpaprika_async-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.1/PKG-INFO` & `coinpaprika_async-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinpaprika_async
-Version: 3.0.1
+Version: 3.0.2
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
 Keywords: coinpaprika_async api cryptocurrency async httpx client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `coinpaprika_async-3.0.1/README.md` & `coinpaprika_async-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.1/coinpaprika_async/coinpaprika_async_client.py` & `coinpaprika_async-3.0.2/src/coinpaprika_async/coinpaprika_async_client.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.1/coinpaprika_async.egg-info/PKG-INFO` & `coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinpaprika-async
-Version: 3.0.1
+Version: 3.0.2
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
 Keywords: coinpaprika_async api cryptocurrency async httpx client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `coinpaprika_async-3.0.1/setup.py` & `coinpaprika_async-3.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name="coinpaprika_async",
-    version="3.0.1",
+    version="3.0.2",
     author="DroidZed",
     author_email="droid.zed77@outlook.com",
     description="An asynchronous client for the coinpaprika API.",
-    packages=["coinpaprika_async", "coinpaprika_async.api"],
     url="https://github.com/DroidZed/coinpaprika-async-client.git",
     license="MIT",
     install_requires=["httpx"],
     keywords="coinpaprika_async api cryptocurrency async httpx client",
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `coinpaprika_async-3.0.1/tests/test_client.py` & `coinpaprika_async-3.0.2/tests/test_client.py`

 * *Files identical despite different names*

