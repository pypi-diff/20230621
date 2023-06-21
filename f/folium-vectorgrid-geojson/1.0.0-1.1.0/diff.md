# Comparing `tmp/folium_vectorgrid_geojson-1.0.0.tar.gz` & `tmp/folium_vectorgrid_geojson-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folium_vectorgrid_geojson-1.0.0.tar", max compression
+gzip compressed data, was "folium_vectorgrid_geojson-1.1.0.tar", max compression
```

## Comparing `folium_vectorgrid_geojson-1.0.0.tar` & `folium_vectorgrid_geojson-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1060 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.0.0/LICENSE
--rw-r--r--   0        0        0      116 2023-06-20 16:54:57.280806 folium_vectorgrid_geojson-1.0.0/folium_vectorgrid_geojson/__init__.py
--rw-r--r--   0        0        0     4337 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.0.0/folium_vectorgrid_geojson/vectorgrid.py
--rw-r--r--   0        0        0     4360 2023-06-20 13:06:27.363853 folium_vectorgrid_geojson-1.0.0/folium_vectorgrid_geojson/vectorgrid_geojson.py
--rw-r--r--   0        0        0     2027 2023-06-20 16:54:40.512812 folium_vectorgrid_geojson-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3699 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.0.0/readme.md
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 folium_vectorgrid_geojson-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.0/LICENSE
+-rw-r--r--   0        0        0      146 2023-06-21 14:54:04.178169 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/__init__.py
+-rw-r--r--   0        0        0     3936 2023-06-21 14:47:04.377711 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/heat_map.py
+-rw-r--r--   0        0        0     5596 2023-06-21 14:38:37.225122 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/template/leaflet_heat.min.js
+-rw-r--r--   0        0        0     4337 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid.py
+-rw-r--r--   0        0        0     4360 2023-06-20 13:06:27.363853 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid_geojson.py
+-rw-r--r--   0        0        0     2027 2023-06-21 14:53:49.186153 folium_vectorgrid_geojson-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3699 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.0/readme.md
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 folium_vectorgrid_geojson-1.1.0/PKG-INFO
```

### Comparing `folium_vectorgrid_geojson-1.0.0/LICENSE` & `folium_vectorgrid_geojson-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.0.0/folium_vectorgrid_geojson/vectorgrid.py` & `folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid.py`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.0.0/folium_vectorgrid_geojson/vectorgrid_geojson.py` & `folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid_geojson.py`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.0.0/pyproject.toml` & `folium_vectorgrid_geojson-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "folium-vectorgrid-geojson"
 #name = "folium-vectorgrid"
-version = "1.0.0"
+version = "1.1.0"
 description = "VectorGrid plugin for folium"
 repository = "https://github.com/zarandras/folium-vectorgrid"
 authors = ["Lukács Gábor <lukacs.hod@gmail.com>", "Molnár András <molnar.andras.jozsef@gmail.com>", "Benjamin Ramser <ahoi@ipwnd.pw>"]
 license = "MIT"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
```

### Comparing `folium_vectorgrid_geojson-1.0.0/readme.md` & `folium_vectorgrid_geojson-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.0.0/PKG-INFO` & `folium_vectorgrid_geojson-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folium-vectorgrid-geojson
-Version: 1.0.0
+Version: 1.1.0
 Summary: VectorGrid plugin for folium
 Home-page: https://github.com/zarandras/folium-vectorgrid
 License: MIT
 Author: Lukács Gábor
 Author-email: lukacs.hod@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: folium-vectorgrid-geojson Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: folium-vectorgrid-geojson Version: 1.1.0 Summary:
 VectorGrid plugin for folium Home-page: https://github.com/zarandras/folium-
 vectorgrid License: MIT Author: LukÃ¡cs GÃ¡bor Author-email:
 lukacs.hod@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: folium (>=0.14.0,<0.15.0) Project-URL: Repository, https://
```

