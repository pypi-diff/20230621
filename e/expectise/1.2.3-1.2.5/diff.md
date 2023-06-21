# Comparing `tmp/expectise-1.2.3.tar.gz` & `tmp/expectise-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/expectise-1.2.3.tar", last modified: Thu Jan 19 17:31:02 2023, max compression
+gzip compressed data, was "dist/expectise-1.2.5.tar", last modified: Wed Jun 21 13:38:35 2023, max compression
```

## Comparing `expectise-1.2.3.tar` & `expectise-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 17:31:02.981848 expectise-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)      555 2023-01-19 17:31:02.981848 expectise-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-01-19 17:30:42.000000 expectise-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 17:31:02.981848 expectise-1.2.3/expectise/
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-01-19 17:30:42.000000 expectise-1.2.3/expectise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-01-19 17:30:42.000000 expectise-1.2.3/expectise/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-01-19 17:30:42.000000 expectise-1.2.3/expectise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    12382 2023-01-19 17:30:42.000000 expectise-1.2.3/expectise/expect.py
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-01-19 17:30:42.000000 expectise-1.2.3/expectise/expectations.py
--rw-r--r--   0 runner    (1001) docker     (122)     3986 2023-01-19 17:30:42.000000 expectise-1.2.3/expectise/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 17:31:02.981848 expectise-1.2.3/expectise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      555 2023-01-19 17:31:02.000000 expectise-1.2.3/expectise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-19 17:31:02.000000 expectise-1.2.3/expectise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-19 17:31:02.000000 expectise-1.2.3/expectise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-01-19 17:31:02.000000 expectise-1.2.3/expectise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-01-19 17:30:42.000000 expectise-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-01-19 17:31:02.981848 expectise-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-01-19 17:30:42.000000 expectise-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 13:38:35.139940 expectise-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-06-21 13:38:35.139940 expectise-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-06-21 13:38:14.000000 expectise-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 13:38:35.139940 expectise-1.2.5/expectise/
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-21 13:38:14.000000 expectise-1.2.5/expectise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-06-21 13:38:14.000000 expectise-1.2.5/expectise/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-06-21 13:38:14.000000 expectise-1.2.5/expectise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12933 2023-06-21 13:38:14.000000 expectise-1.2.5/expectise/expect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-06-21 13:38:14.000000 expectise-1.2.5/expectise/expectations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-06-21 13:38:14.000000 expectise-1.2.5/expectise/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 13:38:35.139940 expectise-1.2.5/expectise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-06-21 13:38:35.000000 expectise-1.2.5/expectise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-21 13:38:35.000000 expectise-1.2.5/expectise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 13:38:35.000000 expectise-1.2.5/expectise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-21 13:38:35.000000 expectise-1.2.5/expectise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-21 13:38:14.000000 expectise-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-21 13:38:35.143940 expectise-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-06-21 13:38:14.000000 expectise-1.2.5/setup.py
```

### Comparing `expectise-1.2.3/PKG-INFO` & `expectise-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: expectise
-Version: 1.2.3
+Version: 1.2.5
 Summary: Mocking API and function calls in Python - inspired by Ruby's RSpec-Mocks.
 Home-page: https://github.com/tcassou/expectise
-Download-URL: https://github.com/tcassou/expectise/archive/1.2.3.tar.gz
+Download-URL: https://github.com/tcassou/expectise/archive/1.2.5.tar.gz
 Keywords: python,testing,mocking,unit,tests
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
```

### Comparing `expectise-1.2.3/README.md` & `expectise-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `expectise-1.2.3/expectise/diff.py` & `expectise-1.2.5/expectise/diff.py`

 * *Files identical despite different names*

### Comparing `expectise-1.2.3/expectise/expect.py` & `expectise-1.2.5/expectise/expect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+from enum import Enum
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import TYPE_CHECKING
 
 from .diff import Diff
 from .exceptions import EnvironmentError
 from .exceptions import ExpectationError
 
+
 if TYPE_CHECKING:
     # Prevent circular dependency
     from .mocks import Mock
 
 
+class Lifespan(Enum):
+    PERMANENT = "PERMANENT"
+    TEMPORARY = "TEMPORARY"
+
+
 class Expect(object):
     """
     Mocking function calls for unit tests purposes, refer to the README for more details and examples.
     """
 
     # Dict of classes with at least one method mocked, shared between Expect instances: {'class_name': class}
     class_h = {}
@@ -254,16 +261,29 @@
 
         cls.method_h[(class_name, method_name)]["mock"].disable()
 
     @classmethod
     def tear_down(cls) -> None:
         """Check for any method called less times than expected, and raise an AssertionError is any is found."""
         message = ""
-        for (class_name, method_name), args in cls.method_h.items():
+        temporary_mocks = []
+        for key, args in cls.method_h.items():
+            (class_name, method_name) = key
             remain = args["expected"] - args["performed"]
             if remain > 0:
                 message += f"`{method_name}` from class `{class_name}` still expected to be called {remain} time(s).\n"
-            # Resetting Expect parameters and original methods, keeping the reference to the Mock object
-            cls.set_up(cls.method_h[(class_name, method_name)]["mock"])
+            # Resetting Expect parameters and original methods, keeping the reference to the Mock object,
+            # if it's a permanent mock (e.g.: set with the mock_if decorator)
+            mock = cls.method_h[key]["mock"]
+
+            if mock.lifespan is Lifespan.PERMANENT:
+                cls.set_up(mock)
+            elif mock.lifespan is Lifespan.TEMPORARY:
+                mock.disable()
+                temporary_mocks.append(key)
+
+        # Fully removing all references to temporary mocks
+        for key in temporary_mocks:
+            cls.method_h.pop(key)
 
         # If some calls are still expected, message is not empty, so asserting False with the appropriate message
         assert not message, message
```

### Comparing `expectise-1.2.3/expectise/mocks.py` & `expectise-1.2.5/expectise/mocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 from typing import Callable
 from typing import Type
 
 from .exceptions import EnvironmentError
 from .expect import Expect
+from .expect import Lifespan
 
 
 class Mock:
     """Represent a mocked method and its behaviour depending on the environment context."""
 
-    def __init__(self, klass: Type, method: Callable, env_name: str, env_value: str) -> None:
+    def __init__(self, klass: Type, method: Callable, env_name: str, env_value: str, lifespan: Lifespan) -> None:
         self.klass = klass
         self.method = method
         self.is_classmethod = isinstance(method, classmethod)
         self.is_staticmethod = isinstance(method, staticmethod)
         self.is_property = isinstance(method, property)
         self.env_name = env_name
         self.env_value = env_value
+        self.lifespan = lifespan
 
     @property
     def name(self) -> str:
         """Return the mocked method name, depending on the type of method mocked."""
         if self.is_classmethod or self.is_staticmethod:
             return self.method.__func__.__name__
         if self.is_property:
@@ -54,15 +56,15 @@
     def enable(self):
         """Replace the mocked method with its surrogate."""
         Expect.set_up(self)
 
 
 def mock(klass: Type, method: Callable, env_name: str, env_value: str) -> None:
     """Enable mocking of an object method by replacing it with a surrogate, requiring subsequent `Expect` statements."""
-    Mock(klass, method, env_name, env_value).enable()
+    Mock(klass, method, env_name, env_value, lifespan=Lifespan.TEMPORARY).enable()
 
 
 def mock_if(env_name: str, env_value: str) -> Type:
     """
     Decorator to identify which methods should be mocked, only in case the right environment variable is set to the
     right value. Example:
 
@@ -74,15 +76,15 @@
     class MockDecorator:
         def __init__(self, method: Callable) -> None:
             """
             Decorator class, that takes as input the method to be mocked:
             * if the environment conditions are met, the method is marked as to be mocked for later calls
             * if not, the method is left unchanged.
             """
-            self.mock = Mock(None, method, env_name, env_value)
+            self.mock = Mock(None, method, env_name, env_value, lifespan=Lifespan.PERMANENT)
 
         def __set_name__(self, owner: Type, name: str) -> None:
             """
             At interpretation time when the MockDecorator object is created, the surrounding class is not created yet.
             As soon as it is, this `__set_name__` method is called, which gives us a way to know and record the class or
             object that owns the method.
             """
```

### Comparing `expectise-1.2.3/expectise.egg-info/PKG-INFO` & `expectise-1.2.5/expectise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: expectise
-Version: 1.2.3
+Version: 1.2.5
 Summary: Mocking API and function calls in Python - inspired by Ruby's RSpec-Mocks.
 Home-page: https://github.com/tcassou/expectise
-Download-URL: https://github.com/tcassou/expectise/archive/1.2.3.tar.gz
+Download-URL: https://github.com/tcassou/expectise/archive/1.2.5.tar.gz
 Keywords: python,testing,mocking,unit,tests
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
```

### Comparing `expectise-1.2.3/setup.py` & `expectise-1.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from distutils.core import setup
 
 
-version = "1.2.3"
+version = "1.2.5"
 name = "expectise"
 
 setup(
     name=name,
     packages=[name],
     version=version,
     description="Mocking API and function calls in Python - inspired by Ruby's RSpec-Mocks.",
```

