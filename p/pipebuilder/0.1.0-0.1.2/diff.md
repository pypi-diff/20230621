# Comparing `tmp/pipebuilder-0.1.0.tar.gz` & `tmp/pipebuilder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipebuilder-0.1.0.tar", last modified: Sun Jun 18 06:59:17 2023, max compression
+gzip compressed data, was "pipebuilder-0.1.2.tar", last modified: Wed Jun 21 06:06:09 2023, max compression
```

## Comparing `pipebuilder-0.1.0.tar` & `pipebuilder-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1073 2023-06-18 06:27:57.093129 pipebuilder-0.1.0/LICENSE
--rw-r--r--   0        0        0       15 2023-06-18 06:27:57.093434 pipebuilder-0.1.0/README.md
--rw-r--r--   0        0        0     1056 2023-06-18 06:59:17.816965 pipebuilder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 pipebuilder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-18 06:27:57.093129 pipebuilder-0.1.2/LICENSE
+-rw-r--r--   0        0        0       13 2023-06-21 05:35:12.714940 pipebuilder-0.1.2/README.md
+-rw-r--r--   0        0        0     1056 2023-06-21 06:06:09.474669 pipebuilder-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 pipebuilder-0.1.2/PKG-INFO
```

### Comparing `pipebuilder-0.1.0/LICENSE` & `pipebuilder-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipebuilder-0.1.0/pyproject.toml` & `pipebuilder-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pipebuilder"
-version = "0.1.0"
+version = "0.1.2"
 description = "Use LLMs to build pipelines to connect systems."
 authors = [
     { name = "Doug Hudgeon", email = "doug.hudgeon@managedfunctions.com" },
 ]
 dependencies = [
     "amazon-textract-textractor",
     "arrow",
```

### Comparing `pipebuilder-0.1.0/PKG-INFO` & `pipebuilder-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipebuilder
-Version: 0.1.0
+Version: 0.1.2
 Summary: Use LLMs to build pipelines to connect systems.
 Author-Email: Doug Hudgeon <doug.hudgeon@managedfunctions.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: amazon-textract-textractor
 Requires-Dist: arrow
 Requires-Dist: boto3
@@ -39,8 +39,8 @@
 Requires-Dist: sentence-splitter
 Requires-Dist: Unidecode
 Requires-Dist: xlrd
 Requires-Dist: xmltodict
 Requires-Dist: zeep
 Description-Content-Type: text/markdown
 
-# pipegenerator
+# pipebuilder
```

