# Comparing `tmp/stackstac-0.4.3.tar.gz` & `tmp/stackstac-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackstac-0.4.3.tar", last modified: Wed Sep 14 17:47:42 2022, max compression
+gzip compressed data, was "stackstac-0.4.4.tar", last modified: Wed Jun 21 19:16:48 2023, max compression
```

## Comparing `stackstac-0.4.3.tar` & `stackstac-0.4.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0 gabe       (501) staff       (20)     1068 2021-03-10 03:30:35.531271 stackstac-0.4.3/LICENSE
--rw-r--r--   0 gabe       (501) staff       (20)     6966 2022-09-07 05:41:54.766458 stackstac-0.4.3/README.md
--rw-r--r--   0 gabe       (501) staff       (20)     1958 2022-09-14 17:47:04.507144 stackstac-0.4.3/pyproject.toml
--rw-r--r--   0 gabe       (501) staff       (20)     1366 2022-09-07 17:17:15.667142 stackstac-0.4.3/stackstac/__init__.py
--rw-r--r--   0 gabe       (501) staff       (20)     6439 2021-12-01 04:34:55.343474 stackstac-0.4.3/stackstac/accumulate_metadata.py
--rw-r--r--   0 gabe       (501) staff       (20)    13359 2022-09-14 17:19:20.647258 stackstac-0.4.3/stackstac/geom_utils.py
--rw-r--r--   0 gabe       (501) staff       (20)     1654 2022-07-28 16:28:01.972749 stackstac-0.4.3/stackstac/nodata_reader.py
--rw-r--r--   0 gabe       (501) staff       (20)     7012 2022-07-28 16:28:01.973793 stackstac-0.4.3/stackstac/ops.py
--rw-r--r--   0 gabe       (501) staff       (20)    23118 2022-09-14 17:19:20.647656 stackstac-0.4.3/stackstac/prepare.py
--rw-r--r--   0 gabe       (501) staff       (20)     1864 2022-01-12 06:02:04.816902 stackstac-0.4.3/stackstac/raster_spec.py
--rw-r--r--   0 gabe       (501) staff       (20)     4010 2022-07-28 16:28:01.975713 stackstac-0.4.3/stackstac/reader_protocol.py
--rw-r--r--   0 gabe       (501) staff       (20)     3664 2021-04-16 21:46:02.542883 stackstac-0.4.3/stackstac/rio_env.py
--rw-r--r--   0 gabe       (501) staff       (20)    17126 2022-09-07 00:23:58.349402 stackstac-0.4.3/stackstac/rio_reader.py
--rw-r--r--   0 gabe       (501) staff       (20)    35622 2022-09-07 00:23:58.349816 stackstac-0.4.3/stackstac/show.py
--rw-r--r--   0 gabe       (501) staff       (20)     5668 2022-09-07 16:56:01.012846 stackstac-0.4.3/stackstac/stac_types.py
--rw-r--r--   0 gabe       (501) staff       (20)    15458 2022-09-07 16:56:01.013231 stackstac-0.4.3/stackstac/stack.py
--rw-r--r--   0 gabe       (501) staff       (20)        0 2022-02-02 05:43:37.784385 stackstac-0.4.3/stackstac/testing/__init__.py
--rw-r--r--   0 gabe       (501) staff       (20)     2041 2022-07-28 16:28:01.979569 stackstac-0.4.3/stackstac/testing/strategies.py
--rw-r--r--   0 gabe       (501) staff       (20)        0 2022-02-02 05:43:37.785349 stackstac-0.4.3/stackstac/tests/__init__.py
--rw-r--r--   0 gabe       (501) staff       (20)     2851 2022-07-28 16:28:01.980144 stackstac-0.4.3/stackstac/tests/test_mosaic.py
--rw-r--r--   0 gabe       (501) staff       (20)     5773 2022-09-07 16:56:01.013584 stackstac-0.4.3/stackstac/tests/test_stac_types.py
--rw-r--r--   0 gabe       (501) staff       (20)     6705 2022-09-07 00:23:58.350224 stackstac-0.4.3/stackstac/tests/test_to_dask.py
--rw-r--r--   0 gabe       (501) staff       (20)      523 2021-03-10 03:30:35.659899 stackstac-0.4.3/stackstac/timer.py
--rw-r--r--   0 gabe       (501) staff       (20)     8889 2022-09-07 00:23:58.350514 stackstac-0.4.3/stackstac/to_dask.py
--rw-------   0 gabe       (501) staff       (20)     7365 2022-09-14 17:47:42.307315 stackstac-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2021-03-10 03:30:35.531271 stackstac-0.4.4/LICENSE
+-rw-r--r--   0        0        0     6966 2022-09-07 05:41:54.766458 stackstac-0.4.4/README.md
+-rw-r--r--   0        0        0     1899 2023-06-21 19:16:22.764590 stackstac-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1366 2022-09-07 17:17:15.667142 stackstac-0.4.4/stackstac/__init__.py
+-rw-r--r--   0        0        0     6452 2023-06-21 18:53:26.804274 stackstac-0.4.4/stackstac/accumulate_metadata.py
+-rw-r--r--   0        0        0    13359 2022-09-14 20:15:58.212022 stackstac-0.4.4/stackstac/geom_utils.py
+-rw-r--r--   0        0        0     1654 2022-07-28 16:28:01.972749 stackstac-0.4.4/stackstac/nodata_reader.py
+-rw-r--r--   0        0        0     7012 2022-07-28 16:28:01.973793 stackstac-0.4.4/stackstac/ops.py
+-rw-r--r--   0        0        0    23345 2023-06-21 01:39:49.253106 stackstac-0.4.4/stackstac/prepare.py
+-rw-r--r--   0        0        0     1864 2022-01-12 06:02:04.816902 stackstac-0.4.4/stackstac/raster_spec.py
+-rw-r--r--   0        0        0     4010 2022-07-28 16:28:01.975713 stackstac-0.4.4/stackstac/reader_protocol.py
+-rw-r--r--   0        0        0     3664 2021-04-16 21:46:02.542883 stackstac-0.4.4/stackstac/rio_env.py
+-rw-r--r--   0        0        0    17138 2023-06-21 01:39:49.266322 stackstac-0.4.4/stackstac/rio_reader.py
+-rw-r--r--   0        0        0    35622 2022-09-07 00:23:58.349816 stackstac-0.4.4/stackstac/show.py
+-rw-r--r--   0        0        0     5668 2022-09-07 16:56:01.012846 stackstac-0.4.4/stackstac/stac_types.py
+-rw-r--r--   0        0        0    15458 2022-09-07 16:56:01.013231 stackstac-0.4.4/stackstac/stack.py
+-rw-r--r--   0        0        0        0 2022-02-02 05:43:37.784385 stackstac-0.4.4/stackstac/testing/__init__.py
+-rw-r--r--   0        0        0     2041 2022-07-28 16:28:01.979569 stackstac-0.4.4/stackstac/testing/strategies.py
+-rw-r--r--   0        0        0        0 2022-02-02 05:43:37.785349 stackstac-0.4.4/stackstac/tests/__init__.py
+-rw-r--r--   0        0        0     2851 2022-07-28 16:28:01.980144 stackstac-0.4.4/stackstac/tests/test_mosaic.py
+-rw-r--r--   0        0        0     5773 2022-09-07 16:56:01.013584 stackstac-0.4.4/stackstac/tests/test_stac_types.py
+-rw-r--r--   0        0        0     6705 2022-09-07 00:23:58.350224 stackstac-0.4.4/stackstac/tests/test_to_dask.py
+-rw-r--r--   0        0        0      524 2023-06-21 01:39:49.274722 stackstac-0.4.4/stackstac/timer.py
+-rw-r--r--   0        0        0     8889 2022-11-10 23:58:40.511304 stackstac-0.4.4/stackstac/to_dask.py
+-rw-r--r--   0        0        0     7365 1970-01-01 00:00:00.000000 stackstac-0.4.4/PKG-INFO
```

### Comparing `stackstac-0.4.3/LICENSE` & `stackstac-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/README.md` & `stackstac-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/pyproject.toml` & `stackstac-0.4.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "rasterio<2.0.0,>=1.3.0",
     "xarray>=0.18",
 ]
 description = "Load a STAC collection into xarray with dask"
 name = "stackstac"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
-version = "0.4.3"
+version = "0.4.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://stackstac.readthedocs.io/en/latest/index.html"
 repository = "https://github.com/gjoseph92/stackstac"
@@ -31,17 +31,17 @@
     "scipy<2.0.0,>=1.6.1",
     "ipyleaflet<1.0.0,>=0.13.6",
     "ipywidgets<8.0.0,>=7.6.3",
     "matplotlib>=3.4.1",
 ]
 
 [tool.pdm.dev-dependencies]
-binder = [
+docs-examples = [
     "Bottleneck>=1.3.2",
-    "coiled>=0.2.27",
+    "coiled>=0.2.50",
     "geogif>=0",
     "jupyter-server-proxy>=3.2.0",
     "jupyterlab-geojson>=3.1.2",
     "jupyterlab-system-monitor>=0.8.0",
     "planetary-computer>=0.4.3",
     "pystac-client>=0.3",
     "sat-search>=0.3.0",
@@ -66,19 +66,19 @@
 test = [
     "hypothesis<7.0.0,>=6.35.0",
     "pytest<7.0.0,>=6.2.5",
 ]
 util = [
     "py-spy",
     "pystac>=1",
-    "scheduler-profilers @ git+https://github.com/gjoseph92/scheduler-profilers.git@main",
     "graphviz>=0.16",
     "snakeviz>=2.1.0",
     "sphinx-autobuild>=2021.3.14",
     "twine>=3.4.1",
+    "dask-pyspy>=0.4.0",
 ]
 
 [build-system]
 build-backend = "pdm.pep517.api"
 requires = [
     "pdm-pep517",
 ]
```

### Comparing `stackstac-0.4.3/stackstac/__init__.py` & `stackstac-0.4.4/stackstac/__init__.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/accumulate_metadata.py` & `stackstac-0.4.4/stackstac/accumulate_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         props_arr = np.squeeze(
             np.array(
                 props,
                 # Avoid DeprecationWarning creating ragged arrays when elements are lists/tuples of different lengths
                 dtype="object"
                 if (
                     isinstance(props, _ourlist)
-                    and len(set(len(x) for x in props if isinstance(x, (list, tuple))))
+                    and len(set(len(x) if isinstance(x, (list, tuple)) else type(x) for x in props))
                     > 1
                 )
                 else None,
             )
         )
 
         if (
```

### Comparing `stackstac-0.4.3/stackstac/geom_utils.py` & `stackstac-0.4.4/stackstac/geom_utils.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/nodata_reader.py` & `stackstac-0.4.4/stackstac/nodata_reader.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/ops.py` & `stackstac-0.4.4/stackstac/ops.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/prepare.py` & `stackstac-0.4.4/stackstac/prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Optional,
     Set,
     Union,
     Tuple,
     List,
     Dict,
     Any,
-    cast,
 )
 import warnings
 
 
 import affine
 import numpy as np
 import pandas as pd
@@ -160,15 +159,15 @@
                     raise ValueError(
                         f"Cannot pick a common CRS, since assets have multiple CRSs: asset {id!r} of item "
                         f"{item_i} {item['id']!r} is in EPSG:{asset_epsg}, "
                         f"but assets before it were in EPSG:{out_epsg}.\n\n"
                         "Please specify a CRS with the `epsg=` argument."
                     )
 
-            out_epsg = cast(int, out_epsg)
+            assert isinstance(out_epsg, int), f"`out_epsg` not found. {out_epsg=}"
             # ^ because if it was None initially, and we didn't error out in the above check, it's now always set
 
             if bounds_latlon is not None and out_bounds is None:
                 out_bounds = bounds = geom_utils.reproject_bounds(
                     bounds_latlon, 4326, out_epsg
                 )
                 # NOTE: we wait to reproject until now, so we can use the inferred CRS
@@ -223,40 +222,14 @@
                                 bbox_lonlat, 4326, out_epsg
                             )
                             item_bbox_proj = asset_bbox_proj
                             # ^ so we can reuse for other assets
                     else:
                         asset_bbox_proj = item_bbox_proj
 
-            # Auto-compute bounds
-            if bounds is None:
-                if asset_bbox_proj is None:
-                    raise ValueError(
-                        f"Cannot automatically compute the bounds, "
-                        f"since asset {id!r} on item {item_i} {item['id']!r} "
-                        f"doesn't provide enough metadata to determine its spatial extent.\n"
-                        f"We'd need at least one of (in order of preference):\n"
-                        f"- The `proj:bbox` field set on the asset, or on the item\n"
-                        f"- The `proj:shape` and `proj:transform` fields set on the asset, or on the item\n"
-                        f"- A `bbox` set on the item {item['id']!r}\n\n"
-                        "Please specify the `bounds=` or `bounds_latlon=` argument to set the output bounds manually."
-                    )
-                out_bounds = (
-                    asset_bbox_proj
-                    if out_bounds is None
-                    else geom_utils.union_bounds(asset_bbox_proj, out_bounds)
-                )
-            else:
-                # Drop asset if it doesn't overlap with the output bounds at all
-                if asset_bbox_proj is not None and not geom_utils.bounds_overlap(
-                    asset_bbox_proj, bounds
-                ):
-                    # I've got a blank space in my ndarray, baby / And I'll write your name
-                    continue
-
             # Auto-compute resolutions
             if resolution is None:
                 # Prefer computing resolutions from a geotrans, if it exists
                 if asset_transform is not None and asset_epsg is not None:
                     asset_affine = asset_affine or affine.Affine(*asset_transform[:6])
                     if asset_epsg == out_epsg:
                         # Fastpath-ish when asset is already in the output CRS:
@@ -316,22 +289,50 @@
                     out_resolutions_xy = (
                         # TODO do you always want the smallest resolution?
                         # Maybe support setting for controlling this (min, max, mode, etc)?
                         min(res_x, out_resolutions_xy[0]),
                         min(res_y, out_resolutions_xy[1]),
                     )
 
+            # Auto-compute bounds
+            # We do this last, so that if we have to skip all items (due to non-overlap),
+            # we still get the spatial information needed to construct an array of NaNs.
+            if bounds is None:
+                if asset_bbox_proj is None:
+                    raise ValueError(
+                        f"Cannot automatically compute the bounds, "
+                        f"since asset {id!r} on item {item_i} {item['id']!r} "
+                        f"doesn't provide enough metadata to determine its spatial extent.\n"
+                        f"We'd need at least one of (in order of preference):\n"
+                        f"- The `proj:bbox` field set on the asset, or on the item\n"
+                        f"- The `proj:shape` and `proj:transform` fields set on the asset, or on the item\n"
+                        f"- A `bbox` set on the item {item['id']!r}\n\n"
+                        "Please specify the `bounds=` or `bounds_latlon=` argument to set the output bounds manually."
+                    )
+                out_bounds = (
+                    asset_bbox_proj
+                    if out_bounds is None
+                    else geom_utils.union_bounds(asset_bbox_proj, out_bounds)
+                )
+            else:
+                # Drop asset if it doesn't overlap with the output bounds at all
+                if asset_bbox_proj is not None and not geom_utils.bounds_overlap(
+                    asset_bbox_proj, bounds
+                ):
+                    # I've got a blank space in my ndarray, baby / And I'll write your name
+                    continue
+
             # Phew, we figured out all the spatial stuff! Now actually store the information we care about.
             asset_table[item_i, asset_i] = (asset["href"], asset_bbox_proj)
             # ^ NOTE: If `asset_bbox_proj` is None, NumPy automatically converts it to NaNs
 
     # At this point, everything has been set (or there was as error)
-    out_bounds = cast(Bbox, out_bounds)
-    out_resolutions_xy = cast(Resolutions, out_resolutions_xy)
-    out_epsg = cast(int, out_epsg)
+    assert out_bounds, f"{out_bounds=}"
+    assert out_resolutions_xy is not None, f"{out_resolutions_xy=}"
+    assert out_epsg is not None, f"{out_epsg=}"
 
     if snap_bounds:
         out_bounds = geom_utils.snapped_bounds(out_bounds, out_resolutions_xy)
     spec = RasterSpec(
         epsg=out_epsg,
         bounds=out_bounds,
         resolutions_xy=out_resolutions_xy,
```

### Comparing `stackstac-0.4.3/stackstac/raster_spec.py` & `stackstac-0.4.4/stackstac/raster_spec.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/reader_protocol.py` & `stackstac-0.4.4/stackstac/reader_protocol.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/rio_env.py` & `stackstac-0.4.4/stackstac/rio_env.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/rio_reader.py` & `stackstac-0.4.4/stackstac/rio_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,16 +397,17 @@
                 warnings.warn(msg)
                 return nodata_for_window(window, self.fill_value, self.dtype)
 
             raise RuntimeError(msg) from e
 
         if self.rescale:
             scale, offset = reader.scale_offset
-            if scale != 1 and offset != 0:
+            if scale != 1:
                 result *= scale
+            if offset != 0:
                 result += offset
 
         result = result.astype(self.dtype, copy=False)
         result = np.ma.filled(result, fill_value=self.fill_value)
         return result
 
     def close(self) -> None:
```

### Comparing `stackstac-0.4.3/stackstac/show.py` & `stackstac-0.4.4/stackstac/show.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/stac_types.py` & `stackstac-0.4.4/stackstac/stac_types.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/stack.py` & `stackstac-0.4.4/stackstac/stack.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/testing/strategies.py` & `stackstac-0.4.4/stackstac/testing/strategies.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/tests/test_mosaic.py` & `stackstac-0.4.4/stackstac/tests/test_mosaic.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/tests/test_stac_types.py` & `stackstac-0.4.4/stackstac/tests/test_stac_types.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/tests/test_to_dask.py` & `stackstac-0.4.4/stackstac/tests/test_to_dask.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/stackstac/timer.py` & `stackstac-0.4.4/stackstac/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from timeit import default_timer
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 @contextmanager
-def time(statement: str, level=logging.INFO):
+def time(statement: str, level=logging.DEBUG):
     start = default_timer()
     error = None
     try:
         yield
     except Exception as e:
         error = e
     finally:
```

### Comparing `stackstac-0.4.3/stackstac/to_dask.py` & `stackstac-0.4.4/stackstac/to_dask.py`

 * *Files identical despite different names*

### Comparing `stackstac-0.4.3/PKG-INFO` & `stackstac-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackstac
-Version: 0.4.3
+Version: 0.4.4
 Summary: Load a STAC collection into xarray with dask
 License: MIT
 Author-email: Gabe Joseph <gjoseph92@gmail.com>
 Requires-Python: >=3.8,<4.0
 Provides-Extra: viz
 Project-URL: homepage, https://stackstac.readthedocs.io/en/latest/index.html
 Project-URL: repository, https://github.com/gjoseph92/stackstac
```

