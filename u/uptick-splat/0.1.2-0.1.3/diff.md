# Comparing `tmp/uptick_splat-0.1.2.tar.gz` & `tmp/uptick_splat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptick_splat-0.1.2.tar", max compression
+gzip compressed data, was "uptick_splat-0.1.3.tar", max compression
```

## Comparing `uptick_splat-0.1.2.tar` & `uptick_splat-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.2/README.md
--rw-r--r--   0        0        0      387 2023-06-21 05:13:49.184262 uptick_splat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      235 2023-06-13 23:54:01.062233 uptick_splat-0.1.2/uptick_splat/__init__.py
--rw-r--r--   0        0        0     1934 2023-06-13 23:54:01.062502 uptick_splat-0.1.2/uptick_splat/config.py
--rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.2/uptick_splat/exceptions.py
--rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.2/uptick_splat/logging.py
--rw-r--r--   0        0        0     4110 2023-06-21 05:13:27.027945 uptick_splat-0.1.2/uptick_splat/utils.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-03-16 03:30:05.342454 uptick_splat-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2359 2023-06-13 23:54:01.060386 uptick_splat-0.1.3/README.md
+-rw-r--r--   0        0        0      387 2023-06-21 06:50:34.236452 uptick_splat-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-21 06:42:33.330065 uptick_splat-0.1.3/uptick_splat/__init__.py
+-rw-r--r--   0        0        0     1934 2023-06-21 06:37:44.327612 uptick_splat-0.1.3/uptick_splat/config.py
+-rw-r--r--   0        0        0       53 2023-06-13 23:54:01.062748 uptick_splat-0.1.3/uptick_splat/exceptions.py
+-rw-r--r--   0        0        0       91 2023-06-13 23:54:01.062996 uptick_splat-0.1.3/uptick_splat/logging.py
+-rw-r--r--   0        0        0     6796 2023-06-21 06:45:11.994237 uptick_splat-0.1.3/uptick_splat/utils.py
+-rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 uptick_splat-0.1.3/PKG-INFO
```

### Comparing `uptick_splat-0.1.2/LICENSE.md` & `uptick_splat-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.2/README.md` & `uptick_splat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.2/uptick_splat/config.py` & `uptick_splat-0.1.3/uptick_splat/config.py`

 * *Files identical despite different names*

### Comparing `uptick_splat-0.1.2/uptick_splat/utils.py` & `uptick_splat-0.1.3/uptick_splat/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import json
 import os
 import re
 from json import JSONDecodeError
 from typing import Dict, List, Optional, cast
 from uuid import uuid4
 
@@ -14,22 +15,31 @@
     pass
 
 
 def strip_dangerous_s3_chars(filename: str) -> str:
     return re.sub(r"[^0-9a-zA-Z_\.\-\s]", "", filename)
 
 
-def pdf_with_splat(
+def pdf_from_html(
     body_html: str,
     *,
     bucket_name: Optional[str] = None,
     s3_filepath: Optional[str] = None,
+    javascript: bool = False,
     fields: Optional[Dict] = None,
     conditions: Optional[List[List]] = None,
 ) -> Optional[bytes]:
+    """Generates a pdf from html using the splat lambda function.
+
+    :param body_html: the html to convert to pdf
+    :param bucket_name: the bucket to upload the html to. defaults to config.default_bucket_name
+    :param s3_filepath: the path to upload the pdf to. defaults to a random path in the bucket
+    :param fields: additional fields to add to the presigned url
+    :param conditions: additional conditions to add to the presigned url
+    """
     bucket_name = bucket_name or config.default_bucket_name
     if not bucket_name:
         raise SplatPDFGenerationFailure(
             "Invalid configuration: no bucket name provided"
         )
 
     is_streaming = not bool(s3_filepath)
@@ -70,15 +80,19 @@
     document_url = s3_client.generate_presigned_url(
         "get_object",
         Params={"Bucket": bucket_name, "Key": html_key},
         ExpiresIn=1800,
     )
 
     splat_body = json.dumps(
-        {"document_url": document_url, "presigned_url": presigned_url}
+        {
+            "document_url": document_url,
+            "presigned_url": presigned_url,
+            "javascript": javascript,
+        }
     )
 
     response = lambda_client.invoke(
         FunctionName=config.function_name,
         Payload=json.dumps({"body": splat_body}),
     )
 
@@ -116,14 +130,70 @@
     # ==== Failure ====
     # Lambda timeout et al.
     elif error_message := splat_response.get("errorMessage"):
         raise SplatPDFGenerationFailure(
             f"Error returned from lambda invocation: {error_message}"
         )
     # All other errors
+    else:
+        # Try to extract an error message from splat response
+        try:
+            splat_error = json.loads(splat_response["body"])["errors"][0]
+        except (KeyError, JSONDecodeError):
+            splat_error = splat_response
+        raise SplatPDFGenerationFailure(f"Error returned from splat: {splat_error}")
+
+
+def pdf_from_html_without_s3(
+    body_html: str,
+    javascript: bool = False,
+) -> Optional[bytes]:
+    """Generates a pdf from html without using s3. This is useful for small pdfs and html documents.
+
+    The maximum size of the html document is 6MB. The maximum size of the pdf is 6MB.
+    """
+    session = config.get_session_fn()
+    lambda_client = session.client(
+        "lambda",
+        region_name=config.function_region,
+        config=Config(read_timeout=60 * 15, retries={"max_attempts": 0}),
+    )
+
+    splat_body = json.dumps({"document_content": body_html, "javascript": javascript})
+
+    response = lambda_client.invoke(
+        FunctionName=config.function_name,
+        Payload=json.dumps({"body": splat_body}),
+    )
+
+    # Check response of the invocation. Note that a successful invocation doesn't mean the PDF was generated.
+    if response.get("StatusCode") != 200:
+        raise SplatPDFGenerationFailure(
+            "Invalid response while invoking splat lambda -"
+            f" {response.get('StatusCode')}"
+        )
+
+    # Parse lambda response
+    try:
+        splat_response = json.loads(response["Payload"].read().decode("utf-8"))
+    except (KeyError, AttributeError):
+        raise SplatPDFGenerationFailure("Invalid lambda response format")
+    except JSONDecodeError:
+        raise SplatPDFGenerationFailure("Error decoding splat response body as json")
+
+    # ==== Success ====
+    if splat_response.get("statusCode") == 200:
+        return base64.b64decode(splat_response.get("body"))
+    # ==== Failure ====
+    # Lambda timeout et al.
+    elif error_message := splat_response.get("errorMessage"):
+        raise SplatPDFGenerationFailure(
+            f"Error returned from lambda invocation: {error_message}"
+        )
+    # All other errors
     else:
         # Try to extract an error message from splat response
         try:
             splat_error = json.loads(splat_response["body"])["errors"][0]
         except (KeyError, JSONDecodeError):
             splat_error = splat_response
         raise SplatPDFGenerationFailure(f"Error returned from splat: {splat_error}")
```

### Comparing `uptick_splat-0.1.2/PKG-INFO` & `uptick_splat-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptick-splat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django library for invoking splat
 Author: william chu
 Author-email: william.chu@uptickhq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

