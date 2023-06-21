# Comparing `tmp/atro-pylog-0.0.2.tar.gz` & `tmp/atro-pylog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pylog-0.0.2.tar", last modified: Sat Jun 17 14:02:03 2023, max compression
+gzip compressed data, was "atro-pylog-0.0.3.tar", last modified: Wed Jun 21 19:47:17 2023, max compression
```

## Comparing `atro-pylog-0.0.2.tar` & `atro-pylog-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-17 14:02:03.139477 atro-pylog-0.0.2/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-17 14:02:03.139477 atro-pylog-0.0.2/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.2/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-17 14:02:03.139477 atro-pylog-0.0.2/atro_pylog.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-17 14:02:03.000000 atro-pylog-0.0.2/atro_pylog.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      248 2023-06-17 14:02:03.000000 atro-pylog-0.0.2/atro_pylog.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-17 14:02:03.000000 atro-pylog-0.0.2/atro_pylog.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-17 14:02:03.000000 atro-pylog-0.0.2/atro_pylog.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-17 14:02:03.139477 atro-pylog-0.0.2/pylog/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      850 2023-06-17 14:01:09.000000 atro-pylog-0.0.2/pylog/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      463 2023-06-17 13:29:38.000000 atro-pylog-0.0.2/pylog/logger.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      371 2023-06-17 13:29:38.000000 atro-pylog-0.0.2/pylog/logger_type.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      567 2023-06-17 13:29:39.000000 atro-pylog-0.0.2/pylog/loguru.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1695 2023-06-17 14:01:23.000000 atro-pylog-0.0.2/pylog/opentelemetry.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-17 14:02:03.139477 atro-pylog-0.0.2/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)      942 2023-06-17 14:01:58.000000 atro-pylog-0.0.2/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.3/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/atro_pylog.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      333 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       91 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/pylog/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1225 2023-06-21 19:43:16.000000 atro-pylog-0.0.3/pylog/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      855 2023-06-21 19:15:38.000000 atro-pylog-0.0.3/pylog/level.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      968 2023-06-21 19:45:29.000000 atro-pylog-0.0.3/pylog/logger_base.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      371 2023-06-21 19:10:23.000000 atro-pylog-0.0.3/pylog/logger_type.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      992 2023-06-21 19:43:59.000000 atro-pylog-0.0.3/pylog/loguru_logger.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     2175 2023-06-21 19:32:22.000000 atro-pylog-0.0.3/pylog/opentelemetry_logger.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      492 2023-06-21 19:31:58.000000 atro-pylog-0.0.3/pylog/settings.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1118 2023-06-21 19:47:00.000000 atro-pylog-0.0.3/setup.py
```

### Comparing `atro-pylog-0.0.2/PKG-INFO` & `atro-pylog-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.2/atro_pylog.egg-info/PKG-INFO` & `atro-pylog-0.0.3/atro_pylog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.2/setup.py` & `atro-pylog-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pylog",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
+    install_requires=[
+        "loguru",
+        "opentelemetry-api",
+        "opentelemetry-exporter-otlp-proto-grpc",
+        "opentelemetry-sdk",
+        "pydantic",
+    ],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

