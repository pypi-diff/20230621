# Comparing `tmp/lapixdl-0.9.0.tar.gz` & `tmp/lapixdl-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapixdl-0.9.0.tar", last modified: Mon Sep  5 16:37:03 2022, max compression
+gzip compressed data, was "lapixdl-0.9.1.tar", last modified: Wed Oct 26 13:39:05 2022, max compression
```

## Comparing `lapixdl-0.9.0.tar` & `lapixdl-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:37:03.672202 lapixdl-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-09-05 16:36:54.000000 lapixdl-0.9.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     4485 2022-09-05 16:37:03.672202 lapixdl-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-09-05 16:36:54.000000 lapixdl-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:37:03.668202 lapixdl-0.9.0/lapixdl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    12956 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:37:03.668202 lapixdl-0.9.0/lapixdl/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (121)    25382 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/evaluation/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/evaluation/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7670 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/evaluation/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:37:03.668202 lapixdl-0.9.0/lapixdl/formats/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/formats/annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/formats/labelbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-09-05 16:36:54.000000 lapixdl-0.9.0/lapixdl/formats/lapix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:37:03.668202 lapixdl-0.9.0/lapixdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4485 2022-09-05 16:37:03.000000 lapixdl-0.9.0/lapixdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-09-05 16:37:03.000000 lapixdl-0.9.0/lapixdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 16:37:03.000000 lapixdl-0.9.0/lapixdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-05 16:37:03.000000 lapixdl-0.9.0/lapixdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-05 16:37:03.000000 lapixdl-0.9.0/lapixdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-05 16:37:03.672202 lapixdl-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-05 16:36:54.000000 lapixdl-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:39:05.440279 lapixdl-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-26 13:38:56.000000 lapixdl-0.9.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-10-26 13:39:05.440279 lapixdl-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-10-26 13:38:56.000000 lapixdl-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:39:05.440279 lapixdl-0.9.1/lapixdl/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:39:05.440279 lapixdl-0.9.1/lapixdl/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/commands/converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17887 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:39:05.440279 lapixdl-0.9.1/lapixdl/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25382 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/evaluation/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/evaluation/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7670 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/evaluation/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:39:05.440279 lapixdl-0.9.1/lapixdl/formats/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7364 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/formats/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/formats/labelbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/formats/lapix.py
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-10-26 13:38:56.000000 lapixdl-0.9.1/lapixdl/formats/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:39:05.440279 lapixdl-0.9.1/lapixdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-10-26 13:39:05.000000 lapixdl-0.9.1/lapixdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-26 13:39:05.000000 lapixdl-0.9.1/lapixdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 13:39:05.000000 lapixdl-0.9.1/lapixdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-26 13:39:05.000000 lapixdl-0.9.1/lapixdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-26 13:39:05.000000 lapixdl-0.9.1/lapixdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-26 13:39:05.000000 lapixdl-0.9.1/lapixdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-26 13:39:05.440279 lapixdl-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-26 13:38:56.000000 lapixdl-0.9.1/setup.py
```

### Comparing `lapixdl-0.9.0/LICENCE` & `lapixdl-0.9.1/LICENCE`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/PKG-INFO` & `lapixdl-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapixdl
-Version: 0.9.0
+Version: 0.9.1
 Summary: Utils for Computer Vision Deep Learning research
 Home-page: https://github.com/lapix-ufsc/lapixdl
 Author: LAPiX
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -111,27 +111,27 @@
 #### Example of conversion from **Labelbox** to **COCO** labels format:
 
 ```python
 import json
 
 from lapixdl.formats import labelbox_to_coco
 
-# convert it to a intermediary format
+# A map categories between labelbox schematic id and category ID
 map_categories = {
   '<schematic id from labelbox>': 1 # category id
 }
 
-# convert it
+# The categories section in the COCO format
 categories_coco = [{
   'supercategory': None,
   'name': 'example_category',
   'id': 1
 }]
 
-# create the full COCO OD file
+# Convert it and create the COCO OD data
 coco_dict = labelbox_to_coco(
   'labelbox_export_file.json',
   map_categories,
   categories_coco,
   target = 'object detection',
   image_shape = (1200, 1600)
 )
```

### Comparing `lapixdl-0.9.0/README.md` & `lapixdl-0.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -96,27 +96,27 @@
 #### Example of conversion from **Labelbox** to **COCO** labels format:
 
 ```python
 import json
 
 from lapixdl.formats import labelbox_to_coco
 
-# convert it to a intermediary format
+# A map categories between labelbox schematic id and category ID
 map_categories = {
   '<schematic id from labelbox>': 1 # category id
 }
 
-# convert it
+# The categories section in the COCO format
 categories_coco = [{
   'supercategory': None,
   'name': 'example_category',
   'id': 1
 }]
 
-# create the full COCO OD file
+# Convert it and create the COCO OD data
 coco_dict = labelbox_to_coco(
   'labelbox_export_file.json',
   map_categories,
   categories_coco,
   target = 'object detection',
   image_shape = (1200, 1600)
 )
```

### Comparing `lapixdl-0.9.0/lapixdl/base.py` & `lapixdl-0.9.1/lapixdl/base.py`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/lapixdl/convert.py` & `lapixdl-0.9.1/lapixdl/convert.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from __future__ import annotations
 
 import multiprocessing
+import os
+import sys
+from collections import defaultdict
 from itertools import chain
 from typing import Any
+from typing import Iterator
 
 import numpy as np
 import pandas as pd
+from PIL import Image
+from PIL import ImageDraw
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 
 from lapixdl.base import basename
+from lapixdl.formats.annotation import Annotation
 from lapixdl.formats.lapix import LapixDataFrame
+from lapixdl.formats.mask import Mask
 
 
 # -----------------------------------------------------------------------
 # Functions to work with data from LabelBox (lbox)
 def lbox_geo_to_shapely(object: dict[str, Any]) -> Polygon | Point | np.nan:
     """Convert the labelbox geometries into shapely geometries
     (For polygons or Points)
@@ -297,14 +305,162 @@
         'info': info_coco if isinstance(info_coco, dict) else {}
     }
 
     return coco_od
 
 
 # -----------------------------------------------------------------------
+# Functions to work with lapix DataFrame
+def lapix_to_annotations(lapix_df: LapixDataFrame) -> list[Annotation]:
+    return [
+        Annotation(
+            row['geometry'],
+            row['category_id'],
+            row['iscrowd'] if 'iscrowd' in row else 0
+        )
+        for _, row in lapix_df.iterrows()
+    ]
+
+
+def lapix_to_masks(
+    lapix_df: LapixDataFrame,
+    draw_order: tuple[int, ...] | None = None,
+) -> Iterator[tuple[str, Mask]]:
+    df_groupped = lapix_df.groupby('image_id')
+    for _, df_by_img in df_groupped:
+        annotations = lapix_to_annotations(df_by_img)
+
+        w = df_by_img['image_width'].unique()[0]
+        h = df_by_img['image_height'].unique()[0]
+        image_name = basename(df_by_img.iloc[0]['image_name'])
+
+        yield (
+            image_name,
+            annotations_to_mask(annotations, int(w), int(h), draw_order)
+        )
+
+
+# -----------------------------------------------------------------------
+# Functions to generate masks
+def sort_annotations_to_draw(
+    annotations: list[Annotation],
+    draw_order: tuple[int, ...] | None = None
+) -> list[Annotation]:
+    '''Sorts the annotations based on the draw_order. If draw_order
+    is None sorts in ascending order based on the category value'''
+    items = defaultdict(list)
+
+    for ann in annotations:
+        items[ann.category_id].append(ann)
+
+    if draw_order is None:
+        draw_order = tuple(np.unique(list(items)))
+    elif not isinstance(draw_order, tuple):
+        raise ValueError('Unexpected value for `draw_order`. The value needs to be a tuple of int or None.')
+
+    out = [ann for cat in draw_order for ann in items[cat]]
+
+    return out
+
+
+def draw_annotation(
+    target: Image.Image,
+    annotation: Annotation,
+    value: int | tuple[int, int, int],
+) -> Image.Image:
+    '''Image: Draw an Annotation into the target (an Image)'''
+    for geo in annotation:
+        pol_x, pol_y = geo.exterior.coords.xy
+        coords = list(zip(pol_x, pol_y))
+        ImageDraw.Draw(target).polygon(coords, fill=value)
+
+    return target
+
+
+def annotations_to_mask(
+    annotations: list[Annotation],
+    width: int = 1600,
+    height: int = 1200,
+    draw_order: tuple[int, ...] | None = None,
+) -> Mask:
+    """Creates a Mask with the specified shape based on the annotations"""
+    shape = (height, width)
+
+    annotations_sorted = sort_annotations_to_draw(annotations, draw_order)
+
+    out = Image.fromarray(np.zeros(shape, dtype=np.uint8))
+    for ann in annotations_sorted:
+        out = draw_annotation(out, ann, ann.category_id)
+
+    return Mask(np.array(out))
+
+
+def __save_masks_as_files(
+    lapix_df: LapixDataFrame,
+    output_directory: str,
+    mask_extension: str = '.png',
+    draw_order: tuple[int, ...] | None = None,
+) -> None:
+
+    for image_name, mask in lapix_to_masks(lapix_df, draw_order):
+        out_path = os.path.join(
+            output_directory,
+            image_name + mask_extension
+        )
+        mask.save(out_path)
+
+
+def save_lapixdf_as_masks(
+    lapix_df: LapixDataFrame,
+    output_directory: str,
+    mask_extension: str = '.png',
+    draw_order: tuple[int, ...] | None = None,
+    processes: int = 1
+) -> None:
+    '''Saves masks as files based on the annotations from a Lapix DataFrame
+
+    Args:
+        lapix_df (LapixDataFrame): The data in the Lapix format. Needs to
+    have the following columns: `image_id` and `geometry`.
+        output_directory (str): The directory where the images should be
+    saved.
+        mask_extension (str): The image file extension/type. Defaults to
+    '.png'.
+        draw_order (tuple[int, ...] | None): If draw_order is None sorts
+    in ascending order based on the category value. Otherwise this will
+    draw the masks based on the tuple sequence.
+        processes (int): The number of processes to be used to perform
+    the conversion.
+
+    '''
+    img_ids = lapix_df['image_id'].unique()
+
+    if len(img_ids) == 0:
+        print('There is no annotation to save as mask.', file=sys.stderr)
+        return
+
+    images_ids_splitted = np.array_split(img_ids, processes)
+    print(
+        f'Starting to save {len(img_ids)} semantic segmentation masks using '
+        f'{processes} processes with {len(images_ids_splitted[0])} masks per process...',
+    )
+
+    workers = multiprocessing.Pool(processes=processes)
+    procs = []
+
+    for images_ids in images_ids_splitted:
+        df_to_process = lapix_df.loc[lapix_df['image_id'].isin(images_ids), :]
+        p = workers.apply_async(__save_masks_as_files, (df_to_process, output_directory, mask_extension, draw_order))
+        procs.append(p)
+
+    workers.close()
+    workers.join()
+
+
+# -----------------------------------------------------------------------
 # Functions to convert from x to y directly (ex: labelbox to coco)
 def labelbox_to_coco(
     labelbox_filename: str,
     schematic_to_id: dict[str, int],
     categories_coco: list[dict[str, str]],
     *,
     target: str = 'OD',
```

### Comparing `lapixdl-0.9.0/lapixdl/evaluation/evaluate.py` & `lapixdl-0.9.1/lapixdl/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/lapixdl/evaluation/model.py` & `lapixdl-0.9.1/lapixdl/evaluation/model.py`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/lapixdl/evaluation/plot.py` & `lapixdl-0.9.1/lapixdl/evaluation/plot.py`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/lapixdl/evaluation/visualize.py` & `lapixdl-0.9.1/lapixdl/evaluation/visualize.py`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/lapixdl/formats/annotation.py` & `lapixdl-0.9.1/lapixdl/formats/annotation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
+from copy import copy
 from dataclasses import dataclass
 
+from shapely.geometry import MultiPolygon
 from shapely.geometry import Polygon
 
 
 @dataclass
 class BBox:
     """Bounding Box data structure
 
@@ -20,14 +22,24 @@
     upper_left_x: int
     upper_left_y: int
     width: int
     height: int
     cls: int
     score: float | None = None
 
+    def __post_init__(self):
+        if self.upper_left_x < 0 or self.upper_left_y < 0:
+            raise ValueError(f'The upper left (x, y) should be positive values. Got ({self.upper_left_x}, {self.upper_left_y})')
+
+        if self.width <= 0:
+            raise ValueError(f'The width should be bigger than zero. Got {self.width}')
+
+        if self.height <= 0:
+            raise ValueError(f'The height should be bigger than zero. Got {self.height}')
+
     @property
     def upper_left_point(self) -> tuple[int, int]:
         """Tuple[int, int]: (X,Y) of the upper left point of the Bounding Box."""
         return (
             self.upper_left_x,
             self.upper_left_y
         )
@@ -148,15 +160,58 @@
         return self.area + bbox.area - (intersection_area or self.intersection_area_with(bbox))
 
     def to_polygon(self) -> Polygon:
         """Polygon: A shapely polygon from the coordinates of the bbox"""
         return Polygon(self.coords)
 
 
-def bounds_to_BBox(bounds: tuple[float], category_id: int) -> BBox:
+@dataclass
+class Annotation:
+    geometry: Polygon | MultiPolygon
+    category_id: int
+    iscrowd: int = 0
+
+    @property
+    def bbox(self) -> BBox:
+        return bounds_to_bbox(self.geometry.bounds, self.category_id)
+
+    @property
+    def _geo_type(self) -> str:
+        return self.geometry.geom_type
+
+    @property
+    def xywh_bbox(self) -> list[int]:
+        bbox = self.bbox
+        return [bbox.upper_left_x, bbox.upper_left_y, bbox.width, bbox.height]
+
+    def __iter__(self) -> Annotation:
+        self._idx = 0
+
+        if self._geo_type == 'MultiPolygon':
+            self._geometries = list(self.geometry.geoms)
+        elif self._geo_type == 'Polygon':
+            self._geometries = [self.geometry]
+        else:
+            raise TypeError(f'Unexpected geometry type (`{self._geo_type}`) - expected `MultiPolygon` or `Polygon`')
+
+        return self
+
+    def __next__(self) -> Polygon:
+        if self._idx < len(self._geometries):
+            out = self._geometries[self._idx]
+            self._idx += 1
+            return out
+        else:
+            raise StopIteration
+
+    def copy(self) -> Annotation:
+        return copy(self)
+
+
+def bounds_to_bbox(bounds: tuple[float], category_id: int) -> BBox:
     """Generate a BBox from a tuple of bounds
 
     Args:
         bounds (tuple[float]): A tuple of floats in the following order
     (min_x, min_y, max_x, max_y)
         category_id: A category id fot the BBox
```

### Comparing `lapixdl-0.9.0/lapixdl/formats/labelbox.py` & `lapixdl-0.9.1/lapixdl/formats/labelbox.py`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/lapixdl/formats/lapix.py` & `lapixdl-0.9.1/lapixdl/formats/lapix.py`

 * *Files identical despite different names*

### Comparing `lapixdl-0.9.0/lapixdl.egg-info/PKG-INFO` & `lapixdl-0.9.1/lapixdl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapixdl
-Version: 0.9.0
+Version: 0.9.1
 Summary: Utils for Computer Vision Deep Learning research
 Home-page: https://github.com/lapix-ufsc/lapixdl
 Author: LAPiX
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -111,27 +111,27 @@
 #### Example of conversion from **Labelbox** to **COCO** labels format:
 
 ```python
 import json
 
 from lapixdl.formats import labelbox_to_coco
 
-# convert it to a intermediary format
+# A map categories between labelbox schematic id and category ID
 map_categories = {
   '<schematic id from labelbox>': 1 # category id
 }
 
-# convert it
+# The categories section in the COCO format
 categories_coco = [{
   'supercategory': None,
   'name': 'example_category',
   'id': 1
 }]
 
-# create the full COCO OD file
+# Convert it and create the COCO OD data
 coco_dict = labelbox_to_coco(
   'labelbox_export_file.json',
   map_categories,
   categories_coco,
   target = 'object detection',
   image_shape = (1200, 1600)
 )
```

### Comparing `lapixdl-0.9.0/setup.cfg` & `lapixdl-0.9.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lapixdl
-version = 0.9.0
+version = 0.9.1
 description = Utils for Computer Vision Deep Learning research
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lapix-ufsc/lapixdl
 author = LAPiX
 license = MIT
 license_file = LICENCE
@@ -16,22 +16,28 @@
 
 [options]
 packages = find:
 install_requires = 
 	matplotlib
 	numpy
 	pandas
+	pillow
 	pyarrow
 	seaborn
 	shapely
 	tqdm
+	typing-extensions
 python_requires = >=3.7
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
 
+[options.entry_points]
+console_scripts = 
+	lapixdl = lapixdl.commands.main:main
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

