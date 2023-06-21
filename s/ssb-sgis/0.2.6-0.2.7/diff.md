# Comparing `tmp/ssb_sgis-0.2.6.tar.gz` & `tmp/ssb_sgis-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.2.6.tar", max compression
+gzip compressed data, was "ssb_sgis-0.2.7.tar", max compression
```

## Comparing `ssb_sgis-0.2.6.tar` & `ssb_sgis-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1074 2023-06-14 06:46:13.344762 ssb_sgis-0.2.6/LICENSE
--rw-r--r--   0        0        0     7543 2023-06-14 06:46:13.344762 ssb_sgis-0.2.6/README.md
--rw-r--r--   0        0        0     2539 2023-06-14 06:46:34.180997 ssb_sgis-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2334 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-14 06:46:34.180997 ssb_sgis-0.2.6/src/sgis/dapla.py
--rw-r--r--   0        0        0      576 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8080 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    17659 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5870 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    14520 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    11862 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6888 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    20336 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     9722 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/to_geodataframe.py
--rw-r--r--   0        0        0     2674 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    23631 2023-06-14 06:46:34.180997 ssb_sgis-0.2.6/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1923 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20499 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    18490 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/map.py
--rw-r--r--   0        0        0    15961 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6218 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12433 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    12369 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9375 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3359 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    66761 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12643 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6767 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/py.typed
--rw-r--r--   0        0        0     3774 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 06:43:58.051659 ssb_sgis-0.2.7/LICENSE
+-rw-r--r--   0        0        0     7543 2023-06-21 06:43:58.051659 ssb_sgis-0.2.7/README.md
+-rw-r--r--   0        0        0     2539 2023-06-21 06:44:22.819867 ssb_sgis-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2368 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/dapla.py
+-rw-r--r--   0        0        0      576 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8080 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    17659 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5870 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11862 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    22646 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     9887 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     2674 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0     6479 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/examine.py
+-rw-r--r--   0        0        0    23631 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1923 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20499 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    18611 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    15961 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    12369 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9375 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66761 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6767 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/py.typed
+-rw-r--r--   0        0        0     3774 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.7/PKG-INFO
```

### Comparing `ssb_sgis-0.2.6/LICENSE` & `ssb_sgis-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/README.md` & `ssb_sgis-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/pyproject.toml` & `ssb_sgis-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.2.6"
+version = "0.2.7"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.2.6/src/sgis/__init__.py` & `ssb_sgis-0.2.7/src/sgis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     get_overlapping_polygon_indices,
     get_overlapping_polygon_product,
     get_overlapping_polygons,
     get_polygon_clusters,
 )
 from .geopandas_tools.to_geodataframe import to_gdf
 from .helpers import get_name
+from .maps.examine import Examine
 from .maps.explore import Explore
 from .maps.httpserver import run_html_server
 from .maps.legend import Legend
 from .maps.maps import clipmap, explore, qtm, samplemap
 from .maps.thematicmap import ThematicMap
 from .networkanalysis.closing_network_holes import (
     close_network_holes,
```

### Comparing `ssb_sgis-0.2.6/src/sgis/dapla.py` & `ssb_sgis-0.2.7/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/exceptions.py` & `ssb_sgis-0.2.7/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/general.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Functions for polygon geometries."""
+import functools
 import warnings
 
 import geopandas as gpd
 import networkx as nx
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from shapely import (
     area,
+    difference,
     get_exterior_ring,
     get_interior_ring,
     get_num_interior_rings,
     get_parts,
     polygons,
 )
 from shapely.ops import unary_union
@@ -453,154 +455,172 @@
     unique = unique[unique.overlap != unique.index_right]
     series = unique.set_index("index_right").overlap
     series.index.name = None
 
     return series
 
 
-def close_small_holes(
+def close_all_holes(
     gdf: GeoDataFrame | GeoSeries,
-    max_area: int | float,
     *,
+    without_islands: bool = True,
     copy: bool = True,
 ) -> GeoDataFrame | GeoSeries:
-    """Closes holes in polygons if the area is less than the given maximum.
+    """Closes all holes in polygons.
 
     It takes a GeoDataFrame or GeoSeries of polygons and
-    fills the holes that are smaller than the specified area given in units of
-    either square meters ('max_m2') or square kilometers ('max_km2').
+    returns the outer circle.
 
     Args:
         gdf: GeoDataFrame or GeoSeries of polygons.
-        max_area: The maximum area in the unit of the GeoDataFrame's crs.
         copy: if True (default), the input GeoDataFrame or GeoSeries is copied.
             Defaults to True.
 
     Returns:
         A GeoDataFrame or GeoSeries of polygons with closed holes in the geometry
         column.
 
-    Raises:
-        ValueError: If the coordinate reference system of the GeoDataFrame is not in
-            meter units.
-        ValueError: If both 'max_m2' and 'max_km2' is given.
-
     Examples
     --------
-
     Let's create a circle with a hole in it.
 
-    >>> from sgis import close_small_holes, buff, to_gdf
+    >>> from sgis import close_all_holes, buff, to_gdf
     >>> point = to_gdf([260000, 6650000], crs=25833)
     >>> point
                             geometry
     0  POINT (260000.000 6650000.000)
     >>> circle = buff(point, 1000)
     >>> small_circle = buff(point, 500)
     >>> circle_with_hole = circle.overlay(small_circle, how="difference")
     >>> circle_with_hole.area
     0    2.355807e+06
     dtype: float64
 
-    Close holes smaller than 1 square kilometer (1 million square meters).
+    Close the hole.
 
-    >>> holes_closed = close_small_holes(circle_with_hole, max_area=1_000_000)
+    >>> holes_closed = close_all_holes(circle_with_hole)
     >>> holes_closed.area
     0    3.141076e+06
     dtype: float64
-
-    The hole will not be closed if it is larger.
-
-    >>> holes_closed = close_small_holes(circle_with_hole, max_area=1_000)
-    >>> holes_closed.area
-    0    2.355807e+06
-    dtype: float64
     """
-    if copy:
-        gdf = gdf.copy()
-
-    if isinstance(gdf, GeoDataFrame):
-        gdf["geometry"] = gdf.geometry.map(
-            lambda x: _close_small_holes_poly(x, max_area)
+    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
+        raise ValueError(
+            f"'gdf' should be of type GeoDataFrame or GeoSeries. Got {type(gdf)}"
         )
-        return gdf
 
-    elif isinstance(gdf, gpd.GeoSeries):
-        return gdf.map(lambda x: _close_small_holes_poly(x, max_area))
+    if copy:
+        gdf = gdf.copy()
 
+    if without_islands:
+        all_geoms = gdf.unary_union
+        if isinstance(gdf, GeoDataFrame):
+            gdf["geometry"] = gdf.geometry.map(
+                lambda x: _close_all_holes_no_islands(x, all_geoms)
+            )
+            return gdf
+        else:
+            return gdf.map(lambda x: _close_all_holes_no_islands(x, all_geoms))
     else:
-        raise ValueError(
-            f"'gdf' should be of type GeoDataFrame or GeoSeries. Got {type(gdf)}"
-        )
+        if isinstance(gdf, GeoDataFrame):
+            gdf["geometry"] = gdf.geometry.map(_close_all_holes)
+            return gdf
+        else:
+            return gdf.map(_close_all_holes)
 
 
-def close_all_holes(
+def close_small_holes(
     gdf: GeoDataFrame | GeoSeries,
+    max_area: int | float,
     *,
+    without_islands: bool = True,
     copy: bool = True,
 ) -> GeoDataFrame | GeoSeries:
-    """Closes all holes in polygons.
+    """Closes holes in polygons if the area is less than the given maximum.
 
     It takes a GeoDataFrame or GeoSeries of polygons and
-    returns the outer circle.
+    fills the holes that are smaller than the specified area given in units of
+    either square meters ('max_m2') or square kilometers ('max_km2').
 
     Args:
         gdf: GeoDataFrame or GeoSeries of polygons.
+        max_area: The maximum area in the unit of the GeoDataFrame's crs.
         copy: if True (default), the input GeoDataFrame or GeoSeries is copied.
             Defaults to True.
 
     Returns:
         A GeoDataFrame or GeoSeries of polygons with closed holes in the geometry
         column.
 
+    Raises:
+        ValueError: If the coordinate reference system of the GeoDataFrame is not in
+            meter units.
+        ValueError: If both 'max_m2' and 'max_km2' is given.
+
     Examples
     --------
+
     Let's create a circle with a hole in it.
 
-    >>> from sgis import close_all_holes, buff, to_gdf
+    >>> from sgis import close_small_holes, buff, to_gdf
     >>> point = to_gdf([260000, 6650000], crs=25833)
     >>> point
                             geometry
     0  POINT (260000.000 6650000.000)
     >>> circle = buff(point, 1000)
     >>> small_circle = buff(point, 500)
     >>> circle_with_hole = circle.overlay(small_circle, how="difference")
     >>> circle_with_hole.area
     0    2.355807e+06
     dtype: float64
 
-    Close the hole.
+    Close holes smaller than 1 square kilometer (1 million square meters).
 
-    >>> holes_closed = close_all_holes(circle_with_hole)
+    >>> holes_closed = close_small_holes(circle_with_hole, max_area=1_000_000)
     >>> holes_closed.area
     0    3.141076e+06
     dtype: float64
-    """
-    if copy:
-        gdf = gdf.copy()
 
-    def close_all_holes_func(poly):
-        return unary_union(polygons(get_exterior_ring(get_parts(poly))))
+    The hole will not be closed if it is larger.
 
-    close_all_holes_func = np.vectorize(close_all_holes_func)
+    >>> holes_closed = close_small_holes(circle_with_hole, max_area=1_000)
+    >>> holes_closed.area
+    0    2.355807e+06
+    dtype: float64
+    """
+    if not isinstance(gdf, (GeoSeries, GeoDataFrame)):
+        raise ValueError(
+            f"'gdf' should be of type GeoDataFrame or GeoSeries. Got {type(gdf)}"
+        )
 
-    if isinstance(gdf, GeoDataFrame):
-        gdf["geometry"] = close_all_holes_func(gdf.geometry)
-        return gdf
+    if copy:
+        gdf = gdf.copy()
 
-    elif isinstance(gdf, gpd.GeoSeries):
-        return close_all_holes_func(gdf)
+    if without_islands:
+        all_geoms = gdf.unary_union
 
+        if isinstance(gdf, GeoDataFrame):
+            gdf["geometry"] = gdf.geometry.map(
+                lambda x: _close_small_holes_no_islands(x, max_area, all_geoms)
+            )
+            return gdf
+        else:
+            return gdf.map(
+                lambda x: _close_small_holes_no_islands(x, max_area, all_geoms)
+            )
     else:
-        raise ValueError(
-            f"'gdf' should be of type GeoDataFrame or GeoSeries. Got {type(gdf)}"
-        )
+        if isinstance(gdf, GeoDataFrame):
+            gdf["geometry"] = gdf.geometry.map(
+                lambda x: _close_small_holes(x, max_area)
+            )
+            return gdf
+        else:
+            return gdf.map(lambda x: _close_small_holes(x, max_area))
 
 
-def _close_small_holes_poly(poly, max_area):
+def _close_small_holes(poly, max_area):
     """Closes cmall holes within one shapely geometry of polygons."""
 
     # start with a list containing the polygon,
     # then append all holes smaller than 'max_km2' to the list.
     holes_closed = [poly]
     singlepart = get_parts(poly)
     for part in singlepart:
@@ -608,11 +628,60 @@
 
         if not (n_interior_rings):
             continue
 
         for n in range(n_interior_rings):
             hole = polygons(get_interior_ring(part, n))
 
+            print(area(hole))
+
             if area(hole) < max_area:
                 holes_closed.append(hole)
 
     return unary_union(holes_closed)
+
+
+def _close_small_holes_no_islands(poly, max_area, all_geoms):
+    """Closes small holes within one shapely geometry of polygons."""
+
+    # start with a list containing the polygon,
+    # then append all holes smaller than 'max_km2' to the list.
+    holes_closed = [poly]
+    singlepart = get_parts(poly)
+    for part in singlepart:
+        n_interior_rings = get_num_interior_rings(part)
+
+        if not (n_interior_rings):
+            continue
+
+        for n in range(n_interior_rings):
+            hole = polygons(get_interior_ring(part, n))
+            no_islands = unary_union(hole.difference(all_geoms))
+            if area(no_islands) < max_area:
+                holes_closed.append(no_islands)
+
+    return unary_union(holes_closed)
+
+
+def _close_all_holes(poly):
+    return unary_union(polygons(get_exterior_ring(get_parts(poly))))
+
+
+def _close_all_holes_no_islands(poly, all_geoms):
+    """Closes all holes within one shapely geometry of polygons."""
+
+    # start with a list containing the polygon,
+    # then append all holes smaller than 'max_km2' to the list.
+    holes_closed = [poly]
+    singlepart = get_parts(poly)
+    for part in singlepart:
+        n_interior_rings = get_num_interior_rings(part)
+
+        if not (n_interior_rings):
+            continue
+
+        for n in range(n_interior_rings):
+            hole = polygons(get_interior_ring(part, n))
+            no_islands = unary_union(hole.difference(all_geoms))
+            holes_closed.append(no_islands)
+
+    return unary_union(holes_closed)
```

### Comparing `ssb_sgis-0.2.6/src/sgis/geopandas_tools/to_geodataframe.py` & `ssb_sgis-0.2.7/src/sgis/geopandas_tools/to_geodataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numbers
 from collections.abc import Iterator, Sized
 
 import geopandas as gpd
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from pandas.api.types import is_array_like, is_dict_like, is_list_like
-from shapely import Geometry, wkb, wkt
+from shapely import Geometry, box, wkb, wkt
 from shapely.geometry import Point
 from shapely.ops import unary_union
 
 
 def to_gdf(
     geom: Geometry
     | str
@@ -164,14 +164,16 @@
 
     if len(geom.keys()) == 1:
         key = list(geom.keys())[0]
         if isinstance(geom, dict):
             geoseries = GeoSeries(
                 _make_shapely_geoms(list(geom.values())[0]), index=index
             )
+        elif isinstance(geom, pd.Series):
+            geoseries = GeoSeries(_make_shapely_geoms(geom), index=index)
         else:
             geoseries = GeoSeries(_make_shapely_geoms(geom.iloc[:, 0]), index=index)
         return GeoDataFrame({key: geoseries}, geometry=key, crs=crs, **kwargs)
 
     if geometry and geom_col not in geom or isinstance(geom, pd.DataFrame):
         raise ValueError("Cannot find geometry column(s)", geometry)
 
@@ -288,13 +290,15 @@
             except Exception:
                 pass
         return unary_union([_make_one_shapely_geom(g) for g in geom])
 
     elif len(geom) == 2 or len(geom) == 3:
         return Point(geom)
 
+    elif len(geom) == 4:
+        return box(*geom)
     else:
         raise ValueError(
             "If 'geom' is an iterable, each item should consist of "
-            "wkt, wkb or 2/3 coordinates (x, y, z). Got ",
+            "wkt, wkb or (x, y (z) or bbox). Got ",
             geom,
         )
```

### Comparing `ssb_sgis-0.2.6/src/sgis/helpers.py` & `ssb_sgis-0.2.7/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/maps/explore.py` & `ssb_sgis-0.2.7/src/sgis/maps/explore.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/maps/httpserver.py` & `ssb_sgis-0.2.7/src/sgis/maps/httpserver.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/maps/legend.py` & `ssb_sgis-0.2.7/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/maps/map.py` & `ssb_sgis-0.2.7/src/sgis/maps/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,14 +463,16 @@
         else:
             if len(bins) == self._k + 1:
                 bins = bins[1:]
 
             if gdf[self._column].isna().all():
                 return np.repeat(len(bins), len(gdf))
 
+            # need numpy.nan instead of pd.NA as of now
+            gdf[self._column] = gdf[self._column].fillna(np.nan)
             classified = np.searchsorted(bins, gdf[self._column])
 
         return classified
 
     def _push_classification(self, classified: np.ndarray) -> np.ndarray:
         """Push classes downwards if gaps in classification sequence.
```

### Comparing `ssb_sgis-0.2.6/src/sgis/maps/maps.py` & `ssb_sgis-0.2.7/src/sgis/maps/maps.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.2.7/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/cutting_lines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.2.7/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/src/sgis/read_parquet.py` & `ssb_sgis-0.2.7/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.6/PKG-INFO` & `ssb_sgis-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.2.6
+Version: 0.2.7
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
```

