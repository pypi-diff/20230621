# Comparing `tmp/readme-metrics-3.0.0.tar.gz` & `tmp/readme-metrics-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme-metrics-3.0.0.tar", last modified: Fri Apr 14 14:14:35 2023, max compression
+gzip compressed data, was "readme-metrics-3.0.1.tar", last modified: Wed Jun 21 16:21:37 2023, max compression
```

## Comparing `readme-metrics-3.0.0.tar` & `readme-metrics-3.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-14 14:14:35.906556 readme-metrics-3.0.0/
--rw-r--r--   0 domh       (501) staff       (20)      725 2022-08-22 12:38:51.000000 readme-metrics-3.0.0/LICENSE
--rw-r--r--   0 domh       (501) staff       (20)     2414 2023-04-14 14:14:35.906420 readme-metrics-3.0.0/PKG-INFO
--rw-r--r--   0 domh       (501) staff       (20)     2091 2023-02-22 13:36:42.000000 readme-metrics-3.0.0/README.md
-drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-14 14:14:35.905538 readme-metrics-3.0.0/readme_metrics/
--rw-r--r--   0 domh       (501) staff       (20)     3856 2022-09-06 16:49:05.000000 readme-metrics-3.0.0/readme_metrics/Metrics.py
--rw-r--r--   0 domh       (501) staff       (20)     5998 2022-09-06 16:49:05.000000 readme-metrics-3.0.0/readme_metrics/MetricsApiConfig.py
--rw-r--r--   0 domh       (501) staff       (20)     4225 2022-08-22 12:38:51.000000 readme-metrics-3.0.0/readme_metrics/MetricsMiddleware.py
--rw-r--r--   0 domh       (501) staff       (20)    14362 2022-09-15 09:53:54.000000 readme-metrics-3.0.0/readme_metrics/PayloadBuilder.py
--rw-r--r--   0 domh       (501) staff       (20)     1246 2022-04-13 15:12:08.000000 readme-metrics-3.0.0/readme_metrics/ResponseInfoWrapper.py
--rw-r--r--   0 domh       (501) staff       (20)     1107 2023-04-14 14:08:19.000000 readme-metrics-3.0.0/readme_metrics/VerifyWebhook.py
--rw-r--r--   0 domh       (501) staff       (20)      147 2023-04-14 14:12:56.000000 readme-metrics-3.0.0/readme_metrics/__init__.py
--rw-r--r--   0 domh       (501) staff       (20)     1868 2022-09-06 16:49:05.000000 readme-metrics-3.0.0/readme_metrics/django.py
--rw-r--r--   0 domh       (501) staff       (20)     2021 2022-08-24 14:21:21.000000 readme-metrics-3.0.0/readme_metrics/flask_readme.py
--rw-r--r--   0 domh       (501) staff       (20)     1565 2023-02-22 13:36:42.000000 readme-metrics-3.0.0/readme_metrics/publisher.py
--rw-r--r--   0 domh       (501) staff       (20)      357 2022-09-06 09:57:52.000000 readme-metrics-3.0.0/readme_metrics/util.py
-drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-14 14:14:35.906244 readme-metrics-3.0.0/readme_metrics.egg-info/
--rw-r--r--   0 domh       (501) staff       (20)     2414 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/PKG-INFO
--rw-r--r--   0 domh       (501) staff       (20)      549 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 domh       (501) staff       (20)        1 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 domh       (501) staff       (20)       50 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/requires.txt
--rw-r--r--   0 domh       (501) staff       (20)       15 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/top_level.txt
--rw-r--r--   0 domh       (501) staff       (20)       38 2023-04-14 14:14:35.906601 readme-metrics-3.0.0/setup.cfg
--rw-r--r--   0 domh       (501) staff       (20)      650 2022-08-22 12:38:51.000000 readme-metrics-3.0.0/setup.py
+drwxr-xr-x   0 erunion    (501) staff       (20)        0 2023-06-21 16:21:37.503307 readme-metrics-3.0.1/
+-rw-r--r--   0 erunion    (501) staff       (20)      725 2022-08-10 16:07:18.000000 readme-metrics-3.0.1/LICENSE
+-rw-r--r--   0 erunion    (501) staff       (20)     2414 2023-06-21 16:21:37.503189 readme-metrics-3.0.1/PKG-INFO
+-rw-r--r--   0 erunion    (501) staff       (20)     2091 2022-12-16 18:11:05.000000 readme-metrics-3.0.1/README.md
+drwxr-xr-x   0 erunion    (501) staff       (20)        0 2023-06-21 16:21:37.502494 readme-metrics-3.0.1/readme_metrics/
+-rw-r--r--   0 erunion    (501) staff       (20)     3856 2022-09-06 16:40:49.000000 readme-metrics-3.0.1/readme_metrics/Metrics.py
+-rw-r--r--   0 erunion    (501) staff       (20)     5998 2022-09-06 16:40:49.000000 readme-metrics-3.0.1/readme_metrics/MetricsApiConfig.py
+-rw-r--r--   0 erunion    (501) staff       (20)     4225 2022-08-31 22:56:37.000000 readme-metrics-3.0.1/readme_metrics/MetricsMiddleware.py
+-rw-r--r--   0 erunion    (501) staff       (20)    14358 2023-06-21 16:11:20.000000 readme-metrics-3.0.1/readme_metrics/PayloadBuilder.py
+-rw-r--r--   0 erunion    (501) staff       (20)     1246 2022-08-10 16:07:18.000000 readme-metrics-3.0.1/readme_metrics/ResponseInfoWrapper.py
+-rw-r--r--   0 erunion    (501) staff       (20)     1107 2023-04-28 19:11:49.000000 readme-metrics-3.0.1/readme_metrics/VerifyWebhook.py
+-rw-r--r--   0 erunion    (501) staff       (20)      147 2023-06-21 16:13:37.000000 readme-metrics-3.0.1/readme_metrics/__init__.py
+-rw-r--r--   0 erunion    (501) staff       (20)     1868 2022-09-06 16:40:49.000000 readme-metrics-3.0.1/readme_metrics/django.py
+-rw-r--r--   0 erunion    (501) staff       (20)     2021 2022-08-15 15:46:25.000000 readme-metrics-3.0.1/readme_metrics/flask_readme.py
+-rw-r--r--   0 erunion    (501) staff       (20)     3642 2023-04-28 19:11:49.000000 readme-metrics-3.0.1/readme_metrics/publisher.py
+-rw-r--r--   0 erunion    (501) staff       (20)      357 2022-09-03 06:58:47.000000 readme-metrics-3.0.1/readme_metrics/util.py
+drwxr-xr-x   0 erunion    (501) staff       (20)        0 2023-06-21 16:21:37.503046 readme-metrics-3.0.1/readme_metrics.egg-info/
+-rw-r--r--   0 erunion    (501) staff       (20)     2414 2023-06-21 16:21:37.000000 readme-metrics-3.0.1/readme_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 erunion    (501) staff       (20)      549 2023-06-21 16:21:37.000000 readme-metrics-3.0.1/readme_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 erunion    (501) staff       (20)        1 2023-06-21 16:21:37.000000 readme-metrics-3.0.1/readme_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 erunion    (501) staff       (20)       50 2023-06-21 16:21:37.000000 readme-metrics-3.0.1/readme_metrics.egg-info/requires.txt
+-rw-r--r--   0 erunion    (501) staff       (20)       15 2023-06-21 16:21:37.000000 readme-metrics-3.0.1/readme_metrics.egg-info/top_level.txt
+-rw-r--r--   0 erunion    (501) staff       (20)       38 2023-06-21 16:21:37.503339 readme-metrics-3.0.1/setup.cfg
+-rw-r--r--   0 erunion    (501) staff       (20)      650 2022-08-15 16:25:29.000000 readme-metrics-3.0.1/setup.py
```

### Comparing `readme-metrics-3.0.0/LICENSE` & `readme-metrics-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/PKG-INFO` & `readme-metrics-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-metrics
-Version: 3.0.0
+Version: 3.0.1
 Summary: ReadMe API Metrics SDK
 Home-page: https://github.com/readmeio/metrics-sdks/tree/main/packages/python
 Author: ReadMe
 Author-email: support@readme.io
 Description-Content-Type: text/markdown
 Provides-Extra: Flask
 Provides-Extra: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.0 Summary: ReadMe API
+Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.1 Summary: ReadMe API
 Metrics SDK Home-page: https://github.com/readmeio/metrics-sdks/tree/main/
 packages/python Author: ReadMe Author-email: support@readme.io Description-
 Content-Type: text/markdown Provides-Extra: Flask Provides-Extra: Django
 License-File: LICENSE # ReadMe Metrics
 [https://user-images.githubusercontent.com/33762/182927634-2aebeb46-c215-4ac3-
                             9e98-61f931e33583.png]
             Track usage of your API and troubleshoot issues faster.
```

### Comparing `readme-metrics-3.0.0/README.md` & `readme-metrics-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics/Metrics.py` & `readme-metrics-3.0.1/readme_metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics/MetricsApiConfig.py` & `readme-metrics-3.0.1/readme_metrics/MetricsApiConfig.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics/MetricsMiddleware.py` & `readme-metrics-3.0.1/readme_metrics/MetricsMiddleware.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics/PayloadBuilder.py` & `readme-metrics-3.0.1/readme_metrics/PayloadBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections.abc import Mapping
 import importlib
 import json
 from json import JSONDecodeError
 from logging import Logger
-import os
 import platform
 import time
 
 from typing import List, Optional
 from urllib import parse
 import uuid
 
@@ -97,15 +96,15 @@
 
     def _get_har_creator_comment(self):
         # arm64-darwin21.3.0/3.8.9
         return (
             platform.machine()
             + "-"
             + platform.system().lower()
-            + os.uname().release
+            + platform.uname().release
             + "/"
             + platform.python_version()
         )
 
     def _validate_group(self, group: Optional[dict]):
         if group is None:
             return None
```

### Comparing `readme-metrics-3.0.0/readme_metrics/ResponseInfoWrapper.py` & `readme-metrics-3.0.1/readme_metrics/ResponseInfoWrapper.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics/VerifyWebhook.py` & `readme-metrics-3.0.1/readme_metrics/VerifyWebhook.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics/django.py` & `readme-metrics-3.0.1/readme_metrics/django.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics/flask_readme.py` & `readme-metrics-3.0.1/readme_metrics/flask_readme.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/readme_metrics.egg-info/PKG-INFO` & `readme-metrics-3.0.1/readme_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-metrics
-Version: 3.0.0
+Version: 3.0.1
 Summary: ReadMe API Metrics SDK
 Home-page: https://github.com/readmeio/metrics-sdks/tree/main/packages/python
 Author: ReadMe
 Author-email: support@readme.io
 Description-Content-Type: text/markdown
 Provides-Extra: Flask
 Provides-Extra: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.0 Summary: ReadMe API
+Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.1 Summary: ReadMe API
 Metrics SDK Home-page: https://github.com/readmeio/metrics-sdks/tree/main/
 packages/python Author: ReadMe Author-email: support@readme.io Description-
 Content-Type: text/markdown Provides-Extra: Flask Provides-Extra: Django
 License-File: LICENSE # ReadMe Metrics
 [https://user-images.githubusercontent.com/33762/182927634-2aebeb46-c215-4ac3-
                             9e98-61f931e33583.png]
             Track usage of your API and troubleshoot issues faster.
```

### Comparing `readme-metrics-3.0.0/readme_metrics.egg-info/SOURCES.txt` & `readme-metrics-3.0.1/readme_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.0/setup.py` & `readme-metrics-3.0.1/setup.py`

 * *Files identical despite different names*

