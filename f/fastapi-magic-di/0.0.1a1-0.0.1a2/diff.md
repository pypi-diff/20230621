# Comparing `tmp/fastapi_magic_di-0.0.1a1.tar.gz` & `tmp/fastapi_magic_di-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_magic_di-0.0.1a1.tar", max compression
+gzip compressed data, was "fastapi_magic_di-0.0.1a2.tar", max compression
```

## Comparing `fastapi_magic_di-0.0.1a1.tar` & `fastapi_magic_di-0.0.1a2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2023-06-19 15:24:15.936987 fastapi_magic_di-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     6594 2023-06-20 22:43:28.229677 fastapi_magic_di-0.0.1a1/README.md
--rw-r--r--   0        0        0      135 2023-06-20 23:10:27.653763 fastapi_magic_di-0.0.1a1/fastapi_di/__init__.py
--rw-r--r--   0        0        0      194 2023-06-13 12:43:05.534905 fastapi_magic_di-0.0.1a1/fastapi_di/_client.py
--rw-r--r--   0        0        0     3726 2023-06-20 21:07:58.474624 fastapi_magic_di-0.0.1a1/fastapi_di/_injector.py
--rw-r--r--   0        0        0      647 2023-06-20 23:11:38.870175 fastapi_magic_di-0.0.1a1/fastapi_di/_provide.py
--rw-r--r--   0        0        0      323 2023-06-20 15:38:00.089246 fastapi_magic_di-0.0.1a1/fastapi_di/app.py
--rw-r--r--   0        0        0     1263 2023-06-20 17:39:08.841831 fastapi_magic_di-0.0.1a1/fastapi_di/env_fields.py
--rw-r--r--   0        0        0        0 2023-06-20 23:11:07.065409 fastapi_magic_di-0.0.1a1/fastapi_di/py.typed
--rw-r--r--   0        0        0      642 2023-06-20 17:22:25.327646 fastapi_magic_di-0.0.1a1/fastapi_di/testing.py
--rw-r--r--   0        0        0      574 2023-06-20 23:12:17.565646 fastapi_magic_di-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 fastapi_magic_di-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-19 15:24:15.936987 fastapi_magic_di-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     6594 2023-06-20 22:43:28.229677 fastapi_magic_di-0.0.1a2/README.md
+-rw-r--r--   0        0        0      147 2023-06-20 23:22:15.224570 fastapi_magic_di-0.0.1a2/fastapi_di/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-20 23:22:25.948116 fastapi_magic_di-0.0.1a2/fastapi_di/_client.py
+-rw-r--r--   0        0        0     3726 2023-06-20 21:07:58.474624 fastapi_magic_di-0.0.1a2/fastapi_di/_injector.py
+-rw-r--r--   0        0        0      647 2023-06-20 23:11:38.870175 fastapi_magic_di-0.0.1a2/fastapi_di/_provide.py
+-rw-r--r--   0        0        0      323 2023-06-20 15:38:00.089246 fastapi_magic_di-0.0.1a2/fastapi_di/app.py
+-rw-r--r--   0        0        0     1263 2023-06-20 17:39:08.841831 fastapi_magic_di-0.0.1a2/fastapi_di/env_fields.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:11:07.065409 fastapi_magic_di-0.0.1a2/fastapi_di/py.typed
+-rw-r--r--   0        0        0      642 2023-06-20 17:22:25.327646 fastapi_magic_di-0.0.1a2/fastapi_di/testing.py
+-rw-r--r--   0        0        0      574 2023-06-20 23:23:00.525445 fastapi_magic_di-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 fastapi_magic_di-0.0.1a2/PKG-INFO
```

### Comparing `fastapi_magic_di-0.0.1a1/LICENSE` & `fastapi_magic_di-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a1/README.md` & `fastapi_magic_di-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a1/fastapi_di/_injector.py` & `fastapi_magic_di-0.0.1a2/fastapi_di/_injector.py`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a1/fastapi_di/_provide.py` & `fastapi_magic_di-0.0.1a2/fastapi_di/_provide.py`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a1/fastapi_di/env_fields.py` & `fastapi_magic_di-0.0.1a2/fastapi_di/env_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a1/fastapi_di/testing.py` & `fastapi_magic_di-0.0.1a2/fastapi_di/testing.py`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a1/pyproject.toml` & `fastapi_magic_di-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-magic-di"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "Dependency Injector for FastAPI that makes your life easier"
 authors = ["Nikita Zavadin <zavadin142@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "fastapi_di"}, {include = "fastapi_di/py.typed"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fastapi_magic_di-0.0.1a1/PKG-INFO` & `fastapi_magic_di-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-magic-di
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Dependency Injector for FastAPI that makes your life easier
 License: MIT
 Author: Nikita Zavadin
 Author-email: zavadin142@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

