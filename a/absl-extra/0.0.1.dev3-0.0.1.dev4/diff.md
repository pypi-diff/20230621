# Comparing `tmp/absl_extra-0.0.1.dev3.tar.gz` & `tmp/absl_extra-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.1.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.1.dev4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.1.dev3.tar` & `absl_extra-0.0.1.dev4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1578 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/Readme.md
--rw-r--r--   0        0        0       61 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/__init__.py
--rw-r--r--   0        0        0     1443 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/logging_utils.py
--rw-r--r--   0        0        0     2487 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/notifier.py
--rw-r--r--   0        0        0     3654 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/tasks.py
--rw-r--r--   0        0        0     4474 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/absl_extra/tf_utils.py
--rw-r--r--   0        0        0      880 2023-06-21 21:15:16.707316 absl_extra-0.0.1.dev3/pyproject.toml
--rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 absl_extra-0.0.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1578 2023-06-21 21:34:04.643204 absl_extra-0.0.1.dev4/Readme.md
+-rw-r--r--   0        0        0       61 2023-06-21 21:34:04.643204 absl_extra-0.0.1.dev4/absl_extra/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-21 21:34:04.643204 absl_extra-0.0.1.dev4/absl_extra/logging_utils.py
+-rw-r--r--   0        0        0     2487 2023-06-21 21:34:04.643204 absl_extra-0.0.1.dev4/absl_extra/notifier.py
+-rw-r--r--   0        0        0     3654 2023-06-21 21:34:04.643204 absl_extra-0.0.1.dev4/absl_extra/tasks.py
+-rw-r--r--   0        0        0     4474 2023-06-21 21:34:04.643204 absl_extra-0.0.1.dev4/absl_extra/tf_utils.py
+-rw-r--r--   0        0        0      880 2023-06-21 21:34:04.643204 absl_extra-0.0.1.dev4/pyproject.toml
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 absl_extra-0.0.1.dev4/PKG-INFO
```

### Comparing `absl_extra-0.0.1.dev3/Readme.md` & `absl_extra-0.0.1.dev4/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev3/absl_extra/notifier.py` & `absl_extra-0.0.1.dev4/absl_extra/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev3/absl_extra/tasks.py` & `absl_extra-0.0.1.dev4/absl_extra/tasks.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev3/absl_extra/tf_utils.py` & `absl_extra-0.0.1.dev4/absl_extra/tf_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev3/pyproject.toml` & `absl_extra-0.0.1.dev4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.1dev3"
+version = "0.0.1dev4"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.1.dev3/PKG-INFO` & `absl_extra-0.0.1.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

