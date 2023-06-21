# Comparing `tmp/orthanc-server-extensions-3.3.0.tar.gz` & `tmp/orthanc-server-extensions-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthanc-server-extensions-3.3.0.tar", last modified: Mon Jan 30 14:39:19 2023, max compression
+gzip compressed data, was "orthanc-server-extensions-3.4.0.tar", last modified: Wed Jun 21 00:52:10 2023, max compression
```

## Comparing `orthanc-server-extensions-3.3.0.tar` & `orthanc-server-extensions-3.4.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3891 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)     4906 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/orthanc_ext/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/event_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/http_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     1905 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/logging_configurator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/orthanc.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/orthanc_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/python_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/anonymization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/auto_forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/auto_retries.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/kafka_event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/nats_event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/orthanc_ext/scripts/rabbitmq_event_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2023-01-30 14:39:19.000000 orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-01-30 14:39:19.000000 orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-30 14:39:19.000000 orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-30 14:39:19.000000 orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-01-30 14:39:19.000000 orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-30 14:39:19.000000 orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:39:19.709365 orthanc-server-extensions-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_anonymization.py
--rw-r--r--   0 runner    (1001) docker     (122)     2845 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_auto_forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     3922 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_auto_retries.py
--rw-r--r--   0 runner    (1001) docker     (122)     8157 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_event_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_logging_configurator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_notifications_kafka.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_notifications_nats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2515 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_notifications_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_orthanc_api_consistency.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-01-30 14:39:17.000000 orthanc-server-extensions-3.3.0/tests/test_orthanc_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 00:52:10.191870 orthanc-server-extensions-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3891 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5591 2023-06-21 00:52:10.191870 orthanc-server-extensions-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 00:52:10.187870 orthanc-server-extensions-3.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4906 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 00:52:10.187870 orthanc-server-extensions-3.4.0/orthanc_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/event_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/executor_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/http_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1905 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/logging_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/orthanc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/orthanc_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/python_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 00:52:10.191870 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/anonymization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/auto_forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/auto_retries.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/kafka_event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/nats_event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/orthanc_ext/scripts/rabbitmq_event_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 00:52:10.191870 orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5591 2023-06-21 00:52:10.000000 orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-06-21 00:52:10.000000 orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 00:52:10.000000 orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 00:52:10.000000 orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-21 00:52:10.000000 orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-21 00:52:10.000000 orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-21 00:52:10.191870 orthanc-server-extensions-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 00:52:10.191870 orthanc-server-extensions-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_anonymization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_auto_forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3922 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_auto_retries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8157 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_event_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_executor_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_logging_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_notifications_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_notifications_nats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2515 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_notifications_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_orthanc_api_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-06-21 00:52:08.000000 orthanc-server-extensions-3.4.0/tests/test_orthanc_api_handler.py
```

### Comparing `orthanc-server-extensions-3.3.0/CONTRIBUTING.rst` & `orthanc-server-extensions-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/HISTORY.rst` & `orthanc-server-extensions-3.4.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/LICENSE` & `orthanc-server-extensions-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/PKG-INFO` & `orthanc-server-extensions-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc-server-extensions
-Version: 3.3.0
+Version: 3.4.0
 Summary: An Orthanc python plugin based framework to extend Orthanc's feature set with testable Python scripts 
 Home-page: https://github.com/walkIT-nl/orthanc-server-extensions
 Author: WalkIT
 Author-email: code@walkit.nl
 License: GNU Affero General Public License v3
 Keywords: orthanc testing
 Platform: UNKNOWN
```

### Comparing `orthanc-server-extensions-3.3.0/README.rst` & `orthanc-server-extensions-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/docs/Makefile` & `orthanc-server-extensions-3.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/docs/conf.py` & `orthanc-server-extensions-3.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/docs/installation.rst` & `orthanc-server-extensions-3.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/docs/make.bat` & `orthanc-server-extensions-3.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/docs/usage.rst` & `orthanc-server-extensions-3.4.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/event_dispatcher.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/event_dispatcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import asyncio
 import inspect
 import json
 import logging
 from dataclasses import dataclass
 
+from orthanc_ext.executor_utilities import SequentialHybridExecutor
 from orthanc_ext.http_utilities import create_internal_client, get_rest_api_base_url, \
     get_certificate, ClientType
 from orthanc_ext.logging_configurator import python_logging
 from orthanc_ext.python_utilities import ensure_iterable, create_reverse_type_dict
 
 
 def register_event_handlers(
         event_handlers,
         orthanc_module,
         sync_client,
         async_client=None,
-        logging_configuration=python_logging):
+        logging_configuration=python_logging,
+        handler_executor=SequentialHybridExecutor):
     logging_configuration(orthanc_module)
 
     @dataclass
     class ChangeEvent:
         change_type: int
         resource_type: int
         resource_id: str
@@ -35,50 +36,39 @@
         return create_reverse_type_dict(orthanc_type)
 
     event_types = create_type_index(orthanc_module.ChangeType)
     resource_types = create_type_index(orthanc_module.ResourceType)
 
     event_handlers = {k: ensure_iterable(v) for k, v in event_handlers.items()}
 
+    executor = handler_executor(sync_client, async_client)
+
     def unhandled_event_logger(event, _):
         logging.debug(f'no handler registered for {event_types[event.change_type]}')
 
-    async def on_change_async(async_handlers):
-        return_values = await asyncio.gather(*async_handlers, return_exceptions=True)
-
-        for index, return_value in enumerate(return_values):
-            if isinstance(return_value, BaseException):
-                logging.exception(
-                    'execution of %s failed; %s', async_handlers[index], repr(return_value))
-
-        return return_values
-
-    def get_validated_async_client(async_client):
-        if async_client is None:
-            raise ValueError('a configured async_client is required when using async handlers')
-        return async_client
-
     def OnChange(change_type, resource_type, resource_id):
         event = ChangeEvent(change_type, resource_type, resource_id)
         handlers = event_handlers.get(change_type, [unhandled_event_logger])
 
-        return_values = [
-            handler(event, sync_client)
-            for handler in handlers
-            if not inspect.iscoroutinefunction(handler)
-        ]
-        async_handlers = [
-            handler(event, get_validated_async_client(async_client))
-            for handler in handlers
-            if inspect.iscoroutinefunction(handler)
-        ]
+        sync_handlers = get_sync_handlers(handlers)
+        async_handlers = get_async_handlers(handlers)
 
-        return return_values + asyncio.run(on_change_async(async_handlers))
+        return executor.invoke_all(event, sync_handlers, async_handlers)
 
     orthanc_module.RegisterOnChangeCallback(OnChange)
 
+    return executor
+
+
+def get_async_handlers(handlers):
+    return [handler for handler in handlers if inspect.iscoroutinefunction(handler)]
+
+
+def get_sync_handlers(handlers):
+    return [handler for handler in handlers if not inspect.iscoroutinefunction(handler)]
+
 
 def create_session(orthanc, client_type=ClientType.SYNC):
     config = json.loads(orthanc.GetConfiguration())
     return create_internal_client(
         get_rest_api_base_url(config), orthanc.GenerateRestApiAuthorizationToken(),
         get_certificate(config), client_type)
```

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/http_utilities.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/http_utilities.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/logging_configurator.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/logging_configurator.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/orthanc.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/orthanc.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/orthanc_utilities.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/orthanc_utilities.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/python_utilities.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/python_utilities.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/scripts/anonymization.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/scripts/anonymization.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/scripts/auto_forward.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/scripts/auto_forward.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/scripts/auto_retries.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/scripts/auto_retries.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/scripts/event_publisher.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/scripts/event_publisher.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/scripts/kafka_event_publisher.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/scripts/kafka_event_publisher.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/scripts/nats_event_publisher.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/scripts/nats_event_publisher.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_ext/scripts/rabbitmq_event_publisher.py` & `orthanc-server-extensions-3.4.0/orthanc_ext/scripts/rabbitmq_event_publisher.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/PKG-INFO` & `orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc-server-extensions
-Version: 3.3.0
+Version: 3.4.0
 Summary: An Orthanc python plugin based framework to extend Orthanc's feature set with testable Python scripts 
 Home-page: https://github.com/walkIT-nl/orthanc-server-extensions
 Author: WalkIT
 Author-email: code@walkit.nl
 License: GNU Affero General Public License v3
 Keywords: orthanc testing
 Platform: UNKNOWN
```

### Comparing `orthanc-server-extensions-3.3.0/orthanc_server_extensions.egg-info/SOURCES.txt` & `orthanc-server-extensions-3.4.0/orthanc_server_extensions.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 orthanc_ext/__init__.py
 orthanc_ext/event_dispatcher.py
+orthanc_ext/executor_utilities.py
 orthanc_ext/http_utilities.py
 orthanc_ext/logging_configurator.py
 orthanc_ext/orthanc.py
 orthanc_ext/orthanc_utilities.py
 orthanc_ext/python_utilities.py
 orthanc_ext/scripts/__init__.py
 orthanc_ext/scripts/anonymization.py
@@ -38,13 +39,14 @@
 tests/__init__.py
 tests/entry_point.py
 tests/test_anonymization.py
 tests/test_auto_forward.py
 tests/test_auto_retries.py
 tests/test_event_dispatcher.py
 tests/test_event_publisher.py
+tests/test_executor_utilities.py
 tests/test_logging_configurator.py
 tests/test_notifications_kafka.py
 tests/test_notifications_nats.py
 tests/test_notifications_rabbitmq.py
 tests/test_orthanc_api_consistency.py
 tests/test_orthanc_api_handler.py
```

### Comparing `orthanc-server-extensions-3.3.0/setup.cfg` & `orthanc-server-extensions-3.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.3.0
+current_version = 3.4.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `orthanc-server-extensions-3.3.0/setup.py` & `orthanc-server-extensions-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,10 +47,10 @@
         'nats-event-publisher': ['cloudevents', 'nats-py'],
         'kafka-event-publisher': ['cloudevents', 'aiokafka'],
         'rabbitmq-event-publisher': ['cloudevents', 'aio-pika']
     },
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/walkIT-nl/orthanc-server-extensions',
-    version='3.3.0',
+    version='3.4.0',
     zip_safe=False,
 )
```

### Comparing `orthanc-server-extensions-3.3.0/tests/entry_point.py` & `orthanc-server-extensions-3.4.0/tests/entry_point.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_anonymization.py` & `orthanc-server-extensions-3.4.0/tests/test_anonymization.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,18 @@
             'ID': 1,
             'Path': '/series/1.2.4',
             'PatientID': '123',
             'Type': 'boe'
         })
     anonymize_series(client, '1.2.3')
     assert store.called
-    assert caplog.messages == ['Anonymized "/series/1.2.3" to "/series/1.2.4"']
+    assert caplog.messages == [
+        'HTTP Request: POST https://localhost:8042/series/1.2.3/anonymize "HTTP/1.1 200 OK"',
+        'Anonymized "/series/1.2.3" to "/series/1.2.4"'
+    ]
 
 
 @respx.mock
 def test_reidentify_series_shall_leverage_orthanc_merge_to_replace_patient_study_module_tags(
         caplog):
     caplog.set_level(logging.INFO)
```

### Comparing `orthanc-server-extensions-3.3.0/tests/test_auto_forward.py` & `orthanc-server-extensions-3.4.0/tests/test_auto_forward.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 
 
 @respx.mock
 def test_autoforward_on_match_shall_start_start_modality_store(caplog):
     store = respx.post('/modalities/pacs/store').respond(200, text='study-uuid')
     register_and_trigger_handler([DicomReceivedMatcher(lambda uid, _: True, lambda uid, _: 'pacs')])
     assert store.called
-    assert caplog.messages == ['DICOM export to modality "pacs" started for resource "study-uuid"']
+    assert caplog.messages == [
+        'HTTP Request: POST https://localhost:8042/modalities/pacs/store "HTTP/1.1 200 OK"',
+        'DICOM export to modality "pacs" started for resource "study-uuid"'
+    ]
 
 
 @respx.mock
 def test_autoforward_on_multiple_matches_shall_start_start_modality_store(caplog):
     instances = respx.get('/series/study-uuid/instances').respond(
         200, json=[{
             'ID': 'b99cd218-ae67f0d7-70324b6b-2b095801-f858dedf'
@@ -50,17 +53,24 @@
     matcher1 = DicomReceivedMatcher(is_not_dicom_origin, lambda uid, _: 'pacs1')
     matcher2 = DicomReceivedMatcher(lambda uid, _: True, lambda uid, _: 'pacs2')
     register_and_trigger_handler([matcher1, matcher2])
     assert instances.called
     assert origin.called
     assert pacs1.called
     assert pacs2.called
+
+    url = 'https://localhost:8042'
     assert caplog.messages == [
+        f'HTTP Request: GET {url}/series/study-uuid/instances "HTTP/1.1 200 OK"',
+        'HTTP Request: GET '
+        f'{url}/instances/b99cd218-ae67f0d7-70324b6b-2b095801-f858dedf/metadata/Origin '
+        '"HTTP/1.1 200 OK"', f'HTTP Request: POST {url}/modalities/pacs1/store "HTTP/1.1 200 OK"',
         'DICOM export to modality "pacs1" started for resource "study-uuid"',
-        'DICOM export to modality "pacs2" started for resource "study-uuid"'
+        f'HTTP Request: POST {url}/modalities/pacs2/store "HTTP/1.1 '
+        '200 OK"', 'DICOM export to modality "pacs2" started for resource "study-uuid"'
     ]
 
 
 def test_autoforward_on_no_match_shall_log_and_continue(caplog):
     register_and_trigger_handler([
         DicomReceivedMatcher(lambda uid, _: False, lambda uid, _: 'pacs')
     ])
```

### Comparing `orthanc-server-extensions-3.3.0/tests/test_auto_retries.py` & `orthanc-server-extensions-3.4.0/tests/test_auto_retries.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_event_dispatcher.py` & `orthanc-server-extensions-3.4.0/tests/test_event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_event_publisher.py` & `orthanc-server-extensions-3.4.0/tests/test_event_publisher.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_logging_configurator.py` & `orthanc-server-extensions-3.4.0/tests/test_logging_configurator.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_notifications_kafka.py` & `orthanc-server-extensions-3.4.0/tests/test_notifications_kafka.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_notifications_nats.py` & `orthanc-server-extensions-3.4.0/tests/test_notifications_nats.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_notifications_rabbitmq.py` & `orthanc-server-extensions-3.4.0/tests/test_notifications_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `orthanc-server-extensions-3.3.0/tests/test_orthanc_api_consistency.py` & `orthanc-server-extensions-3.4.0/tests/test_orthanc_api_consistency.py`

 * *Files identical despite different names*

