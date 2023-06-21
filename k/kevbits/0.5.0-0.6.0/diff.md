# Comparing `tmp/kevbits-0.5.0.tar.gz` & `tmp/kevbits-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kevbits-0.5.0.tar", max compression
+gzip compressed data, was "kevbits-0.6.0.tar", max compression
```

## Comparing `kevbits-0.5.0.tar` & `kevbits-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.5.0/kevbits/__init__.py
--rw-r--r--   0        0        0     2465 2023-03-12 08:27:49.741866 kevbits-0.5.0/kevbits/logconfig.py
--rw-r--r--   0        0        0      631 2023-03-12 08:27:49.627869 kevbits-0.5.0/kevbits/math.py
--rw-r--r--   0        0        0     2250 2023-03-12 08:27:49.744867 kevbits-0.5.0/kevbits/misc.py
--rw-r--r--   0        0        0     5875 2023-05-31 09:41:12.200066 kevbits-0.5.0/kevbits/sgconv.py
--rw-r--r--   0        0        0      916 2023-05-31 09:46:25.231068 kevbits-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      219 2023-03-12 07:21:14.714981 kevbits-0.5.0/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 kevbits-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.6.0/kevbits/__init__.py
+-rw-r--r--   0        0        0     2553 2023-06-21 05:44:31.101857 kevbits-0.6.0/kevbits/logconfig.py
+-rw-r--r--   0        0        0      631 2023-03-12 08:27:49.627869 kevbits-0.6.0/kevbits/math.py
+-rw-r--r--   0        0        0     2671 2023-06-21 06:07:50.391403 kevbits-0.6.0/kevbits/misc.py
+-rw-r--r--   0        0        0     5875 2023-05-31 09:41:12.200066 kevbits-0.6.0/kevbits/sgconv.py
+-rw-r--r--   0        0        0      916 2023-06-21 06:11:26.994605 kevbits-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-03-12 07:21:14.714981 kevbits-0.6.0/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 kevbits-0.6.0/PKG-INFO
```

### Comparing `kevbits-0.5.0/kevbits/logconfig.py` & `kevbits-0.6.0/kevbits/logconfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 import logging
 import logging.config
 
 import sys
 import time
 import re
 import os
-from typing import Any
+from typing import Any, Optional
 
 from kevbits.misc import map_dict_deep
 
 
 class GmTimeFormatter(logging.Formatter):
     "Use UTC timestamp for log messages."
 
-    def __init__(self, fmt=None, datefmt=None):
+    def __init__(self, fmt: Optional[str] = None, datefmt: Optional[str] = None):
         super().__init__(fmt=fmt, datefmt=datefmt)
         self.converter = time.gmtime
 
 
-def gmtime_formatter_factory(fmt, datefmt):
+def gmtime_formatter_factory(fmt: Optional[str] = None, datefmt: Optional[str] = None):
     "Factory function which is referred to from .yaml file."
     return GmTimeFormatter(fmt, datefmt)
 
 
 rx_expandvars = re.compile(r"(.*?)(\${.*?})(.*)")
```

### Comparing `kevbits-0.5.0/kevbits/math.py` & `kevbits-0.6.0/kevbits/math.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.5.0/kevbits/sgconv.py` & `kevbits-0.6.0/kevbits/sgconv.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.5.0/pyproject.toml` & `kevbits-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kevbits"
-version = "0.5.0"
+version = "0.6.0"
 description = "Small helper functions and objects"
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kevbits-0.5.0/PKG-INFO` & `kevbits-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevbits
-Version: 0.5.0
+Version: 0.6.0
 Summary: Small helper functions and objects
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

