# Comparing `tmp/openmock-2.3.2.tar.gz` & `tmp/openmock-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmock-2.3.2.tar", max compression
+gzip compressed data, was "openmock-2.3.3.tar", max compression
```

## Comparing `openmock-2.3.2.tar` & `openmock-2.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1081 2023-06-19 17:10:42.530135 openmock-2.3.2/LICENSE
--rw-r--r--   0        0        0     4946 2023-06-19 17:10:42.530135 openmock-2.3.2/README.md
--rw-r--r--   0        0        0      830 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/__init__.py
--rw-r--r--   0        0        0      121 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/behaviour/__init__.py
--rw-r--r--   0        0        0      475 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/behaviour/server_failure.py
--rw-r--r--   0        0        0     1100 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/fake_cluster.py
--rw-r--r--   0        0        0     1179 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/fake_indices.py
--rw-r--r--   0        0        0    40327 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/fake_opensearch.py
--rw-r--r--   0        0        0     2154 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/normalize_hosts.py
--rw-r--r--   0        0        0      732 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/utilities/__init__.py
--rw-r--r--   0        0        0      451 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/utilities/decorator.py
--rw-r--r--   0        0        0     2302 2023-06-19 17:10:42.530135 openmock-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-21 14:12:04.681585 openmock-2.3.3/LICENSE
+-rw-r--r--   0        0        0     4946 2023-06-21 14:12:04.681585 openmock-2.3.3/README.md
+-rw-r--r--   0        0        0      830 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/behaviour/__init__.py
+-rw-r--r--   0        0        0      475 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/behaviour/server_failure.py
+-rw-r--r--   0        0        0     1100 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/fake_cluster.py
+-rw-r--r--   0        0        0     1179 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/fake_indices.py
+-rw-r--r--   0        0        0    40327 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/fake_opensearch.py
+-rw-r--r--   0        0        0     2154 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/normalize_hosts.py
+-rw-r--r--   0        0        0      732 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/utilities/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-21 14:12:04.681585 openmock-2.3.3/openmock/utilities/decorator.py
+-rw-r--r--   0        0        0     2302 2023-06-21 14:12:04.681585 openmock-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.3/PKG-INFO
```

### Comparing `openmock-2.3.2/LICENSE` & `openmock-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/README.md` & `openmock-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/openmock/__init__.py` & `openmock-2.3.3/openmock/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/openmock/fake_cluster.py` & `openmock-2.3.3/openmock/fake_cluster.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/openmock/fake_indices.py` & `openmock-2.3.3/openmock/fake_indices.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/openmock/fake_opensearch.py` & `openmock-2.3.3/openmock/fake_opensearch.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/openmock/normalize_hosts.py` & `openmock-2.3.3/openmock/normalize_hosts.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/openmock/utilities/__init__.py` & `openmock-2.3.3/openmock/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.2/pyproject.toml` & `openmock-2.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmock"
-version = "2.3.2"
+version = "2.3.3"
 description = "Python OpenSearch Mock for test purposes"
 authors = ["Marcos Cardoso",
     "Mathew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["opensearch", "mocking", "testing"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/matthewdeanmartin/openmock"
```

### Comparing `openmock-2.3.2/PKG-INFO` & `openmock-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmock
-Version: 2.3.2
+Version: 2.3.3
 Summary: Python OpenSearch Mock for test purposes
 Home-page: https://github.com/matthewdeanmartin/openmock
 License: MIT
 Keywords: opensearch,mocking,testing
 Author: Marcos Cardoso
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
```

