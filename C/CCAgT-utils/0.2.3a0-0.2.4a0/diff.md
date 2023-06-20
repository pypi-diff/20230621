# Comparing `tmp/CCAgT_utils-0.2.3a0.tar.gz` & `tmp/CCAgT_utils-0.2.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CCAgT_utils-0.2.3a0.tar", last modified: Mon Apr 11 19:54:15 2022, max compression
+gzip compressed data, was "CCAgT_utils-0.2.4a0.tar", last modified: Sun May  1 21:51:28 2022, max compression
```

## Comparing `CCAgT_utils-0.2.3a0.tar` & `CCAgT_utils-0.2.4a0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:15.536407 CCAgT_utils-0.2.3a0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:15.536407 CCAgT_utils-0.2.3a0/CCAgT_utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6491 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:15.536407 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/
--rw-r--r--   0 runner    (1001) docker     (121)    22230 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/CCAgT.py
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/COCO.py
--rw-r--r--   0 runner    (1001) docker     (121)     6347 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/LabelBox.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    13609 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/converters/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11581 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/describe.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    16910 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    10506 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/split.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:15.536407 CCAgT_utils-0.2.3a0/CCAgT_utils/types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/types/alias.py
--rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/types/annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/types/checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/types/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/types/mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:15.536407 CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7702 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/_show.py
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 19:54:15.536407 CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11041 2022-04-11 19:54:15.000000 CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-04-11 19:54:15.000000 CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 19:54:15.000000 CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-11 19:54:15.000000 CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-11 19:54:15.000000 CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-11 19:54:15.000000 CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11041 2022-04-11 19:54:15.536407 CCAgT_utils-0.2.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10137 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-04-11 19:54:15.540408 CCAgT_utils-0.2.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-11 19:54:03.000000 CCAgT_utils-0.2.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:28.376934 CCAgT_utils-0.2.4a0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:28.372934 CCAgT_utils-0.2.4a0/CCAgT_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:28.376934 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/
+-rw-r--r--   0 runner    (1001) docker     (121)    22233 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/CCAgT.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/COCO.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6347 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/LabelBox.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/masks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13609 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/converters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11581 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16910 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10506 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/slice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/split.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:28.376934 CCAgT_utils-0.2.4a0/CCAgT_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/types/alias.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/types/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/types/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/types/colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/types/mask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:28.376934 CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7702 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/_show.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 21:51:28.372934 CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11041 2022-05-01 21:51:27.000000 CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-05-01 21:51:28.000000 CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-01 21:51:27.000000 CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-01 21:51:28.000000 CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-01 21:51:28.000000 CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-01 21:51:28.000000 CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    11041 2022-05-01 21:51:28.376934 CCAgT_utils-0.2.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10137 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-05-01 21:51:28.376934 CCAgT_utils-0.2.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-01 21:51:09.000000 CCAgT_utils-0.2.4a0/setup.py
```

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/categories.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,18 @@
     name: str
     color: Color
     labelbox_schemaId: str | None = None
     minimal_area: int = 0
     supercategory: str | None = None
     isthing: int = 1
 
+    @property
+    def category(self) -> Categories:
+        return Categories(self.id)
+
 
 class CategoriesInfos():
     def __init__(
         self,
         categories_info: list[dict[str, Any]] | None = None,
     ) -> None:
         if isinstance(categories_info, list):
```

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/checkers.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/checkers.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/converters/CCAgT.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/converters/CCAgT.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,15 +505,15 @@
     annotations_panoptic = []
 
     _out_dir = out_dir
 
     if df['image_width'].nunique() == df['image_height'].nunique() == 1:
         w = int(df['image_width'].unique()[0])
         h = int(df['image_height'].unique()[0])
-        output_template = np.zeros((h, w, 3), dtype=np.uint8)
+        output_template = Image.fromarray(np.zeros((h, w, 3), dtype=np.uint8))
     else:
         output_template = None
 
     for img_id, df_by_img in df.groupby('image_id'):
         img_name = df_by_img.iloc[0]['image_name']
         output_basename = basename(img_name) + '.png'
         panoptic_record = {
@@ -528,38 +528,38 @@
                 row['iscrowd'],
                 row['color'],
             ) for _, row in df_by_img.iterrows()
         ])
 
         segments_info = []
 
-        if isinstance(output_template, np.ndarray):
+        if isinstance(output_template, Image.Image):
             out = output_template.copy()
         else:
             w = int(df_by_img['image_width'].unique()[0])
             h = int(df_by_img['image_height'].unique()[0])
-            out = np.zeros((h, w, 3), dtype=np.uint8)
+            out = Image.fromarray(np.zeros((h, w, 3), dtype=np.uint8))
 
         for ann in annotations_sorted:
-            out = draw_annotation(out, ann, ann.color.rgb, out.shape[:2])
+            out = draw_annotation(out, ann, ann.color.rgb)
             segments_info.append({
                 'id': COCO_PS.color_to_id(ann.color),
                 'category_id': ann.category_id,
                 'area': int(ann.geometry.area),
                 'bbox': ann.coco_bbox,
                 'iscrowd': ann.iscrowd,
             })
 
         panoptic_record['segments_info'] = segments_info
 
         if split_by_slide:
             _out_dir = os.path.join(out_dir, df_by_img.iloc[0]['slide_id'])
 
         output_filename = os.path.join(_out_dir, output_basename)
-        Image.fromarray(out).save(output_filename)
+        out.save(output_filename)
         annotations_panoptic.append(panoptic_record)
     return annotations_panoptic
 
 
 @get_traceback
 def single_core_to_OD_COCO(df: pd.DataFrame, decimals: int = 2) -> list[dict[str, Any]]:
     return df.apply(
```

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/converters/COCO.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/converters/COCO.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/converters/LabelBox.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/converters/LabelBox.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/converters/main.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/converters/main.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/converters/masks.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/converters/masks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import collections
 
 import numpy as np
-from skimage.draw import polygon
+from PIL import Image
+from PIL import ImageDraw
 
 from CCAgT_utils.categories import Categories
 from CCAgT_utils.types.annotation import Annotation
 from CCAgT_utils.types.mask import Mask
 
 # Order of categories IDs available at the metadata
 DRAW_ORDER = (
@@ -35,27 +36,25 @@
     width: int = 1600,
     height: int = 1200,
 ) -> Mask:
     shape = (height, width)
 
     annotations_sorted = order_annotations_to_draw(annotations)
 
-    out = np.zeros(shape, dtype=np.uint8)
+    out = Image.fromarray(np.zeros(shape, dtype=np.uint8))
     for ann in annotations_sorted:
-        out = draw_annotation(out, ann, ann.category_id, shape)
+        out = draw_annotation(out, ann, ann.category_id)
 
-    return Mask(out)
+    return Mask(np.array(out))
 
 
 def draw_annotation(
-    target: np.ndarray,
+    target: Image.Image,
     annotation: Annotation,
     value: int | tuple[int, int, int],
-    shape: tuple[int, int] | None = None,
-) -> np.ndarray:
+) -> Image.Image:
     for geo in annotation:
         pol_x, pol_y = geo.exterior.coords.xy
-
-        _x, _y = polygon(pol_y, pol_x, shape)
-        target[_x, _y] = value
+        coords = list(zip(pol_x, pol_y))
+        ImageDraw.Draw(target).polygon(coords, fill=value)
 
     return target
```

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/converters/utils.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/converters/utils.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/describe.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/describe.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/main.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/main.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/prepare.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/prepare.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/slice.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/slice.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/split.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/split.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/types/annotation.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/types/annotation.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/types/checkers.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/types/checkers.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/types/colors.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/types/colors.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/types/mask.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/types/mask.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/utils.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/utils.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/_show.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/_show.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/main.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/main.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils/visualization/plot.py` & `CCAgT_utils-0.2.4a0/CCAgT_utils/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/PKG-INFO` & `CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CCAgT-utils
-Version: 0.2.3a0
+Version: 0.2.4a0
 Summary: A framework of utilities to help at the use of the CCAgT dataset
 Home-page: https://github.com/johnnv1/CCAgT_dataset_utils
 Author: João Gustavo Atkinson Amorim
 Author-email: joaogustavoamorim@gmail.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `CCAgT_utils-0.2.3a0/CCAgT_utils.egg-info/SOURCES.txt` & `CCAgT_utils-0.2.4a0/CCAgT_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/LICENSE` & `CCAgT_utils-0.2.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/PKG-INFO` & `CCAgT_utils-0.2.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CCAgT_utils
-Version: 0.2.3a0
+Version: 0.2.4a0
 Summary: A framework of utilities to help at the use of the CCAgT dataset
 Home-page: https://github.com/johnnv1/CCAgT_dataset_utils
 Author: João Gustavo Atkinson Amorim
 Author-email: joaogustavoamorim@gmail.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `CCAgT_utils-0.2.3a0/README.md` & `CCAgT_utils-0.2.4a0/README.md`

 * *Files identical despite different names*

### Comparing `CCAgT_utils-0.2.3a0/setup.cfg` & `CCAgT_utils-0.2.4a0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CCAgT_utils
-version = 0.2.3-alpha
+version = 0.2.4-alpha
 description = A framework of utilities to help at the use of the CCAgT dataset
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/johnnv1/CCAgT_dataset_utils
 author = João Gustavo Atkinson Amorim
 author_email = joaogustavoamorim@gmail.com
 license = Apache-2.0
@@ -25,17 +25,15 @@
 install_requires = 
 	matplotlib>=3.5.1
 	networkx>=2.6.3
 	numpy>=1.21.5
 	pandas>=1.1.5
 	pillow>=9.0.1
 	pyarrow>=7.0.0
-	scikit-image>=0.19.2
 	shapely>=1.8.0
-	virtualenv>=20.0.8
 python_requires = >=3.7
 
 [options.packages.find]
 exclude = 
 	tests*
 	data*
```

