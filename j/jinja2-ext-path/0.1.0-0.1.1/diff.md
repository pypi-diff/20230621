# Comparing `tmp/jinja2_ext_path-0.1.0.tar.gz` & `tmp/jinja2_ext_path-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_ext_path-0.1.0.tar", max compression
+gzip compressed data, was "jinja2_ext_path-0.1.1.tar", max compression
```

## Comparing `jinja2_ext_path-0.1.0.tar` & `jinja2_ext_path-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-06-20 15:23:28.897264 jinja2_ext_path-0.1.0/README.md
--rw-r--r--   0        0        0       42 2023-06-20 16:09:59.656031 jinja2_ext_path-0.1.0/jinja2_ext_path/__init__.py
--rw-r--r--   0        0        0      525 2023-06-20 15:30:51.795105 jinja2_ext_path-0.1.0/jinja2_ext_path/path_extension.py
--rw-r--r--   0        0        0      428 2023-06-20 15:56:49.347511 jinja2_ext_path-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 jinja2_ext_path-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-20 15:23:28.897264 jinja2_ext_path-0.1.1/README.md
+-rw-r--r--   0        0        0       42 2023-06-20 16:09:59.656031 jinja2_ext_path-0.1.1/jinja2_ext_path/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-20 15:30:51.795105 jinja2_ext_path-0.1.1/jinja2_ext_path/path_extension.py
+-rw-r--r--   0        0        0      464 2023-06-21 09:32:06.391991 jinja2_ext_path-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 jinja2_ext_path-0.1.1/PKG-INFO
```

### Comparing `jinja2_ext_path-0.1.0/README.md` & `jinja2_ext_path-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jinja2_ext_path-0.1.0/jinja2_ext_path/path_extension.py` & `jinja2_ext_path-0.1.1/jinja2_ext_path/path_extension.py`

 * *Files identical despite different names*

### Comparing `jinja2_ext_path-0.1.0/PKG-INFO` & `jinja2_ext_path-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: jinja2-ext-path
-Version: 0.1.0
+Version: 0.1.1
 Summary: Filters from `os.path` for jinja2
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 # jinja2-ext-path
 
     $ pip install jinja2-ext-path
```

