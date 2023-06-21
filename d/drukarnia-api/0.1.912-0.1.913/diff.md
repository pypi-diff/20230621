# Comparing `tmp/drukarnia-api-0.1.912.tar.gz` & `tmp/drukarnia-api-0.1.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drukarnia-api-0.1.912.tar", last modified: Tue Jun 20 17:23:02 2023, max compression
+gzip compressed data, was "drukarnia-api-0.1.913.tar", last modified: Wed Jun 21 18:56:04 2023, max compression
```

## Comparing `drukarnia-api-0.1.912.tar` & `drukarnia-api-0.1.913.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/article.py
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/author.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/shortcuts/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/article.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/author.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/shortcuts/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:56:04.383361 drukarnia-api-0.1.913/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/setup.py
```

### Comparing `drukarnia-api-0.1.912/LICENSE` & `drukarnia-api-0.1.913/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/PKG-INFO` & `drukarnia-api-0.1.913/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.912
+Version: 0.1.913
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -28,31 +28,28 @@
 
 ## Simple Usage
 ```python
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
-    # Retrieve all results
-    authors = await Search().find_author('cupomanka')
-    # Get the first search result
-    author = authors[0]
-
-    # Collect all data about the user
-    await author.collect_data()
-
-    # Get user articles
-    articles = await author.articles
-
-    # Print all titles
-    for article in articles:
-        print(article.title)
-
-    # Close the session (we are still considering the best way to make it seamless)
-    await author.close_session()
+    async with Search() as search_engine:
+        authors = await search_engine.find_author('cupomanka') 
+        # Get the first search result
+        author = authors[0]
+
+        # Collect all data about the user
+        await author.collect_data()
+
+        # Get user articles
+        articles = await author.articles
+
+        # Print all titles
+        for article in articles:
+            print(article.title)
 
 
 if __name__ == '__main__':
     import asyncio
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(get_author_article_titles())
```

### Comparing `drukarnia-api-0.1.912/README.md` & `drukarnia-api-0.1.913/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,28 @@
 
 ## Simple Usage
 ```python
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
-    # Retrieve all results
-    authors = await Search().find_author('cupomanka')
-    # Get the first search result
-    author = authors[0]
-
-    # Collect all data about the user
-    await author.collect_data()
-
-    # Get user articles
-    articles = await author.articles
-
-    # Print all titles
-    for article in articles:
-        print(article.title)
-
-    # Close the session (we are still considering the best way to make it seamless)
-    await author.close_session()
+    async with Search() as search_engine:
+        authors = await search_engine.find_author('cupomanka') 
+        # Get the first search result
+        author = authors[0]
+
+        # Collect all data about the user
+        await author.collect_data()
+
+        # Get user articles
+        articles = await author.articles
+
+        # Print all titles
+        for article in articles:
+            print(article.title)
 
 
 if __name__ == '__main__':
     import asyncio
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(get_author_article_titles())
```

### Comparing `drukarnia-api-0.1.912/drukarnia_api/article.py` & `drukarnia-api-0.1.913/drukarnia_api/article.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/drukarnia_api/author.py` & `drukarnia-api-0.1.913/drukarnia_api/author.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/connection.py` & `drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Callable, Dict, Generator, Tuple, List, Iterable
 import inspect
 from drukarnia_api.drukarnia_base.exceptions import DrukarniaAPIError
 
 
 async def _from_response(response: ClientResponse, output: str or List[str] or None) -> Any:
 
-    if response.status not in [200, 201]:
+    if not (200 <= int(response.status) < 300):
         data = await response.json()
         raise DrukarniaAPIError(data['message'], response.status,
                                 response.request_info.method, str(response.request_info.url))
 
     if isinstance(output, str):
         data = await _from_response(response, [output])
         return data[0]
@@ -43,43 +43,45 @@
     def __init__(self, session: ClientSession = None, headers: dict = None,
                  create_user_agent: bool = True, *args, **kwargs):
 
         # Save the aiohttp session
         if session:
             self.session = session
         else:
-            headers_ = {}
+            headers_ = {'Content-Type': 'application/json'}
             if headers:
                 headers_ = headers
 
             if create_user_agent:
                 from fake_useragent import UserAgent
 
                 headers_['User-Agent'] = UserAgent().random
 
             self.session = ClientSession(base_url=self.base_url, headers=headers_, *args, **kwargs)
 
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.session.close()
+
     def _update_headers(self, new_data, inplace: bool = True) -> dict:
         if inplace:
             self.session.headers.update(new_data)
 
         return dict(self.session.headers) | new_data
 
     async def request(self, method: str, url: str, output: str or list = None, **kwargs) -> Any:
 
         if (method in ['post', 'put', 'patch']) and isinstance(kwargs.get('data', {}), dict):
             # if data parameter will be passed as None, (e.g. not passed at all)
             # aiohttp will switch to aplication/octet media type
             # which is not supported by Drukarnia API
 
             kwargs['data'] = json.dumps(kwargs.get('data', {}))
-            headers = self._update_headers({'Content-Type': 'application/json'}, inplace=False)
-
-            async with self.session.request(method.upper(), url, headers=headers, **kwargs) as response:
-                return await _from_response(response, output)
 
         async with self.session.request(method.upper(), url, **kwargs) as response:
             return await _from_response(response, output)
 
     async def request_pool(self, heuristics: Iterable[Dict[str, Any]]) -> Tuple:
         # Create tasks
         tasks = [self.request(**kwargs)
```

### Comparing `drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/element.py` & `drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/element.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/exceptions.py` & `drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/exceptions.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/drukarnia_api/search.py` & `drukarnia-api-0.1.913/drukarnia_api/search.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/drukarnia_api/shortcuts/class_generator.py` & `drukarnia-api-0.1.913/drukarnia_api/shortcuts/class_generator.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/drukarnia_api/tag.py` & `drukarnia-api-0.1.913/drukarnia_api/tag.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-0.1.913/drukarnia_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.912
+Version: 0.1.913
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -28,31 +28,28 @@
 
 ## Simple Usage
 ```python
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
-    # Retrieve all results
-    authors = await Search().find_author('cupomanka')
-    # Get the first search result
-    author = authors[0]
-
-    # Collect all data about the user
-    await author.collect_data()
-
-    # Get user articles
-    articles = await author.articles
-
-    # Print all titles
-    for article in articles:
-        print(article.title)
-
-    # Close the session (we are still considering the best way to make it seamless)
-    await author.close_session()
+    async with Search() as search_engine:
+        authors = await search_engine.find_author('cupomanka') 
+        # Get the first search result
+        author = authors[0]
+
+        # Collect all data about the user
+        await author.collect_data()
+
+        # Get user articles
+        articles = await author.articles
+
+        # Print all titles
+        for article in articles:
+            print(article.title)
 
 
 if __name__ == '__main__':
     import asyncio
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(get_author_article_titles())
```

### Comparing `drukarnia-api-0.1.912/drukarnia_api.egg-info/SOURCES.txt` & `drukarnia-api-0.1.913/drukarnia_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.912/setup.py` & `drukarnia-api-0.1.913/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="0.1.912",
+    version="0.1.913",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
```

