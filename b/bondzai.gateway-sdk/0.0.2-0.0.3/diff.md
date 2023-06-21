# Comparing `tmp/bondzai.gateway-sdk-0.0.2.tar.gz` & `tmp/bondzai.gateway-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-sdk-0.0.2.tar", last modified: Tue Jun 20 15:59:53 2023, max compression
+gzip compressed data, was "bondzai.gateway-sdk-0.0.3.tar", last modified: Wed Jun 21 10:31:20 2023, max compression
```

## Comparing `bondzai.gateway-sdk-0.0.2.tar` & `bondzai.gateway-sdk-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 15:59:53.494250 bondzai.gateway-sdk-0.0.2/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-06-20 15:59:53.494310 bondzai.gateway-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      155 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 15:59:53.491273 bondzai.gateway-sdk-0.0.2/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 15:59:53.493051 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/
--rw-r--r--   0 theo       (501) staff       (20)      139 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     9552 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/agent.py
--rw-r--r--   0 theo       (501) staff       (20)     2494 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/commands.py
--rw-r--r--   0 theo       (501) staff       (20)      257 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/config.py
--rw-r--r--   0 theo       (501) staff       (20)     5589 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     3983 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/events.py
--rw-r--r--   0 theo       (501) staff       (20)     4384 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/gateway.py
--rw-r--r--   0 theo       (501) staff       (20)     3318 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/message.py
--rw-r--r--   0 theo       (501) staff       (20)      812 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/request.py
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/responses.py
--rw-r--r--   0 theo       (501) staff       (20)      570 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/timer.py
--rw-r--r--   0 theo       (501) staff       (20)      738 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 15:59:53.494036 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-06-20 15:59:53.000000 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      735 2023-06-20 15:59:53.000000 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-20 15:59:53.000000 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-20 15:59:53.000000 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       61 2023-06-20 15:59:53.000000 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-06-20 15:59:53.000000 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-20 15:59:53.000000 bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)    21241 2023-06-20 15:59:28.000000 bondzai.gateway-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-06-20 15:59:53.494566 bondzai.gateway-sdk-0.0.2/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:38.317738 bondzai.gateway-sdk-0.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/NOTICE
+-rwxrwxrwx   0 root         (0) root         (0)      604 2023-06-21 10:58:38.318739 bondzai.gateway-sdk-0.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      155 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:37.675229 bondzai.gateway-sdk-0.0.3/bondzai/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:38.103502 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/
+-rwxrwxrwx   0 root         (0) root         (0)      139 2023-06-21 10:58:27.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9552 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/agent.py
+-rwxrwxrwx   0 root         (0) root         (0)     2494 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/commands.py
+-rwxrwxrwx   0 root         (0) root         (0)      257 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     6243 2023-06-21 10:58:27.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)     3983 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/gateway.py
+-rwxrwxrwx   0 root         (0) root         (0)     3318 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/message.py
+-rwxrwxrwx   0 root         (0) root         (0)      812 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/request.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/responses.py
+-rwxrwxrwx   0 root         (0) root         (0)      570 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/timer.py
+-rwxrwxrwx   0 root         (0) root         (0)      738 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:38.293371 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      604 2023-06-21 10:58:37.000000 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      735 2023-06-21 10:58:37.000000 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:58:37.000000 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-21 10:58:37.000000 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)       61 2023-06-21 10:58:37.000000 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-21 10:58:37.000000 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:58:36.000000 bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)    21241 2023-06-21 10:56:58.000000 bondzai.gateway-sdk-0.0.3/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      775 2023-06-21 10:58:38.323005 bondzai.gateway-sdk-0.0.3/setup.cfg
```

### Comparing `bondzai.gateway-sdk-0.0.2/NOTICE` & `bondzai.gateway-sdk-0.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/PKG-INFO` & `bondzai.gateway-sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/agent.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/agent.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/commands.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/commands.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/enums.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -217,7 +217,32 @@
     OP_PARAM_MATRIX = 0x90001403
     OP_PARAM_EMPTY = 0x90008000
     OP_PARAM_MODE = 0x90008001
     OP_PARAM_REMOVENFIRST = 0x90008003
     OP_PARAM_SHAPE = 0x90008005
 
 
+class KPITypes(Enum):
+    KPI_FREE = 0
+    KPI_TRAINING_TIME_START = 1
+    KPI_TRAINING_TIME_STOP = 2
+    KPI_TRAINING_DATASET_SIZE = 3
+    KPI_TRAINING_NET_SIZE = 4
+    KPI_TRAINING_WM_SIZE = 5
+    KPI_INFER_TIME_START = 6
+    KPI_INFER_TIME_STOP = 7
+    KPI_INFER_WM_SIZE = 8
+    KPI_PREPROC_TIME_START = 9
+    KPI_PREPROC_TIME_STOP = 10
+    KPI_PREPROC_I_TIME_START = 11
+    KPI_PREPROC_I_TIME_STOP = 12
+    KPI_POSTPROC_TIME_START = 13
+    KPI_POSTPROC_TIME_STOP = 14
+    KPI_OTHER_TIME_START = 15
+    KPI_OTHER_TIME_STOP = 16
+    KPI_SIZE_BYTE = 17
+    KPI_SIZE_KBYTE = 18
+    KPI_QI = 19
+    KPI_OTHER_FLOAT = 20
+    KPI_TRAINING_NET_LAYERS = 21
+
+
```

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/events.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/gateway.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/gateway.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/message.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/message.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/request.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/timer.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/timer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai/gateway_sdk/utils.py` & `bondzai.gateway-sdk-0.0.3/bondzai/gateway_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/PKG-INFO` & `bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.2/bondzai.gateway_sdk.egg-info/SOURCES.txt` & `bondzai.gateway-sdk-0.0.3/bondzai.gateway_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/pyproject.toml` & `bondzai.gateway-sdk-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.2/setup.cfg` & `bondzai.gateway-sdk-0.0.3/setup.cfg`

 * *Files identical despite different names*

