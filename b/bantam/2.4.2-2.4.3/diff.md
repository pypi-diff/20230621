# Comparing `tmp/bantam-2.4.2.tar.gz` & `tmp/bantam-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.4.2.tar", last modified: Tue Jun 20 02:14:40 2023, max compression
+gzip compressed data, was "bantam-2.4.3.tar", last modified: Wed Jun 21 04:42:10 2023, max compression
```

## Comparing `bantam-2.4.2.tar` & `bantam-2.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-20 02:14:40.132470 bantam-2.4.2/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.2/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.2/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-20 02:14:40.132470 bantam-2.4.2/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-20 02:13:31.000000 bantam-2.4.2/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.2/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.2/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.2/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.2/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    21101 2023-06-17 16:17:43.000000 bantam-2.4.2/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.2/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.2/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    50846 2023-06-20 02:13:08.000000 bantam-2.4.2/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.2/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.2/src/bantam/js_async.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4821 2023-06-17 16:39:40.000000 bantam-2.4.2/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.2/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.2/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.2/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.2/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.2/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.2/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.2/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:42:10.512422 bantam-2.4.3/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.3/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.3/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-21 04:42:10.512422 bantam-2.4.3/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-21 04:41:13.000000 bantam-2.4.3/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.508422 bantam-2.4.3/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.3/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.3/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.3/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.3/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22873 2023-06-21 04:39:45.000000 bantam-2.4.3/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.3/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.3/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    50578 2023-06-21 03:43:56.000000 bantam-2.4.3/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.3/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.3/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-21 04:42:10.000000 bantam-2.4.3/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:42:10.512422 bantam-2.4.3/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5623 2023-06-21 04:28:06.000000 bantam-2.4.3/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.3/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.3/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.3/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.3/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.3/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.3/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.3/test/test_js_async.py
```

### Comparing `bantam-2.4.2/PKG-INFO` & `bantam-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.2
+Version: 2.4.3
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.2
+Download-URL: https://github.com/bantam/dist/2.4.3
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.2/setup.py` & `bantam-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.4.2"
+VERSION = "2.4.3"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.4.2/src/bantam/__init__.py` & `bantam-2.4.3/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/src/bantam/api.py` & `bantam-2.4.3/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/src/bantam/autogen/main.py` & `bantam-2.4.3/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/src/bantam/client.py` & `bantam-2.4.3/src/bantam/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,19 @@
 from bantam.api import API, RestMethod
 
 __all__ = ["WebInterface"]
 
 C = TypeVar('C', bound="WebInterface")
 
 
+class InvocationError(Exception):
+    def __init__(self, message: str):
+        self.message = message
+
+
 # noinspection PyProtectedMember
 class WebInterface(ABC):
 
     _clients: Dict[str, Any] = {}
 
     @classmethod
     def _generate_url_args(cls, kwargs, self_id: Optional[str] = None):
@@ -140,49 +145,56 @@
         async def class_method(cls_, *args, **kwargs_):
             nonlocal api, end_point
             # noinspection PyBroadException
             try:
                 arg_spec = inspect.getfullargspec(api._func)
             except Exception:
                 arg_spec = inspect.getfullargspec(api._func.__func__)
+            if len(arg_spec) - 1 < len(args):
+                raise TypeError(f"Too many arguments supplied in call to {api.name}")
             if arg_spec.varargs is None:
                 kwargs_.update({
                     arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
                 })
             else:
                 kwargs_[arg_spec.varargs] = args
             # noinspection PyBroadException
             rest_method = api._func._bantam_web_api.method
-            if rest_method.value == RestMethod.GET.value:
-                url_args = cls._generate_url_args(kwargs=kwargs_)
-                url = f"{base_url}{url_args}"
-                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.get(url) as resp:
-                        resp.raise_for_status()
-                        data = (await resp.content.read()).decode('utf-8')
-                        if api.is_constructor:
-                            if hasattr(clazz, 'jsonrepr'):
-                                repr_ = clazz.jsonrepr(data)
-                                self_id = repr_[api.uuid_param or 'uuid']
-                            else:
-                                repr_ = json.loads(data)
-                                self_id = repr_[api.uuid_param or 'uuid']
-                            return cls_(self_id)
-                        return conversions.from_str(data, api.return_type)
-            else:
-                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
-                                      for k, v in kwargs_.items()})
+            data = None
+            try:
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.post(base_url, data=payload) as resp:
-                        resp.raise_for_status()
-                        data = (await resp.content.read()).decode('utf-8')
-                        if api.is_constructor:
-                            self_id = json.loads(data)[api.uuid_param or 'uuid']
-                            return cls_(self_id)
-                        return conversions.from_str(data, api.return_type)
+                    if rest_method.value == RestMethod.GET.value:
+                        url_args = cls._generate_url_args(kwargs=kwargs_)
+                        url = f"{base_url}{url_args}"
+                        async with session.get(url) as resp:
+                            data = (await resp.content.read()).decode('utf-8')
+                            resp.raise_for_status()
+                            if api.is_constructor:
+                                if hasattr(clazz, 'jsonrepr'):
+                                    repr_ = clazz.jsonrepr(data)
+                                    self_id = repr_[api.uuid_param or 'uuid']
+                                else:
+                                    repr_ = json.loads(data)
+                                    self_id = repr_[api.uuid_param or 'uuid']
+                                return cls_(self_id)
+                            return conversions.from_str(data, api.return_type)
+                    else:
+                        payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
+                                              for k, v in kwargs_.items()})
+                        async with session.post(base_url, data=payload) as resp:
+                            data = (await resp.content.read()).decode('utf-8')
+                            resp.raise_for_status()
+                            if api.is_constructor:
+                                self_id = json.loads(data)[api.uuid_param or 'uuid']
+                                return cls_(self_id)
+                            return conversions.from_str(data, api.return_type)
+            except aiohttp.ClientResponseError as e:
+                error_body = data if resp is not None else "<<no response text/traceback info>>"
+                error_body += f"\n\nRequest to {api.name} failed: {e.message}"
+                raise InvocationError(error_body)
 
         setattr(clazz, name, class_method)
 
     @classmethod
     def _add_class_method_streamed(cls, clazz: Type, impl_name: str, end_point: str, method,
                                    common_headers: dict):
         if not hasattr(method, '_bantam_web_api'):
@@ -205,48 +217,53 @@
                 arg_spec = inspect.getfullargspec(api._func)
             except Exception:
                 arg_spec = inspect.getfullargspec(api._func.__func__)
             kwargs.update({
                 arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
             })
             rest_method = api._func._bantam_web_api.method
-            if rest_method.value == RestMethod.GET.value:
-                url_args = cls._generate_url_args(kwargs=kwargs)
-                url = f"{base_url}{url_args}"
-                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.get(url) as resp:
-                        resp.raise_for_status()
-                        buffer = ""
-                        async for data, _ in resp.content.iter_chunks():
-                            if data:
-                                if api.return_type != bytes:
-                                    buffer += data.decode('utf-8')
-                                    *data_items, buffer = buffer.split('\0')
-                                    for datum in data_items:
-                                        yield conversions.from_str(datum, api.return_type)
-                                else:
-                                    data = data.decode('utf-8')
-                                    yield conversions.from_str(data, api.return_type)
-            else:
-                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
-                                      for k, v in kwargs.items()})
-                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.post(base_url, data=payload) as resp:
-                        buffer = ""
-                        async for data, _ in resp.content.iter_chunks():
-                            resp.raise_for_status()
-                            if data:
-                                if api.return_type != bytes:
-                                    buffer += data.decode('utf-8')
-                                    *data_items, buffer = buffer.split('\0')
-                                    for datum in data_items:
-                                        yield conversions.from_str(datum, api.return_type)
-                                else:
-                                    data = data.decode('utf-8')
-                                    yield conversions.from_str(data, api.return_type)
+            try:
+                if rest_method.value == RestMethod.GET.value:
+                    url_args = cls._generate_url_args(kwargs=kwargs)
+                    url = f"{base_url}{url_args}"
+                    async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                        async with session.get(url) as resp:
+                            resp.raise_for_status()
+                            buffer = ""
+                            async for data, _ in resp.content.iter_chunks():
+                                if data:
+                                    if api.return_type != bytes:
+                                        buffer += data.decode('utf-8')
+                                        *data_items, buffer = buffer.split('\0')
+                                        for datum in data_items:
+                                            yield conversions.from_str(datum, api.return_type)
+                                    else:
+                                        data = data.decode('utf-8')
+                                        yield conversions.from_str(data, api.return_type)
+                else:
+                    payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
+                                          for k, v in kwargs.items()})
+                    async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                        async with session.post(base_url, data=payload) as resp:
+                            buffer = ""
+                            async for data, _ in resp.content.iter_chunks():
+                                resp.raise_for_status()
+                                if data:
+                                    if api.return_type != bytes:
+                                        buffer += data.decode('utf-8')
+                                        *data_items, buffer = buffer.split('\0')
+                                        for datum in data_items:
+                                            yield conversions.from_str(datum, api.return_type)
+                                    else:
+                                        data = data.decode('utf-8')
+                                        yield conversions.from_str(data, api.return_type)
+            except aiohttp.ClientResponseError as e:
+                body = resp.content if resp is not None else "<<no response text/traceback info>>"
+                body += f"\n\nRequest to {api.name} failed: {e.message}"
+                raise Exception(body)
 
         setattr(clazz, name, class_method_streamed)
 
     @classmethod
     def _add_instance_method(cls, clazz: Type, impl_name: str, end_point: str, method,
                              common_headers: dict):
         # class/static methods
@@ -266,34 +283,39 @@
             except Exception:
                 arg_spec = inspect.getfullargspec(api._func.__func__)
             kwargs_.update({
                 arg_spec.args[n]: arg for n, arg in enumerate(args)
             })
             # noinspection PyBroadException
             rest_method = api._func._bantam_web_api.method
-            if rest_method.value == RestMethod.GET.value:
-                url_args = cls._generate_url_args(self_id=self.self_id, kwargs=kwargs_)
-                url = f"{base_url}{url_args}"
-                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.get(url) as resp:
-                        resp.raise_for_status()
-                        data = (await resp.content.read()).decode('utf-8')
-                        return conversions.from_str(data, api.return_type)
-            else:
-                kwargs_['self'] = self.self_id
-                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
-                                      for k, v in kwargs_.items()})
-                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.post(base_url, data=payload) as resp:
-                        resp.raise_for_status()
-                        data = (await resp.content.read()).decode('utf-8')
-                        if api.is_constructor:
-                            self_id = json.loads(data)['self_id']
-                            return clazz(self_id)
-                        return conversions.from_str(data, api.return_type)
+            try:
+                if rest_method.value == RestMethod.GET.value:
+                    url_args = cls._generate_url_args(self_id=self.self_id, kwargs=kwargs_)
+                    url = f"{base_url}{url_args}"
+                    async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                        async with session.get(url) as resp:
+                            resp.raise_for_status()
+                            data = (await resp.content.read()).decode('utf-8')
+                            return conversions.from_str(data, api.return_type)
+                else:
+                    kwargs_['self'] = self.self_id
+                    payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
+                                          for k, v in kwargs_.items()})
+                    async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                        async with session.post(base_url, data=payload) as resp:
+                            resp.raise_for_status()
+                            data = (await resp.content.read()).decode('utf-8')
+                            if api.is_constructor:
+                                self_id = json.loads(data)['self_id']
+                                return clazz(self_id)
+                            return conversions.from_str(data, api.return_type)
+            except aiohttp.ClientResponseError as e:
+                body = resp.content if resp is not None else "<<no response text/traceback info>>"
+                body += f"\n\nRequest to {api.name} failed: {e.message}"
+                raise Exception(body)
 
         setattr(clazz, name, instance_method)
 
     @classmethod
     def _add_instance_method_streamed(cls, clazz: Type, impl_name: str, end_point: str, method,
                                       common_headers: dict):
         # class/static methods
@@ -306,49 +328,55 @@
         async def instance_method_streamed(self, *args, **kwargs_):
             nonlocal api, end_point, base_url
             arg_spec = inspect.getfullargspec(api._func)
             kwargs_.update({
                 arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
             })
             rest_method = api.method
-            if rest_method == RestMethod.GET:
-                url_args = cls._generate_url_args(self_id=self.self_id, kwargs=kwargs_)
-                url = f"{base_url}{url_args}"
-                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.get(url) as resp:
-                        resp.raise_for_status()
-                        buffer = ""
-                        async for data, _ in resp.content.iter_chunks():
-                            if data:
-                                if api.return_type != bytes:
-                                    buffer += data.decode('utf-8')
-                                    *data_items, buffer = buffer.split('\0')
-                                    for datum in data_items:
-                                        yield conversions.from_str(datum, api.return_type)
-                                else:
-                                    data = data.decode('utf-8')
-                                    yield conversions.from_str(data, api.return_type)
-            else:
-                url = f"{base_url}?self={self.self_id}"
-                kwargs_['self'] = self.self_id
-                payload = json.dumps({k: conversions.to_str(v) for k, v in kwargs_.items()})
-                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
-                    async with session.post(url, data=payload) as resp:
-                        resp.raise_for_status()
-                        buffer = ""
-                        async for data, _ in resp.content.iter_chunks():
-                            if data:
-                                if api.return_type != bytes:
-                                    buffer += data.decode('utf-8')
-                                    *data_items, buffer = buffer.split('\0')
-                                    for datum in data_items:
-                                        yield conversions.from_str(datum, api.return_type)
-                                else:
-                                    data = data.decode('utf-8')
-                                    yield conversions.from_str(data, api.return_type)
+            try:
+                if rest_method == RestMethod.GET:
+                    url_args = cls._generate_url_args(self_id=self.self_id, kwargs=kwargs_)
+                    url = f"{base_url}{url_args}"
+                    async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                        async with session.get(url) as resp:
+                            resp.raise_for_status()
+                            buffer = ""
+                            async for data, _ in resp.content.iter_chunks():
+                                if data:
+                                    if api.return_type != bytes:
+                                        buffer += data.decode('utf-8')
+                                        *data_items, buffer = buffer.split('\0')
+                                        for datum in data_items:
+                                            yield conversions.from_str(datum, api.return_type)
+                                    else:
+                                        data = data.decode('utf-8')
+                                        yield conversions.from_str(data, api.return_type)
+                else:
+                    url = f"{base_url}?self={self.self_id}"
+                    kwargs_['self'] = self.self_id
+                    payload = json.dumps({k: conversions.to_str(v) for k, v in kwargs_.items()})
+                    async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                        async with session.post(url, data=payload) as resp:
+                            resp.raise_for_status()
+                            buffer = ""
+                            async for data, _ in resp.content.iter_chunks():
+                                if data:
+                                    if api.return_type != bytes:
+                                        buffer += data.decode('utf-8')
+                                        *data_items, buffer = buffer.split('\0')
+                                        for datum in data_items:
+                                            yield conversions.from_str(datum, api.return_type)
+                                    else:
+                                        data = data.decode('utf-8')
+                                        yield conversions.from_str(data, api.return_type)
+            except aiohttp.ClientResponseError as e:
+                body = resp.content if resp is not None else "<<no response text/traceback info>>"
+                body += f"\n\nRequest to {api.name} failed: {e.message}"
+                raise Exception(body)
+
         setattr(clazz, name, instance_method_streamed)
 
     # noinspection PyPep8Naming
     @classmethod
     def ClientEndpointMapping(cls: C, impl_name: Optional[str] = None,
                               common_headers: Optional[dict] = None) -> Mapping[str, C]:
         if cls == WebInterface:
```

### Comparing `bantam-2.4.2/src/bantam/conversions.py` & `bantam-2.4.3/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/src/bantam/decorators.py` & `bantam-2.4.3/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/src/bantam/http.py` & `bantam-2.4.3/src/bantam/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,25 @@
 
 def wrap(app, op):
     async def wrapper(request):
         return await op(app, request)
     return wrapper
 
 
+async def response_from_exception(request, reason: str, code: int = 400):
+    text = traceback.format_exc()
+    resp = Response(status=code,
+                    reason=reason,
+                    text=text,
+                    content_type="text/plain"
+                    )
+    await resp.prepare(request)
+    return resp
+
+
 # noinspection PyUnresolvedReferences
 class WebApplication:
     """
     Main class for running a WebApplication server. See the documentation for *aiohttp* for information on the various
     parameters.  Additional parameters for this class are:
 
     :param static_path: root path to where static files will be kept, mapped to a route "/static", if provided
@@ -328,22 +339,32 @@
                                     expire_obj=method._bantam_web_api.expire_object,
                                     timeout=method._bantam_web_api.timeout,
                                     uuid_param=method._bantam_web_api.uuid_param)(immediate)
                             immediate._bantam_web_api._clazz = clazz
                             # handles case of _expire !-> expire
                             immediate._bantam_web_api._name = method._bantam_web_api.name
                         elif hasattr(method, '_bantam_web_api'):
+                            parameters1 = inspect.signature(method).parameters
+                            if 'cls' in parameters1:
+                                del parameters1['cls']
+                            parameters2 = inspect.signature(method).parameters
+                            if 'cls' in parameters1:
+                                del parameters2['cls']
                             has_diff_web_api = (
                                 method._bantam_web_api.method != immediate._bantam_web_api.method
                                 or method._bantam_web_api.content_type != immediate._bantam_web_api.content_type
                                 or method._bantam_web_api.is_constructor != immediate._bantam_web_api.is_constructor
+                                or (inspect.signature(method).return_annotation !=
+                                    inspect.signature(immediate).return_annotation)
+                                or parameters1 != parameters2
                             )
                             if has_diff_web_api:
                                 raise ValueError(
-                                    f"Mismatch in @web_api specifications in {class_name}.{method_name}"
+                                    f"Mismatch in @web_api specifications, parameter names/types or return type"
+                                    f"in {class_name}.{method_name}"
                                     f" and {ancestor.__name__}.{method_name}"
                                 )
                             elif method._bantam_web_api.arg_annotations != immediate._bantam_web_api.arg_annotations:
                                 raise TypeError(
                                     f"Mismatch in name and/or type specifications between {class_name}.{method_name}"
                                     f" and {ancestor.__name__}.{method_name}"
                                 )
@@ -643,31 +664,52 @@
                     else:
                         raise ValueError(f"Unknown method {method} in @web-api")
                     try:
                         postprocess = postprocess or app.postprocessor
                         postprocess(response) if postprocess else response
                     except Exception as e:
                         text = traceback.format_exc()
-                        resp_ = Response(status=400, text=f"Error in post-processing of response: {e}\n{text}")
+                        resp_ = Response(status=400, reason=f"Exception in processing: {e}", text=text,
+                                         content_type="text/plain")
                         await resp_.prepare(request)
                         return resp_
                     return response
+                except PermissionError as e:
+                    return await response_from_exception(
+                        code=401,
+                        request=request,
+                        reason=f"PermissionError with request: {str(e)}"
+                    )
+                except TypeError as e:
+                    return await response_from_exception(
+                        code=400,
+                        request=request,
+                        reason=f"Improperly formatted query: {str(e)}"
+                    )
+                except HTTPException:
+                    raise
                 except (CancelledError, ConnectionResetError, ClientConnectionError):
                     raise
+                except Exception as e:
+                    return await response_from_exception(
+                        request,
+                        code=400,
+                        reason=f"General exception in request: {str(e)}"
+                    )
                 except BaseException as e:
-                    text = traceback.format_exc()
-                    resp_ = Response(status=500, reason=f"Server error: {e}",
-                                     body=f"Server error: {e}\n{text}", content_type="test/plain")
-                    await resp_.prepare(request)
-                    return resp_
+                    return await response_from_exception(
+                        request,
+                        code=500,
+                        reason=f"General exception when processing request: {str(e)}"
+                    )
             resp_q = asynciomultiplexer.AsyncAdaptorQueue(1)
             await cls.MainThread.start(invoke_proper(), resp_q)
             resp = await resp_q.get()
             if isinstance(resp, Exception):
-                raise
+                raise resp
             return resp
 
         invoke.clazz = WebApplication._instance_methods_class_map.get(api) if is_instance_method else None
         if method == RestMethod.GET:
             # noinspection PyProtectedMember
             WebApplication.register_route_get(route, invoke, api, api._real_func.__module__)
         elif method == RestMethod.POST:
@@ -743,36 +785,30 @@
                 #  streamed response through async generator:
                 #################
                 # underlying function has yielded a result rather than turning
                 # process the yielded value and allow execution to resume from yielding task
                 content_type = "text-streamed; charset=x-user-defined"
                 response = StreamResponse(status=200, reason='OK', headers={'Content-Type': content_type})
                 await response.prepare(request)
-                try:
-                    # iterate to get the one (and hopefully only) yielded element:
-                    # noinspection PyTypeChecker
-                    async for res in result:
-                        try:
-                            serialized = _serialize_return_value(res, encoding)
-                            if not isinstance(res, bytes):
-                                serialized += b'\0'
-                            await response.write(serialized)
-                        except (CancelledError, ConnectionResetError, ClientConnectionError):
-                            if api.on_disconnect is not None:
-                                if inspect.iscoroutinefunction(api.on_disconnect):
-                                    await api.on_disconnect(res)
-                                else:
-                                    api.on_disconnect(res)
-                            raise
+                # iterate to get the one (and hopefully only) yielded element:
+                # noinspection PyTypeChecker
+                async for res in result:
+                    try:
+                        serialized = _serialize_return_value(res, encoding)
+                        if not isinstance(res, bytes):
+                            serialized += b'\0'
+                        await response.write(serialized)
+                    except (CancelledError, ConnectionResetError, ClientConnectionError):
+                        if api.on_disconnect is not None:
+                            if inspect.iscoroutinefunction(api.on_disconnect):
+                                await api.on_disconnect(res)
+                            else:
+                                api.on_disconnect(res)
+                        raise
 
-                except (CancelledError, ConnectionResetError, ClientConnectionError):
-                    raise
-                except Exception as e:
-                    print(str(e))
-                    raise asyncio.CancelledError(f"Error in server-side logic: {e}") from e
                 await response.write_eof()
                 return response
             else:
                 #################
                 #  regular response
                 #################
                 result = await result
@@ -794,37 +830,14 @@
                         uuid, cls.ObjectRepo.DEFAULT_OBJECT_EXPIRATION))
                 else:
                     result = _serialize_return_value(result, encoding)
                 resp = Response(status=200, body=result if result is not None else b"Success",
                                 content_type=content_type)
                 await resp.prepare(request)
                 return resp
-        except PermissionError as e:
-            resp = Response(status=401,
-                            reason=f"Improperly formatted query: {str(e)}\n{traceback.format_exc()}",
-                            text=f"Improperly formatted query: {str(e)}\n{traceback.format_exc()}",
-                            )
-            await resp.prepare(request)
-            return resp
-        except TypeError as e:
-            resp = Response(status=400,
-                            reason=f"Improperly formatted query: {str(e)}\n{traceback.format_exc()}",
-                            text=f"Improperly formatted query: {str(e)}\n{traceback.format_exc()}",
-                            )
-            await resp.prepare(request)
-            return resp
-        except HTTPException:
-            raise
-        except Exception as e:
-            resp = Response(status=400,
-                            reason=f"Exception: {e}: \n{traceback.format_exc()}",
-                            text=f"Exception: {e}: \n{traceback.format_exc()}",
-                            )
-            await resp.prepare(request)
-            return resp
         finally:
             # noinspection PyUnresolvedReferences,PyProtectedMember
             del cls._context[sys._getframe(0)]
 
     @classmethod
     async def _invoke_post_api_wrapper(cls, api: API, content_type: str, request: Request,
                                        **addl_args: Any) -> Union[Response, StreamResponse]:
@@ -999,30 +1012,14 @@
                     return resp
                 else:
                     result = _serialize_return_value(await awaitable, encoding)
                 resp = Response(status=200, body=result if result is not None else b"Success",
                                 content_type=content_type)
                 await resp.prepare(request)
                 return resp
-
-        except TypeError as e:
-            resp = Response(status=400, text=f"Improperly formatted query: {str(e)}")
-            await resp.prepare(request)
-            return resp
-        except HTTPException as e:
-            resp = Response(status=e.status_code, text=str(e))
-            await resp.prepare(request)
-            return resp
-        except (CancelledError, ConnectionResetError, ClientConnectionError):
-            raise
-        except Exception as e:
-            text = f"Exception: {e}\n {traceback.format_exc()}"
-            resp = Response(status=500, text=text)
-            await resp.prepare(request)
-            return resp
         finally:
             # noinspection PyUnresolvedReferences,PyProtectedMember
             del cls._context[sys._getframe(0)]
 
 
 def _convert_request_param(value: str, typ: Type) -> Any:
     """
```

### Comparing `bantam-2.4.2/src/bantam/js.py` & `bantam-2.4.3/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/src/bantam/js_async.py` & `bantam-2.4.3/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.3/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.2
+Version: 2.4.3
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.2
+Download-URL: https://github.com/bantam/dist/2.4.3
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.2/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.3/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/test/test_client_get.py` & `bantam-2.4.3/test/test_client_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import asyncio
 from asyncio import CancelledError
 from contextlib import suppress
 from pathlib import Path
 import sys
+
+from bantam.client import InvocationError
+
 if True:
     sys.path.insert(0, str(Path(__file__).parent / 'example'))
 from pathlib import Path
 
 import pytest
 from bantam.http import WebApplication
 
@@ -117,7 +120,24 @@
             assert item == str(29)
             count += 1
         assert count == 200
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
+
+
+@pytest.mark.asyncio
+async def test_client_instance_raises_exception(tmpdir):
+    from class_rest_get import RestAPIExampleAsyncInterface
+    app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
+    task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
+    try:
+        await asyncio.sleep(1)
+        Client = RestAPIExampleAsyncInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
+        with pytest.raises(InvocationError) as e:
+            await Client.raise_exception()
+        assert "ValueError: Fake exception raised for testing purposes." in e.value.message
+    finally:
+        task.cancel()
+        with suppress(CancelledError):
+            await task
```

### Comparing `bantam-2.4.2/test/test_client_post.py` & `bantam-2.4.3/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/test/test_client_post_inherited_apis.py` & `bantam-2.4.3/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/test/test_conversions.py` & `bantam-2.4.3/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/test/test_decorators.py` & `bantam-2.4.3/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/test/test_js.py` & `bantam-2.4.3/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.2/test/test_js_async.py` & `bantam-2.4.3/test/test_js_async.py`

 * *Files identical despite different names*

