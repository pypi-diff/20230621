# Comparing `tmp/fb-python-sdk-1.1.2.tar.gz` & `tmp/fb-python-sdk-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb-python-sdk-1.1.2.tar", last modified: Mon May 15 14:50:11 2023, max compression
+gzip compressed data, was "fb-python-sdk-1.1.3.tar", last modified: Wed Jun 21 12:11:13 2023, max compression
```

## Comparing `fb-python-sdk-1.1.2.tar` & `fb-python-sdk-1.1.3.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.948225 fb-python-sdk-1.1.2/
--rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.2/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)    10444 2023-05-15 14:50:11.947834 fb-python-sdk-1.1.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     9372 2023-05-15 14:37:00.000000 fb-python-sdk-1.1.2/README.md
--rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/dev-requirements.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.932296 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    10444 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1142 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      218 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       34 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.939515 fb-python-sdk-1.1.2/fbclient/
--rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/category.py
--rw-r--r--   0 mac        (501) staff       (20)    17863 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.2/fbclient/client.py
--rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.2/fbclient/common_types.py
--rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.2/fbclient/config.py
--rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)    12389 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     9022 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.2/fbclient/event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/event_types.py
--rw-r--r--   0 mac        (501) staff       (20)     9517 2023-04-16 06:51:44.000000 fb-python-sdk-1.1.2/fbclient/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)     3688 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/status.py
--rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/status_types.py
--rw-r--r--   0 mac        (501) staff       (20)    10647 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.2/fbclient/streaming.py
--rw-r--r--   0 mac        (501) staff       (20)      629 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.2/fbclient/update_processor.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.942814 fb-python-sdk-1.1.2/fbclient/utils/
--rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/exponential_backoff_jitter_strategy.py
--rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/http_client.py
--rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/repeatable_task.py
--rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/rwlock.py
--rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/utils/variation_splitting_algorithm.py
--rw-r--r--   0 mac        (501) staff       (20)       18 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.2/fbclient/version.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.944519 fb-python-sdk-1.1.2/intergration_tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.2/intergration_tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      942 2023-05-15 05:29:46.000000 fb-python-sdk-1.1.2/intergration_tests/readme.py
--rw-r--r--   0 mac        (501) staff       (20)     1398 2023-05-15 14:42:32.000000 fb-python-sdk-1.1.2/intergration_tests/run_in_start_no_wait.py
--rw-------   0 mac        (501) staff       (20)     1437 2023-05-15 14:42:24.000000 fb-python-sdk-1.1.2/intergration_tests/run_in_start_wait.py
--rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-15 14:50:11.948310 fb-python-sdk-1.1.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1851 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.2/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.947298 fb-python-sdk-1.1.2/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.2/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/tests/test_data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/tests/test_data_update_status_provider.py
--rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/tests/test_evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/tests/test_event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)    10823 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.2/tests/test_fbclient.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.679507 fb-python-sdk-1.1.3/
+-rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.3/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)    10444 2023-06-21 12:11:13.678982 fb-python-sdk-1.1.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     9372 2023-05-15 14:37:00.000000 fb-python-sdk-1.1.3/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/dev-requirements.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.662927 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)    10444 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1210 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      218 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       34 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.670471 fb-python-sdk-1.1.3/fbclient/
+-rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/category.py
+-rw-r--r--   0 mac        (501) staff       (20)    17863 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.3/fbclient/client.py
+-rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.3/fbclient/common_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.3/fbclient/config.py
+-rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)    12389 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     9022 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.3/fbclient/event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/event_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     3176 2023-06-21 11:37:24.000000 fb-python-sdk-1.1.3/fbclient/flag_change_notification.py
+-rw-r--r--   0 mac        (501) staff       (20)    10087 2023-06-21 12:02:10.000000 fb-python-sdk-1.1.3/fbclient/interfaces.py
+-rw-r--r--   0 mac        (501) staff       (20)     1595 2023-06-21 10:36:01.000000 fb-python-sdk-1.1.3/fbclient/notice_broadcaster.py
+-rw-r--r--   0 mac        (501) staff       (20)     3688 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/status.py
+-rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/status_types.py
+-rw-r--r--   0 mac        (501) staff       (20)    10647 2023-06-21 12:02:22.000000 fb-python-sdk-1.1.3/fbclient/streaming.py
+-rw-r--r--   0 mac        (501) staff       (20)      629 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.3/fbclient/update_processor.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.673530 fb-python-sdk-1.1.3/fbclient/utils/
+-rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/exponential_backoff_jitter_strategy.py
+-rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/http_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/repeatable_task.py
+-rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/rwlock.py
+-rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/utils/variation_splitting_algorithm.py
+-rw-r--r--   0 mac        (501) staff       (20)       18 2023-06-21 12:09:03.000000 fb-python-sdk-1.1.3/fbclient/version.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.675238 fb-python-sdk-1.1.3/intergration_tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.3/intergration_tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      942 2023-05-15 05:29:46.000000 fb-python-sdk-1.1.3/intergration_tests/readme.py
+-rw-r--r--   0 mac        (501) staff       (20)     1398 2023-05-15 14:42:32.000000 fb-python-sdk-1.1.3/intergration_tests/run_in_start_no_wait.py
+-rw-------   0 mac        (501) staff       (20)     1437 2023-06-21 12:05:39.000000 fb-python-sdk-1.1.3/intergration_tests/run_in_start_wait.py
+-rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-21 12:11:13.679608 fb-python-sdk-1.1.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1851 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.678363 fb-python-sdk-1.1.3/tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.3/tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/tests/test_data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/tests/test_data_update_status_provider.py
+-rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/tests/test_evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/tests/test_event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)    10823 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.3/tests/test_fbclient.py
```

### Comparing `fb-python-sdk-1.1.2/LICENSE` & `fb-python-sdk-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/PKG-INFO` & `fb-python-sdk-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fb-python-sdk-1.1.2/README.md` & `fb-python-sdk-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fb_python_sdk.egg-info/PKG-INFO` & `fb-python-sdk-1.1.3/fb_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fb-python-sdk-1.1.2/fb_python_sdk.egg-info/SOURCES.txt` & `fb-python-sdk-1.1.3/fb_python_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 fbclient/client.py
 fbclient/common_types.py
 fbclient/config.py
 fbclient/data_storage.py
 fbclient/evaluator.py
 fbclient/event_processor.py
 fbclient/event_types.py
+fbclient/flag_change_notification.py
 fbclient/interfaces.py
+fbclient/notice_broadcaster.py
 fbclient/status.py
 fbclient/status_types.py
 fbclient/streaming.py
 fbclient/update_processor.py
 fbclient/version.py
 fbclient/utils/__init__.py
 fbclient/utils/exponential_backoff_jitter_strategy.py
```

### Comparing `fb-python-sdk-1.1.2/fbclient/__init__.py` & `fb-python-sdk-1.1.3/fbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/category.py` & `fb-python-sdk-1.1.3/fbclient/category.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/client.py` & `fb-python-sdk-1.1.3/fbclient/client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/common_types.py` & `fb-python-sdk-1.1.3/fbclient/common_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/config.py` & `fb-python-sdk-1.1.3/fbclient/config.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/data_storage.py` & `fb-python-sdk-1.1.3/fbclient/data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/evaluator.py` & `fb-python-sdk-1.1.3/fbclient/evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/event_processor.py` & `fb-python-sdk-1.1.3/fbclient/event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/event_types.py` & `fb-python-sdk-1.1.3/fbclient/event_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/interfaces.py` & `fb-python-sdk-1.1.3/fbclient/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -261,7 +261,38 @@
 
     @abstractmethod
     def stop(self):
         """
         Shuts down the connection to feature flag center
         """
         pass
+
+
+class Notice(ABC):
+    """
+    This is not an insight event to be sent to FeatBit Flag Center; it is a notification to the SDK.
+    """
+    @property
+    @abstractmethod
+    def notice_type(self) -> str:
+        """
+        Returns the type of this notice
+        """
+        pass
+
+
+class Notifier(ABC):
+
+    @abstractmethod
+    def handle(self, notice: Notice):
+        """
+        Handles the notice
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """
+        Returns the name of this notifier
+        """
+        pass
```

### Comparing `fb-python-sdk-1.1.2/fbclient/status.py` & `fb-python-sdk-1.1.3/fbclient/status.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/status_types.py` & `fb-python-sdk-1.1.3/fbclient/status_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/streaming.py` & `fb-python-sdk-1.1.3/fbclient/streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.is_reconn = is_reconn
         self.state = state
 
     def __call__(self):
         return self.is_self_close
 
 
-def _data_to_dict(data: dict) -> tuple[int, dict]:
+def _data_to_dict(data: dict) -> Tuple[int, dict]:
     version = 0
     all_data = {}
     flags = {}
     segments = {}
     all_data[FEATURE_FLAGS] = flags
     all_data[SEGMENTS] = segments
     for flag in data['featureFlags']:
```

### Comparing `fb-python-sdk-1.1.2/fbclient/update_processor.py` & `fb-python-sdk-1.1.3/fbclient/update_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/utils/__init__.py` & `fb-python-sdk-1.1.3/fbclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/utils/exponential_backoff_jitter_strategy.py` & `fb-python-sdk-1.1.3/fbclient/utils/exponential_backoff_jitter_strategy.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/utils/http_client.py` & `fb-python-sdk-1.1.3/fbclient/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/utils/repeatable_task.py` & `fb-python-sdk-1.1.3/fbclient/utils/repeatable_task.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/utils/rwlock.py` & `fb-python-sdk-1.1.3/fbclient/utils/rwlock.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/fbclient/utils/variation_splitting_algorithm.py` & `fb-python-sdk-1.1.3/fbclient/utils/variation_splitting_algorithm.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/intergration_tests/readme.py` & `fb-python-sdk-1.1.3/intergration_tests/readme.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/intergration_tests/run_in_start_no_wait.py` & `fb-python-sdk-1.1.3/intergration_tests/run_in_start_no_wait.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/intergration_tests/run_in_start_wait.py` & `fb-python-sdk-1.1.3/intergration_tests/run_in_start_wait.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fbclient.config import Config
 from fbclient.utils import log
 
 logging.basicConfig(level=logging.DEBUG,
                     format='%(asctime)s,%(msecs)d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
                     datefmt='%m-%d %H:%M')
 
-env_secret = 'fXWjg00OTEa-M_iBCyYiBwFPfdBisjAkiY3ycIMOWw1Q'
+env_secret = '9T0GABTXokagxhUZ81hUnws9_E2uOpIEyTjScBRr6JKA'
 
 config = Config(env_secret, event_url='http://localhost:5100', streaming_url='ws://localhost:5100')
 
 set_config(config)
 
 client = get()
```

### Comparing `fb-python-sdk-1.1.2/setup.py` & `fb-python-sdk-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/tests/test_data_storage.py` & `fb-python-sdk-1.1.3/tests/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/tests/test_data_update_status_provider.py` & `fb-python-sdk-1.1.3/tests/test_data_update_status_provider.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/tests/test_evaluator.py` & `fb-python-sdk-1.1.3/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/tests/test_event_processor.py` & `fb-python-sdk-1.1.3/tests/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.2/tests/test_fbclient.py` & `fb-python-sdk-1.1.3/tests/test_fbclient.py`

 * *Files identical despite different names*

