# Comparing `tmp/aanalytics2-0.3.5.tar.gz` & `tmp/aanalytics2-0.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalytics2-0.3.5.tar", last modified: Tue Jun 20 19:48:06 2023, max compression
+gzip compressed data, was "aanalytics2-0.4.0.post1.tar", last modified: Tue Jun 20 19:59:13 2023, max compression
```

## Comparing `aanalytics2-0.3.5.tar` & `aanalytics2-0.4.0.post1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 19:48:06.307506 aanalytics2-0.3.5/
--rw-rw-rw-   0        0        0     1781 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/.gitignore
--rw-rw-rw-   0        0        0    10337 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4574 2023-06-20 19:48:06.308503 aanalytics2-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3418 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 19:48:06.207851 aanalytics2-0.3.5/aanalytics2/
--rw-rw-rw-   0        0        0     5205 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/aanalytics2/CSV_Column_and_Query_String_Reference.pickle
--rw-rw-rw-   0        0        0      177 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/aanalytics2/__init__.py
--rw-rw-rw-   0        0        0       21 2023-06-20 19:47:33.000000 aanalytics2-0.3.5/aanalytics2/__version__.py
--rw-rw-rw-   0        0        0     2872 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/aanalytics2/aanalytics14.py
--rw-rw-rw-   0        0        0   162415 2023-06-19 13:03:19.000000 aanalytics2-0.3.5/aanalytics2/aanalytics2.py
--rw-rw-rw-   0        0        0      700 2023-06-16 16:01:24.000000 aanalytics2-0.3.5/aanalytics2/config.py
--rw-rw-rw-   0        0        0     8123 2023-06-19 07:48:09.000000 aanalytics2-0.3.5/aanalytics2/configs.py
--rw-rw-rw-   0        0        0    11517 2023-06-19 07:55:29.000000 aanalytics2-0.3.5/aanalytics2/connector.py
--rw-rw-rw-   0        0        0     1637 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/aanalytics2/eventType_usageLogs.pickle
--rw-rw-rw-   0        0        0    12776 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/aanalytics2/ingestion.py
--rw-rw-rw-   0        0        0    10668 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/aanalytics2/projects.py
--rw-rw-rw-   0        0        0    17764 2023-05-10 18:33:43.000000 aanalytics2-0.3.5/aanalytics2/requestCreator.py
--rw-rw-rw-   0        0        0     6765 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/aanalytics2/supported_tags.pickle
--rw-rw-rw-   0        0        0     3871 2023-06-19 07:55:21.000000 aanalytics2-0.3.5/aanalytics2/token_provider.py
--rw-rw-rw-   0        0        0    10180 2023-05-10 18:33:43.000000 aanalytics2-0.3.5/aanalytics2/workspace.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:48:06.227825 aanalytics2-0.3.5/aanalytics2.egg-info/
--rw-rw-rw-   0        0        0     4574 2023-06-20 19:48:05.000000 aanalytics2-0.3.5/aanalytics2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2023-06-20 19:48:06.000000 aanalytics2-0.3.5/aanalytics2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 19:48:05.000000 aanalytics2-0.3.5/aanalytics2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-06-20 19:48:05.000000 aanalytics2-0.3.5/aanalytics2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 19:48:05.000000 aanalytics2-0.3.5/aanalytics2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 19:48:06.290551 aanalytics2-0.3.5/docs/
--rw-rw-rw-   0        0        0    27866 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/BAPI_REF.png
--rw-rw-rw-   0        0        0    29602 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/DIAPI_REF.png
--rw-rw-rw-   0        0        0        0 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/analytics.md
--rw-rw-rw-   0        0        0     1833 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/authenticating_without_config_json.md
--rw-rw-rw-   0        0        0     5293 2023-06-19 11:15:26.000000 aanalytics2-0.3.5/docs/getting_started.md
--rw-rw-rw-   0        0        0     9677 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/ingestion.md
--rw-rw-rw-   0        0        0     3967 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/legacyAnalytics.md
--rw-rw-rw-   0        0        0     4069 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/logging.md
--rw-rw-rw-   0        0        0    40838 2023-05-10 18:33:43.000000 aanalytics2-0.3.5/docs/main.md
--rw-rw-rw-   0        0        0     8789 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/projects.md
--rw-rw-rw-   0        0        0     9580 2023-06-19 13:04:29.000000 aanalytics2-0.3.5/docs/releases.md
--rw-rw-rw-   0        0        0     6182 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/requestCreator.md
--rw-rw-rw-   0        0        0     1980 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/test.md
--rw-rw-rw-   0        0        0     3349 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/docs/workspace.md
--rw-rw-rw-   0        0        0     1478 2023-06-20 12:07:59.000000 aanalytics2-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      134 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-06-20 19:48:06.311494 aanalytics2-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1873 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:48:06.303665 aanalytics2-0.3.5/test/
--rw-rw-rw-   0        0        0        0 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/test/__init__.py
--rw-rw-rw-   0        0        0      907 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/test/test_configuration.py
--rw-rw-rw-   0        0        0     2538 2023-05-10 18:37:43.000000 aanalytics2-0.3.5/test/test_core_analytics.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:59:13.551857 aanalytics2-0.4.0.post1/
+-rw-rw-rw-   0        0        0     1781 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/.gitignore
+-rw-rw-rw-   0        0        0    10337 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4580 2023-06-20 19:59:13.552852 aanalytics2-0.4.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     3418 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 19:59:13.350366 aanalytics2-0.4.0.post1/aanalytics2/
+-rw-rw-rw-   0        0        0     5205 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/aanalytics2/CSV_Column_and_Query_String_Reference.pickle
+-rw-rw-rw-   0        0        0      177 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/aanalytics2/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-20 19:58:17.000000 aanalytics2-0.4.0.post1/aanalytics2/__version__.py
+-rw-rw-rw-   0        0        0     2872 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/aanalytics2/aanalytics14.py
+-rw-rw-rw-   0        0        0   162415 2023-06-19 13:03:19.000000 aanalytics2-0.4.0.post1/aanalytics2/aanalytics2.py
+-rw-rw-rw-   0        0        0      700 2023-06-16 16:01:24.000000 aanalytics2-0.4.0.post1/aanalytics2/config.py
+-rw-rw-rw-   0        0        0     8123 2023-06-19 07:48:09.000000 aanalytics2-0.4.0.post1/aanalytics2/configs.py
+-rw-rw-rw-   0        0        0    11517 2023-06-19 07:55:29.000000 aanalytics2-0.4.0.post1/aanalytics2/connector.py
+-rw-rw-rw-   0        0        0     1637 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/aanalytics2/eventType_usageLogs.pickle
+-rw-rw-rw-   0        0        0    12776 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/aanalytics2/ingestion.py
+-rw-rw-rw-   0        0        0    10668 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/aanalytics2/projects.py
+-rw-rw-rw-   0        0        0    17764 2023-05-10 18:33:43.000000 aanalytics2-0.4.0.post1/aanalytics2/requestCreator.py
+-rw-rw-rw-   0        0        0     6765 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/aanalytics2/supported_tags.pickle
+-rw-rw-rw-   0        0        0     3871 2023-06-19 07:55:21.000000 aanalytics2-0.4.0.post1/aanalytics2/token_provider.py
+-rw-rw-rw-   0        0        0    10180 2023-05-10 18:33:43.000000 aanalytics2-0.4.0.post1/aanalytics2/workspace.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:59:13.384375 aanalytics2-0.4.0.post1/aanalytics2.egg-info/
+-rw-rw-rw-   0        0        0     4580 2023-06-20 19:59:12.000000 aanalytics2-0.4.0.post1/aanalytics2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2023-06-20 19:59:13.000000 aanalytics2-0.4.0.post1/aanalytics2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:59:12.000000 aanalytics2-0.4.0.post1/aanalytics2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-06-20 19:59:12.000000 aanalytics2-0.4.0.post1/aanalytics2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 19:59:12.000000 aanalytics2-0.4.0.post1/aanalytics2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 19:59:13.490224 aanalytics2-0.4.0.post1/docs/
+-rw-rw-rw-   0        0        0    27866 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/BAPI_REF.png
+-rw-rw-rw-   0        0        0    29602 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/DIAPI_REF.png
+-rw-rw-rw-   0        0        0        0 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/analytics.md
+-rw-rw-rw-   0        0        0     1833 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/authenticating_without_config_json.md
+-rw-rw-rw-   0        0        0     5293 2023-06-19 11:15:26.000000 aanalytics2-0.4.0.post1/docs/getting_started.md
+-rw-rw-rw-   0        0        0     9677 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/ingestion.md
+-rw-rw-rw-   0        0        0     3967 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/legacyAnalytics.md
+-rw-rw-rw-   0        0        0     4069 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/logging.md
+-rw-rw-rw-   0        0        0    40838 2023-05-10 18:33:43.000000 aanalytics2-0.4.0.post1/docs/main.md
+-rw-rw-rw-   0        0        0     8789 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/projects.md
+-rw-rw-rw-   0        0        0     9580 2023-06-19 13:04:29.000000 aanalytics2-0.4.0.post1/docs/releases.md
+-rw-rw-rw-   0        0        0     6182 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/requestCreator.md
+-rw-rw-rw-   0        0        0     1980 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/test.md
+-rw-rw-rw-   0        0        0     3349 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/docs/workspace.md
+-rw-rw-rw-   0        0        0     1478 2023-06-20 19:58:19.000000 aanalytics2-0.4.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0      134 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 19:59:13.558221 aanalytics2-0.4.0.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1873 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:59:13.546017 aanalytics2-0.4.0.post1/test/
+-rw-rw-rw-   0        0        0        0 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/test/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/test/test_configuration.py
+-rw-rw-rw-   0        0        0     2538 2023-05-10 18:37:43.000000 aanalytics2-0.4.0.post1/test/test_core_analytics.py
```

### Comparing `aanalytics2-0.3.5/.gitignore` & `aanalytics2-0.4.0.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/LICENSE` & `aanalytics2-0.4.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/PKG-INFO` & `aanalytics2-0.4.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalytics2
-Version: 0.3.5
+Version: 0.4.0.post1
 Summary: Adobe Analytics API 2.0 and 1.4 python wrapper
 Home-page: https://github.com/pitchmuc/adobe-analytics-api-2.0
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/adobe-analytics-api-2.0
 Project-URL: changelog, https://github.com/pitchmuc/adobe-analytics-api-2.0/blob/master/docs/releases.md
```

### Comparing `aanalytics2-0.3.5/README.md` & `aanalytics2-0.4.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/CSV_Column_and_Query_String_Reference.pickle` & `aanalytics2-0.4.0.post1/aanalytics2/CSV_Column_and_Query_String_Reference.pickle`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/aanalytics14.py` & `aanalytics2-0.4.0.post1/aanalytics2/aanalytics14.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/aanalytics2.py` & `aanalytics2-0.4.0.post1/aanalytics2/aanalytics2.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/config.py` & `aanalytics2-0.4.0.post1/aanalytics2/config.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/configs.py` & `aanalytics2-0.4.0.post1/aanalytics2/configs.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/connector.py` & `aanalytics2-0.4.0.post1/aanalytics2/connector.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/eventType_usageLogs.pickle` & `aanalytics2-0.4.0.post1/aanalytics2/eventType_usageLogs.pickle`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/ingestion.py` & `aanalytics2-0.4.0.post1/aanalytics2/ingestion.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/projects.py` & `aanalytics2-0.4.0.post1/aanalytics2/projects.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/requestCreator.py` & `aanalytics2-0.4.0.post1/aanalytics2/requestCreator.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/supported_tags.pickle` & `aanalytics2-0.4.0.post1/aanalytics2/supported_tags.pickle`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/token_provider.py` & `aanalytics2-0.4.0.post1/aanalytics2/token_provider.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2/workspace.py` & `aanalytics2-0.4.0.post1/aanalytics2/workspace.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/aanalytics2.egg-info/PKG-INFO` & `aanalytics2-0.4.0.post1/aanalytics2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalytics2
-Version: 0.3.5
+Version: 0.4.0.post1
 Summary: Adobe Analytics API 2.0 and 1.4 python wrapper
 Home-page: https://github.com/pitchmuc/adobe-analytics-api-2.0
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/adobe-analytics-api-2.0
 Project-URL: changelog, https://github.com/pitchmuc/adobe-analytics-api-2.0/blob/master/docs/releases.md
```

### Comparing `aanalytics2-0.3.5/aanalytics2.egg-info/SOURCES.txt` & `aanalytics2-0.4.0.post1/aanalytics2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/BAPI_REF.png` & `aanalytics2-0.4.0.post1/docs/BAPI_REF.png`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/DIAPI_REF.png` & `aanalytics2-0.4.0.post1/docs/DIAPI_REF.png`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/authenticating_without_config_json.md` & `aanalytics2-0.4.0.post1/docs/authenticating_without_config_json.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/getting_started.md` & `aanalytics2-0.4.0.post1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/ingestion.md` & `aanalytics2-0.4.0.post1/docs/ingestion.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/legacyAnalytics.md` & `aanalytics2-0.4.0.post1/docs/legacyAnalytics.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/logging.md` & `aanalytics2-0.4.0.post1/docs/logging.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/main.md` & `aanalytics2-0.4.0.post1/docs/main.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/projects.md` & `aanalytics2-0.4.0.post1/docs/projects.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/releases.md` & `aanalytics2-0.4.0.post1/docs/releases.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/requestCreator.md` & `aanalytics2-0.4.0.post1/docs/requestCreator.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/test.md` & `aanalytics2-0.4.0.post1/docs/test.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/docs/workspace.md` & `aanalytics2-0.4.0.post1/docs/workspace.md`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/pyproject.toml` & `aanalytics2-0.4.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/setup.py` & `aanalytics2-0.4.0.post1/setup.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/test/test_configuration.py` & `aanalytics2-0.4.0.post1/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `aanalytics2-0.3.5/test/test_core_analytics.py` & `aanalytics2-0.4.0.post1/test/test_core_analytics.py`

 * *Files identical despite different names*

