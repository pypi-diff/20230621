# Comparing `tmp/static_osm_indexer-0.2.0.tar.gz` & `tmp/static_osm_indexer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_osm_indexer-0.2.0.tar", last modified: Thu Nov 17 14:46:24 2022, max compression
+gzip compressed data, was "static_osm_indexer-0.2.1.tar", last modified: Wed Jun 21 12:14:17 2023, max compression
```

## Comparing `static_osm_indexer-0.2.0.tar` & `static_osm_indexer-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2022-11-17 14:46:24.888491 static_osm_indexer-0.2.0/
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     4546 2022-11-17 14:46:24.888491 static_osm_indexer-0.2.0/PKG-INFO
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     3807 2022-11-17 13:22:20.000000 static_osm_indexer-0.2.0/README.md
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     2098 2022-11-17 10:33:52.000000 static_osm_indexer-0.2.0/pyproject.toml
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)       38 2022-11-17 14:46:24.888491 static_osm_indexer-0.2.0/setup.cfg
-drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2022-11-17 14:46:24.886492 static_osm_indexer-0.2.0/static_osm_indexer/
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)    12392 2022-11-16 11:26:15.000000 static_osm_indexer-0.2.0/static_osm_indexer/extract_road_network.py
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     2809 2022-11-17 13:02:26.000000 static_osm_indexer-0.2.0/static_osm_indexer/generate_full_map.py
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     6522 2022-11-17 13:18:26.000000 static_osm_indexer-0.2.0/static_osm_indexer/generate_mbtiles.py
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)      243 2022-11-13 12:38:30.000000 static_osm_indexer-0.2.0/static_osm_indexer/helpers.py
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     3562 2022-11-16 10:33:03.000000 static_osm_indexer-0.2.0/static_osm_indexer/index_locations_names.py
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     5766 2022-11-14 13:15:56.000000 static_osm_indexer-0.2.0/static_osm_indexer/list_named_locations.py
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     3369 2022-11-15 13:04:41.000000 static_osm_indexer-0.2.0/static_osm_indexer/road_network_to_geojson.py
-drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2022-11-17 14:46:24.887492 static_osm_indexer-0.2.0/static_osm_indexer/static_assets/
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     4100 2022-11-17 14:44:17.000000 static_osm_indexer-0.2.0/static_osm_indexer/static_assets/index.html
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)    73847 2022-11-14 12:39:34.000000 static_osm_indexer-0.2.0/static_osm_indexer/static_assets/osm_liberty.json
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     1827 2022-11-13 09:04:36.000000 static_osm_indexer-0.2.0/static_osm_indexer/static_assets/text_search.bundle.js
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     2618 2022-11-14 11:48:01.000000 static_osm_indexer-0.2.0/static_osm_indexer/static_assets/tilemaker_config.json
-drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2022-11-17 14:46:24.887492 static_osm_indexer-0.2.0/static_osm_indexer.egg-info/
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)     4546 2022-11-17 14:46:24.000000 static_osm_indexer-0.2.0/static_osm_indexer.egg-info/PKG-INFO
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)      767 2022-11-17 14:46:24.000000 static_osm_indexer-0.2.0/static_osm_indexer.egg-info/SOURCES.txt
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)        1 2022-11-17 14:46:24.000000 static_osm_indexer-0.2.0/static_osm_indexer.egg-info/dependency_links.txt
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)      451 2022-11-17 14:46:24.000000 static_osm_indexer-0.2.0/static_osm_indexer.egg-info/entry_points.txt
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)      130 2022-11-17 14:46:24.000000 static_osm_indexer-0.2.0/static_osm_indexer.egg-info/requires.txt
--rw-r--r--   0 jacopo    (1000) jacopo    (1000)       19 2022-11-17 14:46:24.000000 static_osm_indexer-0.2.0/static_osm_indexer.egg-info/top_level.txt
+drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2023-06-21 12:14:17.347464 static_osm_indexer-0.2.1/
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     4708 2023-06-21 12:14:17.346464 static_osm_indexer-0.2.1/PKG-INFO
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     3969 2022-11-21 13:17:48.000000 static_osm_indexer-0.2.1/README.md
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     2098 2023-06-21 12:12:48.000000 static_osm_indexer-0.2.1/pyproject.toml
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)       38 2023-06-21 12:14:17.347464 static_osm_indexer-0.2.1/setup.cfg
+drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2023-06-21 12:14:17.343464 static_osm_indexer-0.2.1/static_osm_indexer/
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)    12392 2022-11-16 11:26:15.000000 static_osm_indexer-0.2.1/static_osm_indexer/extract_road_network.py
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     2809 2022-11-17 13:02:26.000000 static_osm_indexer-0.2.1/static_osm_indexer/generate_full_map.py
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     6522 2022-11-17 13:18:26.000000 static_osm_indexer-0.2.1/static_osm_indexer/generate_mbtiles.py
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)      243 2022-11-13 12:38:30.000000 static_osm_indexer-0.2.1/static_osm_indexer/helpers.py
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     3562 2022-11-16 10:33:03.000000 static_osm_indexer-0.2.1/static_osm_indexer/index_locations_names.py
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     5766 2022-11-14 13:15:56.000000 static_osm_indexer-0.2.1/static_osm_indexer/list_named_locations.py
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     3369 2022-11-15 13:04:41.000000 static_osm_indexer-0.2.1/static_osm_indexer/road_network_to_geojson.py
+drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2023-06-21 12:14:17.346464 static_osm_indexer-0.2.1/static_osm_indexer/static_assets/
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     4072 2023-06-21 12:11:31.000000 static_osm_indexer-0.2.1/static_osm_indexer/static_assets/index.html
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)    63722 2023-06-13 21:25:28.000000 static_osm_indexer-0.2.1/static_osm_indexer/static_assets/maplibre-gl.css
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)   760516 2023-06-13 21:23:51.000000 static_osm_indexer-0.2.1/static_osm_indexer/static_assets/maplibre-gl.js
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)    73847 2022-11-14 12:39:34.000000 static_osm_indexer-0.2.1/static_osm_indexer/static_assets/osm_liberty.json
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     1827 2022-11-13 09:04:36.000000 static_osm_indexer-0.2.1/static_osm_indexer/static_assets/text_search.bundle.js
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     2618 2022-11-14 11:48:01.000000 static_osm_indexer-0.2.1/static_osm_indexer/static_assets/tilemaker_config.json
+drwxr-xr-x   0 jacopo    (1000) jacopo    (1000)        0 2023-06-21 12:14:17.344464 static_osm_indexer-0.2.1/static_osm_indexer.egg-info/
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)     4708 2023-06-21 12:14:17.000000 static_osm_indexer-0.2.1/static_osm_indexer.egg-info/PKG-INFO
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)      864 2023-06-21 12:14:17.000000 static_osm_indexer-0.2.1/static_osm_indexer.egg-info/SOURCES.txt
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)        1 2023-06-21 12:14:17.000000 static_osm_indexer-0.2.1/static_osm_indexer.egg-info/dependency_links.txt
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)      451 2023-06-21 12:14:17.000000 static_osm_indexer-0.2.1/static_osm_indexer.egg-info/entry_points.txt
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)      130 2023-06-21 12:14:17.000000 static_osm_indexer-0.2.1/static_osm_indexer.egg-info/requires.txt
+-rw-r--r--   0 jacopo    (1000) jacopo    (1000)       19 2023-06-21 12:14:17.000000 static_osm_indexer-0.2.1/static_osm_indexer.egg-info/top_level.txt
```

### Comparing `static_osm_indexer-0.2.0/PKG-INFO` & `static_osm_indexer-0.2.1/static_osm_indexer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: static_osm_indexer
-Version: 0.2.0
+Name: static-osm-indexer
+Version: 0.2.1
 Summary: Tool to process OSM files, mainly for static sites
 Author-email: Jacopo Farina <jacopo1.farina@gmail.com>
 Maintainer-email: Jacopo Farina <jacopo1.farina@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jacopofar/static-osm-indexer
 Project-URL: Bug Tracker, https://github.com/jacopofar/static-osm-indexer/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,18 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 # Static OSM indexer
 
+__[Result demo](https://jacopofarina.eu/experiments/italy_static_map/)__
+
+__[Technical article](https://jacopofarina.eu/posts/static-maps-part-3-text-search/)__
+
 __NOTE__ this project is not production ready at all, maybe never will, but may be useful nonetheless.
 
 ![screenshot of a map created with this tool](screenshot.png)
 
 This is a collection of scripts that can process data extracts from OpenStreetMap (PBF files) allowing the creation of __static sites__ (that is, a bunch of file hosted without any backend processing) to do a few useful operations:
 
 * display an interactive map (zoom, pan, scroll) based on vector tiles
```

### Comparing `static_osm_indexer-0.2.0/README.md` & `static_osm_indexer-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Static OSM indexer
 
+__[Result demo](https://jacopofarina.eu/experiments/italy_static_map/)__
+
+__[Technical article](https://jacopofarina.eu/posts/static-maps-part-3-text-search/)__
+
 __NOTE__ this project is not production ready at all, maybe never will, but may be useful nonetheless.
 
 ![screenshot of a map created with this tool](screenshot.png)
 
 This is a collection of scripts that can process data extracts from OpenStreetMap (PBF files) allowing the creation of __static sites__ (that is, a bunch of file hosted without any backend processing) to do a few useful operations:
 
 * display an interactive map (zoom, pan, scroll) based on vector tiles
```

### Comparing `static_osm_indexer-0.2.0/pyproject.toml` & `static_osm_indexer-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: GIS",
 ]
-version = "0.2.0"
+version = "0.2.1"
 
 
 [project.urls]
 "Homepage" = "https://github.com/jacopofar/static-osm-indexer"
 "Bug Tracker" = "https://github.com/jacopofar/static-osm-indexer/issues"
 
 [project.scripts]
```

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/extract_road_network.py` & `static_osm_indexer-0.2.1/static_osm_indexer/extract_road_network.py`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/generate_full_map.py` & `static_osm_indexer-0.2.1/static_osm_indexer/generate_full_map.py`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/generate_mbtiles.py` & `static_osm_indexer-0.2.1/static_osm_indexer/generate_mbtiles.py`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/index_locations_names.py` & `static_osm_indexer-0.2.1/static_osm_indexer/index_locations_names.py`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/list_named_locations.py` & `static_osm_indexer-0.2.1/static_osm_indexer/list_named_locations.py`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/road_network_to_geojson.py` & `static_osm_indexer-0.2.1/static_osm_indexer/road_network_to_geojson.py`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/static_assets/index.html` & `static_osm_indexer-0.2.1/static_osm_indexer/static_assets/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 <!DOCTYPE html>
 <html>
 
 <head>
     <meta charset="utf-8" />
     <title>Demo for vector</title>
     <meta name="viewport" content="initial-scale=1,maximum-scale=1,user-scalable=no" />
-    <script src="https://unpkg.com/maplibre-gl@2.1.9/dist/maplibre-gl.js"></script>
-    <link href="https://unpkg.com/maplibre-gl@2.1.9/dist/maplibre-gl.css" rel="stylesheet" />
+    <!-- Maplibre 3.1.0, incorporated in the repo -->
+    <script src="maplibre-gl.js"></script>
+    <link href="maplibre-gl.css" rel="stylesheet" />
     <style>
         body {
             margin: 0;
             padding: 0;
         }
 
         #app-flex-container {
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
 
+
 ****** Static map demo ******
 [                    ]
```

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/static_assets/osm_liberty.json` & `static_osm_indexer-0.2.1/static_osm_indexer/static_assets/osm_liberty.json`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/static_assets/text_search.bundle.js` & `static_osm_indexer-0.2.1/static_osm_indexer/static_assets/text_search.bundle.js`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer/static_assets/tilemaker_config.json` & `static_osm_indexer-0.2.1/static_osm_indexer/static_assets/tilemaker_config.json`

 * *Files identical despite different names*

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer.egg-info/PKG-INFO` & `static_osm_indexer-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: static-osm-indexer
-Version: 0.2.0
+Name: static_osm_indexer
+Version: 0.2.1
 Summary: Tool to process OSM files, mainly for static sites
 Author-email: Jacopo Farina <jacopo1.farina@gmail.com>
 Maintainer-email: Jacopo Farina <jacopo1.farina@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jacopofar/static-osm-indexer
 Project-URL: Bug Tracker, https://github.com/jacopofar/static-osm-indexer/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,18 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 # Static OSM indexer
 
+__[Result demo](https://jacopofarina.eu/experiments/italy_static_map/)__
+
+__[Technical article](https://jacopofarina.eu/posts/static-maps-part-3-text-search/)__
+
 __NOTE__ this project is not production ready at all, maybe never will, but may be useful nonetheless.
 
 ![screenshot of a map created with this tool](screenshot.png)
 
 This is a collection of scripts that can process data extracts from OpenStreetMap (PBF files) allowing the creation of __static sites__ (that is, a bunch of file hosted without any backend processing) to do a few useful operations:
 
 * display an interactive map (zoom, pan, scroll) based on vector tiles
```

### Comparing `static_osm_indexer-0.2.0/static_osm_indexer.egg-info/SOURCES.txt` & `static_osm_indexer-0.2.1/static_osm_indexer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,10 +10,12 @@
 static_osm_indexer.egg-info/PKG-INFO
 static_osm_indexer.egg-info/SOURCES.txt
 static_osm_indexer.egg-info/dependency_links.txt
 static_osm_indexer.egg-info/entry_points.txt
 static_osm_indexer.egg-info/requires.txt
 static_osm_indexer.egg-info/top_level.txt
 static_osm_indexer/static_assets/index.html
+static_osm_indexer/static_assets/maplibre-gl.css
+static_osm_indexer/static_assets/maplibre-gl.js
 static_osm_indexer/static_assets/osm_liberty.json
 static_osm_indexer/static_assets/text_search.bundle.js
 static_osm_indexer/static_assets/tilemaker_config.json
```

