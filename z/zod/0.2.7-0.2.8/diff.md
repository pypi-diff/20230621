# Comparing `tmp/zod-0.2.7.tar.gz` & `tmp/zod-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.2.7.tar", max compression
+gzip compressed data, was "zod-0.2.8.tar", max compression
```

## Comparing `zod-0.2.7.tar` & `zod-0.2.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-05-25 12:01:49.078296 zod-0.2.7/LICENSE
--rw-r--r--   0        0        0     4809 2023-05-25 12:01:49.078296 zod-0.2.7/README.md
--rw-r--r--   0        0        0     1783 2023-05-25 12:01:49.078296 zod-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      982 2023-05-25 12:01:49.078296 zod-0.2.7/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-05-25 12:01:49.078296 zod-0.2.7/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-05-25 12:01:49.078296 zod-0.2.7/zod/anno/lane.py
--rw-r--r--   0        0        0     4354 2023-05-25 12:01:49.078296 zod-0.2.7/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-05-25 12:01:49.082297 zod-0.2.7/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    14496 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/download_zod.py
--rw-r--r--   0        0        0     7431 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6049 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1324 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/utils.py
--rw-r--r--   0        0        0     3682 2023-05-25 12:01:49.082297 zod-0.2.7/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-05-25 12:01:49.082297 zod-0.2.7/zod/constants.py
--rw-r--r--   0        0        0      184 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-05-25 12:01:49.082297 zod-0.2.7/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12061 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0     1016 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      123 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8031 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-05-25 12:01:49.082297 zod-0.2.7/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-05-25 12:01:49.082297 zod-0.2.7/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     8041 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lidar_3d.py
--rw-r--r--   0        0        0     6028 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-05-25 12:01:49.082297 zod-0.2.7/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-05-25 12:01:49.082297 zod-0.2.7/zod/zod_drives.py
--rw-r--r--   0        0        0      577 2023-05-25 12:01:49.082297 zod-0.2.7/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-05-25 12:01:49.082297 zod-0.2.7/zod/zod_sequences.py
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-21 10:05:53.391525 zod-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4809 2023-06-21 10:05:53.391525 zod-0.2.8/README.md
+-rw-r--r--   0        0        0     1783 2023-06-21 10:05:53.395525 zod-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-06-21 10:05:53.395525 zod-0.2.8/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-06-21 10:05:53.395525 zod-0.2.8/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/lane.py
+-rw-r--r--   0        0        0     4931 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    14496 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     7431 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6032 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1324 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/utils.py
+-rw-r--r--   0        0        0     4658 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-06-21 10:05:53.395525 zod-0.2.8/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12046 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0      437 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      355 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8399 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-06-21 10:05:53.399526 zod-0.2.8/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-06-21 10:05:53.399526 zod-0.2.8/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-06-21 10:05:53.399526 zod-0.2.8/zod/zod_drives.py
+-rw-r--r--   0        0        0     1047 2023-06-21 10:05:53.399526 zod-0.2.8/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-06-21 10:05:53.399526 zod-0.2.8/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.8/PKG-INFO
```

### Comparing `zod-0.2.7/LICENSE` & `zod-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/README.md` & `zod-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/pyproject.toml` & `zod-0.2.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.2.7"
+version = "0.2.8"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.2.7/zod/__init__.py` & `zod-0.2.8/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/_zod_dataset.py` & `zod-0.2.8/zod/_zod_dataset.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/anno/lane.py` & `zod-0.2.8/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/anno/object.py` & `zod-0.2.8/zod/anno/object.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,46 @@
     "TrafficSignal",
     "TrafficGuide",
     "DynamicBarrier",
 )
 OBJECT_CLASSES = (
     *OBJECT_CLASSES_DYNAMIC,
     *OBJECT_CLASSES_STATIC,
-    "Inconclusive",
+    "Unclear",
+)
+
+CLASSES_WITH_SUBCLASSES = ("Vehicle", "VulnerableVehicle", "TrafficSign", "TrafficSignal")
+VEHICLE_SUBCLASSES = (
+    "Car",
+    "Van",
+    "Truck",
+    "Bus",
+    "Trailer",
+    "TramTrain",
+    "HeavyEquip",
+    "Emergency",
+    "Other",
+)
+VULNERABLE_VEHICLE_SUBCLASSES = (
+    "Bicycle",
+    "Motorcycle",
+    "Stroller",
+    "Wheelchair",
+    "PersonalTransporter",
+    "NoRider",
+    "Other",
+)
+OBJECT_SUBCLASSES = (
+    *[cls_ for cls_ in OBJECT_CLASSES if cls_ not in CLASSES_WITH_SUBCLASSES],
+    *[f"Vehicle_{type_}" for type_ in VEHICLE_SUBCLASSES],
+    *[f"VulnerableVehicle_{type_}" for type_ in VULNERABLE_VEHICLE_SUBCLASSES],
+    "TrafficSign_Front",
+    "TrafficSign_Back",
+    "TrafficSignal_Front",
+    "TrafficSignal_Back",
 )
 
 
 @dataclass
 class ObjectAnnotation:
     """Class to store dynamic object information."""
 
@@ -45,19 +76,45 @@
     object_type: Optional[str]
     occlusion_level: Optional[str]
     artificial: Optional[str]
     with_rider: Optional[bool]
     emergency: Optional[bool]
     traffic_content_visible: Optional[bool]
 
+    @property
+    def superclass(self):
+        """Get the super-class of the object."""
+        return self.name
+
+    @property
+    def subclass(self):
+        """Get the sub-class of the object."""
+        if self.unclear:
+            return f"Unclear"
+        superclass = self.superclass
+        if superclass not in CLASSES_WITH_SUBCLASSES:
+            return superclass
+        if self.artificial is True:
+            return f"{superclass}_Artificial"
+        if self.traffic_content_visible is not None:
+            return f"{superclass}_{'Front' if self.traffic_content_visible else 'Back'}"
+        if self.with_rider is False:
+            return f"{superclass}_NoRider"
+        if self.emergency is True and superclass == "Vehicle":
+            return f"{superclass}_Emergency"  # other superclasses have too few emergency objs
+        if self.object_type is not None:
+            return f"{superclass}_{self.object_type}"
+        # the above should have been exhaustive
+        raise ValueError("Object subclass could not be determined")
+
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> ObjectAnnotation:
         """Create an ObjectAnnotation from a dictionary."""
         properties: Dict[str, Any] = data["properties"]
-        unclear = (properties["class"] == "Inconclusive") or properties["unclear"]
+
         box2d = Box2D.from_points(points=data["geometry"]["coordinates"], frame=Camera.FRONT)
         box3d = None
         if "location_3d" in properties:
             box3d = Box3D(
                 center=np.array(properties["location_3d"]["coordinates"]),
                 size=np.array(
                     [
@@ -70,69 +127,32 @@
                     properties["orientation_3d_qw"],
                     properties["orientation_3d_qx"],
                     properties["orientation_3d_qy"],
                     properties["orientation_3d_qz"],
                 ),
                 frame=Lidar.VELODYNE,
             )
-        with_rider = properties.get("with_rider")
-        with_rider = with_rider if with_rider is None else with_rider == "True"
-        tcv = properties.get("traffic_content_visible")
-        tcv = tcv if tcv is None else tcv == "True"
+
+        def _parse_bool_prop(key: str) -> Optional[bool]:
+            return None if key not in properties else properties[key] == "True"
+
+        superclass, obj_type = properties["class"], properties.get("type")
+        unclear = "Inconclusive" in (superclass, obj_type) or properties["unclear"]
+        if superclass == "Inconclusive":
+            superclass = "Unclear"
         return cls(
             uuid=properties["annotation_uuid"],
             box2d=box2d,
             box3d=box3d,
             unclear=unclear,
-            name=properties["class"],
-            object_type=properties.get("type", None),
+            name=superclass,
+            object_type=obj_type,
             occlusion_level=properties.get("occlusion_ratio", None),
             artificial=properties.get("artificial", None),
-            with_rider=with_rider,
+            with_rider=_parse_bool_prop("with_rider"),
             emergency=properties.get("emergency", None),
-            traffic_content_visible=tcv,
+            traffic_content_visible=_parse_bool_prop("traffic_content_visible"),
         )
 
-    def should_ignore_object(self, require_3d: bool = True) -> bool:
-        """Check if the object should be ignored.
-
-        Returns:
-            True if the object should be ignored.
-        """
-        # Remove unclear objects
-        if self.unclear:
-            return True
-        # Remove objects that dont have 3d box
-        if self.box3d is None and require_3d:
-            return True
-        # If the object is artificial, reflection or an image, ignore it
-        if self.artificial not in (None, "None"):
-            return True
-
-        # Class specific removals
-        if self.name == "Vehicle":
-            if self.object_type not in (
-                "Car",
-                "Bus",
-                "Truck",
-                "Van",
-                "Trailer",
-                "HeavyEquip",
-            ):
-                return True
-        elif self.name == "VulnerableVehicle":
-            if self.object_type not in ("Bicycle", "Motorcycle"):
-                return True
-            return not self.with_rider
-        elif self.name == "Pedestrian":
-            pass
-        elif self.name == "TrafficSign":
-            return not self.traffic_content_visible
-
-        elif self.name == "TrafficSignal":
-            return not self.traffic_content_visible
-
-        return False
-
 
 # Compatibility with old naming
 AnnotatedObject = ObjectAnnotation
```

### Comparing `zod-0.2.7/zod/anno/parser.py` & `zod-0.2.8/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/anno/tsr/class_map.py` & `zod-0.2.8/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/anno/tsr/traffic_sign.py` & `zod-0.2.8/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/cli/download_zod.py` & `zod-0.2.8/zod/cli/download_zod.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/cli/extract_tsr_patches.py` & `zod-0.2.8/zod/cli/extract_tsr_patches.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/cli/generate_coco_json.py` & `zod-0.2.8/zod/cli/generate_coco_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         {
             # avoid collisions by assuming max 1k objects per frame
             "id": int(frame.info.id) * 1000 + obj_idx,
             "image_id": int(frame.info.id),
             "category_id": CATEGORY_NAME_TO_ID[obj.name],
             "bbox": [round(val, 2) for val in obj.box2d.xywh.tolist()],
             "area": round(obj.box2d.area, 2),
-            "iscrowd": obj.should_ignore_object(require_3d=False),
+            "iscrowd": obj.subclass == "Unclear",
         }
         for obj_idx, obj in enumerate(objs)
         if obj.name in classes
     ]
     return image_dict, anno_dicts
```

### Comparing `zod-0.2.7/zod/cli/main.py` & `zod-0.2.8/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/cli/utils.py` & `zod-0.2.8/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/cli/visualize_lidar.py` & `zod-0.2.8/zod/cli/visualize_lidar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+from typing import List
+
 import numpy as np
 import typer
 from rich import print
 from rich.panel import Panel
 
 from zod import ZodFrames, ZodSequences
+from zod.constants import AnnotationProject
 from zod.data_classes import LidarData
+from zod.data_classes.box import Box3D
 from zod.utils.utils import zfill_id
 
 app = typer.Typer(no_args_is_help=True)
 
 IMPORT_ERROR = (
     "zod does not ship with open3d, which is required for interactive point cloud "
     "visualization.\nPlease install it manually: pip install open3d"
 )
 
 
-def _visualize(data: LidarData):
+def _visualize(data: LidarData, boxes: List[Box3D] = None):
     try:
         import open3d as o3d
     except ImportError:
         print(Panel(IMPORT_ERROR, title="Warning! Missing Dependency", border_style="red"))
         exit(1)
     from matplotlib import cm
 
@@ -27,35 +31,56 @@
     pcd.points = o3d.utility.Vector3dVector(data.points)
     # color the pointcloud according to the timestamp
     # timestamps = data.timestamps
     # color = (timestamps - timestamps.min()) / (timestamps.max() - timestamps.min())
     color = np.log(data.intensity)
     # use a nice colormap
     pcd.colors = o3d.utility.Vector3dVector(cm.get_cmap("jet")(color)[:, :3])
-    # Draw coordinate frame
-    o3d.visualization.draw_geometries(
-        [pcd, o3d.geometry.TriangleMesh.create_coordinate_frame(size=1.0)]
-    )
+
+    # if boxes are provided, render them as rigid bodies
+    if boxes:
+        o3d_boxes = []
+        for box in boxes:
+            o3d_box = o3d.geometry.OrientedBoundingBox.create_from_points(
+                o3d.utility.Vector3dVector(box.corners)
+            )
+            o3d_box.color = (0.98, 0.63, 0.01)
+            o3d_boxes.append(o3d_box)
+        o3d.visualization.draw_geometries(
+            [pcd, *o3d_boxes, o3d.geometry.TriangleMesh.create_coordinate_frame(size=1.0)]
+        )
+    else:
+        o3d.visualization.draw_geometries(
+            [pcd, o3d.geometry.TriangleMesh.create_coordinate_frame(size=1.0)]
+        )
 
 
 @app.command(no_args_is_help=True)
 def frames(
     dataset_root: str = typer.Option(..., help="Path to the dataset root"),
     version: str = typer.Option(..., help="Version of the dataset"),
     frame_id: int = typer.Option(..., help="Frame id to visualize"),
     num_before: int = typer.Option(0, help="Number of frames before the given frame id"),
     num_after: int = typer.Option(0, help="Number of frames after the given frame id"),
+    with_bounding_boxes: bool = typer.Option(
+        False, help="if bounding boxes of center-frame are to be rendered"
+    ),
 ):
     """Visualize the lidar data for a given frame id."""
     zod_frames = ZodFrames(dataset_root=dataset_root, version=version)
     if zfill_id(frame_id) not in zod_frames.get_all_ids():
         raise ValueError(f"Frame id must be one of {zod_frames.get_all_ids()}.")
     frame = zod_frames[frame_id]
     data = frame.get_aggregated_lidar(num_before=num_before, num_after=num_after)
-    _visualize(data)
+    if with_bounding_boxes:
+        annos = frame.get_annotation(project=AnnotationProject.OBJECT_DETECTION)
+        boxes = [anno.box3d for anno in annos if anno.box3d is not None]
+    else:
+        boxes = []
+    _visualize(data, boxes=boxes)
 
 
 @app.command(no_args_is_help=True)
 def sequences(
     dataset_root: str = typer.Option(..., help="Path to the dataset root"),
     version: str = typer.Option(..., help="Version of the dataset"),
     sequence_id: int = typer.Option(..., help="Frame id to visualize"),
```

### Comparing `zod-0.2.7/zod/constants.py` & `zod-0.2.8/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/box.py` & `zod-0.2.8/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/calibration.py` & `zod-0.2.8/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/ego_motion.py` & `zod-0.2.8/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/frame.py` & `zod-0.2.8/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/geometry.py` & `zod-0.2.8/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/info.py` & `zod-0.2.8/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/metadata.py` & `zod-0.2.8/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/sensor.py` & `zod-0.2.8/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/sequence.py` & `zod-0.2.8/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/data_classes/vehicle_data.py` & `zod-0.2.8/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_experimental/eval.py` & `zod-0.2.8/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_experimental/matching.py` & `zod-0.2.8/zod/eval/detection/_experimental/matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """Split the ground truth objects into valid and dont-care objects."""
 
     # valid ground truth objects
     valid_gt: List[ObjectAnnotation] = []
     # dont-care ground truth objects
     dont_care_gt: List[ObjectAnnotation] = []
     for gt in ground_truth:
-        if gt.name not in eval_classes or gt.should_ignore_object():
+        if gt.name not in eval_classes or gt.unclear:
             dont_care_gt.append(gt)
         else:
             valid_gt.append(gt)
 
     return valid_gt, dont_care_gt
```

### Comparing `zod-0.2.7/zod/eval/detection/_experimental/utils.py` & `zod-0.2.8/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.2.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.2.8/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.2.8/zod/eval/detection/eval_nuscenes_style.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 PER_CLASS_SUMMARY = """
 {cls}:
     mAP:  {mAP:.4f}
     mATE: {mATE:.4f}
     mASE: {mASE:.4f}
     mAOE: {mAOE:.4f}"""
 
+# for reference
 NUSCENES_DEFAULT_SETTINGS = {
     "class_range": {
         "Vehicle": 50,
         "VulnerableVehicle": 40,
         "Pedestrian": 30,
         "TrafficSign": 30,
         "TrafficSignal": 30,
@@ -50,30 +51,42 @@
     "dist_th_tp": 2.0,
     "min_recall": 0.1,
     "min_precision": 0.1,
     "max_boxes_per_sample": 500,
     "mean_ap_weight": 5,
 }
 
+# our settings
+ZOD_DEFAULT_SETTINGS = {
+    "class_range": {cls_name: 250 for cls_name in EVALUATION_CLASSES},
+    "dist_fcn": "center_distance",
+    "dist_ths": [0.5, 1.0, 2.0, 4.0],
+    "dist_th_tp": 2.0,
+    "min_recall": 0.1,
+    "min_precision": 0.1,
+    "max_boxes_per_sample": 500,
+    "mean_ap_weight": 5,
+}
+
 
 def evaluate_nuscenes_style(
     gt_boxes: EvalBoxes,
     det_boxes: EvalBoxes,
     verbose: bool = False,
     output_path: str = None,
     verify_coordinate_system: bool = True,
 ) -> Dict[str, float]:
     """Perform nuscenes evaluation based on a number of groundtruths and detections."""
     if verify_coordinate_system:
         _check_coordinate_system(gt_boxes)
 
-    detection_cfg = DetectionConfig(**NUSCENES_DEFAULT_SETTINGS)
+    detection_cfg = DetectionConfig(**ZOD_DEFAULT_SETTINGS)
     detection_metrics = DetectionMetrics(detection_cfg)
 
-    class_ranges = {k: (0, v) for k, v in NUSCENES_DEFAULT_SETTINGS["class_range"].items()}
+    class_ranges = {k: (0, v) for k, v in ZOD_DEFAULT_SETTINGS["class_range"].items()}
 
     # filter according to the default nuscenes settings
     gt_boxes = _filter_eval_boxes_on_ranges(gt_boxes, class_ranges)
     det_boxes = _filter_eval_boxes_on_ranges(det_boxes, class_ranges)
 
     metrics = {
         dist_th: _nuscenes_evaluate(gt_boxes, det_boxes, dist_th=dist_th)
@@ -85,15 +98,14 @@
         # They evaluate the ap across all thresholds
         for dist_th in detection_cfg.dist_ths:
             detection_metrics.add_label_ap(
                 detection_name=zod_cls,
                 dist_th=dist_th,
                 ap=metrics[dist_th][zod_cls]["ap"],
             )
-
         # They evaluate the tp across only one threshold
         for metric in VALID_TP_METRICS:
             detection_metrics.add_label_tp(
                 zod_cls, metric, metrics[detection_cfg.dist_th_tp][zod_cls][metric]
             )
 
     if verbose:
@@ -136,19 +148,23 @@
     dist_th: float = 1,
     min_precision: float = 0.1,
     min_recall: float = 0.1,
 ) -> Dict[str, float]:
     """Perform nuscenes evaluation based on a number of groundtruths and detections."""
     metrics = {}
 
+    existing_classes = set()
+    for box in gt_boxes.all:
+        existing_classes.add(box.detection_name)
+
     for cls in EVALUATION_CLASSES:
-        # ensure that we have samples for this class in the gt data
-        n_samples = sum(1 for box in gt_boxes.all if box.detection_name == cls)
-        if n_samples == 0:
+        if cls not in existing_classes:
+            # ensure that we have samples for this class in the gt data
             continue
+
         md = accumulate(
             gt_boxes,
             det_boxes,
             cls,
             dist_fcn=dist_fcn,
             dist_th=dist_th,
         )
```

### Comparing `zod-0.2.7/zod/utils/compensation.py` & `zod-0.2.8/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/utils/geometry.py` & `zod-0.2.8/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/utils/polygon_transformations.py` & `zod-0.2.8/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/utils/utils.py` & `zod-0.2.8/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/utils/visualization.py` & `zod-0.2.8/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/bev_utils.py` & `zod-0.2.8/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/colorlabeler.py` & `zod-0.2.8/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/lidar_3d.py` & `zod-0.2.8/zod/visualization/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/lidar_bev.py` & `zod-0.2.8/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/lidar_on_image.py` & `zod-0.2.8/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/object_visualization.py` & `zod-0.2.8/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/oxts_on_image.py` & `zod-0.2.8/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/oxts_visualization.py` & `zod-0.2.8/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/visualization/polygon_utils.py` & `zod-0.2.8/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/zod_drives.py` & `zod-0.2.8/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/zod/zod_sequences.py` & `zod-0.2.8/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.7/PKG-INFO` & `zod-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.2.7
+Version: 0.2.8
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

