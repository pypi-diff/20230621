# Comparing `tmp/target_s3_delta-0.0.5.tar.gz` & `tmp/target_s3_delta-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_s3_delta-0.0.5.tar", max compression
+gzip compressed data, was "target_s3_delta-0.0.6.tar", max compression
```

## Comparing `target_s3_delta-0.0.5.tar` & `target_s3_delta-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.5/README.md
--rw-r--r--   0        0        0     1050 2023-06-21 12:48:48.754929 target_s3_delta-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.5/target_s3_delta/__init__.py
--rw-r--r--   0        0        0     3837 2023-06-21 09:02:13.335808 target_s3_delta-0.0.5/target_s3_delta/sinks.py
--rw-r--r--   0        0        0     4056 2023-06-21 11:07:58.467362 target_s3_delta-0.0.5/target_s3_delta/target.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.6/README.md
+-rw-r--r--   0        0        0     1050 2023-06-21 14:04:18.164708 target_s3_delta-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.6/target_s3_delta/__init__.py
+-rw-r--r--   0        0        0     3837 2023-06-21 09:02:13.335808 target_s3_delta-0.0.6/target_s3_delta/sinks.py
+-rw-r--r--   0        0        0     4050 2023-06-21 14:03:49.110942 target_s3_delta-0.0.6/target_s3_delta/target.py
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.6/PKG-INFO
```

### Comparing `target_s3_delta-0.0.5/pyproject.toml` & `target_s3_delta-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-s3-delta"
-version = "0.0.5"
+version = "0.0.6"
 description = "`target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["resul yurttakalan"]
 keywords = [
     "ELT",
     "s3-delta",
 ]
```

### Comparing `target_s3_delta-0.0.5/target_s3_delta/sinks.py` & `target_s3_delta-0.0.6/target_s3_delta/sinks.py`

 * *Files identical despite different names*

### Comparing `target_s3_delta-0.0.5/target_s3_delta/target.py` & `target_s3_delta-0.0.6/target_s3_delta/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,21 +94,21 @@
             return
 
         write_deltalake(
             path,
             data,
             schema=first_batch.schema,
             storage_options=storage_options,
-            mode=self.config.get("mode"),
+            mode=mode,
             overwrite_schema=True,
             partition_by=partition_by,
             max_rows_per_file=self.config.get("max_rows_per_file"),
         )
 
-        self.logger.info(f"Transaction has created.")
+        self.logger.info(f"Transaction has created. Mode: {mode}")
 
     def _process_endofpipe(self):
         state = copy.deepcopy(self._latest_state)
         self._drain_all(self._sinks_to_clear, 1)
 
         for sink in self._sinks_to_clear:
             sink.clean_up()
```

### Comparing `target_s3_delta-0.0.5/PKG-INFO` & `target_s3_delta-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-s3-delta
-Version: 0.0.5
+Version: 0.0.6
 Summary: `target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,s3-delta
 Author: resul yurttakalan
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

