# Comparing `tmp/localstack-2.1.1.dev20230605083031.tar.gz` & `tmp/localstack-2.1.1.dev20230621080533.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-2.1.1.dev20230605083031.tar", last modified: Mon Jun  5 08:33:37 2023, max compression
+gzip compressed data, was "localstack-2.1.1.dev20230621080533.tar", last modified: Wed Jun 21 08:09:17 2023, max compression
```

## Comparing `localstack-2.1.1.dev20230605083031.tar` & `localstack-2.1.1.dev20230621080533.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/PKG-INFO
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/localstack.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/top_level.txt
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/localstack_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-06-05 08:33:36.000000 localstack-2.1.1.dev20230605083031/localstack_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-06-05 08:30:17.000000 localstack-2.1.1.dev20230605083031/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/PKG-INFO
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/localstack.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/top_level.txt
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/localstack_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-06-21 08:09:16.000000 localstack-2.1.1.dev20230621080533/localstack_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-06-21 08:05:16.000000 localstack-2.1.1.dev20230621080533/setup.py
```

### Comparing `localstack-2.1.1.dev20230605083031/PKG-INFO` & `localstack-2.1.1.dev20230621080533/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.1.1.dev20230605083031
+Version: 2.1.1.dev20230621080533
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230605083031
+Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230621080533
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
```

### Comparing `localstack-2.1.1.dev20230605083031/localstack.egg-info/PKG-INFO` & `localstack-2.1.1.dev20230621080533/localstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.1.1.dev20230605083031
+Version: 2.1.1.dev20230621080533
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230605083031
+Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230621080533
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
```

### Comparing `localstack-2.1.1.dev20230605083031/setup.py` & `localstack-2.1.1.dev20230621080533/setup.py`

 * *Files identical despite different names*

