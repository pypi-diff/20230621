# Comparing `tmp/uptick_splat-0.1.4.tar.gz` & `tmp/uptick_splat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptick_splat-0.1.4.tar", max compression
+gzip compressed data, was "uptick_splat-0.1.5.tar", max compression
```

## Comparing `uptick_splat-0.1.4.tar` & `uptick_splat-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.4/README.md
--rw-r--r--   0        0        0      387 2023-06-21 07:10:01.213114 uptick_splat-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-21 06:42:33.330065 uptick_splat-0.1.4/uptick_splat/__init__.py
--rw-r--r--   0        0        0     1934 2023-06-21 06:37:44.327612 uptick_splat-0.1.4/uptick_splat/config.py
--rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.4/uptick_splat/exceptions.py
--rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.4/uptick_splat/logging.py
--rw-r--r--   0        0        0        0 2023-06-21 07:09:53.215637 uptick_splat-0.1.4/uptick_splat/py.typed
--rw-r--r--   0        0        0     6796 2023-06-21 06:45:11.994237 uptick_splat-0.1.4/uptick_splat/utils.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.5/README.md
+-rw-r--r--   0        0        0      387 2023-06-21 07:11:29.962352 uptick_splat-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-21 06:42:33.330065 uptick_splat-0.1.5/uptick_splat/__init__.py
+-rw-r--r--   0        0        0     1934 2023-06-21 06:37:44.327612 uptick_splat-0.1.5/uptick_splat/config.py
+-rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.5/uptick_splat/exceptions.py
+-rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.5/uptick_splat/logging.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:09:53.215637 uptick_splat-0.1.5/uptick_splat/py.typed
+-rw-r--r--   0        0        0     6786 2023-06-21 07:11:23.215051 uptick_splat-0.1.5/uptick_splat/utils.py
+-rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.5/PKG-INFO
```

### Comparing `uptick_splat-0.1.4/LICENSE.md` & `uptick_splat-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.4/README.md` & `uptick_splat-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.4/uptick_splat/config.py` & `uptick_splat-0.1.5/uptick_splat/config.py`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.4/uptick_splat/utils.py` & `uptick_splat-0.1.5/uptick_splat/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             splat_error = splat_response
         raise SplatPDFGenerationFailure(f"Error returned from splat: {splat_error}")
 
 
 def pdf_from_html_without_s3(
     body_html: str,
     javascript: bool = False,
-) -> Optional[bytes]:
+) -> bytes:
     """Generates a pdf from html without using s3. This is useful for small pdfs and html documents.
 
     The maximum size of the html document is 6MB. The maximum size of the pdf is 6MB.
     """
     session = config.get_session_fn()
     lambda_client = session.client(
         "lambda",
```

### Comparing `uptick_splat-0.1.4/PKG-INFO` & `uptick_splat-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptick-splat
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django library for invoking splat
 Author: william chu
 Author-email: william.chu@uptickhq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

