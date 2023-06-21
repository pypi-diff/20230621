# Comparing `tmp/pipebuilder-0.1.2.tar.gz` & `tmp/pipebuilder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipebuilder-0.1.2.tar", last modified: Wed Jun 21 06:06:09 2023, max compression
+gzip compressed data, was "pipebuilder-0.1.3.tar", last modified: Wed Jun 21 06:24:23 2023, max compression
```

## Comparing `pipebuilder-0.1.2.tar` & `pipebuilder-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1073 2023-06-18 06:27:57.093129 pipebuilder-0.1.2/LICENSE
--rw-r--r--   0        0        0       13 2023-06-21 05:35:12.714940 pipebuilder-0.1.2/README.md
--rw-r--r--   0        0        0     1056 2023-06-21 06:06:09.474669 pipebuilder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 pipebuilder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-18 06:27:57.093129 pipebuilder-0.1.3/LICENSE
+-rw-r--r--   0        0        0       13 2023-06-21 05:35:12.714940 pipebuilder-0.1.3/README.md
+-rw-r--r--   0        0        0     1097 2023-06-21 06:24:23.522493 pipebuilder-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 pipebuilder-0.1.3/PKG-INFO
```

### Comparing `pipebuilder-0.1.2/LICENSE` & `pipebuilder-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipebuilder-0.1.2/pyproject.toml` & `pipebuilder-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [project]
 name = "pipebuilder"
-version = "0.1.2"
+version = "0.1.3"
 description = "Use LLMs to build pipelines to connect systems."
 authors = [
     { name = "Doug Hudgeon", email = "doug.hudgeon@managedfunctions.com" },
 ]
+packages = [
+    "core",
+    "clouds",
+]
 dependencies = [
     "amazon-textract-textractor",
     "arrow",
     "boto3",
     "botocore",
     "click",
     "dateparser",
```

### Comparing `pipebuilder-0.1.2/PKG-INFO` & `pipebuilder-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipebuilder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use LLMs to build pipelines to connect systems.
 Author-Email: Doug Hudgeon <doug.hudgeon@managedfunctions.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: amazon-textract-textractor
 Requires-Dist: arrow
 Requires-Dist: boto3
```

