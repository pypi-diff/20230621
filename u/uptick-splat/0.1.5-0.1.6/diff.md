# Comparing `tmp/uptick_splat-0.1.5.tar.gz` & `tmp/uptick_splat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptick_splat-0.1.5.tar", max compression
+gzip compressed data, was "uptick_splat-0.1.6.tar", max compression
```

## Comparing `uptick_splat-0.1.5.tar` & `uptick_splat-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.5/LICENSE.md
--rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.5/README.md
--rw-r--r--   0        0        0      387 2023-06-21 07:11:29.962352 uptick_splat-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-21 06:42:33.330065 uptick_splat-0.1.5/uptick_splat/__init__.py
--rw-r--r--   0        0        0     1934 2023-06-21 06:37:44.327612 uptick_splat-0.1.5/uptick_splat/config.py
--rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.5/uptick_splat/exceptions.py
--rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.5/uptick_splat/logging.py
--rw-r--r--   0        0        0        0 2023-06-21 07:09:53.215637 uptick_splat-0.1.5/uptick_splat/py.typed
--rw-r--r--   0        0        0     6786 2023-06-21 07:11:23.215051 uptick_splat-0.1.5/uptick_splat/utils.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.6/README.md
+-rw-r--r--   0        0        0      387 2023-06-21 09:25:50.349900 uptick_splat-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-21 06:42:33.330065 uptick_splat-0.1.6/uptick_splat/__init__.py
+-rw-r--r--   0        0        0     2288 2023-06-21 09:25:38.548596 uptick_splat-0.1.6/uptick_splat/config.py
+-rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.6/uptick_splat/exceptions.py
+-rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.6/uptick_splat/logging.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:09:53.215637 uptick_splat-0.1.6/uptick_splat/py.typed
+-rw-r--r--   0        0        0     6790 2023-06-21 09:25:33.390552 uptick_splat-0.1.6/uptick_splat/utils.py
+-rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.6/PKG-INFO
```

### Comparing `uptick_splat-0.1.5/LICENSE.md` & `uptick_splat-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.5/README.md` & `uptick_splat-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.5/uptick_splat/config.py` & `uptick_splat-0.1.6/uptick_splat/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from dataclasses import dataclass
 from typing import Any, Callable
+from uuid import uuid4
 
 import boto3
 
 from .logging import logger
 
 
 def get_session() -> Any:
     """This function can be overridden to provide a custom session"""
     session = boto3.session.Session()
     return session
 
 
+def get_tmp_html_key() -> str:
+    """This function can be overridden to provide a custom storage_location for temporary html files"""
+    return f"tmp/{uuid4()}.html"
+
+
 def delete_key(bucket_name: str, path: str) -> None:
     """This function can be overriden to provide a custom delete key function"""
     session = config.get_session()
     s3_client = session.client("s3")
     try:
         s3_client.delete_object(Bucket=bucket_name, Key=path)
     except Exception as e:
@@ -24,14 +30,15 @@
 
 def configure_splat(
     function_region: str = "ap-southeast-2",
     function_name: str = "splat-prod",
     default_bucket_name: str = "",
     default_tagging: str = "ExpireAfter=1w",
     get_session_fn: Callable[[], Any] = get_session,
+    get_tmp_html_key_fn: Callable[[str], str] = get_tmp_html_key,
     delete_key_fn: Callable[[str, str], None] = delete_key,
 ):
     """Configure the splat function.
 
     :param function_region: the default region for the splat function
     :param function_name: the name of the splat function
     :param default_bucket_name: the default bucket name to store html uploaded to s3
@@ -42,23 +49,25 @@
     global config
     config = Config(
         function_region=function_region,
         function_name=function_name,
         default_bucket_name=default_bucket_name,
         default_tagging=default_tagging,
         get_session_fn=get_session_fn,
+        get_tmp_html_key_fn=get_tmp_html_key_fn,
         delete_key_fn=delete_key_fn,
     )
 
 
 @dataclass
 class Config:
     function_region: str
     function_name: str
     default_bucket_name: str
     default_tagging: str
 
     get_session_fn: Callable[[], Any]
+    get_tmp_html_key_fn: Callable[[str], str]
     delete_key_fn: Callable[[str, str], None]
 
 
 configure_splat()
```

### Comparing `uptick_splat-0.1.5/uptick_splat/utils.py` & `uptick_splat-0.1.6/uptick_splat/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             "Content-Type": "application/pdf",
             **fields,
         },
         Conditions=[["starts-with", "$Content-Type", "application/pdf"], *conditions],
     )
 
     # Upload body HTML to s3 and get a link to hand to splat
-    html_key = os.path.join(bucket_name, "tmp", f"{uuid4()}.html")
+    html_key = os.path.join(bucket_name, config.get_tmp_html_key_fn())
 
     s3_client.put_object(
         Body=body_html,
         Bucket=bucket_name,
         Key=html_key,
         Tagging=config.default_tagging,
     )
```

### Comparing `uptick_splat-0.1.5/PKG-INFO` & `uptick_splat-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptick-splat
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django library for invoking splat
 Author: william chu
 Author-email: william.chu@uptickhq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

