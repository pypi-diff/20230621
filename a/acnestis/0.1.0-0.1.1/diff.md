# Comparing `tmp/acnestis-0.1.0.tar.gz` & `tmp/acnestis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acnestis-0.1.0.tar", max compression
+gzip compressed data, was "acnestis-0.1.1.tar", max compression
```

## Comparing `acnestis-0.1.0.tar` & `acnestis-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      145 2023-06-18 16:18:08.342043 acnestis-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-20 13:57:53.944053 acnestis-0.1.0/acnestis/__init__.py
--rw-r--r--   0        0        0     3529 2023-06-18 16:16:33.816675 acnestis-0.1.0/acnestis/command.py
--rw-r--r--   0        0        0      951 2023-06-14 04:04:41.253079 acnestis-0.1.0/acnestis/processing.py
--rw-r--r--   0        0        0     5745 2023-06-18 14:23:59.172269 acnestis-0.1.0/acnestis/steps.py
--rw-r--r--   0        0        0      769 2023-06-18 16:17:22.225705 acnestis-0.1.0/acnestis/yaml.py
--rw-r--r--   0        0        0      619 2023-06-18 14:23:16.851439 acnestis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 acnestis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6770 2023-06-21 18:50:59.994964 acnestis-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:53.944053 acnestis-0.1.1/acnestis/__init__.py
+-rw-r--r--   0        0        0     3529 2023-06-18 16:16:33.816675 acnestis-0.1.1/acnestis/command.py
+-rw-r--r--   0        0        0      951 2023-06-14 04:04:41.253079 acnestis-0.1.1/acnestis/processing.py
+-rw-r--r--   0        0        0     5745 2023-06-18 14:23:59.172269 acnestis-0.1.1/acnestis/steps.py
+-rw-r--r--   0        0        0      769 2023-06-18 16:17:22.225705 acnestis-0.1.1/acnestis/yaml.py
+-rw-r--r--   0        0        0      619 2023-06-21 18:49:18.735646 acnestis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 acnestis-0.1.1/PKG-INFO
```

### Comparing `acnestis-0.1.0/acnestis/command.py` & `acnestis-0.1.1/acnestis/command.py`

 * *Files identical despite different names*

### Comparing `acnestis-0.1.0/acnestis/processing.py` & `acnestis-0.1.1/acnestis/processing.py`

 * *Files identical despite different names*

### Comparing `acnestis-0.1.0/acnestis/steps.py` & `acnestis-0.1.1/acnestis/steps.py`

 * *Files identical despite different names*

### Comparing `acnestis-0.1.0/acnestis/yaml.py` & `acnestis-0.1.1/acnestis/yaml.py`

 * *Files identical despite different names*

### Comparing `acnestis-0.1.0/pyproject.toml` & `acnestis-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acnestis"
-version = "0.1.0"
+version = "0.1.1"
 description = "data collection, aggregation and convertion tool"
 authors = ["oduvan <a.lyabah@checkio.org>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/oduvan/acnestis"
 
 [tool.poetry.dependencies]
```

