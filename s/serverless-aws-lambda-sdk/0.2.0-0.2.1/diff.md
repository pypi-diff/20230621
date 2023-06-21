# Comparing `tmp/serverless-aws-lambda-sdk-0.2.0.tar.gz` & `tmp/serverless-aws-lambda-sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/dist/.tmp-h60s0tzu/serverless-aws-lambda-sdk-0.2.0.tar", last modified: Mon Jun 19 16:00:57 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/dist/.tmp-j4kltbbd/serverless-aws-lambda-sdk-0.2.1.tar", last modified: Wed Jun 21 15:42:54 2023, max compression
```

## Comparing `serverless-aws-lambda-sdk-0.2.0.tar` & `serverless-aws-lambda-sdk-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/api_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/event_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/invocation_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/trace_spans/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/trace_spans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/api_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/event_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/invocation_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/tests/test_sdk.py
```

### Comparing `serverless-aws-lambda-sdk-0.2.0/PKG-INFO` & `serverless-aws-lambda-sdk-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-aws-lambda-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Serverless AWS Lambda SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/aws-lambda-sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/aws-lambda-sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-aws-lambda-sdk-0.2.0/README.md` & `serverless-aws-lambda-sdk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/pyproject.toml` & `serverless-aws-lambda-sdk-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "serverless-sdk~=0.5.0",
+    "serverless-sdk~=0.5.1",
     "serverless-sdk-schema~=0.2.3",
     "typing-extensions~=4.5", # included in Python 3.8 - 3.11
 ]
 [project.optional-dependencies]
 tests = [
     "black>=22.12",
     "boto3>=1.16.112",
```

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/__init__.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/__init__.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/event_tags.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/event_tags.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/response_tags.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/response_tags.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/telemetry.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/telemetry.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/wrapper.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/PKG-INFO` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-aws-lambda-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Serverless AWS Lambda SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/aws-lambda-sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/aws-lambda-sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/SOURCES.txt` & `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.0/tests/test_sdk.py` & `serverless-aws-lambda-sdk-0.2.1/tests/test_sdk.py`

 * *Files identical despite different names*

