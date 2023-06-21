# Comparing `tmp/openborders-0.1.1.tar.gz` & `tmp/openborders-0.1.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openborders-0.1.1.tar", max compression
+gzip compressed data, was "openborders-0.1.1.post0.tar", max compression
```

## Comparing `openborders-0.1.1.tar` & `openborders-0.1.1.post0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      202 2023-06-21 05:01:43.184465 openborders-0.1.1/openborders/__init__.py
--rw-r--r--   0        0        0     5511 2023-06-21 12:12:49.976324 openborders-0.1.1/openborders/cli.py
--rw-r--r--   0        0        0    12956 2023-06-21 08:17:56.339418 openborders-0.1.1/openborders/data.py
--rw-r--r--   0        0        0    10585 2023-06-21 12:14:22.711631 openborders-0.1.1/openborders/indices.py
--rw-r--r--   0        0        0      400 2023-06-20 20:08:55.357752 openborders-0.1.1/openborders/utils.py
--rw-r--r--   0        0        0     1086 2023-06-21 12:48:30.887388 openborders-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      895 2023-06-21 12:18:59.512183 openborders-0.1.1/README.md
--rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 openborders-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      202 2023-06-21 05:01:43.184465 openborders-0.1.1.post0/openborders/__init__.py
+-rw-r--r--   0        0        0     5511 2023-06-21 12:12:49.976324 openborders-0.1.1.post0/openborders/cli.py
+-rw-r--r--   0        0        0    12956 2023-06-21 08:17:56.339418 openborders-0.1.1.post0/openborders/data.py
+-rw-r--r--   0        0        0    10585 2023-06-21 12:14:22.711631 openborders-0.1.1.post0/openborders/indices.py
+-rw-r--r--   0        0        0      400 2023-06-20 20:08:55.357752 openborders-0.1.1.post0/openborders/utils.py
+-rw-r--r--   0        0        0     1092 2023-06-21 12:55:49.396528 openborders-0.1.1.post0/pyproject.toml
+-rw-r--r--   0        0        0      895 2023-06-21 12:18:59.512183 openborders-0.1.1.post0/README.md
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 openborders-0.1.1.post0/PKG-INFO
```

### Comparing `openborders-0.1.1/openborders/cli.py` & `openborders-0.1.1.post0/openborders/cli.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1/openborders/data.py` & `openborders-0.1.1.post0/openborders/data.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1/openborders/indices.py` & `openborders-0.1.1.post0/openborders/indices.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1/pyproject.toml` & `openborders-0.1.1.post0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openborders"
-version = "0.1.1"
+version = "0.1.1-post0"
 description = ""
 authors = ["arnos-stuff <mail@arnov.dev>"]
 readme = "README.md"
 homepage = "https://arnos-stuff.github.io/open-borders-index"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `openborders-0.1.1/README.md` & `openborders-0.1.1.post0/README.md`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1/PKG-INFO` & `openborders-0.1.1.post0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openborders
-Version: 0.1.1
+Version: 0.1.1.post0
 Summary: 
 Home-page: https://arnos-stuff.github.io/open-borders-index
 Author: arnos-stuff
 Author-email: mail@arnov.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

