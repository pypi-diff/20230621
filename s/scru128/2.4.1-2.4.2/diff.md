# Comparing `tmp/scru128-2.4.1.tar.gz` & `tmp/scru128-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scru128-2.4.1.tar", max compression
+gzip compressed data, was "scru128-2.4.2.tar", max compression
```

## Comparing `scru128-2.4.1.tar` & `scru128-2.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2021-09-26 06:39:06.272667 scru128-2.4.1/LICENSE
--rw-r--r--   0        0        0     2491 2023-04-07 13:48:09.594211 scru128-2.4.1/README.md
--rw-r--r--   0        0        0      678 2023-04-07 13:48:09.594923 scru128-2.4.1/pyproject.toml
--rw-r--r--   0        0        0    14816 2023-03-22 22:42:55.073908 scru128-2.4.1/scru128/__init__.py
--rw-r--r--   0        0        0     2134 2022-10-30 06:25:18.337374 scru128-2.4.1/scru128/cli/__init__.py
--rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 scru128-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-09-26 06:39:06.272667 scru128-2.4.2/LICENSE
+-rw-r--r--   0        0        0     2491 2023-06-21 12:08:42.459984 scru128-2.4.2/README.md
+-rw-r--r--   0        0        0      678 2023-06-21 12:13:46.779623 scru128-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0    14816 2023-06-21 12:08:42.461854 scru128-2.4.2/scru128/__init__.py
+-rw-r--r--   0        0        0     2134 2022-10-30 06:25:18.337374 scru128-2.4.2/scru128/cli/__init__.py
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 scru128-2.4.2/PKG-INFO
```

### Comparing `scru128-2.4.1/LICENSE` & `scru128-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scru128-2.4.1/README.md` & `scru128-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `scru128-2.4.1/pyproject.toml` & `scru128-2.4.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scru128"
-version = "2.4.1"
+version = "2.4.2"
 description = "SCRU128: Sortable, Clock and Random number-based Unique identifier"
 license = "Apache-2.0"
 authors = ["LiosK <contact@mail.liosk.net>"]
 readme = "README.md"
 homepage = "https://github.com/scru128/python"
 keywords = ["identifier", "uuid", "guid", "ulid", "ksuid"]
 classifiers = ["Operating System :: OS Independent"]
@@ -14,12 +14,12 @@
 scru128-inspect = "scru128.cli:inspect"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
-mypy = "^1.2.0"
+mypy = "^1.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `scru128-2.4.1/scru128/__init__.py` & `scru128-2.4.2/scru128/__init__.py`

 * *Files identical despite different names*

### Comparing `scru128-2.4.1/scru128/cli/__init__.py` & `scru128-2.4.2/scru128/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `scru128-2.4.1/PKG-INFO` & `scru128-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scru128
-Version: 2.4.1
+Version: 2.4.2
 Summary: SCRU128: Sortable, Clock and Random number-based Unique identifier
 Home-page: https://github.com/scru128/python
 License: Apache-2.0
 Keywords: identifier,uuid,guid,ulid,ksuid
 Author: LiosK
 Author-email: contact@mail.liosk.net
 Requires-Python: >=3.7,<4.0
```

