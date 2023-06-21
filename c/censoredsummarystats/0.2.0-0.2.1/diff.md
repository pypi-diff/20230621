# Comparing `tmp/censoredsummarystats-0.2.0.tar.gz` & `tmp/censoredsummarystats-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.2.0.tar", max compression
+gzip compressed data, was "censoredsummarystats-0.2.1.tar", max compression
```

## Comparing `censoredsummarystats-0.2.0.tar` & `censoredsummarystats-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       45 2023-06-21 07:54:57.798595 censoredsummarystats-0.2.0/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    56356 2023-06-21 07:54:57.799594 censoredsummarystats-0.2.0/censoredsummarystats/statistics.py
--rw-r--r--   0        0        0     2291 2023-06-21 07:54:57.800594 censoredsummarystats-0.2.0/censoredsummarystats/utils.py
--rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.0/LICENSE
--rw-r--r--   0        0        0      558 2023-06-21 08:21:56.981281 censoredsummarystats-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8308 2023-06-21 07:54:57.797594 censoredsummarystats-0.2.0/README.md
--rw-r--r--   0        0        0     8939 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.1/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0    56356 2023-06-21 07:54:57.799594 censoredsummarystats-0.2.1/censoredsummarystats/statistics.py
+-rw-r--r--   0        0        0     2291 2023-06-21 07:54:57.800594 censoredsummarystats-0.2.1/censoredsummarystats/utils.py
+-rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.1/LICENSE
+-rw-r--r--   0        0        0      558 2023-06-21 09:24:12.923481 censoredsummarystats-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8308 2023-06-21 07:54:57.797594 censoredsummarystats-0.2.1/README.md
+-rw-r--r--   0        0        0     8939 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.1/PKG-INFO
```

### Comparing `censoredsummarystats-0.2.0/censoredsummarystats/statistics.py` & `censoredsummarystats-0.2.1/censoredsummarystats/statistics.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.0/censoredsummarystats/utils.py` & `censoredsummarystats-0.2.1/censoredsummarystats/utils.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.0/LICENSE` & `censoredsummarystats-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.0/pyproject.toml` & `censoredsummarystats-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.2.0"
+version = "0.2.1"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 license = "Apache-2.0"
 packages = [{include = "censoredsummarystats"}]
```

### Comparing `censoredsummarystats-0.2.0/README.md` & `censoredsummarystats-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.0/PKG-INFO` & `censoredsummarystats-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 License: Apache-2.0
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

