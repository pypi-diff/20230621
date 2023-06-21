# Comparing `tmp/uptick_splat-0.1.7.tar.gz` & `tmp/uptick_splat-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptick_splat-0.1.7.tar", max compression
+gzip compressed data, was "uptick_splat-0.1.8.tar", max compression
```

## Comparing `uptick_splat-0.1.7.tar` & `uptick_splat-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.7/README.md
--rw-r--r--   0        0        0      387 2023-06-21 09:47:59.548995 uptick_splat-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-21 06:42:33.330065 uptick_splat-0.1.7/uptick_splat/__init__.py
--rw-r--r--   0        0        0     2288 2023-06-21 09:25:38.548596 uptick_splat-0.1.7/uptick_splat/config.py
--rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.7/uptick_splat/exceptions.py
--rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.7/uptick_splat/logging.py
--rw-r--r--   0        0        0        0 2023-06-21 07:09:53.215637 uptick_splat-0.1.7/uptick_splat/py.typed
--rw-r--r--   0        0        0     6779 2023-06-21 09:47:51.086920 uptick_splat-0.1.7/uptick_splat/utils.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.8/README.md
+-rw-r--r--   0        0        0      387 2023-06-21 10:08:20.790155 uptick_splat-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-21 06:42:33.330065 uptick_splat-0.1.8/uptick_splat/__init__.py
+-rw-r--r--   0        0        0     2878 2023-06-21 10:06:57.144193 uptick_splat-0.1.8/uptick_splat/config.py
+-rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.8/uptick_splat/exceptions.py
+-rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.8/uptick_splat/logging.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:09:53.215637 uptick_splat-0.1.8/uptick_splat/py.typed
+-rw-r--r--   0        0        0     6779 2023-06-21 09:47:51.086920 uptick_splat-0.1.8/uptick_splat/utils.py
+-rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.8/PKG-INFO
```

### Comparing `uptick_splat-0.1.7/LICENSE.md` & `uptick_splat-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.7/README.md` & `uptick_splat-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.7/uptick_splat/config.py` & `uptick_splat-0.1.8/uptick_splat/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Callable
+from typing import Any, Callable, Optional
 from uuid import uuid4
 
 import boto3
 
 from .logging import logger
 
 
@@ -16,50 +16,56 @@
 def get_tmp_html_key() -> str:
     """This function can be overridden to provide a custom storage_location for temporary html files"""
     return f"tmp/{uuid4()}.html"
 
 
 def delete_key(bucket_name: str, path: str) -> None:
     """This function can be overriden to provide a custom delete key function"""
-    session = config.get_session()
+    global config
+    session = config.get_session_fn()
     s3_client = session.client("s3")
     try:
         s3_client.delete_object(Bucket=bucket_name, Key=path)
     except Exception as e:
         logger.warning(f"Failed to delete {path} from s3: {e}")
 
 
 def configure_splat(
-    function_region: str = "ap-southeast-2",
-    function_name: str = "splat-prod",
-    default_bucket_name: str = "",
-    default_tagging: str = "ExpireAfter=1w",
-    get_session_fn: Callable[[], Any] = get_session,
-    get_tmp_html_key_fn: Callable[[str], str] = get_tmp_html_key,
-    delete_key_fn: Callable[[str, str], None] = delete_key,
+    function_region: Optional[str] = None,
+    function_name: Optional[str] = None,
+    default_bucket_name: Optional[str] = None,
+    default_tagging: Optional[str] = None,
+    get_session_fn: Optional[Callable[[], Any]] = None,
+    get_tmp_html_key_fn: Optional[Callable[[str], str]] = None,
+    delete_key_fn: Optional[Callable[[str, str], None]] = None,
 ):
     """Configure the splat function.
 
     :param function_region: the default region for the splat function
     :param function_name: the name of the splat function
     :param default_bucket_name: the default bucket name to store html uploaded to s3
     :param default_tagging: the default tag to apply to html uploaded to s3
     :param get_session_fn: a function that returns a boto3 session
     :param default_key_delete_fn: a function that deletes a key from s3
     """
     global config
-    config = Config(
-        function_region=function_region,
-        function_name=function_name,
-        default_bucket_name=default_bucket_name,
-        default_tagging=default_tagging,
-        get_session_fn=get_session_fn,
-        get_tmp_html_key_fn=get_tmp_html_key_fn,
-        delete_key_fn=delete_key_fn,
-    )
+    if function_region is not None:
+        config.function_region = function_region
+    if function_name is not None:
+        config.function_name = function_name
+    if default_bucket_name is not None:
+        config.default_bucket_name = default_bucket_name
+    if default_tagging is not None:
+        config.default_tagging = default_tagging
+    if get_session_fn is not None:
+        config.get_session_fn = get_session_fn
+    if get_tmp_html_key_fn is not None:
+        config.get_tmp_html_key_fn = get_tmp_html_key_fn
+    if delete_key_fn is not None:
+        config.delete_key_fn = delete_key_fn
 
 
 @dataclass
 class Config:
     function_region: str
     function_name: str
     default_bucket_name: str
@@ -67,7 +73,17 @@
 
     get_session_fn: Callable[[], Any]
     get_tmp_html_key_fn: Callable[[str], str]
     delete_key_fn: Callable[[str, str], None]
 
 
 configure_splat()
+
+config = Config(
+    function_region="ap-southeast-2",
+    function_name="splat-prod",
+    default_bucket_name="",
+    default_tagging="ExpireAfter=1w",
+    get_session_fn=get_session,
+    get_tmp_html_key_fn=get_tmp_html_key,
+    delete_key_fn=delete_key,
+)
```

### Comparing `uptick_splat-0.1.7/uptick_splat/utils.py` & `uptick_splat-0.1.8/uptick_splat/utils.py`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.7/PKG-INFO` & `uptick_splat-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptick-splat
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django library for invoking splat
 Author: william chu
 Author-email: william.chu@uptickhq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

