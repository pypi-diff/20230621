# Comparing `tmp/pipebuilder-0.1.4.tar.gz` & `tmp/pipebuilder-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipebuilder-0.1.4.tar", last modified: Wed Jun 21 06:36:17 2023, max compression
+gzip compressed data, was "pipebuilder-0.1.5.tar", last modified: Wed Jun 21 06:39:18 2023, max compression
```

## Comparing `pipebuilder-0.1.4.tar` & `pipebuilder-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-18 06:27:57.093129 pipebuilder-0.1.4/LICENSE
--rw-r--r--   0        0        0       13 2023-06-21 05:35:12.714940 pipebuilder-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-21 06:35:14.335968 pipebuilder-0.1.4/clouds/__init__.py
--rw-r--r--   0        0        0     2115 2023-06-21 06:21:48.685950 pipebuilder-0.1.4/clouds/aws.py
--rw-r--r--   0        0        0     1832 2023-06-21 06:21:48.686128 pipebuilder-0.1.4/clouds/gcp.py
--rw-r--r--   0        0        0        0 2023-06-21 06:35:21.105674 pipebuilder-0.1.4/core/__init__.py
--rw-r--r--   0        0        0     3586 2023-06-21 06:21:48.686365 pipebuilder-0.1.4/core/core.py
--rw-r--r--   0        0        0     1097 2023-06-21 06:36:17.005529 pipebuilder-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 pipebuilder-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-18 06:27:57.093129 pipebuilder-0.1.5/LICENSE
+-rw-r--r--   0        0        0       13 2023-06-21 05:35:12.714940 pipebuilder-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 06:35:14.335968 pipebuilder-0.1.5/clouds/__init__.py
+-rw-r--r--   0        0        0     2115 2023-06-21 06:21:48.685950 pipebuilder-0.1.5/clouds/aws.py
+-rw-r--r--   0        0        0     1832 2023-06-21 06:21:48.686128 pipebuilder-0.1.5/clouds/gcp.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:35:21.105674 pipebuilder-0.1.5/core/__init__.py
+-rw-r--r--   0        0        0     3586 2023-06-21 06:21:48.686365 pipebuilder-0.1.5/core/core.py
+-rw-r--r--   0        0        0     1056 2023-06-21 06:39:18.026059 pipebuilder-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 pipebuilder-0.1.5/PKG-INFO
```

### Comparing `pipebuilder-0.1.4/LICENSE` & `pipebuilder-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pipebuilder-0.1.4/clouds/aws.py` & `pipebuilder-0.1.5/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `pipebuilder-0.1.4/clouds/gcp.py` & `pipebuilder-0.1.5/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `pipebuilder-0.1.4/core/core.py` & `pipebuilder-0.1.5/core/core.py`

 * *Files identical despite different names*

### Comparing `pipebuilder-0.1.4/pyproject.toml` & `pipebuilder-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 [project]
 name = "pipebuilder"
-version = "0.1.4"
+version = "0.1.5"
 description = "Use LLMs to build pipelines to connect systems."
 authors = [
     { name = "Doug Hudgeon", email = "doug.hudgeon@managedfunctions.com" },
 ]
-packages = [
-    "core",
-    "clouds",
-]
 dependencies = [
     "amazon-textract-textractor",
     "arrow",
     "boto3",
     "botocore",
     "click",
     "dateparser",
```

### Comparing `pipebuilder-0.1.4/PKG-INFO` & `pipebuilder-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipebuilder
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use LLMs to build pipelines to connect systems.
 Author-Email: Doug Hudgeon <doug.hudgeon@managedfunctions.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: amazon-textract-textractor
 Requires-Dist: arrow
 Requires-Dist: boto3
```

