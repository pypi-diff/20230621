# Comparing `tmp/eodc-2023.6.2.tar.gz` & `tmp/eodc-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.2.tar", max compression
+gzip compressed data, was "eodc-2023.6.3.tar", max compression
```

## Comparing `eodc-2023.6.2.tar` & `eodc-2023.6.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-20 08:50:46.924532 eodc-2023.6.2/README.md
--rw-r--r--   0        0        0      213 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/dask.py
--rw-r--r--   0        0        0     7909 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/settings.py
--rw-r--r--   0        0        0     1161 2023-06-20 08:50:46.924532 eodc-2023.6.2/pyproject.toml
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 eodc-2023.6.2/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-21 11:35:59.644849 eodc-2023.6.3/README.md
+-rw-r--r--   0        0        0      213 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/dask.py
+-rw-r--r--   0        0        0     8965 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-21 11:35:59.644849 eodc-2023.6.3/eodc/settings.py
+-rw-r--r--   0        0        0     1208 2023-06-21 11:35:59.644849 eodc-2023.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 eodc-2023.6.3/PKG-INFO
```

### Comparing `eodc-2023.6.2/README.md` & `eodc-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.2/eodc/dask.py` & `eodc-2023.6.3/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.2/eodc/faas.py` & `eodc-2023.6.3/eodc/faas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from time import sleep
 
 import argo_workflows
 from argo_workflows.api import workflow_service_api
@@ -32,14 +33,15 @@
 from openeo_executor_bindings.model import OpenEOExecutorParameters
 from pystac import Collection, Item
 from sen2like_processor_bindings.model import BoundingBox as Sen2LikeBoundingBox  # noqa
 from sen2like_processor_bindings.model import (  # noqa
     Sen2LikeParameters,
     sen2like_options,
 )
+from snap_processor_bindings.model import SnapParameters
 
 from eodc import settings
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -48,14 +50,18 @@
     workflow_template_name: str
 
 
 class FaasProcessor(Enum):
     Force = FaasProcessorDetails("force", "faas-force")
     Sen2Like = FaasProcessorDetails("sen2like", "faas-sen2like")
     OpenEO = FaasProcessorDetails("openeo", "faas-openeo-executor")
+    Snap = FaasProcessorDetails("snap", "faas-snap")
+
+
+LABEL_VALIDATION_REGEX = r"(([A-Za-z0-9][-A-Za-z0-9_.]*)?[A-Za-z0-9])?"
 
 
 class FaasProcessorBase(ABC):
     @classmethod
     def get_instance(cls, processor_details):
         return cls(processor_details=processor_details)
 
@@ -67,14 +73,25 @@
         self.api_instance_workflows = workflow_service_api.WorkflowServiceApi(
             self.api_client
         )
         self.processor_details = processor_details
         # TODO: Check here that this workflow template even exists on the server
 
     def submit_workflow(self, **kwargs):
+        if (
+            "user_id" in kwargs
+            and re.match(LABEL_VALIDATION_REGEX, kwargs["user_id"]) is None
+        ):
+            raise ValueError("invalid user_id")
+        if (
+            "job_id" in kwargs
+            and re.match(LABEL_VALIDATION_REGEX, kwargs["job_id"]) is None
+        ):
+            raise ValueError("invalid user_id")
+
         parameters = [
             IoArgoprojWorkflowV1alpha1Parameter(name=k, value=v)
             for k, v in kwargs.items()
         ]
 
         manifest = IoArgoprojWorkflowV1alpha1Workflow(
             metadata=ObjectMeta(
@@ -216,7 +233,28 @@
             openeo_executor_parameters=openeo_parameters.json(),
             openeo_user_id=openeo_user_id,
             openeo_job_id=openeo_job_id,
         )
 
     def get_output_stac_items(self):
         raise NotImplementedError()
+
+
+class Snap(FaasProcessorBase):
+    @classmethod
+    def get_instance(cls):
+        return cls(processor_details=FaasProcessor.Snap.value)
+
+    def submit_workflow(
+        self,
+        snap_parameters: SnapParameters,
+        user_id: str,
+        job_id: str,
+    ):
+        return super().submit_workflow(
+            snap_parameters=snap_parameters.json(),
+            user_id=user_id,
+            job_id=job_id,
+        )
+
+    def get_output_stac_items(self):
+        raise NotImplementedError()
```

### Comparing `eodc-2023.6.2/pyproject.toml` & `eodc-2023.6.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.2"
+version = "2023.6.3"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -25,14 +25,16 @@
 pydantic = "^1.10.7"
 argo-workflows = "6.3.9"
 dask-gateway = "^2022.11.0"
 eodc-faas-force = "2023.6.2"
 eodc-faas-sen2like = "2023.6.2"
 eodc-faas-openeo = "^2023.6.5rc1"
 pystac = "^1.7.3"
+eodc-faas-snap = "^2023.6.2"
+pyproj = "^3.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
```

### Comparing `eodc-2023.6.2/PKG-INFO` & `eodc-2023.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
@@ -17,15 +17,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: argo-workflows (==6.3.9)
 Requires-Dist: dask-gateway (>=2022.11.0,<2023.0.0)
 Requires-Dist: eodc-faas-force (==2023.6.2)
 Requires-Dist: eodc-faas-openeo (>=2023.6.5rc1,<2024.0.0)
 Requires-Dist: eodc-faas-sen2like (==2023.6.2)
+Requires-Dist: eodc-faas-snap (>=2023.6.2,<2024.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyproj (>=3.6.0,<4.0.0)
 Requires-Dist: pystac (>=1.7.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eodcgmbh/eodc-sdk
 Description-Content-Type: text/markdown
 
 # EODC SDK
 ![PyPI - Status](https://img.shields.io/pypi/status/eodc)
```

