# Comparing `tmp/titiler.pgstac-0.4.0.tar.gz` & `tmp/titiler.pgstac-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.pgstac-0.4.0.tar", last modified: Mon May 22 19:15:37 2023, max compression
+gzip compressed data, was "titiler.pgstac-0.4.1.tar", last modified: Wed Jun 21 08:30:16 2023, max compression
```

## Comparing `titiler.pgstac-0.4.0.tar` & `titiler.pgstac-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1097 2023-05-22 19:15:07.041101 titiler.pgstac-0.4.0/LICENSE
--rw-r--r--   0        0        0     4451 2023-05-22 19:15:07.041101 titiler.pgstac-0.4.0/README.md
--rw-r--r--   0        0        0     2618 2023-05-22 19:15:07.149102 titiler.pgstac-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/__init__.py
--rw-r--r--   0        0        0      874 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/db.py
--rw-r--r--   0        0        0     3936 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/dependencies.py
--rw-r--r--   0        0        0    37682 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/factory.py
--rw-r--r--   0        0        0       91 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/logger.py
--rw-r--r--   0        0        0     3860 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/main.py
--rw-r--r--   0        0        0     6797 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/model.py
--rw-r--r--   0        0        0    12695 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/mosaic.py
--rw-r--r--   0        0        0     2642 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/reader.py
--rw-r--r--   0        0        0     3518 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/settings.py
--rw-r--r--   0        0        0      834 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/utils.py
--rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 titiler.pgstac-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-21 08:29:39.269532 titiler.pgstac-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4451 2023-06-21 08:29:39.269532 titiler.pgstac-0.4.1/README.md
+-rw-r--r--   0        0        0     2618 2023-06-21 08:29:39.393534 titiler.pgstac-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/__init__.py
+-rw-r--r--   0        0        0      874 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/db.py
+-rw-r--r--   0        0        0     3936 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/dependencies.py
+-rw-r--r--   0        0        0    37672 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/factory.py
+-rw-r--r--   0        0        0       91 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/logger.py
+-rw-r--r--   0        0        0     3877 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/main.py
+-rw-r--r--   0        0        0     6797 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/model.py
+-rw-r--r--   0        0        0    12695 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/mosaic.py
+-rw-r--r--   0        0        0     2642 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/reader.py
+-rw-r--r--   0        0        0     3518 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/settings.py
+-rw-r--r--   0        0        0      834 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/utils.py
+-rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 titiler.pgstac-0.4.1/PKG-INFO
```

### Comparing `titiler.pgstac-0.4.0/LICENSE` & `titiler.pgstac-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/README.md` & `titiler.pgstac-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/pyproject.toml` & `titiler.pgstac-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
-    "titiler.core>=0.11.6,<0.12",
-    "titiler.mosaic>=0.11.6,<0.12",
+    "titiler.core>=0.11.7,<0.12",
+    "titiler.mosaic>=0.11.7,<0.12",
     "geojson-pydantic",
     "stac-pydantic==2.0.*",
     "fastapi>=0.87,<0.95",
     "starlette>=0.21.0,<0.25",
 ]
 dynamic = []
-version = "0.4.0"
+version = "0.4.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 psycopg = [
     "psycopg[pool]",
```

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/db.py` & `titiler.pgstac-0.4.1/titiler/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/dependencies.py` & `titiler.pgstac-0.4.1/titiler/pgstac/dependencies.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/factory.py` & `titiler.pgstac-0.4.1/titiler/pgstac/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ] = SearchParams
 
     backend_dependency: Type[DefaultDependency] = BackendParams
 
     # Add/Remove some endpoints
     add_statistics: bool = False
 
-    add_map_viewer: bool = False
+    add_viewer: bool = False
 
     add_mosaic_list: bool = False
 
     def register_routes(self) -> None:
         """This Method register routes to the router."""
         self._search_routes()
         if self.add_mosaic_list:
@@ -94,15 +94,15 @@
         self._tilejson_routes()
         self._wmts_routes()
         self._assets_routes()
 
         if self.add_statistics:
             self._statistics_routes()
 
-        if self.add_map_viewer:
+        if self.add_viewer:
             self._map_routes()
 
     def _tiles_routes(self) -> None:
         """register tiles routes."""
 
         @self.router.get("/{searchid}/tiles/{z}/{x}/{y}", **img_endpoint_params)
         @self.router.get(
@@ -406,15 +406,15 @@
                 request, "tilejson", searchid=searchid, TileMatrixSetId=TileMatrixSetId
             )
             if request.query_params._list:
                 tilejson_url += f"?{urlencode(request.query_params._list)}"
 
             tms = self.supported_tms.get(TileMatrixSetId)
             return self.templates.TemplateResponse(
-                name="index.html",
+                name="map.html",
                 context={
                     "request": request,
                     "tilejson_endpoint": tilejson_url,
                     "tms": tms,
                     "resolutions": [tms._resolution(matrix) for matrix in tms],
                 },
                 media_type="text/html",
```

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/main.py` & `titiler.pgstac-0.4.1/titiler/pgstac/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,26 +71,27 @@
 
 ###############################################################################
 # MOSAIC Endpoints
 mosaic = MosaicTilerFactory(
     optional_headers=optional_headers,
     router_prefix="/mosaic",
     add_statistics=True,
-    add_map_viewer=True,
+    add_viewer=True,
     add_mosaic_list=True,
 )
 app.include_router(mosaic.router, tags=["Mosaic"], prefix="/mosaic")
 
 ###############################################################################
 # STAC Item Endpoints
 stac = MultiBaseTilerFactory(
     reader=PgSTACReader,
     path_dependency=ItemPathParams,
     optional_headers=optional_headers,
     router_prefix="/collections/{collection_id}/items/{item_id}",
+    add_viewer=True,
 )
 app.include_router(
     stac.router, tags=["Item"], prefix="/collections/{collection_id}/items/{item_id}"
 )
 
 ###############################################################################
 # Tiling Schemes Endpoints
```

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/model.py` & `titiler.pgstac-0.4.1/titiler/pgstac/model.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/mosaic.py` & `titiler.pgstac-0.4.1/titiler/pgstac/mosaic.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/reader.py` & `titiler.pgstac-0.4.1/titiler/pgstac/reader.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/settings.py` & `titiler.pgstac-0.4.1/titiler/pgstac/settings.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/titiler/pgstac/utils.py` & `titiler.pgstac-0.4.1/titiler/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.0/PKG-INFO` & `titiler.pgstac-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.pgstac
-Version: 0.4.0
+Version: 0.4.1
 Summary: Connect PgSTAC and TiTiler.
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,pgSTAC
 Author-email: Vincent Sarago <vincent@developmentseed.com>,David Bitner <david@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.4.0 Summary: Connect
+Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.4.1 Summary: Connect
 PgSTAC and TiTiler. Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile
 server,pgSTAC Author-email: Vincent Sarago
 developmentseed.com>,David Bitner
 developmentseed.com> Requires-Python: >=3.8 Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

