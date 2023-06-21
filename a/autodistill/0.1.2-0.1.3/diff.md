# Comparing `tmp/autodistill-0.1.2.tar.gz` & `tmp/autodistill-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-0.1.2.tar", last modified: Fri Jun  9 17:07:49 2023, max compression
+gzip compressed data, was "autodistill-0.1.3.tar", last modified: Wed Jun 21 10:36:10 2023, max compression
```

## Comparing `autodistill-0.1.2.tar` & `autodistill-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.730241 autodistill-0.1.2/
--rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-07 11:34:42.000000 autodistill-0.1.2/LICENSE
--rw-r--r--   0 james      (501) staff       (20)    14015 2023-06-09 17:07:49.730047 autodistill-0.1.2/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)    13503 2023-06-09 17:03:43.000000 autodistill-0.1.2/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.727619 autodistill-0.1.2/autodistill/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-09 17:04:08.000000 autodistill-0.1.2/autodistill/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.728978 autodistill-0.1.2/autodistill/core/
--rw-r--r--   0 james      (501) staff       (20)      151 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      516 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/base_model.py
--rw-r--r--   0 james      (501) staff       (20)      114 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/ontology.py
--rw-r--r--   0 james      (501) staff       (20)      236 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/target_model.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.729699 autodistill-0.1.2/autodistill/detection/
--rw-r--r--   0 james      (501) staff       (20)      290 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      580 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/caption_ontology.py
--rw-r--r--   0 james      (501) staff       (20)     1760 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/detection_base_model.py
--rw-r--r--   0 james      (501) staff       (20)      769 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/detection_ontology.py
--rw-r--r--   0 james      (501) staff       (20)      366 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/detection_target_model.py
--rw-r--r--   0 james      (501) staff       (20)     3258 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.728385 autodistill-0.1.2/autodistill.egg-info/
--rw-r--r--   0 james      (501) staff       (20)    14015 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      602 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      142 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       12 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-09 17:07:49.730282 autodistill-0.1.2/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1261 2023-06-09 17:07:46.000000 autodistill-0.1.2/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.729845 autodistill-0.1.2/test/
--rw-r--r--   0 james      (501) staff       (20)       41 2023-06-07 11:34:42.000000 autodistill-0.1.2/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.149181 autodistill-0.1.3/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-21 10:32:32.000000 autodistill-0.1.3/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)    15193 2023-06-21 10:36:10.148941 autodistill-0.1.3/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)    14669 2023-06-21 10:32:32.000000 autodistill-0.1.3/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.145667 autodistill-0.1.3/autodistill/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-06-21 10:32:54.000000 autodistill-0.1.3/autodistill/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.147340 autodistill-0.1.3/autodistill/core/
+-rw-r--r--   0 james      (501) staff       (20)      151 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      516 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      114 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      236 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/target_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.148337 autodistill-0.1.3/autodistill/detection/
+-rw-r--r--   0 james      (501) staff       (20)      290 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      580 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/caption_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)     1760 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/detection_base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      769 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/detection_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      366 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/detection_target_model.py
+-rw-r--r--   0 james      (501) staff       (20)     3258 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.146617 autodistill-0.1.3/autodistill.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)    15193 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      602 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      142 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-21 10:36:10.149228 autodistill-0.1.3/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1273 2023-06-21 10:36:06.000000 autodistill-0.1.3/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.148529 autodistill-0.1.3/test/
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-06-21 10:32:32.000000 autodistill-0.1.3/test/test_hello.py
```

### Comparing `autodistill-0.1.2/LICENSE` & `autodistill-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.2/PKG-INFO` & `autodistill-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.2
+Version: 0.1.3
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
@@ -142,15 +142,17 @@
 ```
 </details>
 
 Additional Base and Target models are [enumerated below](#-available-models).
 
 ## 🚀 Quickstart
 
-See the [Quickstart.ipynb](Quickstart.ipynb) notebook for a quick introduction to `autodistill`. Below, we have condensed key parts of the notebook for a quick introduction to `autodistill`.
+See the [demo Notebook](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-auto-train-yolov8-model-with-autodistill.ipynb) for a quick introduction to `autodistill`. This notebook walks through building a milk container detection model with no labeling.
+
+Below, we have condensed key parts of the notebook for a quick introduction to `autodistill`.
 
 ### Install Packages
 
 For this example, we'll show how to distill [GroundedSAM](https://github.com/IDEA-Research/Grounded-Segment-Anything) into a small [YOLOv8](https://github.com/ultralytics/ultralytics) model using [autodistill-grounded-sam](https://github.com/autodistill/autodistill-grounded-sam) and [autodistill-yolov8](https://github.com/autodistill/autodistill-yolov8).
 
 ```
 pip install autodistill autodistill-grounded-sam autodistill-yolov8
@@ -226,44 +228,59 @@
 tasks first but plan to launch classification support soon! In the future, we hope `autodistill` will also be used for models beyond computer vision.
 
 * ✅ - complete (click row/column header to go to repo)
 * 🚧 - work in progress
 
 ### object detection
 
-| base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | DETR | YOLOv7 | MT-YOLOv6 |
+| base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | [DETR](https://github.com/autodistill/autodistill-detr) | YOLOv7 | MT-YOLOv6 |
 |:---:|:---:|:---:|:---:|:---:|:---:|:---:|
-| [DETIC](https://github.com/autodistill/autodistill-detic) | ✅ | ✅ | ✅ | 🚧 |  |  |
-| [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | ✅ | ✅ | 🚧 |  |  |
-| GroundingDINO | ✅ | ✅ | ✅ | 🚧 |  |  |
-| [OWL-ViT](https://github.com/autodistill/autodistill-owl-vit) | ✅ | ✅ | ✅ | 🚧 |  |  |
+| [DETIC](https://github.com/autodistill/autodistill-detic) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [GroundingDINO](https://github.com/autodistill/autodistill-grounding-dino) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [OWL-ViT](https://github.com/autodistill/autodistill-owl-vit) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [SAM-CLIP](https://github.com/autodistill/autodistill-sam-clip) | ✅ | ✅ | ✅ | ✅ |  |  |
 | Azure DenseCaptions |  |  |  |  |  |  |
 | GLIPv2 |  |  |  |  |  |  |
-| SAM-CLIP |  |  |  |  |  |  |
 
 
 ### instance segmentation
 
 | base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | YOLOv7 | Segformer |
 |:---:|:---:|:---:|:---:|:---:|:---:|
 | [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | 🚧 | 🚧 |  |  |
-| SAM-CLIP |  |  |  |  |  |
+| SAM-CLIP | 🚧 | 🚧 | 🚧 |  |  |
 
 
 ### classification
 
 | base / target | [ViT](https://github.com/autodistill/autodistill-vit) | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) |
 |:---:|:---:|:---:|:---:|
 | [CLIP](https://github.com/autodistill/autodistill-clip) | 🚧 | 🚧 | 🚧 |
-| BLIP-2 |  |  |  |
-| DINOv2 | 🚧 | 🚧 | 🚧 |
+| [DINOv2](https://github.com/autodistill/autodistill-dinov2) | 🚧 | 🚧 | 🚧 |
+| BLIP | 🚧 | 🚧 | 🚧 |
+| ALBEF | 🚧 | 🚧 | 🚧 |
 | GPT-4 |  |  |  |
 | Open Flamingo |  |  |  |
 | PaLM-2 |  |  |  |
 
+## Roboflow Model Deployment Support
+
+You can optionally deploy some Target Models trained using Autodistill on Roboflow. Deploying on Roboflow allows you to use a range of concise SDKs for using your model on the edge, from [roboflow.js](https://docs.roboflow.com/inference/web-browser) for web deployment to [NVIDIA Jetson](https://docs.roboflow.com/inference/nvidia-jetson) devices.
+
+The following Autodistill Target Models are supported by Roboflow for deployment:
+
+| model name | Supported? |
+|:---:|:---:|
+| YOLOv8 Object Detection | ✅ |
+| YOLOv8 Instance Segmentation | ✅ |
+| YOLOv5 Object Detection | ✅ |
+| YOLOv5 Instance Segmentation | ✅ |
+| YOLOv8 Classification |  |
+
 ## 🎬 Video Guides
 
 <p align="left">
 <a href="https://www.youtube.com/watch?v=gKTYMfwPo4M" title="Autodistill: Train YOLOv8 with ZERO Annotations"><img src="https://i.ytimg.com/vi/gKTYMfwPo4M/maxresdefault.jpg" alt="Autodistill: Train YOLOv8 with ZERO Annotations" width="300px" align="left" /></a>
 <a href="https://youtu.be/oEQYStnF2l8"><strong>Autodistill: Train YOLOv8 with ZERO Annotations</strong></a>
 <div><strong>Published: 8 June 2023</strong></div>
 <br/>In this video, we will show you how to use a new library to train a YOLOv8 model to detect bottles moving on a conveyor line. Yes, that's right - zero annotation hours are required! We dive deep into Autodistill's functionality, covering topics from setting up your Python environment and preparing your images, to the thrilling automatic annotation of images. </p>
```

### Comparing `autodistill-0.1.2/README.md` & `autodistill-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,17 @@
 ```
 </details>
 
 Additional Base and Target models are [enumerated below](#-available-models).
 
 ## 🚀 Quickstart
 
-See the [Quickstart.ipynb](Quickstart.ipynb) notebook for a quick introduction to `autodistill`. Below, we have condensed key parts of the notebook for a quick introduction to `autodistill`.
+See the [demo Notebook](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-auto-train-yolov8-model-with-autodistill.ipynb) for a quick introduction to `autodistill`. This notebook walks through building a milk container detection model with no labeling.
+
+Below, we have condensed key parts of the notebook for a quick introduction to `autodistill`.
 
 ### Install Packages
 
 For this example, we'll show how to distill [GroundedSAM](https://github.com/IDEA-Research/Grounded-Segment-Anything) into a small [YOLOv8](https://github.com/ultralytics/ultralytics) model using [autodistill-grounded-sam](https://github.com/autodistill/autodistill-grounded-sam) and [autodistill-yolov8](https://github.com/autodistill/autodistill-yolov8).
 
 ```
 pip install autodistill autodistill-grounded-sam autodistill-yolov8
@@ -211,44 +213,59 @@
 tasks first but plan to launch classification support soon! In the future, we hope `autodistill` will also be used for models beyond computer vision.
 
 * ✅ - complete (click row/column header to go to repo)
 * 🚧 - work in progress
 
 ### object detection
 
-| base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | DETR | YOLOv7 | MT-YOLOv6 |
+| base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | [DETR](https://github.com/autodistill/autodistill-detr) | YOLOv7 | MT-YOLOv6 |
 |:---:|:---:|:---:|:---:|:---:|:---:|:---:|
-| [DETIC](https://github.com/autodistill/autodistill-detic) | ✅ | ✅ | ✅ | 🚧 |  |  |
-| [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | ✅ | ✅ | 🚧 |  |  |
-| GroundingDINO | ✅ | ✅ | ✅ | 🚧 |  |  |
-| [OWL-ViT](https://github.com/autodistill/autodistill-owl-vit) | ✅ | ✅ | ✅ | 🚧 |  |  |
+| [DETIC](https://github.com/autodistill/autodistill-detic) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [GroundingDINO](https://github.com/autodistill/autodistill-grounding-dino) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [OWL-ViT](https://github.com/autodistill/autodistill-owl-vit) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [SAM-CLIP](https://github.com/autodistill/autodistill-sam-clip) | ✅ | ✅ | ✅ | ✅ |  |  |
 | Azure DenseCaptions |  |  |  |  |  |  |
 | GLIPv2 |  |  |  |  |  |  |
-| SAM-CLIP |  |  |  |  |  |  |
 
 
 ### instance segmentation
 
 | base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | YOLOv7 | Segformer |
 |:---:|:---:|:---:|:---:|:---:|:---:|
 | [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | 🚧 | 🚧 |  |  |
-| SAM-CLIP |  |  |  |  |  |
+| SAM-CLIP | 🚧 | 🚧 | 🚧 |  |  |
 
 
 ### classification
 
 | base / target | [ViT](https://github.com/autodistill/autodistill-vit) | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) |
 |:---:|:---:|:---:|:---:|
 | [CLIP](https://github.com/autodistill/autodistill-clip) | 🚧 | 🚧 | 🚧 |
-| BLIP-2 |  |  |  |
-| DINOv2 | 🚧 | 🚧 | 🚧 |
+| [DINOv2](https://github.com/autodistill/autodistill-dinov2) | 🚧 | 🚧 | 🚧 |
+| BLIP | 🚧 | 🚧 | 🚧 |
+| ALBEF | 🚧 | 🚧 | 🚧 |
 | GPT-4 |  |  |  |
 | Open Flamingo |  |  |  |
 | PaLM-2 |  |  |  |
 
+## Roboflow Model Deployment Support
+
+You can optionally deploy some Target Models trained using Autodistill on Roboflow. Deploying on Roboflow allows you to use a range of concise SDKs for using your model on the edge, from [roboflow.js](https://docs.roboflow.com/inference/web-browser) for web deployment to [NVIDIA Jetson](https://docs.roboflow.com/inference/nvidia-jetson) devices.
+
+The following Autodistill Target Models are supported by Roboflow for deployment:
+
+| model name | Supported? |
+|:---:|:---:|
+| YOLOv8 Object Detection | ✅ |
+| YOLOv8 Instance Segmentation | ✅ |
+| YOLOv5 Object Detection | ✅ |
+| YOLOv5 Instance Segmentation | ✅ |
+| YOLOv8 Classification |  |
+
 ## 🎬 Video Guides
 
 <p align="left">
 <a href="https://www.youtube.com/watch?v=gKTYMfwPo4M" title="Autodistill: Train YOLOv8 with ZERO Annotations"><img src="https://i.ytimg.com/vi/gKTYMfwPo4M/maxresdefault.jpg" alt="Autodistill: Train YOLOv8 with ZERO Annotations" width="300px" align="left" /></a>
 <a href="https://youtu.be/oEQYStnF2l8"><strong>Autodistill: Train YOLOv8 with ZERO Annotations</strong></a>
 <div><strong>Published: 8 June 2023</strong></div>
 <br/>In this video, we will show you how to use a new library to train a YOLOv8 model to detect bottles moving on a conveyor line. Yes, that's right - zero annotation hours are required! We dive deep into Autodistill's functionality, covering topics from setting up your Python environment and preparing your images, to the thrilling automatic annotation of images. </p>
```

### Comparing `autodistill-0.1.2/autodistill/core/base_model.py` & `autodistill-0.1.3/autodistill/core/base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.2/autodistill/detection/caption_ontology.py` & `autodistill-0.1.3/autodistill/detection/caption_ontology.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.2/autodistill/detection/detection_base_model.py` & `autodistill-0.1.3/autodistill/detection/detection_base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.2/autodistill/detection/detection_ontology.py` & `autodistill-0.1.3/autodistill/detection/detection_ontology.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.2/autodistill/helpers.py` & `autodistill-0.1.3/autodistill/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.2/autodistill.egg-info/PKG-INFO` & `autodistill-0.1.3/autodistill.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.2
+Version: 0.1.3
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
@@ -142,15 +142,17 @@
 ```
 </details>
 
 Additional Base and Target models are [enumerated below](#-available-models).
 
 ## 🚀 Quickstart
 
-See the [Quickstart.ipynb](Quickstart.ipynb) notebook for a quick introduction to `autodistill`. Below, we have condensed key parts of the notebook for a quick introduction to `autodistill`.
+See the [demo Notebook](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-auto-train-yolov8-model-with-autodistill.ipynb) for a quick introduction to `autodistill`. This notebook walks through building a milk container detection model with no labeling.
+
+Below, we have condensed key parts of the notebook for a quick introduction to `autodistill`.
 
 ### Install Packages
 
 For this example, we'll show how to distill [GroundedSAM](https://github.com/IDEA-Research/Grounded-Segment-Anything) into a small [YOLOv8](https://github.com/ultralytics/ultralytics) model using [autodistill-grounded-sam](https://github.com/autodistill/autodistill-grounded-sam) and [autodistill-yolov8](https://github.com/autodistill/autodistill-yolov8).
 
 ```
 pip install autodistill autodistill-grounded-sam autodistill-yolov8
@@ -226,44 +228,59 @@
 tasks first but plan to launch classification support soon! In the future, we hope `autodistill` will also be used for models beyond computer vision.
 
 * ✅ - complete (click row/column header to go to repo)
 * 🚧 - work in progress
 
 ### object detection
 
-| base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | DETR | YOLOv7 | MT-YOLOv6 |
+| base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | [DETR](https://github.com/autodistill/autodistill-detr) | YOLOv7 | MT-YOLOv6 |
 |:---:|:---:|:---:|:---:|:---:|:---:|:---:|
-| [DETIC](https://github.com/autodistill/autodistill-detic) | ✅ | ✅ | ✅ | 🚧 |  |  |
-| [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | ✅ | ✅ | 🚧 |  |  |
-| GroundingDINO | ✅ | ✅ | ✅ | 🚧 |  |  |
-| [OWL-ViT](https://github.com/autodistill/autodistill-owl-vit) | ✅ | ✅ | ✅ | 🚧 |  |  |
+| [DETIC](https://github.com/autodistill/autodistill-detic) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [GroundingDINO](https://github.com/autodistill/autodistill-grounding-dino) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [OWL-ViT](https://github.com/autodistill/autodistill-owl-vit) | ✅ | ✅ | ✅ | ✅ |  |  |
+| [SAM-CLIP](https://github.com/autodistill/autodistill-sam-clip) | ✅ | ✅ | ✅ | ✅ |  |  |
 | Azure DenseCaptions |  |  |  |  |  |  |
 | GLIPv2 |  |  |  |  |  |  |
-| SAM-CLIP |  |  |  |  |  |  |
 
 
 ### instance segmentation
 
 | base / target | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLO-NAS](https://github.com/autodistill/autodistill-yolonas) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) | YOLOv7 | Segformer |
 |:---:|:---:|:---:|:---:|:---:|:---:|
 | [GroundedSAM](https://github.com/autodistill/autodistill-grounded-sam) | ✅ | 🚧 | 🚧 |  |  |
-| SAM-CLIP |  |  |  |  |  |
+| SAM-CLIP | 🚧 | 🚧 | 🚧 |  |  |
 
 
 ### classification
 
 | base / target | [ViT](https://github.com/autodistill/autodistill-vit) | [YOLOv8](https://github.com/autodistill/autodistill-yolov8) | [YOLOv5](https://github.com/autodistill/autodistill-yolov5) |
 |:---:|:---:|:---:|:---:|
 | [CLIP](https://github.com/autodistill/autodistill-clip) | 🚧 | 🚧 | 🚧 |
-| BLIP-2 |  |  |  |
-| DINOv2 | 🚧 | 🚧 | 🚧 |
+| [DINOv2](https://github.com/autodistill/autodistill-dinov2) | 🚧 | 🚧 | 🚧 |
+| BLIP | 🚧 | 🚧 | 🚧 |
+| ALBEF | 🚧 | 🚧 | 🚧 |
 | GPT-4 |  |  |  |
 | Open Flamingo |  |  |  |
 | PaLM-2 |  |  |  |
 
+## Roboflow Model Deployment Support
+
+You can optionally deploy some Target Models trained using Autodistill on Roboflow. Deploying on Roboflow allows you to use a range of concise SDKs for using your model on the edge, from [roboflow.js](https://docs.roboflow.com/inference/web-browser) for web deployment to [NVIDIA Jetson](https://docs.roboflow.com/inference/nvidia-jetson) devices.
+
+The following Autodistill Target Models are supported by Roboflow for deployment:
+
+| model name | Supported? |
+|:---:|:---:|
+| YOLOv8 Object Detection | ✅ |
+| YOLOv8 Instance Segmentation | ✅ |
+| YOLOv5 Object Detection | ✅ |
+| YOLOv5 Instance Segmentation | ✅ |
+| YOLOv8 Classification |  |
+
 ## 🎬 Video Guides
 
 <p align="left">
 <a href="https://www.youtube.com/watch?v=gKTYMfwPo4M" title="Autodistill: Train YOLOv8 with ZERO Annotations"><img src="https://i.ytimg.com/vi/gKTYMfwPo4M/maxresdefault.jpg" alt="Autodistill: Train YOLOv8 with ZERO Annotations" width="300px" align="left" /></a>
 <a href="https://youtu.be/oEQYStnF2l8"><strong>Autodistill: Train YOLOv8 with ZERO Annotations</strong></a>
 <div><strong>Published: 8 June 2023</strong></div>
 <br/>In this video, we will show you how to use a new library to train a YOLOv8 model to detect bottles moving on a conveyor line. Yes, that's right - zero annotation hours are required! We dive deep into Autodistill's functionality, covering topics from setting up your Python environment and preparing your images, to the thrilling automatic annotation of images. </p>
```

### Comparing `autodistill-0.1.2/autodistill.egg-info/SOURCES.txt` & `autodistill-0.1.3/autodistill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.2/setup.py` & `autodistill-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel", "mkdocs-material", "mkdocs"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

