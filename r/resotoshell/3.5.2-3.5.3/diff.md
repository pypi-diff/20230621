# Comparing `tmp/resotoshell-3.5.2.tar.gz` & `tmp/resotoshell-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.5.2.tar", last modified: Tue Jun 13 13:07:41 2023, max compression
+gzip compressed data, was "resotoshell-3.5.3.tar", last modified: Wed Jun 21 14:21:48 2023, max compression
```

## Comparing `resotoshell-3.5.2.tar` & `resotoshell-3.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:10.000000 resotoshell-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 13:07:41.479379 resotoshell-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 13:03:10.000000 resotoshell-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-13 13:03:10.000000 resotoshell-3.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37345 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:33.000000 resotoshell-3.5.2/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 13:07:41.479379 resotoshell-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 13:03:10.000000 resotoshell-3.5.2/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-06-13 13:03:10.000000 resotoshell-3.5.2/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-13 13:03:10.000000 resotoshell-3.5.2/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.309282 resotoshell-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:17:48.000000 resotoshell-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-21 14:21:48.309282 resotoshell-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-21 14:17:48.000000 resotoshell-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-21 14:17:48.000000 resotoshell-3.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.305282 resotoshell-3.5.3/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37345 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.309282 resotoshell-3.5.3/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:00.000000 resotoshell-3.5.3/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 14:21:48.309282 resotoshell-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.309282 resotoshell-3.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-21 14:17:48.000000 resotoshell-3.5.3/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-06-21 14:17:48.000000 resotoshell-3.5.3/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-21 14:17:48.000000 resotoshell-3.5.3/test/test_protected_files.py
```

### Comparing `resotoshell-3.5.2/PKG-INFO` & `resotoshell-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.2
+Version: 3.5.3
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.5.2/README.md` & `resotoshell-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.2/pyproject.toml` & `resotoshell-3.5.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotoshell"
-version = "3.5.2"
+version = "3.5.3"
 authors = [{name="Some Engineering Inc."}]
 description = "Commandline interpreter to interact with Resoto."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["cloud security"]
 
 dependencies = [
-    "resotolib==3.5.2",
+    "resotolib==3.5.3",
     "prompt-toolkit",
     "rich",
     "resotoclient",
     "aiohttp[speedups]",
 ]
 
 [project.scripts]
```

### Comparing `resotoshell-3.5.2/resotoshell/__main__.py` & `resotoshell-3.5.3/resotoshell/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.2/resotoshell/authorized_client.py` & `resotoshell-3.5.3/resotoshell/authorized_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             if decoded.get("exp", 0) > time.time():
                 return method, jwt_token
         return None
 
     def write(self) -> None:
         if self.dirty:
             self.path.parent.mkdir(mode=0o700, parents=True, exist_ok=True)
-            with open(os.open(self.path, os.O_CREAT | os.O_WRONLY, 0o600), "w+", encoding="utf-8") as f:
+            with open(os.open(self.path, os.O_CREAT | os.O_WRONLY | os.O_TRUNC, 0o600), "w+", encoding="utf-8") as f:
                 self.config.write(f)
 
     @staticmethod
     def default() -> ReshConfig:
         return ReshConfig(Path.home() / ".resoto" / "resh.ini")
```

### Comparing `resotoshell-3.5.2/resotoshell/promptsession.py` & `resotoshell-3.5.3/resotoshell/promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.2/resotoshell/protected_files.py` & `resotoshell-3.5.3/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.2/resotoshell/shell.py` & `resotoshell-3.5.3/resotoshell/shell.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.2/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.5.3/resotoshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.2
+Version: 3.5.3
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.5.2/resotoshell.egg-info/SOURCES.txt` & `resotoshell-3.5.3/resotoshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.2/test/test_promptsession.py` & `resotoshell-3.5.3/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.2/test/test_protected_files.py` & `resotoshell-3.5.3/test/test_protected_files.py`

 * *Files identical despite different names*

