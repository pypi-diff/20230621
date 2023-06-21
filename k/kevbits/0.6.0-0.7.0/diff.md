# Comparing `tmp/kevbits-0.6.0.tar.gz` & `tmp/kevbits-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kevbits-0.6.0.tar", max compression
+gzip compressed data, was "kevbits-0.7.0.tar", max compression
```

## Comparing `kevbits-0.6.0.tar` & `kevbits-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.6.0/kevbits/__init__.py
--rw-r--r--   0        0        0     2553 2023-06-21 05:44:31.101857 kevbits-0.6.0/kevbits/logconfig.py
--rw-r--r--   0        0        0      631 2023-03-12 08:27:49.627869 kevbits-0.6.0/kevbits/math.py
--rw-r--r--   0        0        0     2671 2023-06-21 06:07:50.391403 kevbits-0.6.0/kevbits/misc.py
--rw-r--r--   0        0        0     5875 2023-05-31 09:41:12.200066 kevbits-0.6.0/kevbits/sgconv.py
--rw-r--r--   0        0        0      916 2023-06-21 06:11:26.994605 kevbits-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      219 2023-03-12 07:21:14.714981 kevbits-0.6.0/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 kevbits-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.7.0/kevbits/__init__.py
+-rw-r--r--   0        0        0     2553 2023-06-21 05:44:31.101857 kevbits-0.7.0/kevbits/logconfig.py
+-rw-r--r--   0        0        0      631 2023-03-12 08:27:49.627869 kevbits-0.7.0/kevbits/math.py
+-rw-r--r--   0        0        0     2677 2023-06-21 09:30:31.426729 kevbits-0.7.0/kevbits/misc.py
+-rw-r--r--   0        0        0     5875 2023-05-31 09:41:12.200066 kevbits-0.7.0/kevbits/sgconv.py
+-rw-r--r--   0        0        0      916 2023-06-21 09:31:03.714416 kevbits-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-03-12 07:21:14.714981 kevbits-0.7.0/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 kevbits-0.7.0/PKG-INFO
```

### Comparing `kevbits-0.6.0/kevbits/logconfig.py` & `kevbits-0.7.0/kevbits/logconfig.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.6.0/kevbits/math.py` & `kevbits-0.7.0/kevbits/math.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.6.0/kevbits/misc.py` & `kevbits-0.7.0/kevbits/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Miscellaneous functions
 """
 
 import sys
 import traceback
-from typing import Any, Callable, cast, Type
+from typing import Any, Callable, cast, Type, Dict
 
 
 def boolstr_to_bool(string: str):
     """
     Cast string that describes bool values ("False", "yes", "1", "0")
     into bool type.
     """
@@ -18,15 +18,15 @@
         .replace("true", "1")
         .replace("no", "0")
         .replace("yes", "1")
     )
     return bool(int(t))
 
 
-MapDictType = dict[Any, Any]
+MapDictType = Dict[Any, Any]
 
 
 def map_dict_deep(dict_: MapDictType, mapfunc: Callable[[Any], Any]) -> MapDictType:
     """
     Return a new dictionary whose keys are not changed, and the values (if they are not
     dictionaries) are passed through the map function. If the value is a (nested) dictionary,
     it undergoes the same processing.
```

### Comparing `kevbits-0.6.0/kevbits/sgconv.py` & `kevbits-0.7.0/kevbits/sgconv.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.6.0/pyproject.toml` & `kevbits-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kevbits"
-version = "0.6.0"
+version = "0.7.0"
 description = "Small helper functions and objects"
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kevbits-0.6.0/PKG-INFO` & `kevbits-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevbits
-Version: 0.6.0
+Version: 0.7.0
 Summary: Small helper functions and objects
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

