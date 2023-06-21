# Comparing `tmp/uptick_splat-0.1.1.tar.gz` & `tmp/uptick_splat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptick_splat-0.1.1.tar", max compression
+gzip compressed data, was "uptick_splat-0.1.2.tar", max compression
```

## Comparing `uptick_splat-0.1.1.tar` & `uptick_splat-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     2359 2023-06-13 11:59:59.934897 uptick_splat-0.1.1/README.md
--rw-r--r--   0        0        0      387 2023-06-13 12:00:24.039712 uptick_splat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      235 2023-06-13 11:57:16.823768 uptick_splat-0.1.1/uptick_splat/__init__.py
--rw-r--r--   0        0        0     1934 2023-06-13 11:58:17.816025 uptick_splat-0.1.1/uptick_splat/config.py
--rw-r--r--   0        0        0       53 2023-06-08 06:40:46.477080 uptick_splat-0.1.1/uptick_splat/exceptions.py
--rw-r--r--   0        0        0       91 2023-06-13 10:48:30.358687 uptick_splat-0.1.1/uptick_splat/logging.py
--rw-r--r--   0        0        0     4060 2023-06-13 11:57:07.511702 uptick_splat-0.1.1/uptick_splat/utils.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.2/README.md
+-rw-r--r--   0        0        0      387 2023-06-21 05:13:49.184262 uptick_splat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-06-13 23:54:01.062233 uptick_splat-0.1.2/uptick_splat/__init__.py
+-rw-r--r--   0        0        0     1934 2023-06-13 23:54:01.062502 uptick_splat-0.1.2/uptick_splat/config.py
+-rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.2/uptick_splat/exceptions.py
+-rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.2/uptick_splat/logging.py
+-rw-r--r--   0        0        0     4110 2023-06-21 05:13:27.027945 uptick_splat-0.1.2/uptick_splat/utils.py
+-rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.2/PKG-INFO
```

### Comparing `uptick_splat-0.1.1/LICENSE.md` & `uptick_splat-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.1/README.md` & `uptick_splat-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.1/uptick_splat/config.py` & `uptick_splat-0.1.2/uptick_splat/config.py`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.1/uptick_splat/utils.py` & `uptick_splat-0.1.2/uptick_splat/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,17 @@
             "Invalid configuration: no bucket name provided"
         )
 
     is_streaming = not bool(s3_filepath)
 
     session = config.get_session_fn()
     lambda_client = session.client(
-        "lambda", region_name=config.function_region, config=Config(read_timeout=120)
+        "lambda",
+        region_name=config.function_region,
+        config=Config(read_timeout=60 * 15, retries={"max_attempts": 0}),
     )
     s3_client = session.client("s3")
 
     destination_path = s3_filepath or f"tmp/{uuid4()}.pdf"
     fields = fields or {}
     conditions = conditions or []
```

### Comparing `uptick_splat-0.1.1/PKG-INFO` & `uptick_splat-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptick-splat
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django library for invoking splat
 Author: william chu
 Author-email: william.chu@uptickhq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

