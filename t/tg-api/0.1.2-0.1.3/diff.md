# Comparing `tmp/tg_api-0.1.2.tar.gz` & `tmp/tg_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_api-0.1.2.tar", max compression
+gzip compressed data, was "tg_api-0.1.3.tar", max compression
```

## Comparing `tg_api-0.1.2.tar` & `tg_api-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      645 2023-06-21 19:47:00.821849 tg_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9678 2023-06-21 15:05:59.456733 tg_api-0.1.2/README.md
--rw-r--r--   0        0        0      794 2023-06-21 15:59:24.319237 tg_api-0.1.2/tg_api/__init__.py
--rw-r--r--   0        0        0     3404 2023-06-21 15:05:59.457725 tg_api-0.1.2/tg_api/client.py
--rw-r--r--   0        0        0     2186 2023-06-21 15:05:59.457725 tg_api-0.1.2/tg_api/exceptions.py
--rw-r--r--   0        0        0    11699 2023-06-21 16:00:25.020909 tg_api-0.1.2/tg_api/tg_methods.py
--rw-r--r--   0        0        0    16578 2023-06-21 15:05:59.460721 tg_api-0.1.2/tg_api/tg_types.py
--rw-r--r--   0        0        0    10060 1970-01-01 00:00:00.000000 tg_api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      610 2023-06-21 20:45:29.818903 tg_api-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9678 2023-06-21 15:05:59.456733 tg_api-0.1.3/README.md
+-rw-r--r--   0        0        0      794 2023-06-21 15:59:24.319237 tg_api-0.1.3/tg_api/__init__.py
+-rw-r--r--   0        0        0     3404 2023-06-21 15:05:59.457725 tg_api-0.1.3/tg_api/client.py
+-rw-r--r--   0        0        0     2186 2023-06-21 15:05:59.457725 tg_api-0.1.3/tg_api/exceptions.py
+-rw-r--r--   0        0        0    11699 2023-06-21 16:00:25.020909 tg_api-0.1.3/tg_api/tg_methods.py
+-rw-r--r--   0        0        0    16578 2023-06-21 15:05:59.460721 tg_api-0.1.3/tg_api/tg_types.py
+-rw-r--r--   0        0        0    10060 1970-01-01 00:00:00.000000 tg_api-0.1.3/PKG-INFO
```

### Comparing `tg_api-0.1.2/pyproject.toml` & `tg_api-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tool.poetry]
 name = "tg-api"
-version = "0.1.2"
+version = "0.1.3"
 description = "Thin wrapper around Telegram API"
 authors = ["Ilya Osipov <070809010@mail.ru>", "Evgeny Evseev <pelid80@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
-packages = [{include = "tg_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "0.24.1"
 pydantic = "1.10.8"
 pytest = {version = "7.3.*", extras = ["anyio"]}
 anyio = "3.7.0"
```

### Comparing `tg_api-0.1.2/README.md` & `tg_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tg_api-0.1.2/tg_api/__init__.py` & `tg_api-0.1.3/tg_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tg_api-0.1.2/tg_api/client.py` & `tg_api-0.1.3/tg_api/client.py`

 * *Files identical despite different names*

### Comparing `tg_api-0.1.2/tg_api/exceptions.py` & `tg_api-0.1.3/tg_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg_api-0.1.2/tg_api/tg_methods.py` & `tg_api-0.1.3/tg_api/tg_methods.py`

 * *Files identical despite different names*

### Comparing `tg_api-0.1.2/tg_api/tg_types.py` & `tg_api-0.1.3/tg_api/tg_types.py`

 * *Files identical despite different names*

### Comparing `tg_api-0.1.2/PKG-INFO` & `tg_api-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Thin wrapper around Telegram API
 License: GNU GPLv3
 Author: Ilya Osipov
 Author-email: 070809010@mail.ru
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

