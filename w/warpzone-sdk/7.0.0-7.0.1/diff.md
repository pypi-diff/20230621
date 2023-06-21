# Comparing `tmp/warpzone_sdk-7.0.0.tar.gz` & `tmp/warpzone_sdk-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-7.0.0.tar", max compression
+gzip compressed data, was "warpzone_sdk-7.0.1.tar", max compression
```

## Comparing `warpzone_sdk-7.0.0.tar` & `warpzone_sdk-7.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1121 2023-05-25 13:24:56.626896 warpzone_sdk-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     1182 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3035 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/monitor.py
--rw-r--r--   0        0        0     1486 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/process.py
--rw-r--r--   0        0        0       32 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0     1910 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/signature.py
--rw-r--r--   0        0        0       80 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5636 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       47 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/__init__.py
--rw-r--r--   0        0        0     2882 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/client.py
--rw-r--r--   0        0        0     2509 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/client_async.py
--rw-r--r--   0        0        0      521 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/helpers.py
--rw-r--r--   0        0        0     2470 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/operations.py
--rw-r--r--   0        0        0      219 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3661 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/transform/data.py
--rw-r--r--   0        0        0     1833 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1182 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2844 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3035 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     1486 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/process.py
+-rw-r--r--   0        0        0       32 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0     1910 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/signature.py
+-rw-r--r--   0        0        0       80 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       47 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/__init__.py
+-rw-r--r--   0        0        0     2882 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/client.py
+-rw-r--r--   0        0        0     2509 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/client_async.py
+-rw-r--r--   0        0        0      521 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/helpers.py
+-rw-r--r--   0        0        0     2470 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/operations.py
+-rw-r--r--   0        0        0      219 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2939 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1833 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-7.0.1/PKG-INFO
```

### Comparing `warpzone_sdk-7.0.0/pyproject.toml` & `warpzone_sdk-7.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "7.0.0"
+version = "7.0.1"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Anders Launer Baek-Petersen <alp@energinet.dk>", "Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-7.0.0/warpzone/__init__.py` & `warpzone_sdk-7.0.1/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/blobstorage/client.py` & `warpzone_sdk-7.0.1/warpzone/blobstorage/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Module w.r.t. Azure blob storage logic."""
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import Optional
 
 import pandas as pd
 from azure.core.exceptions import (
     HttpResponseError,
     ServiceRequestError,
     ServiceResponseError,
@@ -24,15 +24,15 @@
         self.metadata = self.metadata if self.metadata else {}
 
     @classmethod
     def from_pandas(
         cls,
         df: pd.DataFrame,
         name: str,
-        metadata: dict = field(default_factory=dict),
+        metadata: dict = None,
         schema: dict = None,
     ):
         content = data.pandas_to_parquet(df, schema=schema)
         return cls(content, name, metadata=metadata)
 
     def to_pandas(self) -> pd.DataFrame:
         return data.parquet_to_pandas(self.content)
```

### Comparing `warpzone_sdk-7.0.0/warpzone/function/functionize.py` & `warpzone_sdk-7.0.1/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/function/integrations.py` & `warpzone_sdk-7.0.1/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/function/monitor.py` & `warpzone_sdk-7.0.1/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/function/process.py` & `warpzone_sdk-7.0.1/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/function/processors/outputs.py` & `warpzone_sdk-7.0.1/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/function/processors/triggers.py` & `warpzone_sdk-7.0.1/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/function/signature.py` & `warpzone_sdk-7.0.1/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/healthchecks/__init__.py` & `warpzone_sdk-7.0.1/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/healthchecks/model.py` & `warpzone_sdk-7.0.1/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/monitor/logs.py` & `warpzone_sdk-7.0.1/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/monitor/traces.py` & `warpzone_sdk-7.0.1/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/servicebus/data/client.py` & `warpzone_sdk-7.0.1/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/servicebus/events/client.py` & `warpzone_sdk-7.0.1/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/tablestorage/client.py` & `warpzone_sdk-7.0.1/warpzone/tablestorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/tablestorage/client_async.py` & `warpzone_sdk-7.0.1/warpzone/tablestorage/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/tablestorage/helpers.py` & `warpzone_sdk-7.0.1/warpzone/tablestorage/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/tablestorage/operations.py` & `warpzone_sdk-7.0.1/warpzone/tablestorage/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/testing/assertions.py` & `warpzone_sdk-7.0.1/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/testing/data.py` & `warpzone_sdk-7.0.1/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/transform/data.py` & `warpzone_sdk-7.0.1/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/warpzone/transform/schema.py` & `warpzone_sdk-7.0.1/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.0/PKG-INFO` & `warpzone_sdk-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 7.0.0
+Version: 7.0.1
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Anders Launer Baek-Petersen
 Author-email: alp@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

