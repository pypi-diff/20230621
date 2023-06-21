# Comparing `tmp/data-spec-validator-3.2.0.tar.gz` & `tmp/data-spec-validator-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/data-spec-validator-3.2.0.tar", last modified: Fri May 26 03:49:04 2023, max compression
+gzip compressed data, was "dist/data-spec-validator-3.3.0.tar", last modified: Wed Jun 21 05:38:15 2023, max compression
```

## Comparing `data-spec-validator-3.2.0.tar` & `data-spec-validator-3.3.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/
--rw-r--r--   0 kilikkuo   (501) staff       (20)    14202 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/PKG-INFO
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/test/
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1813 2023-02-23 07:51:32.000000 data-spec-validator-3.2.0/test/test_nested_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     4764 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/test/test_class_type_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     6069 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/test_decorator_drf.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    58976 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/test_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/test/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1703 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/utils.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     6695 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/test_decorator_dj.py
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/decorator/
--rw-r--r--   0 kilikkuo   (501) staff       (20)       46 2023-05-24 04:08:19.000000 data-spec-validator-3.2.0/data_spec_validator/decorator/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     7125 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/data_spec_validator/decorator/decorators.py
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/spec/
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/
--rw-r--r--   0 kilikkuo   (501) staff       (20)       30 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      917 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/defines.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    19000 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/data_spec_validator/spec/validators.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     7788 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/data_spec_validator/spec/checks.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     3408 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/actions.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      629 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     2101 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/features.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      168 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/utils.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      404 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/wrappers.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     2664 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/defines.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)       22 2023-05-26 03:47:52.000000 data-spec-validator-3.2.0/data_spec_validator/__version__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    10747 2023-05-26 03:47:52.000000 data-spec-validator-3.2.0/README.md
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1253 2023-05-24 06:12:07.000000 data-spec-validator-3.2.0/setup.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      458 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/setup.cfg
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/
--rw-r--r--   0 kilikkuo   (501) staff       (20)    14202 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/PKG-INFO
--rw-r--r--   0 kilikkuo   (501) staff       (20)      939 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/SOURCES.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)       79 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/requires.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)       25 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/top_level.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)        1 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/dependency_links.txt
+drwxr-xr-x   0 hoss       (501) staff       (20)        0 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/
+-rw-r--r--   0 hoss       (501) staff       (20)    11503 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/PKG-INFO
+-rw-r--r--   0 hoss       (501) staff       (20)     1083 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/LICENSE
+drwxr-xr-x   0 hoss       (501) staff       (20)        0 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/test/
+-rw-r--r--   0 hoss       (501) staff       (20)     1813 2023-03-01 05:10:59.000000 data-spec-validator-3.3.0/test/test_nested_spec.py
+-rw-r--r--   0 hoss       (501) staff       (20)     4764 2023-03-01 05:11:07.000000 data-spec-validator-3.3.0/test/test_class_type_spec.py
+-rw-r--r--   0 hoss       (501) staff       (20)     6069 2023-06-16 04:08:10.000000 data-spec-validator-3.3.0/test/test_decorator_drf.py
+-rw-r--r--   0 hoss       (501) staff       (20)    58977 2023-06-16 04:08:10.000000 data-spec-validator-3.3.0/test/test_spec.py
+-rw-r--r--   0 hoss       (501) staff       (20)        0 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/test/__init__.py
+-rw-r--r--   0 hoss       (501) staff       (20)     2159 2023-06-16 04:27:16.000000 data-spec-validator-3.3.0/test/utils.py
+-rw-r--r--   0 hoss       (501) staff       (20)     7706 2023-06-16 04:27:04.000000 data-spec-validator-3.3.0/test/test_decorator_dj.py
+drwxr-xr-x   0 hoss       (501) staff       (20)        0 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator/
+drwxr-xr-x   0 hoss       (501) staff       (20)        0 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator/decorator/
+-rw-r--r--   0 hoss       (501) staff       (20)       46 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/data_spec_validator/decorator/__init__.py
+-rw-r--r--   0 hoss       (501) staff       (20)     7215 2023-06-16 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator/decorator/decorators.py
+drwxr-xr-x   0 hoss       (501) staff       (20)        0 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator/spec/
+drwxr-xr-x   0 hoss       (501) staff       (20)        0 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator/spec/custom_spec/
+-rw-r--r--   0 hoss       (501) staff       (20)       30 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/data_spec_validator/spec/custom_spec/__init__.py
+-rw-r--r--   0 hoss       (501) staff       (20)      917 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/data_spec_validator/spec/custom_spec/defines.py
+-rw-r--r--   0 hoss       (501) staff       (20)    19000 2023-06-16 04:08:10.000000 data-spec-validator-3.3.0/data_spec_validator/spec/validators.py
+-rw-r--r--   0 hoss       (501) staff       (20)     7788 2023-06-16 04:08:10.000000 data-spec-validator-3.3.0/data_spec_validator/spec/checks.py
+-rw-r--r--   0 hoss       (501) staff       (20)     3408 2023-03-01 05:11:07.000000 data-spec-validator-3.3.0/data_spec_validator/spec/actions.py
+-rw-r--r--   0 hoss       (501) staff       (20)      629 2023-03-01 05:11:07.000000 data-spec-validator-3.3.0/data_spec_validator/spec/__init__.py
+-rw-r--r--   0 hoss       (501) staff       (20)     2100 2023-06-16 04:08:10.000000 data-spec-validator-3.3.0/data_spec_validator/spec/features.py
+-rw-r--r--   0 hoss       (501) staff       (20)      168 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/data_spec_validator/spec/utils.py
+-rw-r--r--   0 hoss       (501) staff       (20)      404 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/data_spec_validator/spec/wrappers.py
+-rw-r--r--   0 hoss       (501) staff       (20)     2664 2023-03-01 05:11:07.000000 data-spec-validator-3.3.0/data_spec_validator/spec/defines.py
+-rw-r--r--   0 hoss       (501) staff       (20)        0 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/data_spec_validator/__init__.py
+-rw-r--r--   0 hoss       (501) staff       (20)       22 2023-06-19 07:37:35.000000 data-spec-validator-3.3.0/data_spec_validator/__version__.py
+-rw-r--r--   0 hoss       (501) staff       (20)      309 2023-02-09 08:19:13.000000 data-spec-validator-3.3.0/pyproject.toml
+-rw-r--r--   0 hoss       (501) staff       (20)    10771 2023-06-16 04:08:10.000000 data-spec-validator-3.3.0/README.md
+-rw-r--r--   0 hoss       (501) staff       (20)     1335 2023-06-16 04:08:10.000000 data-spec-validator-3.3.0/setup.py
+-rw-r--r--   0 hoss       (501) staff       (20)      344 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/setup.cfg
+drwxr-xr-x   0 hoss       (501) staff       (20)        0 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator.egg-info/
+-rw-r--r--   0 hoss       (501) staff       (20)    11503 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator.egg-info/PKG-INFO
+-rw-r--r--   0 hoss       (501) staff       (20)      962 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 hoss       (501) staff       (20)       89 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator.egg-info/requires.txt
+-rw-r--r--   0 hoss       (501) staff       (20)       25 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator.egg-info/top_level.txt
+-rw-r--r--   0 hoss       (501) staff       (20)        1 2023-06-21 05:38:15.000000 data-spec-validator-3.3.0/data_spec_validator.egg-info/dependency_links.txt
```

### Comparing `data-spec-validator-3.2.0/test/test_nested_spec.py` & `data-spec-validator-3.3.0/test/test_nested_spec.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/test/test_class_type_spec.py` & `data-spec-validator-3.3.0/test/test_class_type_spec.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/test/test_decorator_drf.py` & `data-spec-validator-3.3.0/test/test_decorator_drf.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/test/test_spec.py` & `data-spec-validator-3.3.0/test/test_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1111,14 +1111,15 @@
         dict(a=1, c=1)
         dict(b=1, c=1)
         dict(a=1)
         dict(b=1)
         dict(c=1)
         dict(d=1)
         """
+
         # ==========================
         class _CondExistOtherFailAOBOCOSpec:
             a = Checker([STR, COND_EXIST], optional=True, COND_EXIST=dict(WITHOUT=['c']))
             b = Checker([STR, COND_EXIST], optional=True, COND_EXIST=dict(WITH=['a'], WITHOUT=['c']))
             c = Checker([STR, COND_EXIST], optional=True, COND_EXIST=dict(WITHOUT=['a']))
 
         assert validate_data_spec(dict(d=1), _CondExistOtherFailAOBOCOSpec)
```

### Comparing `data-spec-validator-3.2.0/test/utils.py` & `data-spec-validator-3.3.0/test/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,41 +29,52 @@
     try:
         import rest_framework  # noqa
     except ImportError:
         return False
     return True
 
 
-def make_request(cls, path='/', method='GET', user=None, headers=None, data=None, qs=None):
+def make_request(cls, path='/', method='GET', user=None, headers=None, data=None, qs=None, is_json=False):
     assert is_django_installed()
-    kwargs = {'REQUEST_METHOD': method, 'PATH_INFO': path, 'wsgi.input': StringIO()}
-    if qs:
-        kwargs.update({'QUERY_STRING': qs})
 
+    from django.core.handlers.asgi import ASGIRequest
     from django.core.handlers.wsgi import WSGIRequest
 
-    req = WSGIRequest(kwargs)
+    if cls is not ASGIRequest:
+        kwargs = {'REQUEST_METHOD': method, 'PATH_INFO': path, 'wsgi.input': StringIO()}
+        if qs:
+            kwargs.update({'QUERY_STRING': qs})
+        req = WSGIRequest(kwargs)
+    else:
+        kwargs = {'path': path, 'method': method}
+        if qs:
+            kwargs.update({'query_string': qs})
+        req = ASGIRequest(kwargs, StringIO())
 
     req.user = user
 
     if headers:
         req.META.update(headers)
 
     if data:
         if method == 'GET':
             setattr(req, 'GET', data)
         elif method in ['POST', 'PUT', 'PATCH', 'DELETE']:
             req.read()  # trigger RawPostDataException and force DRF to load data from req.POST
             req.META.update(
                 {
-                    'CONTENT_TYPE': 'application/x-www-form-urlencoded',
+                    'CONTENT_TYPE': 'application/json' if is_json else 'application/x-www-form-urlencoded',
                     'CONTENT_LENGTH': len(str(data)),
                 }
             )
-            req.POST = data
+            if is_json:
+                req._body = data
+                req.POST = {}
+            else:
+                req.POST = data
 
-    if is_drf_installed() and cls is not WSGIRequest:
+    if is_drf_installed() and cls is not WSGIRequest and cls is not ASGIRequest:
         from rest_framework.parsers import FormParser
         from rest_framework.request import clone_request
 
         return clone_request(cls(req, parsers=[FormParser]), method)
     return req
```

### Comparing `data-spec-validator-3.2.0/test/test_decorator_dj.py` & `data-spec-validator-3.3.0/test/test_decorator_dj.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import itertools
+import json
 import unittest
 from unittest.mock import patch
 
-from parameterized import parameterized
+from parameterized import parameterized, parameterized_class
 
 from data_spec_validator.decorator import dsv, dsv_request_meta
+from data_spec_validator.decorator.decorators import ParseError
 from data_spec_validator.spec import DIGIT_STR, LIST_OF, ONE_OF, STR, Checker, dsv_feature
 
 from .utils import is_django_installed, make_request
 
 try:
     from django.conf import settings
+    from django.core.handlers.asgi import ASGIRequest
     from django.core.handlers.wsgi import WSGIRequest
     from django.http import HttpResponse, HttpResponseBadRequest
     from django.test import RequestFactory
     from django.views import View
 
     settings.configure()
 except Exception:
     # To skip E402 module level import not at top of file
     pass
 
 
+@parameterized_class(('request_class'), [(ASGIRequest,), (WSGIRequest,)])
 @unittest.skipUnless(is_django_installed(), 'Django is not installed')
 class TestDSVDJ(unittest.TestCase):
     def test_decorated_func_returns_error_response(self):
         # arrange
         class _ViewSpec:
             named_arg = Checker([DIGIT_STR])
 
@@ -86,17 +90,17 @@
             view.decorated_func(wsgi_req, named_arg='')
 
     @parameterized.expand(itertools.product([dsv, dsv_request_meta], ['GET', 'POST']))
     def test_data_and_path_named_param_should_combine_together(self, dsv_deco, method):
         # arrange
         payload = {'test_a': 'TEST A'}
         if dsv_deco == dsv:
-            fake_request = make_request(WSGIRequest, method=method, data=payload)
+            fake_request = make_request(self.request_class, method=method, data=payload)
         elif dsv_deco == dsv_request_meta:
-            fake_request = make_request(WSGIRequest, method=method, headers=payload)
+            fake_request = make_request(self.request_class, method=method, headers=payload)
         else:
             assert False
 
         kwargs = {'test_b': 'TEST_B'}
 
         class _ViewSpec:
             test_a = Checker([ONE_OF], ONE_OF='TEST A')
@@ -106,21 +110,23 @@
             @dsv_deco(_ViewSpec)
             def decorated_func(self, req, *_args, **_kwargs):
                 pass
 
         view = _View(request=fake_request)
         view.decorated_func(fake_request, **kwargs)
 
-    @parameterized.expand(['PUT', 'PATCH', 'DELETE'])
-    def test_query_params_with_data(self, method):
+    @parameterized.expand(itertools.product(['POST', 'PUT', 'PATCH', 'DELETE'], [True, False]))
+    def test_query_params_with_data(self, method, is_json):
         # arrange
         qs = 'q_a=3&q_b=true&d.o.t=dot&array[]=a1&array[]=a2&array[]=a3'
         payload = {'test_a': 'TEST A', 'test_f[]': [1, 2, 3]}
 
-        fake_request = make_request(WSGIRequest, method=method, data=payload, qs=qs)
+        if is_json:
+            payload = json.dumps(payload).encode('utf-8')
+        fake_request = make_request(self.request_class, method=method, data=payload, qs=qs, is_json=is_json)
 
         kwargs = {'test_b': 'TEST_B', 'test_c.d.e': 'TEST C.D.E'}
 
         @dsv_feature(strict=True)
         class _ViewSpec:
             q_a = Checker([LIST_OF], LIST_OF=STR)
             q_b = Checker([LIST_OF], LIST_OF=STR)
@@ -135,18 +141,36 @@
             @dsv(_ViewSpec)
             def decorated_func(self, req, *_args, **_kwargs):
                 return True
 
         view = _View(request=fake_request)
         assert view.decorated_func(fake_request, **kwargs)
 
+    @parameterized.expand(['POST', 'PUT', 'PATCH', 'DELETE'])
+    def test_query_params_with_data_in_invalid_json_format(self, method):
+        payload = 'invalid json data'
+
+        fake_request = make_request(self.request_class, method=method, data=payload, is_json=True)
+
+        class _ViewSpec:
+            pass
+
+        class _View(View):
+            @dsv(_ViewSpec)
+            def decorated_func(self, req, *_args, **_kwargs):
+                return True
+
+        view = _View(request=fake_request)
+        with self.assertRaises(ParseError):
+            assert view.decorated_func(fake_request)
+
     def test_req_list_data_with_no_multirow_set(self):
         # arrange
         payload = [{'test_a': 'TEST A1'}, {'test_a': 'TEST A2'}, {'test_a': 'TEST A3'}]
-        fake_request = make_request(WSGIRequest, method='POST', data=payload)
+        fake_request = make_request(self.request_class, method='POST', data=payload)
         kwargs = {'test_b': 'TEST_B'}
 
         class _ViewSingleRowSpec:
             test_a = Checker([STR])
 
         class _View(View):
             @dsv(_ViewSingleRowSpec)
@@ -155,15 +179,15 @@
 
         view = _View(request=fake_request)
         view.decorated_func(fake_request, **kwargs)
 
     def test_req_list_data_with_multirow_true(self):
         # arrange
         payload = [{'test_a': 'TEST A1'}, {'test_a': 'TEST A2'}, {'test_a': 'TEST A3'}]
-        fake_request = make_request(WSGIRequest, method='POST', data=payload)
+        fake_request = make_request(self.request_class, method='POST', data=payload)
         kwargs = {'test_b': 'TEST_B'}
 
         class _ViewSingleRowSpec:
             test_a = Checker([STR])
 
         class _View(View):
             @dsv(_ViewSingleRowSpec, multirow=True)
```

### Comparing `data-spec-validator-3.2.0/data_spec_validator/decorator/decorators.py` & `data-spec-validator-3.3.0/data_spec_validator/decorator/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import json
 from functools import wraps
 from typing import Dict, List, Union
 
 from data_spec_validator.spec import DSVError, raise_if, validate_data_spec
 
 try:
-    import django
+    from django.core.handlers.asgi import ASGIRequest
     from django.core.handlers.wsgi import WSGIRequest
     from django.http import HttpResponseBadRequest, HttpResponseForbidden, QueryDict
     from django.views.generic.base import View
 except ModuleNotFoundError as e:
     print(f'[DSV][WARNING] decorator: "dsv" cannot be used, {e}')
 
 _enabled_drf = False
@@ -16,23 +17,14 @@
     import rest_framework.exceptions as drf_exceptions
     from rest_framework.request import Request
 
     _enabled_drf = True
 except ModuleNotFoundError:
     print('[DSV][INFO] decorator: using "dsv" without djangorestframework')
 
-# try importing ASGIRequest (released since Django 3.0)
-if django.__version__ >= '3':
-    try:
-        from django.core.handlers.asgi import ASGIRequest
-
-        _has_support_asgi_request = True
-    except ModuleNotFoundError:
-        _has_support_asgi_request = False
-
 
 class ValidationError(Exception):
     def __init__(self, message):
         self.message = message
 
 
 class PermissionDenied(Exception):
@@ -46,16 +38,14 @@
 
 
 def _is_wsgi_request(obj):
     return isinstance(obj, WSGIRequest)
 
 
 def _is_asgi_request(obj):
-    if not _has_support_asgi_request:
-        return False
     return isinstance(obj, ASGIRequest)
 
 
 def _is_drf_request(obj):
     return _enabled_drf and isinstance(obj, Request)
 
 
@@ -65,15 +55,14 @@
 
 def _is_view(obj):
     return issubclass(type(obj), View)
 
 
 def _combine_named_params(data, **kwargs):
     def combine_params(_data, params):
-
         raise_if(bool(set(_data.keys()) & set(params.keys())), RuntimeError('Data and URL named param have conflict'))
 
         if isinstance(_data, QueryDict):
             qd = QueryDict(mutable=True)
             qd.update(_data)
             qd.update(params)
             return qd
@@ -110,16 +99,25 @@
             return req_qp
         else:
             if req_qp and issubclass(type(req_qp), dict) and type(req_data) is not list:
                 return {**req_qp, **req_data}
             # TODO: Don't care about the query_params if it's not a dict or the payload is in list.
             return req_data
 
+    def _get_dj_payload(request):
+        content_type = request.headers.get('Content-Type')
+        if content_type == 'application/json':
+            try:
+                return request.body and json.loads(request.body) or {}
+            except Exception:
+                raise ParseError('Unable to parse request body as JSON')
+        return request.POST
+
     if is_wsgi_request or is_asgi_request:
-        data = _collect_data(req.method, req.GET, req.POST)
+        data = _collect_data(req.method, req.GET, _get_dj_payload(req))
     else:
         data = _collect_data(req.method, req.query_params, req.data)
 
     return _combine_named_params(data, **kwargs)
 
 
 def _extract_request(*args):
```

### Comparing `data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/defines.py` & `data-spec-validator-3.3.0/data_spec_validator/spec/custom_spec/defines.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/data_spec_validator/spec/validators.py` & `data-spec-validator-3.3.0/data_spec_validator/spec/validators.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/data_spec_validator/spec/checks.py` & `data-spec-validator-3.3.0/data_spec_validator/spec/checks.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/data_spec_validator/spec/actions.py` & `data-spec-validator-3.3.0/data_spec_validator/spec/actions.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/data_spec_validator/spec/__init__.py` & `data-spec-validator-3.3.0/data_spec_validator/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/data_spec_validator/spec/features.py` & `data-spec-validator-3.3.0/data_spec_validator/spec/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 _FEAT_PARAMS = '__feat_params__'
 
 
 def _process_class(
     cls: Type, strict: bool, any_keys_set: Union[Set[Tuple[str, ...]], None], err_mode: ErrorMode
 ) -> Type:
-
     setattr(cls, _FEAT_PARAMS, _DSVFeatureParams(strict, any_keys_set, err_mode))
 
     return cls
 
 
 def dsv_feature(
     strict: bool = False, any_keys_set: Optional[Set[Tuple[str, ...]]] = None, err_mode=ErrorMode.MSE
```

### Comparing `data-spec-validator-3.2.0/data_spec_validator/spec/defines.py` & `data-spec-validator-3.3.0/data_spec_validator/spec/defines.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.2.0/README.md` & `data-spec-validator-3.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ## Installation
 - Basic usage:
 ```shell
 pip install data-spec-validator
 ```
 - Advance usage (decorator)
-  1. The decorator function `dsv` may depend on `Django` or `djangorestframework`.
+  1. The decorator function `dsv` may depend on `Django` (support v3.0 or later) or `djangorestframework`.
 ```shell
 pip install data-spec-validator[decorator-dj]  # Django Only
 pip install data-spec-validator[decorator]  # Django Rest Framework
 ```
 
 ## Quick Example
 * Do `validate_data_spec` directly wherever you like
```

### Comparing `data-spec-validator-3.2.0/setup.py` & `data-spec-validator-3.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,24 @@
     author_email="pypi@hardcoretech.co",
     description="Validation tool for API/Function parameters",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hardcoretech/data-spec-validator",
     classifiers=[
         "Programming Language :: Python :: 3",
+        "Framework :: Django :: 3",
+        "Framework :: Django :: 4",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"data_spec_validator": "data_spec_validator"},
     packages=setuptools.find_packages(),
     install_requires=[
         "python-dateutil",
     ],
     extras_require={
-        'decorator': ['Django', 'djangorestframework'],
-        'decorator-dj': ['Django'],
+        'decorator': ['Django>=3.0', 'djangorestframework'],
+        'decorator-dj': ['Django>=3.0'],
     },
     python_requires=">=3.6",
     project_urls={"Changelog": "https://github.com/hardcoretech/data-spec-validator/blob/develop/CHANGELOG.md"},
 )
```

### Comparing `data-spec-validator-3.2.0/data_spec_validator.egg-info/SOURCES.txt` & `data-spec-validator-3.3.0/data_spec_validator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 data_spec_validator/__init__.py
 data_spec_validator/__version__.py
 data_spec_validator.egg-info/PKG-INFO
 data_spec_validator.egg-info/SOURCES.txt
 data_spec_validator.egg-info/dependency_links.txt
```

