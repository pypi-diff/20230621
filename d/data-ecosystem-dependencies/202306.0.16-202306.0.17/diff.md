# Comparing `tmp/data_ecosystem_dependencies-202306.0.16.tar.gz` & `tmp/data_ecosystem_dependencies-202306.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_dependencies-202306.0.16.tar", max compression
+gzip compressed data, was "data_ecosystem_dependencies-202306.0.17.tar", max compression
```

## Comparing `data_ecosystem_dependencies-202306.0.16.tar` & `data_ecosystem_dependencies-202306.0.17.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      842 2023-06-20 16:20:32.826916 data_ecosystem_dependencies-202306.0.16/data_ecosystem_dependencies/__init__.py
--rw-r--r--   0        0        0    11357 2023-06-20 16:20:32.826916 data_ecosystem_dependencies-202306.0.16/license.md
--rw-r--r--   0        0        0     2740 2023-06-20 16:24:40.007613 data_ecosystem_dependencies-202306.0.16/pyproject.toml
--rw-r--r--   0        0        0      341 2023-06-20 16:20:32.826916 data_ecosystem_dependencies-202306.0.16/readme.md
--rw-r--r--   0        0        0      160 2023-06-20 16:20:32.826916 data_ecosystem_dependencies-202306.0.16/setup.cfg
--rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.16/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-06-20 23:46:46.930116 data_ecosystem_dependencies-202306.0.17/data_ecosystem_dependencies/__init__.py
+-rw-r--r--   0        0        0    11357 2023-06-20 23:46:46.930116 data_ecosystem_dependencies-202306.0.17/license.md
+-rw-r--r--   0        0        0     2740 2023-06-20 23:51:06.961419 data_ecosystem_dependencies-202306.0.17/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-06-20 23:46:46.930116 data_ecosystem_dependencies-202306.0.17/readme.md
+-rw-r--r--   0        0        0      160 2023-06-20 23:46:46.930116 data_ecosystem_dependencies-202306.0.17/setup.cfg
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.17/PKG-INFO
```

### Comparing `data_ecosystem_dependencies-202306.0.16/data_ecosystem_dependencies/__init__.py` & `data_ecosystem_dependencies-202306.0.17/data_ecosystem_dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.16/license.md` & `data_ecosystem_dependencies-202306.0.17/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.16/pyproject.toml` & `data_ecosystem_dependencies-202306.0.17/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="data_ecosystem_dependencies"
-version="202306.0.16"
+version="202306.0.17"
 description="Data Ecosystem  Dependencies - Python (PADE)"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://github.com/cdcent/data_ecosystem_services"
 repository="https://github.com/cdcent/data_ecosystem_services"
 classifiers=[
```

### Comparing `data_ecosystem_dependencies-202306.0.16/PKG-INFO` & `data_ecosystem_dependencies-202306.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-dependencies
-Version: 202306.0.16
+Version: 202306.0.17
 Summary: Data Ecosystem  Dependencies - Python (PADE)
 Home-page: https://github.com/cdcent/data_ecosystem_services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

