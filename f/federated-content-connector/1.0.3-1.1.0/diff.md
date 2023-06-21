# Comparing `tmp/federated-content-connector-1.0.3.tar.gz` & `tmp/federated-content-connector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-1.0.3.tar", last modified: Thu Jun 15 13:46:12 2023, max compression
+gzip compressed data, was "federated-content-connector-1.1.0.tar", last modified: Wed Jun 21 07:01:48 2023, max compression
```

## Comparing `federated-content-connector-1.0.3.tar` & `federated-content-connector-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8567 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     9586 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/course_metadata_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/management/commands/import_course_runs_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.193713 federated-content-connector-1.0.3/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8567 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.831844 federated-content-connector-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-21 07:01:48.831844 federated-content-connector-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.823843 federated-content-connector-1.1.0/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10613 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/course_metadata_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/commands/import_course_runs_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/commands/refresh_course_runs_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/migrations/0002_coursedetailsimportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.819843 federated-content-connector-1.1.0/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.823843 federated-content-connector-1.1.0/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-21 07:01:48.831844 federated-content-connector-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/tests/test_signals.py
```

### Comparing `federated-content-connector-1.0.3/CHANGELOG.rst` & `federated-content-connector-1.1.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.1.0 – 2023-06-21
+------------------
+* Management command to refresh CourseDetails data
+
 1.0.3 – 2023-06-15
 ------------------
 * backfill all data
 
 1.0.2 – 2023-06-15
 ------------------
 * Handle empty courserun seats.
```

### Comparing `federated-content-connector-1.0.3/LICENSE.txt` & `federated-content-connector-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/PKG-INFO` & `federated-content-connector-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.3
+Version: 1.1.0
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.1.0 – 2023-06-21
+------------------
+* Management command to refresh CourseDetails data
+
 1.0.3 – 2023-06-15
 ------------------
 * backfill all data
 
 1.0.2 – 2023-06-15
 ------------------
 * Handle empty courserun seats.
```

### Comparing `federated-content-connector-1.0.3/README.rst` & `federated-content-connector-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/federated_content_connector/apps.py` & `federated-content-connector-1.1.0/federated_content_connector/apps.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/federated_content_connector/course_metadata_importer.py` & `federated-content-connector-1.1.0/federated_content_connector/course_metadata_importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Course metadata importer."""
 
 import datetime
 import logging
-from urllib.parse import quote_plus, urljoin
+from urllib.parse import quote_plus, urlencode, urljoin
 
 import pytz
 from common.djangoapps.course_modes.models import CourseMode
 from django.contrib.auth import get_user_model
 from django.db.models import Q
 from openedx.core.djangoapps.catalog.models import CatalogIntegration
 from openedx.core.djangoapps.catalog.utils import get_catalog_api_base_url, get_catalog_api_client
@@ -140,14 +140,42 @@
         courses_not_found = list(set(course_keys) - set(course_keys_in_response))
         if courses_not_found:
             logger.info(f'[COURSE_METADATA_IMPORTER] Courses not found in discovery. Courses: {courses_not_found}')
 
         return results
 
     @classmethod
+    def courses(cls, timestamp):
+        """Fetch courses updated since `timestamp`."""
+        query_params = {
+            'timestamp': timestamp,
+            'limit': 50
+        }
+        client = cls.get_api_client()
+        api_base_url = get_catalog_api_base_url()
+        params = urlencode(query_params)
+        api_url = urljoin(f"{api_base_url}/", f"courses/?{params}")
+        results, next_url, total = cls.get_api_reponse(client, api_url)
+        logger.info(f'[COURSE_METADATA_IMPORTER] Total Records are {total}')
+        yield results
+
+        while next_url:
+            results, next_url, __ = cls.get_api_reponse(client, next_url)
+            yield results
+
+    @classmethod
+    def get_api_reponse(cls, client, api_url):
+        """Get response from API."""
+        response = client.get(api_url)
+        response.raise_for_status()
+        courses = response.json()
+        results = courses.get('results', [])
+        return results, courses.get('next'), courses.get('count')
+
+    @classmethod
     def process_courses_details(cls, courserun_locators, courses_details):
         """
         Parse and extract the minimal data that we need.
         """
         log_prefix = 'COURSE_METADATA_IMPORTER'
 
         courses = {}
```

### Comparing `federated-content-connector-1.0.3/federated_content_connector/filters/pipeline.py` & `federated-content-connector-1.1.0/federated_content_connector/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/federated_content_connector/migrations/0001_initial.py` & `federated-content-connector-1.1.0/federated_content_connector/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/federated_content_connector/models.py` & `federated-content-connector-1.1.0/federated_content_connector/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -43,7 +43,49 @@
 
     class Meta:
         """
         Meta class for CourseDetails.
         """
 
         app_label = 'federated_content_connector'
+
+
+class CourseDetailsImportStatus(TimeStampedModel):
+    """
+    CourseDetails import status history.
+
+    .. no_pii:
+    """
+
+    TIMESTAMP_FORMAT = '%Y-%m-%dT%H:%M:%S.%fZ'
+
+    last_successful_import_at = models.DateTimeField(help_text='Timestamp of last data import')
+
+    @classmethod
+    def last_successful_import_timestamp(cls):
+        """
+        Return `last_successful_import_at`.
+        """
+        last_import = cls.objects.first()
+        if last_import:
+            return last_import.last_successful_import_at.strftime(cls.TIMESTAMP_FORMAT)
+
+        return None
+
+    @classmethod
+    def save_last_successful_import_timestamp(cls, timestamp):
+        """
+        Save `last_successful_import_at`.
+        """
+        last_import = cls.objects.first()
+        if last_import:
+            last_import.last_successful_import_at = timestamp
+            last_import.save()
+        else:
+            cls.objects.create(last_successful_import_at=timestamp)
+
+    class Meta:
+        """
+        Meta class for CourseDetailsImportStatus.
+        """
+
+        app_label = 'federated_content_connector'
```

### Comparing `federated-content-connector-1.0.3/federated_content_connector/signals.py` & `federated-content-connector-1.1.0/federated_content_connector/signals.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/federated_content_connector/tasks.py` & `federated-content-connector-1.1.0/federated_content_connector/tasks.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-1.1.0/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-1.1.0/federated_content_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.3
+Version: 1.1.0
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.1.0 – 2023-06-21
+------------------
+* Management command to refresh CourseDetails data
+
 1.0.3 – 2023-06-15
 ------------------
 * backfill all data
 
 1.0.2 – 2023-06-15
 ------------------
 * Handle empty courserun seats.
```

### Comparing `federated-content-connector-1.0.3/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-1.1.0/federated_content_connector.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 federated_content_connector.egg-info/requires.txt
 federated_content_connector.egg-info/top_level.txt
 federated_content_connector/filters/__init__.py
 federated_content_connector/filters/pipeline.py
 federated_content_connector/management/__init__.py
 federated_content_connector/management/commands/__init__.py
 federated_content_connector/management/commands/import_course_runs_metadata.py
+federated_content_connector/management/commands/refresh_course_runs_metadata.py
 federated_content_connector/migrations/0001_initial.py
+federated_content_connector/migrations/0002_coursedetailsimportstatus.py
 federated_content_connector/migrations/__init__.py
 federated_content_connector/settings/__init__.py
 federated_content_connector/settings/common.py
 federated_content_connector/settings/production.py
 federated_content_connector/templates/federated_content_connector/base.html
 requirements/base.in
 requirements/constraints.txt
```

### Comparing `federated-content-connector-1.0.3/requirements/constraints.txt` & `federated-content-connector-1.1.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/setup.py` & `federated-content-connector-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.3/tests/test_signals.py` & `federated-content-connector-1.1.0/tests/test_signals.py`

 * *Files identical despite different names*

