# Comparing `tmp/vanna-0.0.1.tar.gz` & `tmp/vanna-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.1.tar", last modified: Sat May 13 19:29:29 2023, max compression
+gzip compressed data, was "vanna-0.0.2.tar", last modified: Wed Jun 21 20:17:00 2023, max compression
```

## Comparing `vanna-0.0.1.tar` & `vanna-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:29:29.591415 vanna-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-13 19:29:18.000000 vanna-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-13 19:29:29.591415 vanna-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 19:29:18.000000 vanna-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-13 19:29:18.000000 vanna-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 19:29:29.591415 vanna-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:29:29.591415 vanna-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:29:29.591415 vanna-0.0.1/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-13 19:29:18.000000 vanna-0.0.1/src/vanna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:29:29.591415 vanna-0.0.1/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-13 19:29:29.000000 vanna-0.0.1/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-13 19:29:29.000000 vanna-0.0.1/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 19:29:29.000000 vanna-0.0.1/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-13 19:29:29.000000 vanna-0.0.1/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.824407 vanna-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 20:16:48.000000 vanna-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 20:17:00.824407 vanna-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 20:16:48.000000 vanna-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-21 20:16:48.000000 vanna-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:17:00.824407 vanna-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.820407 vanna-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.824407 vanna-0.0.2/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-21 20:16:48.000000 vanna-0.0.2/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-21 20:16:48.000000 vanna-0.0.2/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.824407 vanna-0.0.2/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.1/LICENSE` & `vanna-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.1/PKG-INFO` & `vanna-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vanna-0.0.1/src/vanna.egg-info/PKG-INFO` & `vanna-0.0.2/src/vanna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

