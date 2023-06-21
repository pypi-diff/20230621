# Comparing `tmp/pytest_yls-1.3.3.tar.gz` & `tmp/pytest_yls-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_yls-1.3.3.tar", max compression
+gzip compressed data, was "pytest_yls-1.3.4.tar", max compression
```

## Comparing `pytest_yls-1.3.3.tar` & `pytest_yls-1.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1082 2023-03-29 10:25:36.935449 pytest_yls-1.3.3/LICENSE
--rw-r--r--   0        0        0     1614 2023-03-29 10:25:36.939450 pytest_yls-1.3.3/README.md
--rw-r--r--   0        0        0      531 2023-03-29 10:29:15.370526 pytest_yls-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      340 2023-03-29 10:25:36.939450 pytest_yls-1.3.3/pytest_yls/__init__.py
--rw-r--r--   0        0        0    10120 2023-03-29 10:25:36.939450 pytest_yls-1.3.3/pytest_yls/plugin.py
--rw-r--r--   0        0        0        0 2023-03-29 10:25:36.943450 pytest_yls-1.3.3/pytest_yls/py.typed
--rw-r--r--   0        0        0     1833 2023-03-29 10:25:36.943450 pytest_yls-1.3.3/pytest_yls/utils.py
--rw-r--r--   0        0        0     2311 1970-01-01 00:00:00.000000 pytest_yls-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-03-29 10:25:36.935449 pytest_yls-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1614 2023-03-29 10:25:36.939450 pytest_yls-1.3.4/README.md
+-rw-r--r--   0        0        0      531 2023-06-21 11:24:57.574555 pytest_yls-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-03-29 10:25:36.939450 pytest_yls-1.3.4/pytest_yls/__init__.py
+-rw-r--r--   0        0        0    10120 2023-04-03 12:54:48.417380 pytest_yls-1.3.4/pytest_yls/plugin.py
+-rw-r--r--   0        0        0        0 2023-03-29 10:25:36.943450 pytest_yls-1.3.4/pytest_yls/py.typed
+-rw-r--r--   0        0        0     1833 2023-03-31 16:56:48.407085 pytest_yls-1.3.4/pytest_yls/utils.py
+-rw-r--r--   0        0        0     2311 1970-01-01 00:00:00.000000 pytest_yls-1.3.4/PKG-INFO
```

### Comparing `pytest_yls-1.3.3/LICENSE` & `pytest_yls-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_yls-1.3.3/README.md` & `pytest_yls-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pytest_yls-1.3.3/pyproject.toml` & `pytest_yls-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-yls"
-version = "1.3.3"
+version = "1.3.4"
 description = "Pytest plugin to test the YLS as a whole."
 authors = ["Matej Kastak <matej.kastak@avast.com>"]
 maintainers = ["Matej Kašťák <matej.kastak@avast.com>"]
 readme = "README.md"
 license = "MIT"
 include = ["py.typed", "LICENSE"]
```

### Comparing `pytest_yls-1.3.3/pytest_yls/plugin.py` & `pytest_yls-1.3.4/pytest_yls/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_yls-1.3.3/pytest_yls/utils.py` & `pytest_yls-1.3.4/pytest_yls/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_yls-1.3.3/PKG-INFO` & `pytest_yls-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yls
-Version: 1.3.3
+Version: 1.3.4
 Summary: Pytest plugin to test the YLS as a whole.
 License: MIT
 Author: Matej Kastak
 Author-email: matej.kastak@avast.com
 Maintainer: Matej Kašťák
 Maintainer-email: matej.kastak@avast.com
 Requires-Python: >=3.8,<3.12
```

