# Comparing `tmp/stac_collection_search-0.0.1.tar.gz` & `tmp/stac_collection_search-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_collection_search-0.0.1.tar", last modified: Wed Jun 21 13:42:22 2023, max compression
+gzip compressed data, was "stac_collection_search-0.0.2.tar", last modified: Wed Jun 21 17:56:01 2023, max compression
```

## Comparing `stac_collection_search-0.0.1.tar` & `stac_collection_search-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 13:42:22.352415 stac_collection_search-0.0.1/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2941 2023-06-21 13:42:22.352415 stac_collection_search-0.0.1/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2462 2023-06-21 13:30:42.000000 stac_collection_search-0.0.1/README.md
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-21 13:42:22.352415 stac_collection_search-0.0.1/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-06-21 13:17:43.000000 stac_collection_search-0.0.1/setup.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 13:42:22.352415 stac_collection_search-0.0.1/stac_collection_search/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      128 2023-06-21 10:49:24.000000 stac_collection_search-0.0.1/stac_collection_search/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     3036 2023-06-21 13:11:22.000000 stac_collection_search-0.0.1/stac_collection_search/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 13:42:22.352415 stac_collection_search-0.0.1/stac_collection_search.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2941 2023-06-21 13:42:22.000000 stac_collection_search-0.0.1/stac_collection_search.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      314 2023-06-21 13:42:22.000000 stac_collection_search-0.0.1/stac_collection_search.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-21 13:42:22.000000 stac_collection_search-0.0.1/stac_collection_search.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-06-21 13:42:22.000000 stac_collection_search-0.0.1/stac_collection_search.egg-info/requires.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-06-21 13:42:22.000000 stac_collection_search-0.0.1/stac_collection_search.egg-info/top_level.txt
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 17:56:01.243134 stac_collection_search-0.0.2/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 17:56:01.243134 stac_collection_search-0.0.2/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      946 2023-06-21 17:54:21.000000 stac_collection_search-0.0.2/README.md
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-21 17:56:01.243134 stac_collection_search-0.0.2/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-06-21 17:55:09.000000 stac_collection_search-0.0.2/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 17:56:01.243134 stac_collection_search-0.0.2/stac_collection_search/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      128 2023-06-21 10:49:24.000000 stac_collection_search-0.0.2/stac_collection_search/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     3734 2023-06-21 17:53:10.000000 stac_collection_search-0.0.2/stac_collection_search/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 17:56:01.243134 stac_collection_search-0.0.2/stac_collection_search.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 17:56:01.000000 stac_collection_search-0.0.2/stac_collection_search.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      314 2023-06-21 17:56:01.000000 stac_collection_search-0.0.2/stac_collection_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-21 17:56:01.000000 stac_collection_search-0.0.2/stac_collection_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-06-21 17:56:01.000000 stac_collection_search-0.0.2/stac_collection_search.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-06-21 17:56:01.000000 stac_collection_search-0.0.2/stac_collection_search.egg-info/top_level.txt
```

### Comparing `stac_collection_search-0.0.1/setup.py` & `stac_collection_search-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'STAC Collection Search helper utility'
 LONG_DESCRIPTION = 'STAC Collection Search helper which enables a collection search on the stac-fastapi'
 
 requirements = []
 requirements_file = "./requirements.txt"
 if os.path.isfile(requirements_file):
     with open(requirements_file) as f:
```

### Comparing `stac_collection_search-0.0.1/stac_collection_search/utils.py` & `stac_collection_search-0.0.2/stac_collection_search/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,57 +19,100 @@
     return shapely.geometry.box(*bbox_list)
 
 
 def _get_collections(collection_list_json: dict) -> List[CollectionInfo]:
     return [
         CollectionInfo(
             id=i["id"],
-            spatial_extent=shapely.geometry.MultiPolygon([
-                _get_shapely_object_from_bbox_list(spatial_extent)
-                for spatial_extent in i["extent"]["spatial"]["bbox"]
-            ]),
+            spatial_extent=shapely.geometry.MultiPolygon(
+                [
+                    _get_shapely_object_from_bbox_list(spatial_extent)
+                    for spatial_extent in i["extent"]["spatial"]["bbox"]
+                ]
+            ),
             temporal_extent=TemporalExtent(
                 start=_process_timestamp(i["extent"]["temporal"]["interval"][0][0]),
-                end=_process_timestamp(i["extent"]["temporal"]["interval"][0][1])
-            )
-        ) for i in collection_list_json["collections"]
+                end=_process_timestamp(i["extent"]["temporal"]["interval"][-1][1]),
+            ),
+        )
+        for i in collection_list_json["collections"]
     ]
 
 
 def _process_timestamp(timestamp: str) -> datetime:
     """
     Process a timestamp string into a datetime object.
     """
     if timestamp is None:
         return None
-    for fmt in ['%Y-%m-%dT%H:%M:%S%Z', '%Y-%m-%dT%H:%M:%S%z', '%Y-%m-%dT%H:%M:%S.%f%z', '%Y-%m-%dT%H:%M:%S.%f']:
+    for fmt in [
+        "%Y-%m-%dT%H:%M:%S%Z",
+        "%Y-%m-%dT%H:%M:%S%z",
+        "%Y-%m-%dT%H:%M:%S.%f%z",
+        "%Y-%m-%dT%H:%M:%S.%f",
+    ]:
         try:
             return datetime.datetime.strptime(timestamp, fmt)
         except ValueError:
             continue
     raise ValueError(f"timestamp {timestamp} does not match any known formats")
 
 
-def search_collections(collection_json_dict: dict, spatial_extent: shapely.geometry.Polygon = None,
-                       temporal_extent_start=None, temporal_extent_end=None) -> List[Dict[AnyStr, Any]]:
+def search_collections_verbose_output(
+    collection_json_dict: dict,
+    spatial_extent: shapely.geometry.Polygon = None,
+    temporal_extent_start=None,
+    temporal_extent_end=None,
+) -> List[Dict[AnyStr, Any]]:
     # Ensure that temporal_extent_start and temporal_extent_end are timezone-aware (in UTC)
     if temporal_extent_start and temporal_extent_start.tzinfo is None:
-        temporal_extent_start = temporal_extent_start.replace(tzinfo=datetime.timezone.utc)
+        temporal_extent_start = temporal_extent_start.replace(
+            tzinfo=datetime.timezone.utc
+        )
     if temporal_extent_end and temporal_extent_end.tzinfo is None:
         temporal_extent_end = temporal_extent_end.replace(tzinfo=datetime.timezone.utc)
 
     collection_list = _get_collections(collection_json_dict)
 
     # First, we filter by spatial extent
     collections_spatially_filtered = (
-        [collection for collection in collection_list if spatial_extent.intersects(collection["spatial_extent"])]
-        if spatial_extent else collection_list
+        [
+            collection
+            for collection in collection_list
+            if spatial_extent.intersects(collection["spatial_extent"])
+        ]
+        if spatial_extent
+        else collection_list
     )
 
     # Now we apply time-based filter on spatially filtered collections
     return [
-        collection["id"] for collection in collections_spatially_filtered
-        if (temporal_extent_start is None or collection["temporal_extent"]["end"] is None or
-            collection["temporal_extent"]["end"] >= temporal_extent_start) and
-           (temporal_extent_end is None or collection["temporal_extent"]["start"] is None or
-            collection["temporal_extent"]["start"] <= temporal_extent_end)
+        collection
+        for collection in collections_spatially_filtered
+        if (
+            temporal_extent_start is None
+            or collection["temporal_extent"]["end"] is None
+            or collection["temporal_extent"]["end"] >= temporal_extent_start
+        )
+        and (
+            temporal_extent_end is None
+            or collection["temporal_extent"]["start"] is None
+            or collection["temporal_extent"]["start"] <= temporal_extent_end
+        )
+    ]
+
+
+def search_collections_verbose_output(
+    collection_json_dict: dict,
+    spatial_extent: shapely.geometry.Polygon = None,
+    temporal_extent_start=None,
+    temporal_extent_end=None,
+) -> List[AnyStr]:
+    return [
+        collection["id"]
+        for collection in search_collections_verbose_output(
+            collection_json_dict,
+            spatial_extent,
+            temporal_extent_start,
+            temporal_extent_end,
+        )
     ]
```

