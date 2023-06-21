# Comparing `tmp/autodistill-grounding-dino-0.1.0.tar.gz` & `tmp/autodistill-grounding-dino-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-grounding-dino-0.1.0.tar", last modified: Fri Jun  9 11:11:17 2023, max compression
+gzip compressed data, was "autodistill-grounding-dino-0.1.2.tar", last modified: Wed Jun 21 10:39:33 2023, max compression
```

## Comparing `autodistill-grounding-dino-0.1.0.tar` & `autodistill-grounding-dino-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 11:11:17.974494 autodistill-grounding-dino-0.1.0/
--rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-09 09:14:42.000000 autodistill-grounding-dino-0.1.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     2338 2023-06-09 11:11:17.974371 autodistill-grounding-dino-0.1.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1839 2023-06-09 09:17:58.000000 autodistill-grounding-dino-0.1.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 11:11:17.973175 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/
--rw-r--r--   0 james      (501) staff       (20)       97 2023-06-09 09:11:47.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1840 2023-06-09 09:12:09.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/grounding_dino_model.py
--rw-r--r--   0 james      (501) staff       (20)     3531 2023-06-09 09:11:24.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 11:11:17.974182 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2338 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      403 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      155 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       27 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-09 11:11:17.974535 autodistill-grounding-dino-0.1.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1289 2023-06-09 09:13:28.000000 autodistill-grounding-dino-0.1.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:39:33.923429 autodistill-grounding-dino-0.1.2/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-21 10:38:40.000000 autodistill-grounding-dino-0.1.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2343 2023-06-21 10:39:33.923310 autodistill-grounding-dino-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1844 2023-06-21 10:38:40.000000 autodistill-grounding-dino-0.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:39:33.922419 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino/
+-rw-r--r--   0 james      (501) staff       (20)       97 2023-06-21 10:39:04.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1780 2023-06-21 10:38:40.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino/grounding_dino_model.py
+-rw-r--r--   0 james      (501) staff       (20)     3531 2023-06-21 10:38:59.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:39:33.923138 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2343 2023-06-21 10:39:33.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      403 2023-06-21 10:39:33.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-21 10:39:33.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      135 2023-06-21 10:39:33.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       27 2023-06-21 10:39:33.000000 autodistill-grounding-dino-0.1.2/autodistill_grounding_dino.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-21 10:39:33.923471 autodistill-grounding-dino-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1258 2023-06-21 10:39:00.000000 autodistill-grounding-dino-0.1.2/setup.py
```

### Comparing `autodistill-grounding-dino-0.1.0/LICENSE` & `autodistill-grounding-dino-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-grounding-dino-0.1.0/PKG-INFO` & `autodistill-grounding-dino-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-grounding-dino
-Version: 0.1.0
+Version: 0.1.2
 Summary: GroundingDINO module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-grounding-dino
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,19 +26,19 @@
 
 # Autodistill Grounding DINO Module
 
 This repository contains the code supporting the Grounding DINO base model for use with [Autodistill](https://github.com/autodistill/autodistill).
 
 [Grounding DINO](https://github.com/IDEA-Research/GroundingDINO) is a zero-shot object detection model developed by IDEA Research. You can distill knowledge from Grounding DINO into a smaller model using Autodistill.
 
-Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/groundedsam/).
+Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/grounding-dino/).
 
 ## Installation
 
-To use the Grounded SAM base model, you will need to install the following dependency:
+To use the Grounding DINO base model, you will need to install the following dependency:
 
 ```bash
 pip3 install autodistill-grounding-dino
 ```
 
 ## Quickstart
```

### Comparing `autodistill-grounding-dino-0.1.0/README.md` & `autodistill-grounding-dino-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 # Autodistill Grounding DINO Module
 
 This repository contains the code supporting the Grounding DINO base model for use with [Autodistill](https://github.com/autodistill/autodistill).
 
 [Grounding DINO](https://github.com/IDEA-Research/GroundingDINO) is a zero-shot object detection model developed by IDEA Research. You can distill knowledge from Grounding DINO into a smaller model using Autodistill.
 
-Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/groundedsam/).
+Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/grounding-dino/).
 
 ## Installation
 
-To use the Grounded SAM base model, you will need to install the following dependency:
+To use the Grounding DINO base model, you will need to install the following dependency:
 
 ```bash
 pip3 install autodistill-grounding-dino
 ```
 
 ## Quickstart
```

### Comparing `autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/grounding_dino_model.py` & `autodistill-grounding-dino-0.1.2/autodistill_grounding_dino/grounding_dino_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 import torch
 import cv2
 
 torch.use_deterministic_algorithms(False)
 
 import supervision as sv
 from groundingdino.util.inference import Model
-from segment_anything import SamPredictor
-
-import numpy as np
 from autodistill.detection import CaptionOntology, DetectionBaseModel
 
-from autodistill_grounded_sam.helpers import (
+from autodistill_grounding_dino.helpers import (
     combine_detections,
     load_grounding_dino,
 )
 
 HOME = os.path.expanduser("~")
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
```

### Comparing `autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/helpers.py` & `autodistill-grounding-dino-0.1.2/autodistill_grounding_dino/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/PKG-INFO` & `autodistill-grounding-dino-0.1.2/autodistill_grounding_dino.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-grounding-dino
-Version: 0.1.0
+Version: 0.1.2
 Summary: GroundingDINO module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-grounding-dino
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,19 +26,19 @@
 
 # Autodistill Grounding DINO Module
 
 This repository contains the code supporting the Grounding DINO base model for use with [Autodistill](https://github.com/autodistill/autodistill).
 
 [Grounding DINO](https://github.com/IDEA-Research/GroundingDINO) is a zero-shot object detection model developed by IDEA Research. You can distill knowledge from Grounding DINO into a smaller model using Autodistill.
 
-Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/groundedsam/).
+Read the [Grounding DINO Autodistill documentation](https://autodistill.github.io/autodistill/base_models/grounding-dino/).
 
 ## Installation
 
-To use the Grounded SAM base model, you will need to install the following dependency:
+To use the Grounding DINO base model, you will need to install the following dependency:
 
 ```bash
 pip3 install autodistill-grounding-dino
 ```
 
 ## Quickstart
```

### Comparing `autodistill-grounding-dino-0.1.0/setup.py` & `autodistill-grounding-dino-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     url="https://github.com/autodistill/autodistill-grounding-dino",
     install_requires=[
         "torch",
         "autodistill",
         "numpy>=1.20.0",
         "opencv-python>=4.6.0",
         "rf_groundingdino",
-        "rf_segment_anything",
         "supervision"
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
```

