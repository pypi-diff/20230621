# Comparing `tmp/euclipy-0.3.1.tar.gz` & `tmp/euclipy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euclipy-0.3.1.tar", last modified: Sat Mar 11 22:33:38 2023, max compression
+gzip compressed data, was "euclipy-1.0.0.tar", last modified: Wed Jun 21 01:36:42 2023, max compression
```

## Comparing `euclipy-0.3.1.tar` & `euclipy-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 cvaron    (1000) cvaron    (1000)        0 2023-03-11 22:33:38.665521 euclipy-0.3.1/
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     1051 2023-02-21 00:57:43.000000 euclipy-0.3.1/LICENSE.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       73 2023-02-21 00:57:43.000000 euclipy-0.3.1/MANIFEST.in
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     2111 2023-03-11 22:33:38.665521 euclipy-0.3.1/PKG-INFO
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     1422 2023-03-11 22:33:08.000000 euclipy-0.3.1/README.md
-drwxr-xr-x   0 cvaron    (1000) cvaron    (1000)        0 2023-03-11 22:33:38.665521 euclipy-0.3.1/docs/
-drwxr-xr-x   0 cvaron    (1000) cvaron    (1000)        0 2023-03-11 22:33:38.665521 euclipy-0.3.1/docs/changelog/
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       53 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.0.1-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       77 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.0.2-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       74 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.0.3-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      119 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.1.0-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       50 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.1.1-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       63 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.0-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       60 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.1-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       60 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.10-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       52 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.11-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       96 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.12-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       99 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.13-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       95 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.2-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       70 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.3-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       53 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.4-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      110 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.5-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      205 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.6-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       62 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.7.changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       59 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.8-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       59 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/changelog/0.2.9-changelog.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     1925 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/conf.py
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      574 2023-02-21 00:57:43.000000 euclipy-0.3.1/docs/theorems.txt
-drwxr-xr-x   0 cvaron    (1000) cvaron    (1000)        0 2023-03-11 22:33:38.665521 euclipy-0.3.1/euclipy/
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)        0 2023-02-21 00:57:43.000000 euclipy-0.3.1/euclipy/__init__.py
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)    21541 2023-03-10 23:55:52.000000 euclipy-0.3.1/euclipy/core.py
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      745 2023-03-01 23:38:01.000000 euclipy-0.3.1/euclipy/exceptions.py
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     2819 2023-03-11 00:16:27.000000 euclipy-0.3.1/euclipy/polygon.py
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      471 2023-03-10 23:40:01.000000 euclipy-0.3.1/euclipy/theorems.py
-drwxr-xr-x   0 cvaron    (1000) cvaron    (1000)        0 2023-03-11 22:33:38.665521 euclipy-0.3.1/euclipy.egg-info/
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     2111 2023-03-11 22:33:38.000000 euclipy-0.3.1/euclipy.egg-info/PKG-INFO
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     1069 2023-03-11 22:33:38.000000 euclipy-0.3.1/euclipy.egg-info/SOURCES.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)        1 2023-03-11 22:33:38.000000 euclipy-0.3.1/euclipy.egg-info/dependency_links.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)        6 2023-03-11 22:33:38.000000 euclipy-0.3.1/euclipy.egg-info/requires.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)        8 2023-03-11 22:33:38.000000 euclipy-0.3.1/euclipy.egg-info/top_level.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      108 2023-02-21 00:57:43.000000 euclipy-0.3.1/notes.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)        5 2023-02-21 00:57:43.000000 euclipy-0.3.1/requirements.txt
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       38 2023-03-11 22:33:38.665521 euclipy-0.3.1/setup.cfg
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)      940 2023-03-11 22:33:06.000000 euclipy-0.3.1/setup.py
-drwxr-xr-x   0 cvaron    (1000) cvaron    (1000)        0 2023-03-11 22:33:38.665521 euclipy-0.3.1/tests/
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)       25 2023-02-21 00:57:44.000000 euclipy-0.3.1/tests/__init__.py
--rw-r--r--   0 cvaron    (1000) cvaron    (1000)     8613 2023-03-10 23:47:02.000000 euclipy-0.3.1/tests/test_object_framework.py
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1051 2023-03-18 23:11:56.000000 euclipy-1.0.0/LICENSE.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       73 2023-03-18 23:11:56.000000 euclipy-1.0.0/MANIFEST.in
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2121 2023-06-21 01:36:42.970635 euclipy-1.0.0/PKG-INFO
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1422 2023-03-18 23:11:56.000000 euclipy-1.0.0/README.md
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.960635 euclipy-1.0.0/docs/
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/docs/changelog/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       53 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.0.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       77 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.0.2-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       74 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.0.3-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      119 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.1.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       50 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.1.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       63 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       60 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       60 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.10-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       52 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.11-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       96 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.12-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       99 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.13-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       95 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.2-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       70 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.3-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       53 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.4-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      110 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.5-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      205 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.6-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       62 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.7.changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       59 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.8-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       59 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.2.9-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      236 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.3.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      102 2023-03-18 23:11:56.000000 euclipy-1.0.0/docs/changelog/0.3.1-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      553 2023-06-21 01:31:45.000000 euclipy-1.0.0/docs/changelog/1.0.0-changelog.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1924 2023-06-21 01:20:42.000000 euclipy-1.0.0/docs/conf.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      397 2023-06-21 01:26:36.000000 euclipy-1.0.0/docs/theorems.txt
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/euclipy/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-03-18 23:11:56.000000 euclipy-1.0.0/euclipy/__init__.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    17167 2023-05-30 17:15:14.000000 euclipy-1.0.0/euclipy/core.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)      783 2023-03-19 02:51:14.000000 euclipy-1.0.0/euclipy/exceptions.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    18193 2023-06-21 01:06:56.000000 euclipy-1.0.0/euclipy/geometricobjects.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2962 2023-06-21 00:46:34.000000 euclipy-1.0.0/euclipy/polygon.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1875 2023-06-21 01:17:17.000000 euclipy-1.0.0/euclipy/theorems.py
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/euclipy.egg-info/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     2121 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/PKG-INFO
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1213 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        1 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        6 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/requires.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        8 2023-06-21 01:36:42.000000 euclipy-1.0.0/euclipy.egg-info/top_level.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)        5 2023-03-18 23:11:56.000000 euclipy-1.0.0/requirements.txt
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       38 2023-06-21 01:36:42.970635 euclipy-1.0.0/setup.cfg
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1016 2023-06-21 01:25:03.000000 euclipy-1.0.0/setup.py
+drwxr-xr-x   0 joshuavaron  (1000) joshuavaron  (1000)        0 2023-06-21 01:36:42.970635 euclipy-1.0.0/tests/
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)       27 2023-03-18 23:11:56.000000 euclipy-1.0.0/tests/__init__.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)    19121 2023-06-21 00:46:04.000000 euclipy-1.0.0/tests/test_object_framework.py
+-rw-r--r--   0 joshuavaron  (1000) joshuavaron  (1000)     1588 2023-06-21 01:18:03.000000 euclipy-1.0.0/tests/test_proofs.py
```

### Comparing `euclipy-0.3.1/LICENSE.txt` & `euclipy-1.0.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 Joshua Varon
+Copyright 2023 Joshua Varon
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `euclipy-0.3.1/PKG-INFO` & `euclipy-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: euclipy
-Version: 0.3.1
-Summary: A Euclidean Geometry based library
+Version: 1.0.0
+Summary: A Synthetic Euclidean Geometry based library
 Home-page: 
 Author: Joshua Varon
 Author-email: 32440072+joshuavaron@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://joshuavaron.github.io/euclipy/
 Project-URL: Source Code, https://github.com/joshuavaron/euclipy
 Keywords: geometry,math
```

### Comparing `euclipy-0.3.1/README.md` & `euclipy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `euclipy-0.3.1/docs/conf.py` & `euclipy-1.0.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'Euclipy'
 copyright = '2022, Joshua Varon'
 author = 'Joshua Varon'
 
 # The full version, including alpha/beta/rc tags
-release = '0.2.11'
+release = '1.0.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `euclipy-0.3.1/euclipy/core.py` & `euclipy-1.0.0/euclipy/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,67 +5,125 @@
 
 Typical usage example:
 
     TODO: Provide code example once euclipy can solve some non-trivial problems
 """
 
 import collections
-import functools
 import itertools
 import pprint
 
 import sympy
 
 from euclipy import exceptions
 
 class RegisteredObject:
     """Base class for all euclipy objects that need to be tracked by the central
     registry.
     """
     # Instance methods for initializing/registering and deregistering objects
+    def __new__(cls) -> None:
+        obj = super().__new__(cls)
+        obj._successor = None
+        return obj
 
     def __init__(self, *_args, **_kwargs) -> None:
         """Add object to registry if not already registered
         """
         # __init__ will still be called after __new__ for subclasses that return
         # a previously-created object.  In that case, object should not be
         # initialized/registered again.
         if not hasattr(self, '_registered'):
+            self._successor = None
             # If object lacks a key, use an automatically generated key instead
-            if not hasattr(self, 'key'):
+            if not hasattr(self, '_key'):
                 self.key = self.auto_key()
             self.register()
+            self._callbacks = []
             super().__init__()
 
+    def __getattribute__(self, name):
+        successor = object.__getattribute__(self, '_successor')
+        if successor and name != '_successor' and name != '_predecessor':
+            return getattr(successor, name)
+        return object.__getattribute__(self, name)
+
+    @property
+    def _identifier(self): #pragma: no cover
+        raise NotImplementedError
+
+    @property
+    def key(self):
+        """Key for object in registry
+        """
+        return self._key
+
+    @key.setter
+    def key(self, value):
+        """Set key for object in registry
+        """
+        check_registry = hasattr(self, '_key')
+        self._key = value
+        if check_registry: # pragma: no cover TODO: Remove this line once implemented
+            for obj in self.elements():
+                # TODO: Need to find objects with same obj.key but different key in the registry
+                # TODO: Merging of objects need to fire callbacks to replace all
+                    # references to deregistered objects with surviving object
+                pass
+
     def register(self):
         """Add object to the registry.
         """
         self.get_registry()[self.key] = self
         self._registered = True
 
-    def deregister(self, successor):
-        """Remove object from the registry.
+    def update_key(self, new_key):
+        """Update key for object in registry
         """
+        if self.key != new_key:
+            obj_with_new_key = self.get_registry().get(new_key)
+            if obj_with_new_key:
+                self.replace(obj_with_new_key)
+            else:
+                self.get_registry().pop(self.key)
+                self.key = new_key
+                self.register()
+                self.broadcast_change(None)
+
+    def broadcast_change(self, successor):
+        for callback in self._callbacks:
+            callback(self, successor)
+            if successor:
+                successor.call_when_changed(callback)
+
+    def replace(self, successor):
         assert type(self) is type(successor)
+        # Broadcast replacement to all callbacks
+        self.broadcast_change(successor)
+        # Set successor and deregister self
         self.get_registry().pop(self.key)
-        self.successor = successor
-        successor.predecessor = self
+        successor._predecessor = self
         del self._registered
+        self._successor = successor
+        # TODO: Should also clean up registry
+
+    def call_when_changed(self, callback):
+        self._callbacks.append(callback)
 
     # Class methods for class-level registries
 
     @classmethod
     def auto_key(cls):
         """Automatically generate an integer key for an object of cls
         
         Returns:
             Auto-incremented integer key for object, unique only among
             instances of the same class (not unique among subclasses)
         """
-
+        # TODO: There may not be users of auto_key left.  Consider removing
         if '_auto_key_counter' not in cls.__dict__:
             cls._auto_key_counter = 0
         cls._auto_key_counter += 1
         return cls._auto_key_counter
 
     @classmethod
     def get_registry(cls):
@@ -92,14 +150,31 @@
         """Iterator for all registered elements of cls and its subclasses
         """
         own = cls.elements()
         subs = (_.elements_recursive() for _ in cls.__subclasses__())
         return itertools.chain(own, itertools.chain.from_iterable(subs))
 
     @classmethod
+    def remove_duplicates(cls):
+        sig_obj_map = collections.defaultdict(list)
+        for obj in cls.elements():
+            sig_obj_map[obj._identifier].append(obj)
+        dup_objs_list = [objlist for objlist in sig_obj_map.values() if len(objlist) > 1]
+        if len(dup_objs_list) > 0:
+            assert len(dup_objs_list) == 1
+            dup_objs = dup_objs_list[0]
+            retain = dup_objs[0]
+            for obj in dup_objs[1:]:
+                if issubclass(type(obj), MeasurableGeometricObject):
+                    obj.measure = retain.measure
+                obj.replace(retain)
+            retain.broadcast_change(None)
+            return retain
+
+    @classmethod
     def reset_registry(cls):
         """Reset registry to empty dict
         """
         for _cls in cls.__subclasses__():
             _cls.reset_registry()
         if '_registry' in cls.__dict__:
             del cls._registry
@@ -127,26 +202,37 @@
 class Expression(RegisteredObject):
     """Algebraic expressions and functionality to solve system of equations
     
     TODO: It is possible to insert two equivalent expressions into the registry.
     This can be avoided by prempting instantiation and testing for each
     registered non-zero expression e whether sympy.simplify(e.expr - expr) == 0
     """
+    def __new__(cls, expr, predecessor=None, substitutions=None) -> None:
+        del expr, predecessor, substitutions
+        return super().__new__(cls)
+
     def __init__(self, expr, predecessor=None, substitutions=None) -> None:
         assert isinstance(expr, sympy.Expr)
         self.expr = expr
         if substitutions:
             assert isinstance(substitutions, dict)
         self.substitutions = substitutions
         if predecessor:
-            predecessor.deregister(successor=self)
+            predecessor.replace(successor=self)
         else:
-            self.predecessor = None
+            self._predecessor = None
         super().__init__()
 
+    def __getattribute__(self, name):
+        return object.__getattribute__(self, name)
+
+    @property
+    def _identifier(self):
+        return self.expr
+
     def subs(self, replacements):
         """Make substitutions from replacements in expression (self.expr)
         
         Args:
             replacements: dict mapping sympy symbols to substitutions, e.g.,
                 {x: 3, y: 5}
         
@@ -163,17 +249,17 @@
         if result == self.expr:
             return self
         if result == 0 or len(result.free_symbols) > 0:
             return Expression(result, predecessor=self, substitutions=replacements)
         raise exceptions.SystemOfEquationsError('Expression without free \
             symbols cannot evaluate to a non-zero value.')
 
-    def __repr__(self) -> str:
-        if self.predecessor:
-            rep = ', predecessor=' + repr(self.predecessor)
+    def __repr__(self) -> str: # pragma: no cover
+        if self._predecessor:
+            rep = ', predecessor=' + repr(self._predecessor)
         else:
             rep = ''
         if self.substitutions:
             sub = ', substitutions=' + repr(self.substitutions)
         else:
             sub = ''
         return f'{self.__class__.__name__}({self.expr}{rep}{sub})'
@@ -188,21 +274,32 @@
         # Iterate over list(cls.elements()), because loop changes cls._registry
         for expr in list(cls.elements()):
             expr.subs(replacements)
 
     @classmethod
     def solve_system(cls):
         """Solve expressions for positive values.
-        Raise exception if any variable has a unique non-positive solution.
-        Raise an exception if any variable with non-unique solutions has zero or
-        more than one positive solutions."""
+
+        Returns:
+            - dict mapping symbols to values of solutions
+            - empty dict if no unsolved expressions exist
+            - empty dict system cannot yet be solved but there are no inconsistencies
+        Raises: SystemOfEquationsError if
+            - any variable has a unique non-positive solution.
+            - any variable with non-unique solutions has zero or more than one positive solutions.
+            - the system cannot have any solutions
+        """
 
         # Find valid solutions to the system of equuations, if any
         unsolved = [e for e in cls.elements() if e.expr != 0]
+        if not unsolved:
+            return {}
         solutions = sympy.solve([e.expr for e in unsolved], dict=True)
+        if not solutions:
+            raise exceptions.SystemOfEquationsError('Unsolved expressions with no solution.')
         uniques = set.intersection(*[set(sol.items()) for sol in solutions])
         non_uniques = [set(sol.items()) - uniques for sol in solutions]
         uniques = dict(uniques)
         # Create list of dicts with common keys
         non_uniques = [dict(non_unique) for non_unique in non_uniques]
         uniques_without_free_symbols = {k:v for k, v in uniques.items()
                                         if not v.free_symbols}
@@ -234,21 +331,21 @@
         valid_solutions = uniques_without_free_symbols | non_uniques_solution
 
         # Substitute valid_solutions for variables in expressions
         for expr in unsolved:
             expr = expr.subs(valid_solutions)
         for sym, val in valid_solutions.items():
             MeasurableGeometricObject.substitute_measure_symbol(sym, val)
+        return valid_solutions
 
 
-class GeometricObject (RegisteredObject):
+class GeometricObject(RegisteredObject):
     """Base class for all geometric objects
     """
 
-
 class MeasurableGeometricObject(GeometricObject):
     """Base class for all geometric objects that can be measured
     """
     def __init__(self, *_args, **_kwargs):
         if not hasattr(self, '_measure'):
             self._measure = None
         super().__init__()
@@ -297,16 +394,18 @@
         """Set the measure for object without performing any of the other
         actions that @measure.setter performs. Generally intended for
         class-internal use.
         """
         if measure is None:
             self._measure = self.auto_measure_symbol()
         else:
-            isinstance(measure, (sympy.Symbol, sympy.Number))
-            self._measure = measure
+            if isinstance(measure, (sympy.Symbol, sympy.Number)):
+                self._measure = measure
+            else:
+                raise ValueError(f'Cannot set measure to {measure}.')
 
     @property
     def measure(self):
         """Getter property of measurable objects; creates measure if needed
         """
         if not self.has_measure:
             self.set_measure()
@@ -316,262 +415,37 @@
     def measure(self, new):
         '''
         new can be one of the following:
         - a number (instance of numbers.Numbers)
         - a sympy number (instnace of sympy.Number)
         - a sympy symbol (instance of sympy.Symbol)
         '''
+        #TODO: Add support for different numeric types
         try:
             new = sympy.sympify(new)
         except sympy.SympifyError as exc:
             raise ValueError(f'Cannot set measure to {new}.') from exc
+        if not isinstance(new, (sympy.Symbol, sympy.Number)):
+            raise ValueError(f'Cannot set measure to {new}.')
 
         if self.has_measure:
             old = self._measure
             if isinstance(old, sympy.Symbol):
                 self.substitute_measure_symbol(old, new)
                 Expression.subs_all_expressions({old: new})
-            elif isinstance(old, sympy.Number):
+            else: # old is a sympy.Number
                 if isinstance(new, sympy.Symbol):
                     self.substitute_measure_symbol(new, old)
                     Expression.subs_all_expressions({new: old})
                 elif isinstance(new, sympy.Number):
                     if new != old:
                         raise ValueError(f'Cannot set measure to {new}, \
                             because it is already set to {old}.')
-            else:
-                raise TypeError(f'Cannot set measure to {new}.')
         else:
             self.set_measure(new)
 
-
-@functools.total_ordering
-class Point(GeometricObject):
-    """A point on the Euclidean plane
-    
-    Represents a point on the Euclidean plane, identified by a string label not
-    containing spaces. Upon instantiation, Points are registered in the global
-    registry. Therefore, subsequent attempts to instantiate Point objects with
-    the same label simply return the existing Point object with that label.
-    
-    >>> Point('A') is Point ('A')
-    True
-    
-    Attributes:
-        label: string label not containing spaces
-        key: label is used as the key in the registry
-    """
-    def __new__(cls, label: str):
-        if not isinstance(label, str):
-            raise ValueError('Points require string labels.')
-        registered_point = cls.get(label)
-        if registered_point:
-            return registered_point
-        return cls.__construct(label)
-
-    @classmethod
-    def __construct(cls, label: str):
-        """Create new Point instance
-        
-        Args:
-            label: non-empty string not containing spaces
-            
-        Raises:
-            ValueError if label is empty or contains spaces
-        """
-        if label == '':
-            raise ValueError('Empty string is not a valid Point label.')
-        if ' ' in label:
-            raise ValueError('Spaces are not permitted in Point labels.')
-        obj = super().__new__(cls)
-        obj.key = label
-        obj._pred = set()
-        obj._op = Point.__construct
-        return obj
-
-    def __lt__(self, obj):
-        return self.key < obj.key
-
-    def __eq__(self, obj):
-        return self.key == obj.key
-
-    def __hash__(self):
-        return hash(self.key)
-
-    def __repr__(self) -> str:
-        """Provides string represetnation of point, e.g. 'Point(A)'
-        """
-        return f'{self.__class__.__name__}({self.key})'
-
-def points(pts):
-    """Provides standard representation of point(s) from multiple inputs
-            
-    Args:
-        pts: Point, tuple of Points, or space-delimited point label(s)
-        
-    Returns:
-        Point instance or a tuple of Point instances
-    
-    Raises:
-        ValueError if pts is an invalid representation of point(s)
-
-    Typical use:
-
-    >>> points(Point('A'))
-    Point(A)
-    >>> points('A')
-    Point(A)
-    >>> points((Point('A'), Point('B')))
-    (Point(A), Point(B))
-    >>> points('A B')
-    (Point(A), Point(B))    
-    """
-    if isinstance(pts, Point):
-        return pts
-    if isinstance(pts, str):
-        pts = tuple(Point(pt_label) for pt_label in pts.split(' '))
-    if not (isinstance(pts, tuple) and all(isinstance(p, Point) for p in pts)):
-        raise ValueError('Invalid representation of point(s) as input')
-    if len(pts) != len(set(pts)):
-        raise ValueError('Points are not all distinct')
-    if len(pts) == 1:
-        return pts[0]
-    return pts
-
-
-class Line(GeometricObject):
-    """A line represented by ordered colinear points on the Euclidean plan
-    
-    Attributes:
-        points: tuple of Points, as ordered on the line they are a part of
-    """
-    def __new__(cls, pts):
-        pts = points(pts)
-        if not (isinstance(pts, tuple) and len(pts) > 1):
-            raise ValueError('Instantiating a Line requires >= 2 points.')
-        reg_common_pts = [obj for obj in cls.elements()
-                          if len(set(obj.points).intersection(set(pts))) > 1]
-        if reg_common_pts:
-            for registered in reg_common_pts:
-                pts = cls.bidirectional_order_preserving_merge(registered.points, pts)
-            pts = cls.canonical_ordering(pts)
-            retain = reg_common_pts[0]
-            if pts == retain.points:
-                return retain
-            # Some points have been merged from one or more existing lines from the registry
-            remove = reg_common_pts[1:]
-            retain.points = pts
-            for obj in remove:
-                obj.deregister()
-            return retain
-        # No existing line has two or more points in common with the new line;
-        # create a new line instance
-        obj = super().__new__(cls)
-        obj.points = cls.canonical_ordering(pts)
-        return obj
-
-    def __repr__(self) -> str:
-        return f'{self.__class__.__name__}({" ".join([p.key for p in self.points])})'
-
-    @staticmethod
-    def canonical_ordering(pts):
-        """Canonical ordering of segment endpoints by lexical ordering"""
-        if pts[0] < pts[-1]:
-            return pts
-        return tuple(reversed(pts))
-
-    @staticmethod
-    def bidirectional_order_preserving_merge(s_a, s_b):
-        """Merges two sequences of points, if they can be consistently aligned
-        """
-        def order_preserving_merge(s_a, s_b):
-            if len(s_a) == 0:
-                return tuple(s_b)
-            if len(s_b) == 0:
-                return tuple(s_a)
-            if s_a[0] == s_b[0]:
-                return (s_a[0],) + tuple(order_preserving_merge(s_a[1:], s_b[1:]))
-            if s_a[0] in s_b:
-                return (s_b[0],) + tuple(order_preserving_merge(s_a, s_b[1:]))
-            if s_b[0] in s_a:
-                return (s_a[0],) + tuple(order_preserving_merge(s_a[1:], s_b))
-            # Neither of the first elements are common among the two tuples
-            raise exceptions.ColinearPointSequenceError(
-                'Order of sequences ambiguous.', s_a, s_b)
-
-        common_ordered_as_s_a = tuple(e for e in s_a if e in s_b)
-        if len(common_ordered_as_s_a) < 2:
-            raise exceptions.ColinearPointSequenceError(
-                'Sequences have fewer than two points in common.', s_a, s_b)
-        common_ordered_as_s_b = tuple(e for e in s_b if e in s_a)
-        if common_ordered_as_s_a == common_ordered_as_s_b:
-            return order_preserving_merge(tuple(s_a), tuple(s_b))
-        if common_ordered_as_s_a == tuple(reversed(common_ordered_as_s_b)):
-            return order_preserving_merge(tuple(s_a), tuple(reversed(s_b)))
-        raise exceptions.ColinearPointSequenceError(
-            'Sequences cannot be aligned consistently.', tuple(s_a), tuple(s_b))
-
-    def segments_with_subsegments(self):
-        """All segments contained in the line that have subsegments
-        """
-        pts = self.points
-        num_pts = len(pts)
-        return [Segment((pts[i], pts[i+k]))
-                for k in range(2, num_pts)
-                for i in range(num_pts-k)]
-
-
-class Segment(MeasurableGeometricObject):
-    """A segment represented by its two endpoints on the Euclidean plane
-    """
-    def __new__(cls, pts):
-        '''Argument endpoints is one of the following:
-        - a space separated pair of point labels representing a segment, e.g. 'B A'
-        - a tuple of two Point objects'''
-        pts = points(pts)
-        if not (isinstance(pts, tuple) and len(pts) == 2):
-            raise ValueError('Instantiating a Segment requires exactly 2 points.')
-        # Determine canonical ordering of points (lexical for Segments)
-        ordered_pts = tuple(sorted(pts))
-        # Construct key based on canonically ordered points
-        canonical_key = ' '.join([p.key for p in ordered_pts])
-        # If Segment with canonical_key is already registered, return it
-        registered = cls.get(canonical_key)
-        if registered:
-            return registered
-        return cls.__construct(canonical_key, ordered_pts)
-
-    @classmethod
-    def __construct(cls, key, ordered_pts):
-        obj = super().__new__(cls)
-        obj.points = ordered_pts
-        obj.key = key
-        obj._pred = set(ordered_pts)
-        obj._op = Segment.__construct
-        return obj
-
-    def __repr__(self) -> str:
+    def __repr__(self) -> str: # pragma: no cover
         measure = ', measure=' + repr(self.measure) if self.has_measure else ''
         return f'{self.__class__.__name__}({self.key}{measure})'
 
-    @property
-    def line(self):
-        """Returns the Line that segment lies on
-        """
-        return Line(self.points)
-
-    def atomic_subsegments(self):
-        """Returns a list of all atomic subsegments of the segment
-        
-        Atomic subsegments are subsegments that do not contain other subsegments
-        of the segment.
-        """
-        line_pts = self.line.points
-        pt_l, pt_r = self.points
-        idx_l, idx_r = line_pts.index(pt_l), line_pts.index(pt_r)
-        seg_pts = line_pts[idx_l:idx_r+1]
-        return [Segment((seg_pts[i], seg_pts[i+1]))
-                for i in range(len(seg_pts)-1)]
-
-
 if __name__ == '__main__':
     pass
```

### Comparing `euclipy-0.3.1/euclipy/polygon.py` & `euclipy-1.0.0/euclipy/polygon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Classes representing polygons on the Euclidean plane
 """
-from euclipy.core import GeometricObject, Segment, points
+from euclipy.core import GeometricObject
+from euclipy.geometricobjects import Segment, Angle, points
 
 class Polygon(GeometricObject):
     """A polygon represented by its vertices on the Euclidean plane
     """
     def __new__(cls, pts):
         """Find or construct new Polygon
 
@@ -32,34 +33,33 @@
                                     if set(obj.points) == set(canonical_pts)]
         if existing_with_shared_pts:
             assert len(existing_with_shared_pts) == 1
             # TODO: Replace with custom error InconsistentConstructionError
             raise RuntimeError('Polygon inconsistent with existing polygon.')
         # Create new instance
         return cls.__construct(key, canonical_pts)
-        # obj = super().__new__(cls)
-        # obj.points = canonical_pts
-        # obj.key = key
-        # obj.segments = [Segment((p1, p2)) for p1, p2
-        #                 in zip(obj.points, obj.points[1:] + (obj.points[0],))]
-        # return obj
 
     @classmethod
     def __construct(cls, key, canonical_pts):
         obj = super().__new__(cls)
         obj.key = key
         obj.points = canonical_pts
+        circular_points = obj.points + obj.points[:2]
+        obj.angles = []
+        for i in range(len(obj.points)):
+            obj.angles.append(
+                Angle((circular_points[i], circular_points[i+1], circular_points[i+2])))
         obj.segments = [Segment((p1, p2)) for p1, p2
                         in zip(obj.points, obj.points[1:] + (obj.points[0],))]
-        obj._pred = set(obj.segments)
-        obj._op = cls.__construct
+        # obj._pred = set(obj.segments)
+        # obj._op = cls.__construct
         return obj
 
 
-    def __repr__(self):
+    def __repr__(self): # pragma: no cover
         return f'{self.__class__.__name__}({" ".join([p.key for p in self.points])})'
 
     @staticmethod
     def canonical_points(pts):
         """Provide canonical ordering of points for Polygon
 
         Starts with the lexically smallest point label and preserves order,
@@ -72,8 +72,12 @@
         return pts[min_point_index:] + pts[:min_point_index]
 
 
 class Triangle(Polygon):
     """A triangle represented by its three vertices on the Euclidean plane
     """
     def __new__(cls, pts):
+        return cls.__construct(points(pts))
+
+    @classmethod
+    def __construct(cls, pts):
         return super().__new__(cls, pts)
```

### Comparing `euclipy-0.3.1/euclipy.egg-info/PKG-INFO` & `euclipy-1.0.0/euclipy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: euclipy
-Version: 0.3.1
-Summary: A Euclidean Geometry based library
+Version: 1.0.0
+Summary: A Synthetic Euclidean Geometry based library
 Home-page: 
 Author: Joshua Varon
 Author-email: 32440072+joshuavaron@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://joshuavaron.github.io/euclipy/
 Project-URL: Source Code, https://github.com/joshuavaron/euclipy
 Keywords: geometry,math
```

### Comparing `euclipy-0.3.1/euclipy.egg-info/SOURCES.txt` & `euclipy-1.0.0/euclipy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-notes.txt
 requirements.txt
 setup.py
 docs/conf.py
 docs/theorems.txt
 docs/changelog/0.0.1-changelog.txt
 docs/changelog/0.0.2-changelog.txt
 docs/changelog/0.0.3-changelog.txt
@@ -21,19 +20,24 @@
 docs/changelog/0.2.3-changelog.txt
 docs/changelog/0.2.4-changelog.txt
 docs/changelog/0.2.5-changelog.txt
 docs/changelog/0.2.6-changelog.txt
 docs/changelog/0.2.7.changelog.txt
 docs/changelog/0.2.8-changelog.txt
 docs/changelog/0.2.9-changelog.txt
+docs/changelog/0.3.0-changelog.txt
+docs/changelog/0.3.1-changelog.txt
+docs/changelog/1.0.0-changelog.txt
 euclipy/__init__.py
 euclipy/core.py
 euclipy/exceptions.py
+euclipy/geometricobjects.py
 euclipy/polygon.py
 euclipy/theorems.py
 euclipy.egg-info/PKG-INFO
 euclipy.egg-info/SOURCES.txt
 euclipy.egg-info/dependency_links.txt
 euclipy.egg-info/requires.txt
 euclipy.egg-info/top_level.txt
 tests/__init__.py
-tests/test_object_framework.py
+tests/test_object_framework.py
+tests/test_proofs.py
```

### Comparing `euclipy-0.3.1/setup.py` & `euclipy-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+"""Euclipy - a symbolic Euclidean geometry package
+"""
 from setuptools import setup, find_packages
- 
+
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Education',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='euclipy',
-  version='0.3.1',
-  description='A Euclidean Geometry based library',
-  long_description=open('README.md').read(),
+  version='1.0.0',
+  description='A Synthetic Euclidean Geometry based library',
+  long_description=open('README.md', encoding='utf-8').read(),
   long_description_content_type='text/markdown',
   url='',
   project_urls={
             #"Bug Tracker": "",
             "Documentation": "https://joshuavaron.github.io/euclipy/",
             "Source Code": "https://github.com/joshuavaron/euclipy",
         },
-  author='Joshua Varon',    
+  author='Joshua Varon',
   author_email='32440072+joshuavaron@users.noreply.github.com',
-  license='MIT', 
+  license='MIT',
   classifiers=classifiers,
   keywords='geometry, math',
   packages=find_packages(include=['euclipy']),
-  install_requires=['sympy'] 
+  install_requires=['sympy']
 )
```

