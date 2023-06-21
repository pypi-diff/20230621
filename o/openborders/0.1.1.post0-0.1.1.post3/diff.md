# Comparing `tmp/openborders-0.1.1.post0.tar.gz` & `tmp/openborders-0.1.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openborders-0.1.1.post0.tar", max compression
+gzip compressed data, was "openborders-0.1.1.post3.tar", max compression
```

## Comparing `openborders-0.1.1.post0.tar` & `openborders-0.1.1.post3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      202 2023-06-21 05:01:43.184465 openborders-0.1.1.post0/openborders/__init__.py
--rw-r--r--   0        0        0     5511 2023-06-21 12:12:49.976324 openborders-0.1.1.post0/openborders/cli.py
--rw-r--r--   0        0        0    12956 2023-06-21 08:17:56.339418 openborders-0.1.1.post0/openborders/data.py
--rw-r--r--   0        0        0    10585 2023-06-21 12:14:22.711631 openborders-0.1.1.post0/openborders/indices.py
--rw-r--r--   0        0        0      400 2023-06-20 20:08:55.357752 openborders-0.1.1.post0/openborders/utils.py
--rw-r--r--   0        0        0     1092 2023-06-21 12:55:49.396528 openborders-0.1.1.post0/pyproject.toml
--rw-r--r--   0        0        0      895 2023-06-21 12:18:59.512183 openborders-0.1.1.post0/README.md
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 openborders-0.1.1.post0/PKG-INFO
+-rw-r--r--   0        0        0     1735 2023-06-20 22:08:25.003241 openborders-0.1.1.post3/data/gdim.columns.json
+-rw-r--r--   0        0        0      851 2023-06-20 19:26:13.994401 openborders-0.1.1.post3/data/isocodes.csv
+-rw-r--r--   0        0        0      202 2023-06-21 05:01:43.184465 openborders-0.1.1.post3/openborders/__init__.py
+-rw-r--r--   0        0        0     5511 2023-06-21 12:12:49.976324 openborders-0.1.1.post3/openborders/cli.py
+-rw-r--r--   0        0        0    12956 2023-06-21 08:17:56.339418 openborders-0.1.1.post3/openborders/data.py
+-rw-r--r--   0        0        0    10585 2023-06-21 12:14:22.711631 openborders-0.1.1.post3/openborders/indices.py
+-rw-r--r--   0        0        0      499 2023-06-21 14:04:54.128527 openborders-0.1.1.post3/openborders/utils.py
+-rw-r--r--   0        0        0     1206 2023-06-21 14:07:20.813970 openborders-0.1.1.post3/pyproject.toml
+-rw-r--r--   0        0        0      895 2023-06-21 12:18:59.512183 openborders-0.1.1.post3/README.md
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 openborders-0.1.1.post3/PKG-INFO
```

### Comparing `openborders-0.1.1.post0/openborders/cli.py` & `openborders-0.1.1.post3/openborders/cli.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post0/openborders/data.py` & `openborders-0.1.1.post3/openborders/data.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post0/openborders/indices.py` & `openborders-0.1.1.post3/openborders/indices.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post0/pyproject.toml` & `openborders-0.1.1.post3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 [tool.poetry]
 name = "openborders"
-version = "0.1.1-post0"
+version = "0.1.1-post3"
 description = ""
 authors = ["arnos-stuff <mail@arnov.dev>"]
 readme = "README.md"
 homepage = "https://arnos-stuff.github.io/open-borders-index"
 
+include = [
+    "data/gdim.columns.json",
+    "data/isocodes.csv"
+]
+
 [tool.poetry.dependencies]
 python = "^3.11"
 pandas = "^2.0.2"
 wbdata = "^0.3.0"
 typer-tinydb = "^0.1.4"
 numpy = "^1.25.0"
 openpyxl = "^3.1.2"
@@ -26,14 +31,16 @@
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.14.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.16"
 mike = "^1.1.2"
 typer-cli = "^0.0.13"
 mkgendocs = "^0.9.2"
+pillow = "^9.5.0"
+cairosvg = "^2.7.0"
 
 [tool.poetry.scripts]
 opbd = "openborders.cli:app"
 openborders = "openborders.cli:app"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `openborders-0.1.1.post0/README.md` & `openborders-0.1.1.post3/README.md`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post0/PKG-INFO` & `openborders-0.1.1.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openborders
-Version: 0.1.1.post0
+Version: 0.1.1.post3
 Summary: 
 Home-page: https://arnos-stuff.github.io/open-borders-index
 Author: arnos-stuff
 Author-email: mail@arnov.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

