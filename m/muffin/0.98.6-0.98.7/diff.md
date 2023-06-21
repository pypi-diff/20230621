# Comparing `tmp/muffin-0.98.6.tar.gz` & `tmp/muffin-0.98.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.98.6.tar", max compression
+gzip compressed data, was "muffin-0.98.7.tar", max compression
```

## Comparing `muffin-0.98.6.tar` & `muffin-0.98.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-06-06 06:18:52.842933 muffin-0.98.6/README.rst
--rw-r--r--   0        0        0      982 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/__init__.py
--rw-r--r--   0        0        0     5257 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/app.py
--rw-r--r--   0        0        0       71 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/errors.py
--rw-r--r--   0        0        0     3794 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/manage.py
--rw-r--r--   0        0        0     2857 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/types.py
--rw-r--r--   0        0        0     2888 2023-06-06 06:18:52.842933 muffin-0.98.6/muffin/utils.py
--rw-r--r--   0        0        0     2990 2023-06-06 06:18:52.846933 muffin-0.98.6/pyproject.toml
--rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.6/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-06-21 06:54:54.312661 muffin-0.98.7/README.rst
+-rw-r--r--   0        0        0      982 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/__init__.py
+-rw-r--r--   0        0        0     5257 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/errors.py
+-rw-r--r--   0        0        0     3794 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/handler.py
+-rw-r--r--   0        0        0     8814 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/types.py
+-rw-r--r--   0        0        0     2888 2023-06-21 06:54:54.312661 muffin-0.98.7/muffin/utils.py
+-rw-r--r--   0        0        0     2990 2023-06-21 06:54:54.316661 muffin-0.98.7/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.7/PKG-INFO
```

### Comparing `muffin-0.98.6/README.rst` & `muffin-0.98.7/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/muffin/__init__.py` & `muffin-0.98.7/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/muffin/app.py` & `muffin-0.98.7/muffin/app.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/muffin/errors.py` & `muffin-0.98.7/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/muffin/handler.py` & `muffin-0.98.7/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/muffin/manage.py` & `muffin-0.98.7/muffin/manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             if callable(ctx):
                 ctx = ctx()
             banner += f"Loaded globals: {list(ctx.keys())}\n"
             if ipython:
                 with suppress(ImportError):
                     from IPython.terminal.embed import InteractiveShellEmbed
 
-                    sh = InteractiveShellEmbed(banner1=banner, user_ns=ctx)
+                    sh = InteractiveShellEmbed.instance(banner1=banner, user_ns=ctx)
                     return sh()
 
             code.interact(banner, local=ctx)
 
         self(shell)
 
         def run(host: str = "localhost", port: int = 5000):
```

### Comparing `muffin-0.98.6/muffin/plugins.py` & `muffin-0.98.7/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/muffin/pytest.py` & `muffin-0.98.7/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/muffin/utils.py` & `muffin-0.98.7/muffin/utils.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.6/pyproject.toml` & `muffin-0.98.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.98.6"
+version = "0.98.7"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.98.6/PKG-INFO` & `muffin-0.98.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.98.6
+Version: 0.98.7
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

