# Comparing `tmp/iracing_client-0.1.1.tar.gz` & `tmp/iracing_client-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iracing_client-0.1.1.tar", max compression
+gzip compressed data, was "iracing_client-0.1.1a0.tar", max compression
```

## Comparing `iracing_client-0.1.1.tar` & `iracing_client-0.1.1a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-20 21:10:25.258376 iracing_client-0.1.1/LICENSE
--rw-r--r--   0        0        0     3403 2023-06-20 21:10:25.258376 iracing_client-0.1.1/README.md
--rw-r--r--   0        0        0      575 2023-06-20 21:10:25.258376 iracing_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/__init__.py
--rw-r--r--   0        0        0     4606 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/auth.py
--rw-r--r--   0        0        0        0 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/data/__init__.py
--rw-r--r--   0        0        0     2937 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/data/common.py
--rw-r--r--   0        0        0     2785 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/data/constants.py
--rw-r--r--   0        0        0     9927 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/data/league.py
--rw-r--r--   0        0        0     5450 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/data/member.py
--rw-r--r--   0        0        0      562 2023-06-20 21:10:25.258376 iracing_client-0.1.1/src/iracing_client/trace.py
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 iracing_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/LICENSE
+-rw-r--r--   0        0        0     3403 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/README.md
+-rw-r--r--   0        0        0      581 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/__init__.py
+-rw-r--r--   0        0        0     4606 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/auth.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/data/__init__.py
+-rw-r--r--   0        0        0     2937 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/data/common.py
+-rw-r--r--   0        0        0     2785 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/data/constants.py
+-rw-r--r--   0        0        0     9927 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/data/league.py
+-rw-r--r--   0        0        0     5450 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/data/member.py
+-rw-r--r--   0        0        0      562 2023-06-21 21:28:44.263715 iracing_client-0.1.1a0/src/iracing_client/trace.py
+-rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 iracing_client-0.1.1a0/PKG-INFO
```

### Comparing `iracing_client-0.1.1/LICENSE` & `iracing_client-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/README.md` & `iracing_client-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/pyproject.toml` & `iracing_client-0.1.1a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iracing-client"
-version = "0.1.1"
+version = "0.1.1-alpha"
 description = ""
 authors = ["James Carter <tegatai@gmail.com>"]
 readme = "README.md"
 packages = [{include = "src/iracing_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `iracing_client-0.1.1/src/iracing_client/auth.py` & `iracing_client-0.1.1a0/src/iracing_client/auth.py`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/src/iracing_client/data/common.py` & `iracing_client-0.1.1a0/src/iracing_client/data/common.py`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/src/iracing_client/data/constants.py` & `iracing_client-0.1.1a0/src/iracing_client/data/constants.py`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/src/iracing_client/data/league.py` & `iracing_client-0.1.1a0/src/iracing_client/data/league.py`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/src/iracing_client/data/member.py` & `iracing_client-0.1.1a0/src/iracing_client/data/member.py`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/src/iracing_client/trace.py` & `iracing_client-0.1.1a0/src/iracing_client/trace.py`

 * *Files identical despite different names*

### Comparing `iracing_client-0.1.1/PKG-INFO` & `iracing_client-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iracing-client
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: 
 Author: James Carter
 Author-email: tegatai@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

