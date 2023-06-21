# Comparing `tmp/mozilla-taskgraph-0.1.0.tar.gz` & `tmp/mozilla-taskgraph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-taskgraph-0.1.0.tar", last modified: Wed Jun 21 14:40:09 2023, max compression
+gzip compressed data, was "mozilla-taskgraph-0.1.1.tar", last modified: Wed Jun 21 16:25:39 2023, max compression
```

## Comparing `mozilla-taskgraph-0.1.0.tar` & `mozilla-taskgraph-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 14:40:09.358873 mozilla-taskgraph-0.1.0/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-04-05 14:08:49.000000 mozilla-taskgraph-0.1.0/LICENSE
--rw-r--r--   0 ahal      (1000) ahal      (1000)      659 2023-06-21 14:40:09.358873 mozilla-taskgraph-0.1.0/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)      243 2023-06-16 21:02:54.000000 mozilla-taskgraph-0.1.0/README.md
--rw-r--r--   0 ahal      (1000) ahal      (1000)      531 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.0/pyproject.toml
--rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-06-21 14:40:09.358873 mozilla-taskgraph-0.1.0/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1186 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.0/setup.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 14:40:09.358873 mozilla-taskgraph-0.1.0/src/
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 14:40:09.358873 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph/
--rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 14:40:09.358873 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      659 2023-06-21 14:40:09.000000 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)      320 2023-06-21 14:40:09.000000 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-06-21 14:40:09.000000 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       29 2023-06-21 14:40:09.000000 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       18 2023-06-21 14:40:09.000000 mozilla-taskgraph-0.1.0/src/mozilla_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 14:40:09.358873 mozilla-taskgraph-0.1.0/test/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      126 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.0/test/test_version.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-04-05 14:08:49.000000 mozilla-taskgraph-0.1.1/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      659 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1061 2023-06-21 15:31:38.000000 mozilla-taskgraph-0.1.1/README.md
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      531 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.1/pyproject.toml
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1186 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.1/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.104461 mozilla-taskgraph-0.1.1/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-06-21 16:24:47.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:24:47.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/scriptworker/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:24:47.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1993 2023-06-20 19:46:53.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      659 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      490 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       29 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       18 2023-06-21 16:25:39.000000 mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-21 16:25:39.114461 mozilla-taskgraph-0.1.1/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      126 2023-06-21 14:39:06.000000 mozilla-taskgraph-0.1.1/test/test_version.py
```

### Comparing `mozilla-taskgraph-0.1.0/LICENSE` & `mozilla-taskgraph-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-0.1.0/PKG-INFO` & `mozilla-taskgraph-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 0.1.0
+Version: 0.1.1
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mozilla-taskgraph-0.1.0/pyproject.toml` & `mozilla-taskgraph-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-0.1.0/setup.py` & `mozilla-taskgraph-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-0.1.0/src/mozilla_taskgraph.egg-info/PKG-INFO` & `mozilla-taskgraph-0.1.1/src/mozilla_taskgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 0.1.0
+Version: 0.1.1
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

