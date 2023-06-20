# Comparing `tmp/json_with_comments-1.2.0.tar.gz` & `tmp/json_with_comments-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_with_comments-1.2.0.tar", max compression
+gzip compressed data, was "json_with_comments-1.2.1.tar", max compression
```

## Comparing `json_with_comments-1.2.0.tar` & `json_with_comments-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9619 2023-06-20 19:48:47.418131 json_with_comments-1.2.0/jsonc/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-21 14:37:42.998515 json_with_comments-1.2.0/LICENSE
--rw-r--r--   0        0        0      684 2023-06-20 19:46:34.318451 json_with_comments-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      983 2023-04-21 14:37:42.999515 json_with_comments-1.2.0/README.md
--rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 json_with_comments-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     9625 2023-06-20 23:34:37.242886 json_with_comments-1.2.1/jsonc/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-21 14:37:42.998515 json_with_comments-1.2.1/LICENSE
+-rw-r--r--   0        0        0      684 2023-06-20 23:34:44.890224 json_with_comments-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1076 2023-06-20 19:57:53.411596 json_with_comments-1.2.1/README.md
+-rw-r--r--   0        0        0     1913 1970-01-01 00:00:00.000000 json_with_comments-1.2.1/PKG-INFO
```

### Comparing `json_with_comments-1.2.0/jsonc/__init__.py` & `json_with_comments-1.2.1/jsonc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from collections.abc import Callable
 from copy import deepcopy
 from io import StringIO
 from tokenize import COMMENT, NL, STRING, TokenInfo, generate_tokens, untokenize
 from typing import TYPE_CHECKING, Any, TextIO
 from warnings import warn
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 import json
 import re
 from json import JSONDecoder, JSONEncoder  # for compatibility
 
 if TYPE_CHECKING:
     CommentsDict = dict[str, "Comments"] | dict[int, "Comments"]
     Comments = str | CommentsDict | tuple[str, CommentsDict]
@@ -108,15 +108,15 @@
             comm = None
         return comm, comments
     return None, None
 
 
 def _warn_unused(
     comments: CommentsDict | None,
-    stack: tuple[CommentsDict | None, int | None, str | int],
+    stack: list[tuple[CommentsDict | None, int | None, str | int]],
 ):
     if not comments:
         return
     full_key = ".".join(str(key) for _, _, key in stack[1:])
     if full_key:
         full_key += "."
     for k in comments:
```

### Comparing `json_with_comments-1.2.0/LICENSE` & `json_with_comments-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json_with_comments-1.2.0/pyproject.toml` & `json_with_comments-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-with-comments"
-version = "1.2.0"
+version = "1.2.1"
 description = "JSON with Comments for Python"
 license = "MIT"
 authors = ["Takumasa Nakamura <n.takumasa@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/n-takumasa/json-with-comments"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `json_with_comments-1.2.0/README.md` & `json_with_comments-1.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # JSON with Comments for Python
 [![pypi version](https://img.shields.io/pypi/v/json-with-comments.svg)](https://pypi.python.org/project/json-with-comments)
 [![Python package](https://github.com/n-takumasa/json-with-comments/actions/workflows/python-package.yml/badge.svg)](https://github.com/n-takumasa/json-with-comments/actions/workflows/python-package.yml)
 [![Python Versions](https://img.shields.io/pypi/pyversions/json-with-comments.svg)](https://pypi.org/project/json-with-comments/)
 
 ## Features
-* Remove single line (`//`) and block comments (`/* */`)
-* Remove trailing commas from arrays and objects
+* `load()`, `loads()`
+  * Remove single line (`//`) and block comments (`/* */`)
+  * Remove trailing commas from arrays and objects
+* `dump()`, `dumps()`
+  * Add comments
+  * Add trailing commas
 
 ## Usage
 
 ```sh
 pip install json-with-comments
 ```
```

