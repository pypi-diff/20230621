# Comparing `tmp/yls_yara-1.3.3.tar.gz` & `tmp/yls_yara-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yls_yara-1.3.3.tar", max compression
+gzip compressed data, was "yls_yara-1.3.4.tar", max compression
```

## Comparing `yls_yara-1.3.3.tar` & `yls_yara-1.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1082 2022-10-06 11:41:51.353878 yls_yara-1.3.3/LICENSE
--rw-r--r--   0        0        0      481 2022-10-06 11:41:51.353878 yls_yara-1.3.3/README.md
--rw-r--r--   0        0        0        0 2022-10-06 11:41:51.353878 yls_yara-1.3.3/py.typed
--rw-r--r--   0        0        0      575 2023-03-29 10:30:25.019404 yls_yara-1.3.3/pyproject.toml
--rw-r--r--   0        0        0       38 2023-02-22 16:57:26.188061 yls_yara-1.3.3/yls_yara/__init__.py
--rw-r--r--   0        0        0     2972 2023-02-22 16:57:26.192061 yls_yara-1.3.3/yls_yara/linting.py
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 yls_yara-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-10-06 11:41:51.353878 yls_yara-1.3.4/LICENSE
+-rw-r--r--   0        0        0      481 2022-10-06 11:41:51.353878 yls_yara-1.3.4/README.md
+-rw-r--r--   0        0        0        0 2022-10-06 11:41:51.353878 yls_yara-1.3.4/py.typed
+-rw-r--r--   0        0        0      575 2023-06-21 11:26:40.539193 yls_yara-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-03-31 16:56:48.395088 yls_yara-1.3.4/yls_yara/__init__.py
+-rw-r--r--   0        0        0     2972 2023-03-31 16:56:48.395088 yls_yara-1.3.4/yls_yara/linting.py
+-rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 yls_yara-1.3.4/PKG-INFO
```

### Comparing `yls_yara-1.3.3/LICENSE` & `yls_yara-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yls_yara-1.3.3/pyproject.toml` & `yls_yara-1.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "yls-yara"
-version = "1.3.3"
+version = "1.3.4"
 description = "YLS plugin adding linting using yara-python."
 authors = ["Matej Kastak <matej.kastak@avast.com>"]
 maintainers = ["Matej Kašťák <matej.kastak@avast.com>"]
 readme = "README.md"
 license = "MIT"
 include = ["py.typed", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 yara-python = "^4.2.0"
-yls = "^1.3.3"
+yls = "^1.3.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `yls_yara-1.3.3/yls_yara/linting.py` & `yls_yara-1.3.4/yls_yara/linting.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import os
 import re
 from typing import List
 
 import yara
-
-from yls import hookimpl
-from yls import utils
 from lsprotocol.types import Diagnostic
 from lsprotocol.types import DiagnosticSeverity
 from lsprotocol.types import Position
 
+from yls import hookimpl
+from yls import utils
+
 log = logging.getLogger(__name__)
 
 SOURCE_YARA = "Yara Python"
 
 
 @hookimpl()
 def yls_lint(document) -> List[Diagnostic]:
```

### Comparing `yls_yara-1.3.3/PKG-INFO` & `yls_yara-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: yls-yara
-Version: 1.3.3
+Version: 1.3.4
 Summary: YLS plugin adding linting using yara-python.
 License: MIT
 Author: Matej Kastak
 Author-email: matej.kastak@avast.com
 Maintainer: Matej Kašťák
 Maintainer-email: matej.kastak@avast.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: yara-python (>=4.2.0,<5.0.0)
-Requires-Dist: yls (>=1.3.3,<2.0.0)
+Requires-Dist: yls (>=1.3.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # yls-yara
 
 ![PyPI](https://img.shields.io/pypi/v/yls-yara)
 
 An [YLS](https://www.github.com/avast/yls) plugin adding
```

