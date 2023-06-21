# Comparing `tmp/eodc-2023.6.3.tar.gz` & `tmp/eodc-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.3.tar", max compression
+gzip compressed data, was "eodc-2023.6.4.tar", max compression
```

## Comparing `eodc-2023.6.3.tar` & `eodc-2023.6.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-21 11:35:59.644849 eodc-2023.6.3/README.md
--rw-r--r--   0        0        0      213 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/dask.py
--rw-r--r--   0        0        0     8965 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/settings.py
--rw-r--r--   0        0        0     1208 2023-06-21 11:35:59.644849 eodc-2023.6.3/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 eodc-2023.6.3/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-21 12:47:52.984963 eodc-2023.6.4/README.md
+-rw-r--r--   0        0        0      213 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/dask.py
+-rw-r--r--   0        0        0     9399 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/settings.py
+-rw-r--r--   0        0        0     1208 2023-06-21 12:47:52.984963 eodc-2023.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 eodc-2023.6.4/PKG-INFO
```

### Comparing `eodc-2023.6.3/README.md` & `eodc-2023.6.4/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.3/eodc/dask.py` & `eodc-2023.6.4/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.3/eodc/faas.py` & `eodc-2023.6.4/eodc/faas.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,19 @@
 from openeo_executor_bindings.model import OpenEOExecutorParameters
 from pystac import Collection, Item
 from sen2like_processor_bindings.model import BoundingBox as Sen2LikeBoundingBox  # noqa
 from sen2like_processor_bindings.model import (  # noqa
     Sen2LikeParameters,
     sen2like_options,
 )
-from snap_processor_bindings.model import SnapParameters
+from snap_processor_bindings.model import (  # noqa
+    SnapCorrectionCoefficient,
+    SnapCorrectionMethod,
+    SnapParameters,
+)
 
 from eodc import settings
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -160,15 +164,15 @@
             .read()
             .decode("utf-8")
             .splitlines()
         )
 
     @abstractmethod
     def get_output_stac_items(self):
-        pass
+        raise NotImplementedError()
 
 
 class Force(FaasProcessorBase):
     @classmethod
     def get_instance(cls):
         return cls(processor_details=FaasProcessor.Force.value)
 
@@ -252,9 +256,16 @@
     ):
         return super().submit_workflow(
             snap_parameters=snap_parameters.json(),
             user_id=user_id,
             job_id=job_id,
         )
 
-    def get_output_stac_items(self):
-        raise NotImplementedError()
+    def get_output_stac_items(self, snap_parameters: SnapParameters):
+        collection_file = list(snap_parameters.stac_path.glob("*_collection.json"))[0]
+        snap_output_collection = Collection.from_file(str(collection_file))
+        stac_items = [
+            Item.from_file(link.get_absolute_href())
+            for link in snap_output_collection.get_item_links()
+        ]
+
+        return stac_items
```

### Comparing `eodc-2023.6.3/pyproject.toml` & `eodc-2023.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.3"
+version = "2023.6.4"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2023.6.3/PKG-INFO` & `eodc-2023.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

