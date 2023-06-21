# Comparing `tmp/fiware_pyspark_connector-0.0.6.tar.gz` & `tmp/fiware_pyspark_connector-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiware_pyspark_connector-0.0.6.tar", last modified: Wed Jun 21 09:28:40 2023, max compression
+gzip compressed data, was "fiware_pyspark_connector-0.0.7.tar", last modified: Wed Jun 21 09:31:09 2023, max compression
```

## Comparing `fiware_pyspark_connector-0.0.6.tar` & `fiware_pyspark_connector-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 09:28:40.118082 fiware_pyspark_connector-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-21 09:28:40.115083 fiware_pyspark_connector-0.0.6/FPC/
--rw-rw-rw-   0        0        0        0 2023-06-21 07:44:47.000000 fiware_pyspark_connector-0.0.6/FPC/__init__.py
--rw-rw-rw-   0        0        0    15652 2023-06-21 09:17:50.000000 fiware_pyspark_connector-0.0.6/FPC/connector.py
--rw-rw-rw-   0        0        0     2858 2023-06-21 07:33:02.000000 fiware_pyspark_connector-0.0.6/FPC/connectorconf.py
--rw-rw-rw-   0        0        0     7745 2023-06-21 07:33:02.000000 fiware_pyspark_connector-0.0.6/FPC/subscribing_tool.py
--rw-rw-rw-   0        0        0    34500 2023-06-21 07:33:56.000000 fiware_pyspark_connector-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     6777 2023-06-21 09:28:40.118082 fiware_pyspark_connector-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6207 2023-06-21 07:33:53.000000 fiware_pyspark_connector-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 09:28:40.117083 fiware_pyspark_connector-0.0.6/fiware_pyspark_connector.egg-info/
--rw-rw-rw-   0        0        0     6777 2023-06-21 09:28:40.000000 fiware_pyspark_connector-0.0.6/fiware_pyspark_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-06-21 09:28:40.000000 fiware_pyspark_connector-0.0.6/fiware_pyspark_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 09:28:40.000000 fiware_pyspark_connector-0.0.6/fiware_pyspark_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-21 09:28:40.000000 fiware_pyspark_connector-0.0.6/fiware_pyspark_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-21 09:28:40.000000 fiware_pyspark_connector-0.0.6/fiware_pyspark_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-06-21 07:54:36.000000 fiware_pyspark_connector-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      709 2023-06-21 09:28:40.118082 fiware_pyspark_connector-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 09:31:09.322382 fiware_pyspark_connector-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-21 09:31:09.319247 fiware_pyspark_connector-0.0.7/FPC/
+-rw-rw-rw-   0        0        0        0 2023-06-21 07:44:47.000000 fiware_pyspark_connector-0.0.7/FPC/__init__.py
+-rw-rw-rw-   0        0        0    15652 2023-06-21 09:17:50.000000 fiware_pyspark_connector-0.0.7/FPC/connector.py
+-rw-rw-rw-   0        0        0     2858 2023-06-21 07:33:02.000000 fiware_pyspark_connector-0.0.7/FPC/connectorconf.py
+-rw-rw-rw-   0        0        0     7745 2023-06-21 07:33:02.000000 fiware_pyspark_connector-0.0.7/FPC/subscribing_tool.py
+-rw-rw-rw-   0        0        0    34500 2023-06-21 07:33:56.000000 fiware_pyspark_connector-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     6777 2023-06-21 09:31:09.322382 fiware_pyspark_connector-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6207 2023-06-21 07:33:53.000000 fiware_pyspark_connector-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 09:31:09.321380 fiware_pyspark_connector-0.0.7/fiware_pyspark_connector.egg-info/
+-rw-rw-rw-   0        0        0     6777 2023-06-21 09:31:09.000000 fiware_pyspark_connector-0.0.7/fiware_pyspark_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-06-21 09:31:09.000000 fiware_pyspark_connector-0.0.7/fiware_pyspark_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 09:31:09.000000 fiware_pyspark_connector-0.0.7/fiware_pyspark_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-21 09:31:09.000000 fiware_pyspark_connector-0.0.7/fiware_pyspark_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-21 09:31:09.000000 fiware_pyspark_connector-0.0.7/fiware_pyspark_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-06-21 07:54:36.000000 fiware_pyspark_connector-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      709 2023-06-21 09:31:09.323385 fiware_pyspark_connector-0.0.7/setup.cfg
```

### Comparing `fiware_pyspark_connector-0.0.6/FPC/connector.py` & `fiware_pyspark_connector-0.0.7/FPC/connector.py`

 * *Files identical despite different names*

### Comparing `fiware_pyspark_connector-0.0.6/FPC/connectorconf.py` & `fiware_pyspark_connector-0.0.7/FPC/connectorconf.py`

 * *Files identical despite different names*

### Comparing `fiware_pyspark_connector-0.0.6/FPC/subscribing_tool.py` & `fiware_pyspark_connector-0.0.7/FPC/subscribing_tool.py`

 * *Files identical despite different names*

### Comparing `fiware_pyspark_connector-0.0.6/LICENSE.txt` & `fiware_pyspark_connector-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiware_pyspark_connector-0.0.6/PKG-INFO` & `fiware_pyspark_connector-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiware_pyspark_connector
-Version: 0.0.6
+Version: 0.0.7
 Summary: Connects FIWARE Context Brokers with fiware_pyspark_connector
 Home-page: https://github.com/Engineering-Research-and-Development/fiware-orion-pyspark-connector
 Author: Emilio Cimino
 Author-email: emilio.cimino@outlook.it
 License: "AGPL-3.0-only"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fiware_pyspark_connector-0.0.6/README.md` & `fiware_pyspark_connector-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fiware_pyspark_connector-0.0.6/fiware_pyspark_connector.egg-info/PKG-INFO` & `fiware_pyspark_connector-0.0.7/fiware_pyspark_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiware-pyspark-connector
-Version: 0.0.6
+Version: 0.0.7
 Summary: Connects FIWARE Context Brokers with fiware_pyspark_connector
 Home-page: https://github.com/Engineering-Research-and-Development/fiware-orion-pyspark-connector
 Author: Emilio Cimino
 Author-email: emilio.cimino@outlook.it
 License: "AGPL-3.0-only"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fiware_pyspark_connector-0.0.6/setup.cfg` & `fiware_pyspark_connector-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 6977 6172 655f 7079 7370 6172   = fiware_pyspar
 00000020: 6b5f 636f 6e6e 6563 746f 720d 0a76 6572  k_connector..ver
-00000030: 7369 6f6e 203d 2030 2e30 2e36 0d0a 6175  sion = 0.0.6..au
+00000030: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6175  sion = 0.0.7..au
 00000040: 7468 6f72 203d 2045 6d69 6c69 6f20 4369  thor = Emilio Ci
 00000050: 6d69 6e6f 0d0a 6175 7468 6f72 5f65 6d61  mino..author_ema
 00000060: 696c 203d 2065 6d69 6c69 6f2e 6369 6d69  il = emilio.cimi
 00000070: 6e6f 406f 7574 6c6f 6f6b 2e69 740d 0a64  no@outlook.it..d
 00000080: 6573 6372 6970 7469 6f6e 203d 2043 6f6e  escription = Con
 00000090: 6e65 6374 7320 4649 5741 5245 2043 6f6e  nects FIWARE Con
 000000a0: 7465 7874 2042 726f 6b65 7273 2077 6974  text Brokers wit
```

