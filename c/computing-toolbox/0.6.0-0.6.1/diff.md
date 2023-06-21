# Comparing `tmp/computing-toolbox-0.6.0.tar.gz` & `tmp/computing-toolbox-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.6.0.tar", last modified: Thu Jun 15 19:03:20 2023, max compression
+gzip compressed data, was "computing-toolbox-0.6.1.tar", last modified: Wed Jun 21 19:40:44 2023, max compression
```

## Comparing `computing-toolbox-0.6.0.tar` & `computing-toolbox-0.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:20.952547 computing-toolbox-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 19:03:20.952547 computing-toolbox-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:03:20.952547 computing-toolbox-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:20.948547 computing-toolbox-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:20.948547 computing-toolbox-0.6.0/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:20.948547 computing-toolbox-0.6.0/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:20.948547 computing-toolbox-0.6.0/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/gcp/gs_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:20.952547 computing-toolbox-0.6.0/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-15 19:03:11.000000 computing-toolbox-0.6.0/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:03:20.948547 computing-toolbox-0.6.0/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 19:03:20.000000 computing-toolbox-0.6.0/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-15 19:03:20.000000 computing-toolbox-0.6.0/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:03:20.000000 computing-toolbox-0.6.0/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 19:03:20.000000 computing-toolbox-0.6.0/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 19:03:20.000000 computing-toolbox-0.6.0/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:44.641295 computing-toolbox-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-21 19:40:44.641295 computing-toolbox-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:40:44.641295 computing-toolbox-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:44.637295 computing-toolbox-0.6.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:44.637295 computing-toolbox-0.6.1/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:44.641295 computing-toolbox-0.6.1/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:44.641295 computing-toolbox-0.6.1/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/gcp/gs_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:44.641295 computing-toolbox-0.6.1/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-21 19:40:35.000000 computing-toolbox-0.6.1/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:40:44.637295 computing-toolbox-0.6.1/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-21 19:40:44.000000 computing-toolbox-0.6.1/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-21 19:40:44.000000 computing-toolbox-0.6.1/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:40:44.000000 computing-toolbox-0.6.1/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 19:40:44.000000 computing-toolbox-0.6.1/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 19:40:44.000000 computing-toolbox-0.6.1/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.6.0/LICENSE` & `computing-toolbox-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/PKG-INFO` & `computing-toolbox-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.6.0
+Version: 0.6.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.6.0/README.md` & `computing-toolbox-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/pyproject.toml` & `computing-toolbox-0.6.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.6.1/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.6.1/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/gcp/gs_async.py` & `computing-toolbox-0.6.1/src/computing_toolbox/gcp/gs_async.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.6.1/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.6.1/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.6.1/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/utils/http_async_request.py` & `computing-toolbox-0.6.1/src/computing_toolbox/utils/http_async_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,25 +276,27 @@
         if isinstance(data, list):
             return data
         return [data for _ in range(n)]
 
     def _fix_params(self,
                     urls: list[str],
                     params: list[dict] or dict or None = None,
+                    jsons: list[dict] or dict or None = None,
                     headers: list[dict] or dict or None = None,
                     timeout: float or list[float] = 5,
                     allow_redirects: bool or list[bool] = True,
                     proxies: dict or list[dict] or None = None,
                     request_kwargs: dict or None = None,
                     tqdm_kwargs: dict or None = None):
         """fix parameters from `request` method, used only before `request` method is executed"""
         n_urls = len(urls)
 
         # fix null values -> list
         params = self._expand_to_list(params, n_urls)
+        jsons = self._expand_to_list(jsons, n_urls)
         headers = self._expand_to_list(headers, n_urls)
         timeout = self._expand_to_list(timeout, n_urls)
         allow_redirects = self._expand_to_list(allow_redirects, n_urls)
         proxies = self._expand_to_list(proxies, n_urls)
 
         # fix proxies for aiohttp (because this class use a string proxy representation)
         proxies = [
@@ -304,22 +306,25 @@
 
         # set default kwargs for request
         request_kwargs = request_kwargs if request_kwargs is not None else {}
         request_kwargs = self._expand_to_list(request_kwargs, n_urls)
         request_kwargs = [{
             **{
                 "params": p,
+                "json": j,
                 "headers": h,
                 "timeout": t,
                 "allow_redirects": a,
                 "proxy": x,
             },
             **r
-        } for r, p, h, t, a, x in zip(request_kwargs, params, headers, timeout,
-                                      allow_redirects, proxies)]
+        }
+                          for r, p, j, h, t, a, x in zip(
+                              request_kwargs, params, jsons, headers, timeout,
+                              allow_redirects, proxies)]
         # filter not defined params
         request_kwargs = [{
             k: v
             for k, v in r.items() if v is not None
         } for r in request_kwargs]
 
         # create a tqdm dictionary if necessary
@@ -454,14 +459,15 @@
             # A.5 return results
             return results
 
     def request(self,
                 method: str,
                 urls: list[str],
                 params: list[dict] or dict or None = None,
+                jsons: list[dict] or dict or None = None,
                 headers: list[dict] or dict or None = None,
                 timeout: float or list[float] = 5,
                 allow_redirects: bool or list[bool] = True,
                 proxies: dict or list[dict] or None = None,
                 request_kwargs: dict or None = None,
                 tqdm_kwargs: dict or None = None) -> list[HttpAsyncResponse]:
         """Entry point, this method calls the async code defined above
@@ -470,15 +476,16 @@
         representation.
 
         If you want a progress bar, set tqdm_kwargs as a dictionary,
         {} for a default configuration
 
         :param method: the http method GET,POST,...
         :param urls: the list of urls
-        :param params: additional parameters to be used in the request (default: None)
+        :param params: additional parameters to be used in the GET request (default: None)
+        :param jsons: additional parameters to be used in the POST request (default: None)
         :param headers: the headers to be used in the request (default: None)
         :param timeout: timeout for individual request (default: 5)
         :param allow_redirects: flag to allow redirects (default: True)
         :param proxies: proxy dictionary (default: None(
         :param request_kwargs: additional arguments to be used in the request (default: None)
         :param tqdm_kwargs: parameters for a tqdm progress bar, use {} for default configuration (default: None)
         :return: the list of responses
@@ -492,15 +499,15 @@
         # are updated at run time
         self.method = method
         self.urls = urls
 
         # fix all input parameters as a list if needed, after this step
         # all information is stored in `request_kwargs`
         urls, request_kwargs, tqdm_kwargs = self._fix_params(
-            urls, params, headers, timeout, allow_redirects, proxies,
+            urls, params, jsons, headers, timeout, allow_redirects, proxies,
             request_kwargs, tqdm_kwargs)
 
         # call the request async method `request_many`
         results = asyncio.run(
             self._request_many(method, urls, request_kwargs, tqdm_kwargs))
 
         # compute the execution time by difference
```

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.6.1/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.6.1/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.6.1/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.6.1/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.6.1/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.6.0
+Version: 0.6.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.6.0/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.6.1/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

