# Comparing `tmp/aleph-alpha-client-3.1.2.tar.gz` & `tmp/aleph-alpha-client-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-alpha-client-3.1.2.tar", last modified: Wed May 31 10:01:53 2023, max compression
+gzip compressed data, was "aleph-alpha-client-3.1.3.tar", last modified: Wed Jun 21 09:23:39 2023, max compression
```

## Comparing `aleph-alpha-client-3.1.2.tar` & `aleph-alpha-client-3.1.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/aleph_alpha_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/aleph_alpha_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/detokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:23:39.511562 aleph-alpha-client-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-21 09:23:39.511562 aleph-alpha-client-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:23:39.507562 aleph-alpha-client-3.1.3/aleph_alpha_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/aleph_alpha_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/detokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/aleph_alpha_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:23:39.507562 aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-21 09:23:39.000000 aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-21 09:23:39.000000 aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:23:39.000000 aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 09:23:39.000000 aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 09:23:39.000000 aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:23:39.511562 aleph-alpha-client-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:23:39.511562 aleph-alpha-client-3.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 09:23:28.000000 aleph-alpha-client-3.1.3/tests/test_wildcard_import.py
```

### Comparing `aleph-alpha-client-3.1.2/LICENSE` & `aleph-alpha-client-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/PKG-INFO` & `aleph-alpha-client-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.2
+Version: 3.1.3
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.2/README.md` & `aleph-alpha-client-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/__init__.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     CustomGranularity,
     Explanation,
     ExplanationPostprocessing,
     ExplanationRequest,
     ExplanationResponse,
     ImagePromptItemExplanation,
     ImageScore,
+    PromptGranularity,
     TargetGranularity,
     TargetPromptItemExplanation,
     TargetScore,
     TextPromptItemExplanation,
     TextScore,
     TokenPromptItemExplanation,
     TokenScore,
```

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/aleph_alpha_client.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/aleph_alpha_client.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/completion.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/completion.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/detokenization.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/detokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/document.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/document.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/embedding.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/embedding.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/evaluation.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/evaluation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/explanation.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/prompt.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/qa.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/search.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/summarization.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/summarization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client/tokenization.py` & `aleph-alpha-client-3.1.3/aleph_alpha_client/tokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/PKG-INFO` & `aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.2
+Version: 3.1.3
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/SOURCES.txt` & `aleph-alpha-client-3.1.3/aleph_alpha_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 tests/test_evaluate.py
 tests/test_explanation.py
 tests/test_image.py
 tests/test_prompt.py
 tests/test_qa.py
 tests/test_search.py
 tests/test_summarize.py
-tests/test_tokenize.py
+tests/test_tokenize.py
+tests/test_wildcard_import.py
```

### Comparing `aleph-alpha-client-3.1.2/setup.py` & `aleph-alpha-client-3.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_clients.py` & `aleph-alpha-client-3.1.3/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_complete.py` & `aleph-alpha-client-3.1.3/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_detokenize.py` & `aleph-alpha-client-3.1.3/tests/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_embed.py` & `aleph-alpha-client-3.1.3/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_error_handling.py` & `aleph-alpha-client-3.1.3/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_evaluate.py` & `aleph-alpha-client-3.1.3/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_explanation.py` & `aleph-alpha-client-3.1.3/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_image.py` & `aleph-alpha-client-3.1.3/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_prompt.py` & `aleph-alpha-client-3.1.3/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_qa.py` & `aleph-alpha-client-3.1.3/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_search.py` & `aleph-alpha-client-3.1.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_summarize.py` & `aleph-alpha-client-3.1.3/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.2/tests/test_tokenize.py` & `aleph-alpha-client-3.1.3/tests/test_tokenize.py`

 * *Files identical despite different names*

