# Comparing `tmp/xpublish_wms-0.2.0.tar.gz` & `tmp/xpublish_wms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish_wms-0.2.0.tar", last modified: Mon Jun 19 18:08:55 2023, max compression
+gzip compressed data, was "xpublish_wms-0.2.1.tar", last modified: Wed Jun 21 16:31:46 2023, max compression
```

## Comparing `xpublish_wms-0.2.0.tar` & `xpublish_wms-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.702201 xpublish_wms-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.706200 xpublish_wms-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/xpublish_wms/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 18:08:55.000000 xpublish_wms-0.2.0/xpublish_wms/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/xpublish_wms/wms/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_feature_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_legend_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/xpublish_wms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-19 18:08:55.000000 xpublish_wms-0.2.0/xpublish_wms.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:46.799275 xpublish_wms-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:46.795275 xpublish_wms-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:46.795275 xpublish_wms-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-21 16:31:46.799275 xpublish_wms-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-21 16:31:46.799275 xpublish_wms-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:46.799275 xpublish_wms-0.2.1/xpublish_wms/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 16:31:46.000000 xpublish_wms-0.2.1/xpublish_wms/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:46.799275 xpublish_wms-0.2.1/xpublish_wms/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/wms/get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/wms/get_feature_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/wms/get_legend_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/wms/get_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-21 16:31:20.000000 xpublish_wms-0.2.1/xpublish_wms/wms/get_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:46.799275 xpublish_wms-0.2.1/xpublish_wms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-21 16:31:46.000000 xpublish_wms-0.2.1/xpublish_wms.egg-info/SOURCES.txt
```

### Comparing `xpublish_wms-0.2.0/.github/workflows/publish-to-pypi.yml` & `xpublish_wms-0.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/.github/workflows/tests.yml` & `xpublish_wms-0.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/.pre-commit-config.yaml` & `xpublish_wms-0.2.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.5
   hooks:
     - id: codespell
       args:
         - --quiet-level=2
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.6.0
+  rev: v3.7.0
   hooks:
     - id: pyupgrade
       args:
         - --py36-plus
 
 - repo: https://github.com/asottile/add-trailing-comma
   rev: v2.5.1
```

### Comparing `xpublish_wms-0.2.0/LICENSE.txt` & `xpublish_wms-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/PKG-INFO` & `xpublish_wms-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpublish_wms
-Version: 0.2.0
+Version: 0.2.1
 Summary: WMS plugin for xpublish
 Author-email: Matthew Iannucci <matt.iannucci@rpsgroup.com>
 License: Copyright 2017 AUTHOR NAME
         
         
         Redistribution and use in source and binary forms,
         with or without modification,
```

### Comparing `xpublish_wms-0.2.0/README.md` & `xpublish_wms-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/pyproject.toml` & `xpublish_wms-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/xpublish_wms/grid.py` & `xpublish_wms-0.2.1/xpublish_wms/grid.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/xpublish_wms/plugin.py` & `xpublish_wms-0.2.1/xpublish_wms/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import cachey
 import xarray as xr
 from fastapi import APIRouter, Depends, Request
 from xpublish import Dependencies, Plugin, hookimpl
 
 from .wms import wms_handler
 
-logger = logging.getLogger("cf_wms")
+logger = logging.getLogger("uvicorn")
 
 
 class CfWmsPlugin(Plugin):
     """
     OGC WMS plugin for xpublish
     """
```

### Comparing `xpublish_wms-0.2.0/xpublish_wms/utils.py` & `xpublish_wms-0.2.1/xpublish_wms/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import contextlib
 import logging
 from typing import Tuple, Union
 
+import matplotlib
+import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
 from pyproj import Transformer
 
 from xpublish_wms.grid import GridType
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("uvicorn")
+matplotlib.use("Agg")
 
 
 def lower_case_keys(d: dict) -> dict:
     return {k.lower(): v for k, v in d.items()}
 
 
 def format_timestamp(value):
@@ -99,7 +103,14 @@
             ds[lng_coord].min().values.item(),
             ds[lat_coord].min().values.item(),
             ds[lng_coord].max().values.item(),
             ds[lat_coord].max().values.item(),
         ]
 
     return bbox
+
+
+@contextlib.contextmanager
+def figure_context(*args, **kwargs):
+    fig = plt.figure(*args, **kwargs)
+    yield fig
+    plt.close(fig)
```

### Comparing `xpublish_wms-0.2.0/xpublish_wms/wms/__init__.py` & `xpublish_wms-0.2.1/xpublish_wms/wms/__init__.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/xpublish_wms/wms/get_capabilities.py` & `xpublish_wms-0.2.1/xpublish_wms/wms/get_capabilities.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/xpublish_wms/wms/get_feature_info.py` & `xpublish_wms-0.2.1/xpublish_wms/wms/get_feature_info.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/xpublish_wms/wms/get_legend_info.py` & `xpublish_wms-0.2.1/xpublish_wms/wms/get_legend_info.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/xpublish_wms/wms/get_map.py` & `xpublish_wms-0.2.1/xpublish_wms/wms/get_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 import logging
 from datetime import datetime
 from typing import List, Union
 
 import cachey
 import cartopy.crs as ccrs
 import cf_xarray  # noqa
+import matplotlib
+import matplotlib.cm as cm
 import matplotlib.tri as tri
 import numpy as np
 import pandas as pd
 import xarray as xr
 from fastapi.responses import StreamingResponse
-from matplotlib import cm
-from matplotlib.figure import Figure
 from PIL import Image
 from rasterio.enums import Resampling
 from rasterio.transform import from_bounds
 
 from xpublish_wms.grid import GridType
-from xpublish_wms.utils import to_lnglat
+from xpublish_wms.utils import figure_context, to_lnglat
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("uvicorn")
+matplotlib.use("Agg")
 
 
 class GetMap:
     """
     TODO - Add docstring
     """
 
@@ -364,67 +365,68 @@
             & (y <= (bbox[3] + 0.18)),
         )
         x_sel = x[inds]
         y_sel = y[inds]
         data_sel = data[inds]
         if minmax_only:
             return {
-                "min": float(data_sel.min()),
-                "max": float(data_sel.max()),
+                "min": float(np.nanmin(data_sel)),
+                "max": float(np.nanmax(data_sel)),
             }
 
         tris = tri.Triangulation(x_sel, y_sel)
         data_tris = data_sel[tris.triangles]
         mask = np.where(np.isnan(data_tris), [True], [False])
         triangle_mask = np.any(mask, axis=1)
         tris.set_mask(triangle_mask)
 
         projection = ccrs.Mercator() if self.crs == "EPSG:3857" else ccrs.PlateCarree()
 
         dpi = 80
-        fig = Figure(dpi=dpi, facecolor="none", edgecolor="none")
-        fig.set_alpha(0)
-        fig.set_figheight(self.height / dpi)
-        fig.set_figwidth(self.width / dpi)
-        ax = fig.add_axes(
-            [0.0, 0.0, 1.0, 1.0],
-            xticks=[],
-            yticks=[],
-            projection=projection,
-        )
-        ax.set_axis_off()
-        ax.set_frame_on(False)
-        ax.set_clip_on(False)
-        ax.set_position([0, 0, 1, 1])
-
-        if not self.autoscale:
-            vmin, vmax = self.colorscalerange
-        else:
-            vmin, vmax = [None, None]
-
-        try:
-            # ax.tripcolor(tris, data_sel, transform=ccrs.PlateCarree(), cmap=cmap, shading='flat', vmin=vmin, vmax=vmax)
-            ax.tricontourf(
-                tris,
-                data_sel,
-                transform=ccrs.PlateCarree(),
-                cmap=self.palettename,
-                vmin=vmin,
-                vmax=vmax,
-                levels=80,
+        with figure_context(dpi=dpi, facecolor="none", edgecolor="none") as fig:
+            fig.set_alpha(0)
+            fig.set_figheight(self.height / dpi)
+            fig.set_figwidth(self.width / dpi)
+            ax = fig.add_axes(
+                [0.0, 0.0, 1.0, 1.0],
+                xticks=[],
+                yticks=[],
+                projection=projection,
             )
-            # ax.pcolormesh(x, y, data, transform=ccrs.PlateCarree(), cmap=cmap, vmin=vmin, vmax=vmax)
-        except Exception as e:
-            print(e)
-            print(bbox)
-
-        ax.set_extent(bbox, crs=ccrs.PlateCarree())
-        ax.axis("off")
-
-        fig.savefig(
-            buffer,
-            format="png",
-            transparent=True,
-            pad_inches=0,
-            bbox_inches="tight",
-        )
+            ax.set_axis_off()
+            ax.set_frame_on(False)
+            ax.set_clip_on(False)
+            ax.set_position([0, 0, 1, 1])
+
+            if not self.autoscale:
+                vmin, vmax = self.colorscalerange
+            else:
+                vmin, vmax = [None, None]
+
+            try:
+                # ax.tripcolor(tris, data_sel, transform=ccrs.PlateCarree(), cmap=cmap, shading='flat', vmin=vmin, vmax=vmax)
+                ax.tricontourf(
+                    tris,
+                    data_sel,
+                    transform=ccrs.PlateCarree(),
+                    cmap=self.palettename,
+                    vmin=vmin,
+                    vmax=vmax,
+                    levels=80,
+                )
+                # ax.pcolormesh(x, y, data, transform=ccrs.PlateCarree(), cmap=cmap, vmin=vmin, vmax=vmax)
+            except Exception as e:
+                print(e)
+                print(bbox)
+
+            ax.set_extent(bbox, crs=ccrs.PlateCarree())
+            ax.axis("off")
+
+            fig.savefig(
+                buffer,
+                format="png",
+                transparent=True,
+                pad_inches=0,
+                bbox_inches="tight",
+            )
+
         return True
```

### Comparing `xpublish_wms-0.2.0/xpublish_wms/wms/get_metadata.py` & `xpublish_wms-0.2.1/xpublish_wms/wms/get_metadata.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.2.0/xpublish_wms.egg-info/SOURCES.txt` & `xpublish_wms-0.2.1/xpublish_wms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

