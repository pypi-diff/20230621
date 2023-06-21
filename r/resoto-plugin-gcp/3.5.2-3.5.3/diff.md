# Comparing `tmp/resoto-plugin-gcp-3.5.2.tar.gz` & `tmp/resoto-plugin-gcp-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.5.2.tar", last modified: Tue Jun 13 13:07:52 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.5.3.tar", last modified: Wed Jun 21 14:23:20 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.5.2.tar` & `resoto-plugin-gcp-3.5.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:52.257533 resoto-plugin-gcp-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 13:07:52.257533 resoto-plugin-gcp-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:52.253533 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/gcp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:52.257533 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   284330 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:52.253533 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 13:07:52.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-13 13:07:52.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:52.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 13:07:52.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:18.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 13:07:52.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 13:07:52.000000 resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 13:07:52.257533 resoto-plugin-gcp-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:52.257533 resoto-plugin-gcp-3.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 13:03:10.000000 resoto-plugin-gcp-3.5.2/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.537868 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/gcp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.537868 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24264 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   284330 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.537868 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:27.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.5.2/PKG-INFO` & `resoto-plugin-gcp-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.5.2
+Version: 3.5.3
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.5.2/pyproject.toml` & `resoto-plugin-gcp-3.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-gcp"
 description = "Resoto GCP Collector Plugin"
-version = "3.5.2"
+version = "3.5.3"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.2",
+    "resotolib==3.5.3",
     "google-api-python-client",
     "oauth2client",
     "retrying",
     "tenacity",
 ]
 
 [project.entry-points."resoto.plugins"]
```

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,19 @@
 
         This method kicks off code that adds GCP resources to `self.graph`.
         When collect() finishes the parent thread will take `self.graph` and merge
         it with the global production graph.
         """
         log.debug("plugin: GCP collecting resources")
         assert self.core_feedback, "core_feedback is not set"  # will be set by the outer collector plugin
+        feedback = self.core_feedback.with_context("gcp")
 
         cloud = Cloud(id=self.cloud, name="Gcp")
 
-        credentials = Credentials.all()
+        credentials = Credentials.all(feedback)
         if len(Config.gcp.project) > 0:
             for project in list(credentials.keys()):
                 if project not in Config.gcp.project:
                     del credentials[project]
 
         if len(credentials) == 0:
             return
@@ -64,22 +65,17 @@
                 "credentials": credentials if all(v is None for v in credentials.values()) else None,
             }
             collect_method = collect_in_process
         else:
             collect_method = self.collect_project
 
         with pool_executor(**pool_args) as executor:
+            # noinspection PyTypeChecker
             wait_for = [
-                executor.submit(
-                    collect_method,
-                    project_id,
-                    self.core_feedback.with_context("gcp"),
-                    cloud,
-                    **collect_args,
-                )
+                executor.submit(collect_method, project_id, feedback, cloud, **collect_args)
                 for project_id in credentials.keys()
             ]
             for future in futures.as_completed(wait_for):
                 project_graph = future.result()
                 if not isinstance(project_graph, Graph):
                     log.error(f"Skipping invalid project_graph {type(project_graph)}")
                     continue
```

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/gcp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     response_path: str
     response_regional_sub_path: Optional[str] = None
     set_label_identifier: str = "resource"
     get_identifier: Optional[str] = None
     delete_identifier: Optional[str] = None
     required_iam_permissions: Optional[List[str]] = None
     mutate_iam_permissions: Optional[List[str]] = None
+    expected_errors: Optional[Set[str]] = None
 
     def for_delete(self) -> GcpApiSpec:
         params = self.request_parameter.copy()
         params[self._delete_identifier] = "{resource}"
         if self.is_zone_specific:
             params["zone"] = "{zone}"
         return evolve(
```

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import json
 import concurrent
 import logging
 from concurrent.futures import Executor, Future
 from threading import Lock
-from typing import Callable, List, ClassVar, Optional, TypeVar, Type, Any, Dict
+from typing import Callable, List, ClassVar, Optional, TypeVar, Type, Any, Dict, Set
 from types import TracebackType
 
 from attr import define, field
 from google.auth.credentials import Credentials as GoogleAuthCredentials
 from googleapiclient.errors import HttpError
 
 from resoto_plugin_gcp.gcp_client import GcpClient, GcpApiSpec, InternalZoneProp, RegionProp
@@ -22,15 +22,15 @@
     BaseRegion,
     BaseZone,
     BaseQuota,
     ModelReference,
 )
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph, EdgeKey
-from resotolib.json import from_json as from_js
+from resotolib.json import from_json as from_js, value_in_path
 from resotolib.json_bender import bend, Bender, S, Bend
 from resotolib.types import Json
 from resotolib.config import Config
 
 
 log = logging.getLogger("resoto.plugins.gcp")
 
@@ -396,15 +396,16 @@
         pass
 
     @classmethod
     def collect_resources(cls: Type[GcpResource], builder: GraphBuilder, **kwargs: Any) -> List[GcpResource]:
         # Default behavior: in case the class has an ApiSpec, call the api and call collect.
         log.info(f"[Gcp:{builder.project.id}] Collecting {cls.__name__} with ({kwargs})")
         if spec := cls.api_spec:
-            with GcpErrorHandler(builder.core_feedback, f" in {builder.project.id} kind {cls.kind}"):
+            expected_errors = GcpExpectedErrorCodes | (spec.expected_errors or set())
+            with GcpErrorHandler(builder.core_feedback, expected_errors, f" in {builder.project.id} kind {cls.kind}"):
                 items = builder.client.list(spec, **kwargs)
                 return cls.collect(items, builder)
         return []
 
     @classmethod
     def collect(cls: Type[GcpResource], raw: List[Json], builder: GraphBuilder) -> List[GcpResource]:
         # Default behavior: iterate over json snippets and for each:
@@ -568,44 +569,69 @@
     description: Optional[str] = field(default=None)
     status: Optional[str] = field(default=None)
     zone_available_cpu_platforms: Optional[List[str]] = field(default=None)
     zone_deprecated: Optional[GcpDeprecationStatus] = field(default=None)
     zone_supports_pzs: Optional[bool] = field(default=None)
 
 
+GcpExpectedErrorCodes = {
+    "PERMISSION_DENIED:usageLimits:accessNotConfigured"  # resource not enabled - no resources to expect
+}
+
+
 class GcpErrorHandler:
-    def __init__(self, core_feedback: CoreFeedback, extra_info: str = "") -> None:
+    def __init__(self, core_feedback: CoreFeedback, expected_errors: Set[str], extra_info: str = "") -> None:
         self.core_feedback = core_feedback
         self.extra_info = extra_info
+        self.expected_errors = expected_errors
 
     def __enter__(self) -> "GcpErrorHandler":
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[Exception]],
         exc_value: Optional[Exception],
         traceback: Optional[TracebackType],
     ) -> Optional[bool]:
         if exc_type is None:
             return None
 
-        error_details = exc_value
+        error_details = str(exc_value)
+        errors: Set[str] = set()
         if exc_type is HttpError and isinstance(exc_value, HttpError):
             try:
                 exc_content: Json = json.loads(exc_value.content.decode())
-                error_details = exc_content.get("error", {}).get("message", exc_value)
-            except Exception:
+                status = value_in_path(exc_content, ["error", "status"])
+                errors = {
+                    f'{status}:{error.get("domain", "none")}:{error.get("reason", "none")}'
+                    for error in (value_in_path(exc_content, ["error", "errors"]) or [])
+                }
+                error_details = str(exc_content.get("error", {}).get("message", exc_value))
+            except Exception as ex:
+                errors = {f"ParseError:unknown:{ex}"}
                 pass
+        error_summary = ", ".join(errors)
+
+        if errors and errors.issubset(self.expected_errors):
+            log.info(
+                f"Expected Exception while collecting{self.extra_info} ({exc_type.__name__}): "
+                f"{error_details} Error Codes: {error_summary}. Ignore."
+            )
+            return True
 
         if not Config.gcp.discard_account_on_resource_error:
             self.core_feedback.error(
-                f"Error while collecting{self.extra_info} ({exc_type.__name__}): {error_details}", log
+                f"Error while collecting{self.extra_info} ({exc_type.__name__}): "
+                f"{error_details} Error Codes: {error_summary}",
+                log,
             )
             return True
 
         if exc_type is HttpError and isinstance(exc_value, HttpError):
             if exc_value.resp.status == 403:
-                self.core_feedback.error(f"Access denied{self.extra_info}: {error_details}", log)
+                self.core_feedback.error(
+                    f"Access denied{self.extra_info}: {error_details} Error Codes: {error_summary}", log
+                )
                 return True
 
         return False
```

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/resources/storage.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/storage.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import json
 import os
 import socket
-from resotolib.baseresources import BaseResource
-from resotolib.config import Config
-from resotolib.graph import Graph
-from resotolib.lock import RWLock
-import resotolib.logger
-from typing import Iterable, List, Union, Callable, Any, Dict
+from datetime import datetime
+from typing import Iterable, List, Union, Callable, Any, Dict, Optional
+
+from google.oauth2 import service_account
 from googleapiclient import discovery
-from googleapiclient.errors import HttpError as GoogleApiClientHttpError
 from googleapiclient.discovery_cache.base import Cache as GoogleApiClientCache
-from google.oauth2 import service_account
-from datetime import datetime
+from googleapiclient.errors import HttpError as GoogleApiClientHttpError
 from retrying import retry
 from tenacity import Retrying, stop_after_attempt, retry_if_exception_type
 
-# from google.oauth2.credentials import UserAccessTokenCredentials
+import resotolib.logger
+from resotolib.baseresources import BaseResource
+from resotolib.config import Config
+from resotolib.core.actions import CoreFeedback
+from resotolib.graph import Graph
+from resotolib.lock import RWLock
 
 log = resotolib.logger.getLogger("resoto." + __name__)
 resotolib.logger.getLogger("googleapiclient").setLevel(resotolib.logger.ERROR)
 
 
 SCOPES = ["https://www.googleapis.com/auth/cloud-platform"]
 
@@ -43,49 +43,56 @@
 
 class Credentials:
     _credentials = {}
     _initialized = False
     _lock = RWLock()
 
     @staticmethod
-    def load():
+    def load(feedback: Optional[CoreFeedback] = None):
         with Credentials._lock.write_access:
             if not Credentials._initialized:
                 for sa_data in Config.gcp.service_account:
-                    credentials = load_credentials(sa_data)
-                    for project in list_credential_projects(credentials):
-                        Credentials._credentials[project["id"]] = credentials
+                    try:
+                        log.debug("Loading credentials from %s", sa_data)
+                        credentials = load_credentials(sa_data)
+                        for project in list_credential_projects(credentials):
+                            Credentials._credentials[project["id"]] = credentials
+                    except Exception as e:
+                        log.error("Unable to load credentials from %s", sa_data, exc_info=e)
+                        if feedback is not None:
+                            feedback.error(f"Unable to load credentials from {sa_data}: {e}")
                 Credentials._initialized = True
 
     @staticmethod
     def get(project_id: str):
         Credentials.load()
         with Credentials._lock.read_access:
             return Credentials._credentials.get(project_id)
 
     @staticmethod
-    def all() -> Dict:
-        Credentials.load()
+    def all(feedback: Optional[CoreFeedback] = None) -> Dict:
+        Credentials.load(feedback)
         with Credentials._lock.read_access:
             return dict(Credentials._credentials)
 
     @staticmethod
     def reload():
         with Credentials._lock.write_access:
             Credentials._initialized = False
         Credentials.load()
 
 
-def load_credentials(sa_data: str):
-    if len(sa_data) == 0:
+def load_credentials(path: str):
+    if len(path) == 0:
         return None
-    if os.path.isfile(sa_data):
-        return service_account.Credentials.from_service_account_file(sa_data, scopes=SCOPES)
+    file = os.path.expanduser(path)
+    if os.path.isfile(file):
+        return service_account.Credentials.from_service_account_file(file, scopes=SCOPES)
     else:
-        return service_account.Credentials.from_service_account_info(json.loads(sa_data), scopes=SCOPES)
+        raise ValueError(f"No credentials file found at {file}")
 
 
 @retry(
     stop_max_attempt_number=10,
     wait_exponential_multiplier=3000,
     wait_exponential_max=300000,
     retry_on_exception=retry_on_error,
@@ -111,17 +118,15 @@
             p = {
                 "id": project_id,
                 "name": project_name,
                 "ctime": ctime,
             }
             ret.append(p)
     except GoogleApiClientHttpError:
-        log.error(
-            ("Unable to load projects from cloudresourcemanager" " - falling back to local credentials information")
-        )
+        log.error("Unable to load projects from cloudresourcemanager - falling back to local credentials information")
         p = {
             "id": credentials.project_id,
             "name": credentials.project_id,
         }
         ret.append(p)
     return ret
```

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.5.2
+Version: 3.5.3
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.5.2/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/conftest.py` & `resoto-plugin-gcp-3.5.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/random_client.py` & `resoto-plugin-gcp-3.5.3/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/test_base.py` & `resoto-plugin-gcp-3.5.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/test_billing.py` & `resoto-plugin-gcp-3.5.3/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/test_collector.py` & `resoto-plugin-gcp-3.5.3/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/test_compute.py` & `resoto-plugin-gcp-3.5.3/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/test_config.py` & `resoto-plugin-gcp-3.5.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/test_container.py` & `resoto-plugin-gcp-3.5.3/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.2/test/test_sqladmin.py` & `resoto-plugin-gcp-3.5.3/test/test_sqladmin.py`

 * *Files identical despite different names*

