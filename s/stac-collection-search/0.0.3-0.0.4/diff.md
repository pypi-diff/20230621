# Comparing `tmp/stac_collection_search-0.0.3.tar.gz` & `tmp/stac_collection_search-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_collection_search-0.0.3.tar", last modified: Wed Jun 21 18:15:54 2023, max compression
+gzip compressed data, was "stac_collection_search-0.0.4.tar", last modified: Wed Jun 21 18:52:10 2023, max compression
```

## Comparing `stac_collection_search-0.0.3.tar` & `stac_collection_search-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:15:54.527988 stac_collection_search-0.0.3/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 18:15:54.527988 stac_collection_search-0.0.3/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      946 2023-06-21 17:54:21.000000 stac_collection_search-0.0.3/README.md
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-21 18:15:54.527988 stac_collection_search-0.0.3/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-06-21 18:11:40.000000 stac_collection_search-0.0.3/setup.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:15:54.523988 stac_collection_search-0.0.3/stac_collection_search/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       83 2023-06-21 18:14:31.000000 stac_collection_search-0.0.3/stac_collection_search/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     3712 2023-06-21 18:15:47.000000 stac_collection_search-0.0.3/stac_collection_search/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:15:54.523988 stac_collection_search-0.0.3/stac_collection_search.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 18:15:54.000000 stac_collection_search-0.0.3/stac_collection_search.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      314 2023-06-21 18:15:54.000000 stac_collection_search-0.0.3/stac_collection_search.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-21 18:15:54.000000 stac_collection_search-0.0.3/stac_collection_search.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-06-21 18:15:54.000000 stac_collection_search-0.0.3/stac_collection_search.egg-info/requires.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-06-21 18:15:54.000000 stac_collection_search-0.0.3/stac_collection_search.egg-info/top_level.txt
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:52:10.322627 stac_collection_search-0.0.4/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 18:52:10.318627 stac_collection_search-0.0.4/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      946 2023-06-21 17:54:21.000000 stac_collection_search-0.0.4/README.md
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-21 18:52:10.322627 stac_collection_search-0.0.4/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-06-21 18:51:33.000000 stac_collection_search-0.0.4/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:52:10.318627 stac_collection_search-0.0.4/stac_collection_search/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       83 2023-06-21 18:14:31.000000 stac_collection_search-0.0.4/stac_collection_search/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     4006 2023-06-21 18:46:42.000000 stac_collection_search-0.0.4/stac_collection_search/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:52:10.318627 stac_collection_search-0.0.4/stac_collection_search.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      314 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/top_level.txt
```

### Comparing `stac_collection_search-0.0.3/PKG-INFO` & `stac_collection_search-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac_collection_search
-Version: 0.0.3
+Version: 0.0.4
 Summary: STAC Collection Search helper utility
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 Keywords: python,azure,stac,fastapi,eo,earth observation,spatial,search,collection
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stac_collection_search-0.0.3/README.md` & `stac_collection_search-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `stac_collection_search-0.0.3/setup.py` & `stac_collection_search-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'STAC Collection Search helper utility'
 LONG_DESCRIPTION = 'STAC Collection Search helper which enables a collection search on the stac-fastapi'
 
 requirements = []
 requirements_file = "./requirements.txt"
 if os.path.isfile(requirements_file):
     with open(requirements_file) as f:
```

### Comparing `stac_collection_search-0.0.3/stac_collection_search/utils.py` & `stac_collection_search-0.0.4/stac_collection_search/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         try:
             return datetime.datetime.strptime(timestamp, fmt)
         except ValueError:
             continue
     raise ValueError(f"timestamp {timestamp} does not match any known formats")
 
 
-def search_collections_verbose(
+def search_collections(
     collection_json_dict: dict,
     spatial_extent: shapely.geometry.Polygon = None,
     temporal_extent_start=None,
     temporal_extent_end=None,
 ) -> List[Dict[AnyStr, Any]]:
     # Ensure that temporal_extent_start and temporal_extent_end are timezone-aware (in UTC)
     if temporal_extent_start and temporal_extent_start.tzinfo is None:
@@ -81,38 +81,41 @@
             if spatial_extent.intersects(collection["spatial_extent"])
         ]
         if spatial_extent
         else collection_list
     )
 
     # Now we apply time-based filter on spatially filtered collections
-    return [
-        collection
+    ids = [
+        collection["id"]
         for collection in collections_spatially_filtered
         if (
             temporal_extent_start is None
             or collection["temporal_extent"]["end"] is None
             or collection["temporal_extent"]["end"] >= temporal_extent_start
         )
         and (
             temporal_extent_end is None
             or collection["temporal_extent"]["start"] is None
             or collection["temporal_extent"]["start"] <= temporal_extent_end
         )
     ]
+    return ids
 
 
-def search_collections(
+def search_collections_verbose(
     collection_json_dict: dict,
     spatial_extent: shapely.geometry.Polygon = None,
     temporal_extent_start=None,
     temporal_extent_end=None,
 ) -> List[AnyStr]:
+    
+    ids = search_collections(collection_json_dict=collection_json_dict,
+                                spatial_extent=spatial_extent,
+                                temporal_extent_start=temporal_extent_start,
+                                temporal_extent_end=temporal_extent_end)
+    # filter the collection_json_dict to only include the collections that are in the ids list
     return [
-        collection["id"]
-        for collection in search_collections_verbose_output(
-            collection_json_dict,
-            spatial_extent,
-            temporal_extent_start,
-            temporal_extent_end,
-        )
-    ]
+        collection
+        for collection in collection_json_dict["collections"]
+        if collection["id"] in ids
+    ]
```

### Comparing `stac_collection_search-0.0.3/stac_collection_search.egg-info/PKG-INFO` & `stac_collection_search-0.0.4/stac_collection_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-collection-search
-Version: 0.0.3
+Version: 0.0.4
 Summary: STAC Collection Search helper utility
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 Keywords: python,azure,stac,fastapi,eo,earth observation,spatial,search,collection
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

