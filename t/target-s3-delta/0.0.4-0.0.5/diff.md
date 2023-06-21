# Comparing `tmp/target_s3_delta-0.0.4.tar.gz` & `tmp/target_s3_delta-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_s3_delta-0.0.4.tar", max compression
+gzip compressed data, was "target_s3_delta-0.0.5.tar", max compression
```

## Comparing `target_s3_delta-0.0.4.tar` & `target_s3_delta-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.4/README.md
--rw-r--r--   0        0        0     1050 2023-06-20 13:13:15.254756 target_s3_delta-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.4/target_s3_delta/__init__.py
--rw-r--r--   0        0        0     3649 2023-06-20 13:11:02.183286 target_s3_delta-0.0.4/target_s3_delta/sinks.py
--rw-r--r--   0        0        0     2898 2023-06-20 13:12:25.444286 target_s3_delta-0.0.4/target_s3_delta/target.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.5/README.md
+-rw-r--r--   0        0        0     1050 2023-06-21 12:48:48.754929 target_s3_delta-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.5/target_s3_delta/__init__.py
+-rw-r--r--   0        0        0     3837 2023-06-21 09:02:13.335808 target_s3_delta-0.0.5/target_s3_delta/sinks.py
+-rw-r--r--   0        0        0     4056 2023-06-21 11:07:58.467362 target_s3_delta-0.0.5/target_s3_delta/target.py
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.5/PKG-INFO
```

### Comparing `target_s3_delta-0.0.4/pyproject.toml` & `target_s3_delta-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-s3-delta"
-version = "0.0.4"
+version = "0.0.5"
 description = "`target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["resul yurttakalan"]
 keywords = [
     "ELT",
     "s3-delta",
 ]
```

### Comparing `target_s3_delta-0.0.4/target_s3_delta/sinks.py` & `target_s3_delta-0.0.5/target_s3_delta/sinks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """s3-delta target sink class, which handles writing streams."""
 
 from __future__ import annotations
 
 import os
+import time
 
 from dateutil import parser
 from deltalake import write_deltalake
 from singer_sdk.helpers._typing import (
     DatetimeErrorTreatmentEnum,
     get_datelike_property_type,
     handle_invalid_timestamp_in_record,
@@ -104,11 +105,14 @@
         Args:
             context: Stream partition or context dictionary.
         """
         is_exist = os.path.exists(TEMP_DATA_DIRECTORY)
         if not is_exist:
             os.makedirs(TEMP_DATA_DIRECTORY)
 
+        start_time = time.time()
         df = pd.DataFrame(context["records"])
-        df.to_parquet(f"{TEMP_DATA_DIRECTORY}{context.get('file_path')}")
+        df.to_parquet(f"{TEMP_DATA_DIRECTORY}{context.get('file_path')}", engine="pyarrow")
+        end_time = time.time()
+        self.logger.info(f"Batch writing finished. Duration: {str((end_time - start_time))}")
 
         context["records"] = []
```

### Comparing `target_s3_delta-0.0.4/PKG-INFO` & `target_s3_delta-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-s3-delta
-Version: 0.0.4
+Version: 0.0.5
 Summary: `target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,s3-delta
 Author: resul yurttakalan
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

