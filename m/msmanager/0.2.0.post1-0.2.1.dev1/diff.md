# Comparing `tmp/msmanager-0.2.0.post1.tar.gz` & `tmp/msmanager-0.2.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.2.0.post1.tar", max compression
+gzip compressed data, was "msmanager-0.2.1.dev1.tar", max compression
```

## Comparing `msmanager-0.2.0.post1.tar` & `msmanager-0.2.1.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.0.post1/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.0.post1/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.0.post1/msmanager/__main__.py
--rw-r--r--   0        0        0     5968 2023-05-17 21:50:42.885439 msmanager-0.2.0.post1/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.0.post1/msmanager/config.py
--rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.2.0.post1/msmanager/exceptions.py
--rw-r--r--   0        0        0     3552 2023-06-13 10:23:19.562135 msmanager-0.2.0.post1/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.0.post1/msmanager/models.py
--rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.0.post1/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.0.post1/msmanager/types.py
--rw-r--r--   0        0        0      533 2023-05-17 21:01:49.385592 msmanager-0.2.0.post1/msmanager/units.py
--rw-r--r--   0        0        0      553 2023-06-13 10:24:03.935209 msmanager-0.2.0.post1/pyproject.toml
--rw-r--r--   0        0        0      565 2023-05-16 18:14:53.984547 msmanager-0.2.0.post1/README.md
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 msmanager-0.2.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.1.dev1/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.1.dev1/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.1.dev1/msmanager/__main__.py
+-rw-r--r--   0        0        0     5968 2023-06-21 13:00:00.586899 msmanager-0.2.1.dev1/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.1.dev1/msmanager/config.py
+-rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.2.1.dev1/msmanager/exceptions.py
+-rw-r--r--   0        0        0     3570 2023-06-21 12:56:23.279871 msmanager-0.2.1.dev1/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.1.dev1/msmanager/models.py
+-rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.1.dev1/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.1.dev1/msmanager/types.py
+-rw-r--r--   0        0        0      533 2023-05-17 21:01:49.385592 msmanager-0.2.1.dev1/msmanager/units.py
+-rw-r--r--   0        0        0      552 2023-06-21 13:03:32.126797 msmanager-0.2.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      565 2023-05-16 18:14:53.984547 msmanager-0.2.1.dev1/README.md
+-rw-r--r--   0        0        0     1369 1970-01-01 00:00:00.000000 msmanager-0.2.1.dev1/PKG-INFO
```

### Comparing `msmanager-0.2.0.post1/LICENSE` & `msmanager-0.2.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.0.post1/msmanager/cli.py` & `msmanager-0.2.1.dev1/msmanager/cli.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.0.post1/msmanager/config.py` & `msmanager-0.2.1.dev1/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.0.post1/msmanager/exceptions.py` & `msmanager-0.2.1.dev1/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.0.post1/msmanager/functions.py` & `msmanager-0.2.1.dev1/msmanager/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # ! Standart Functions
 def replaces(string: str, replaceble: Dict[str, str]) -> str:
     for __old, __new in replaceble.items():
         string = string.replace(__old, __new)
     return string
 
 def rich_exception(exception: Exception) -> str:
-    return f"[red]{exception.__class__.__name__}:[/] {' '.join(exception.args)}"
+    return f"[red]{exception.__class__.__name__}:[/] {' '.join([str(i) for i in exception.args])}"
 
 def endicext(string: str) -> str:
     return string + ("[/]" * string.count("]"))
 
 # ! Server Functions
 def wait_start_server(
     server_host: str,
```

### Comparing `msmanager-0.2.0.post1/msmanager/msm.py` & `msmanager-0.2.1.dev1/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.0.post1/msmanager/units.py` & `msmanager-0.2.1.dev1/msmanager/units.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.0.post1/pyproject.toml` & `msmanager-0.2.1.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.2.0.post1"
+version = "0.2.1.dev1"
 description = "Manager for managing Mindusrty servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
```

### Comparing `msmanager-0.2.0.post1/README.md` & `msmanager-0.2.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.0.post1/PKG-INFO` & `msmanager-0.2.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.2.0.post1
+Version: 0.2.1.dev1
 Summary: Manager for managing Mindusrty servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

