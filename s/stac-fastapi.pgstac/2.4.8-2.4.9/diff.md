# Comparing `tmp/stac-fastapi.pgstac-2.4.8.tar.gz` & `tmp/stac-fastapi.pgstac-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.pgstac-2.4.8.tar", last modified: Fri Jun  9 18:28:38 2023, max compression
+gzip compressed data, was "stac-fastapi.pgstac-2.4.9.tar", last modified: Wed Jun 21 21:25:28 2023, max compression
```

## Comparing `stac-fastapi.pgstac-2.4.8.tar` & `stac-fastapi.pgstac-2.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.773734 stac-fastapi.pgstac-2.4.8/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/base_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.777734 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.773734 stac-fastapi.pgstac-2.4.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/clients/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_mgmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/base_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/clients/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_mgmt.py
```

### Comparing `stac-fastapi.pgstac-2.4.8/LICENSE` & `stac-fastapi.pgstac-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/PKG-INFO` & `stac-fastapi.pgstac-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.4.8
+Version: 2.4.9
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.pgstac-2.4.8/README.md` & `stac-fastapi.pgstac-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/setup.py` & `stac-fastapi.pgstac-2.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/app.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/app.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/config.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/core.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
                 ).get_links(extra_links=feature.get("links"))
 
         cleaned_features: List[Item] = []
 
         if settings.use_api_hydrate:
 
             async def _get_base_item(collection_id: str) -> Dict[str, Any]:
-                return await self._get_base_item(collection_id, request)
+                return await self._get_base_item(collection_id, request=request)
 
             base_item_cache = settings.base_item_cache(
                 fetch_base_item=_get_base_item, request=request
             )
 
             for feature in collection.get("features") or []:
                 base_item = await base_item_cache.get(feature.get("collection"))
@@ -263,15 +263,15 @@
             limit: number of items to return.
             token: pagination token.
 
         Returns:
             An ItemCollection.
         """
         # If collection does not exist, NotFoundError wil be raised
-        await self.get_collection(collection_id, request)
+        await self.get_collection(collection_id, request=request)
 
         base_args = {
             "collections": [collection_id],
             "bbox": bbox,
             "datetime": datetime,
             "limit": limit,
             "token": token,
@@ -281,15 +281,15 @@
         for k, v in base_args.items():
             if v is not None and v != []:
                 clean[k] = v
 
         search_request = self.post_request_model(
             **clean,
         )
-        item_collection = await self._search_base(search_request, request)
+        item_collection = await self._search_base(search_request, request=request)
         links = await ItemCollectionLinks(
             collection_id=collection_id, request=request
         ).get_links(extra_links=item_collection["links"])
         item_collection["links"] = links
         return item_collection
 
     async def get_item(
@@ -303,20 +303,20 @@
             item_id: ID of the item.
             collection_id: ID of the collection the item is in.
 
         Returns:
             Item.
         """
         # If collection does not exist, NotFoundError wil be raised
-        await self.get_collection(collection_id, request)
+        await self.get_collection(collection_id, request=request)
 
         search_request = self.post_request_model(
             ids=[item_id], collections=[collection_id], limit=1
         )
-        item_collection = await self._search_base(search_request, request)
+        item_collection = await self._search_base(search_request, request=request)
         if not item_collection["features"]:
             raise NotFoundError(
                 f"Item {item_id} in Collection {collection_id} does not exist."
             )
 
         return Item(**item_collection["features"][0])
 
@@ -329,15 +329,15 @@
 
         Args:
             search_request: search request parameters.
 
         Returns:
             ItemCollection containing items which match the search criteria.
         """
-        item_collection = await self._search_base(search_request, request)
+        item_collection = await self._search_base(search_request, request=request)
         return ItemCollection(**item_collection)
 
     async def get_search(
         self,
         request: Request,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
```

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/db.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/filter.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/filter.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/query.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/links.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/links.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/transactions.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/transactions.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/base_item_cache.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/base_item_cache.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/search.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/search.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/utils.py` & `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/PKG-INFO` & `stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.4.8
+Version: 2.4.9
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/SOURCES.txt` & `stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/tests/api/test_api.py` & `stac-fastapi.pgstac-2.4.9/tests/api/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 from datetime import datetime, timedelta
-from typing import Any, Dict, List
+from typing import Any, Callable, Coroutine, Dict, List, Optional, TypeVar
 from urllib.parse import quote_plus
 
 import orjson
 import pytest
+from fastapi import Request
+from httpx import AsyncClient
 from pystac import Collection, Extent, Item, SpatialExtent, TemporalExtent
+from stac_fastapi.api.app import StacApi
+from stac_fastapi.api.models import create_post_request_model
+from stac_fastapi.extensions.core import FieldsExtension, TransactionExtension
+from stac_fastapi.types import stac as stac_types
+
+from stac_fastapi.pgstac.core import CoreCrudClient, Settings
+from stac_fastapi.pgstac.db import close_db_connection, connect_to_db
+from stac_fastapi.pgstac.transactions import TransactionsClient
+from stac_fastapi.pgstac.types.search import PgstacSearch
 
 STAC_CORE_ROUTES = [
     "GET /",
     "GET /collections",
     "GET /collections/{collection_id}",
     "GET /collections/{collection_id}/items",
     "GET /collections/{collection_id}/items/{item_id}",
@@ -618,7 +629,78 @@
     query = {
         "collections": [collection_id],
         "sortby": [{"field": "properties.eo:cloud_cover", "direction": direction}],
         "limit": 5,
     }
     items = await search(query)
     assert len(items) == 10, items
+
+
+@pytest.mark.asyncio
+async def test_wrapped_function(load_test_data) -> None:
+    # Ensure wrappers, e.g. Planetary Computer's rate limiting, work.
+    # https://github.com/gadomski/planetary-computer-apis/blob/2719ccf6ead3e06de0784c39a2918d4d1811368b/pccommon/pccommon/redis.py#L205-L238
+
+    T = TypeVar("T")
+
+    def wrap() -> (
+        Callable[
+            [Callable[..., Coroutine[Any, Any, T]]],
+            Callable[..., Coroutine[Any, Any, T]],
+        ]
+    ):
+        def decorator(
+            fn: Callable[..., Coroutine[Any, Any, T]]
+        ) -> Callable[..., Coroutine[Any, Any, T]]:
+            async def _wrapper(*args: Any, **kwargs: Any) -> T:
+                request: Optional[Request] = kwargs.get("request")
+                if request:
+                    pass  # This is where rate limiting would be applied
+                else:
+                    raise ValueError(f"Missing request in {fn.__name__}")
+                return await fn(*args, **kwargs)
+
+            return _wrapper
+
+        return decorator
+
+    class Client(CoreCrudClient):
+        @wrap()
+        async def get_collection(
+            self, collection_id: str, request: Request, **kwargs
+        ) -> stac_types.Item:
+            return await super().get_collection(
+                collection_id, request=request, **kwargs
+            )
+
+    settings = Settings(testing=True)
+    extensions = [
+        TransactionExtension(client=TransactionsClient(), settings=settings),
+        FieldsExtension(),
+    ]
+    post_request_model = create_post_request_model(extensions, base_model=PgstacSearch)
+    api = StacApi(
+        client=Client(post_request_model=post_request_model),
+        settings=settings,
+        extensions=extensions,
+        search_post_request_model=post_request_model,
+    )
+    app = api.app
+    await connect_to_db(app)
+    try:
+        async with AsyncClient(app=app) as client:
+            response = await client.post(
+                "http://test/collections",
+                json=load_test_data("test_collection.json"),
+            )
+            assert response.status_code == 200
+            response = await client.post(
+                "http://test/collections/test-collection/items",
+                json=load_test_data("test_item.json"),
+            )
+            assert response.status_code == 200
+            response = await client.get(
+                "http://test/collections/test-collection/items/test-item"
+            )
+            assert response.status_code == 200
+    finally:
+        await close_db_connection(app)
```

### Comparing `stac-fastapi.pgstac-2.4.8/tests/clients/test_postgres.py` & `stac-fastapi.pgstac-2.4.9/tests/clients/test_postgres.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/tests/resources/test_collection.py` & `stac-fastapi.pgstac-2.4.9/tests/resources/test_collection.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/tests/resources/test_conformance.py` & `stac-fastapi.pgstac-2.4.9/tests/resources/test_conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.8/tests/resources/test_item.py` & `stac-fastapi.pgstac-2.4.9/tests/resources/test_item.py`

 * *Files identical despite different names*

