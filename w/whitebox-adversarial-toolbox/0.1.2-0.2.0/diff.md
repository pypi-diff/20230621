# Comparing `tmp/whitebox-adversarial-toolbox-0.1.2.tar.gz` & `tmp/whitebox-adversarial-toolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitebox-adversarial-toolbox-0.1.2.tar", last modified: Fri Jun  9 20:32:46 2023, max compression
+gzip compressed data, was "whitebox-adversarial-toolbox-0.2.0.tar", last modified: Wed Jun 21 10:10:25 2023, max compression
```

## Comparing `whitebox-adversarial-toolbox-0.1.2.tar` & `whitebox-adversarial-toolbox-0.2.0.tar`

### file list

```diff
@@ -1,161 +1,226 @@
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.327180 whitebox-adversarial-toolbox-0.1.2/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/LICENSE
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       66 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/MANIFEST.in
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4259 2023-06-09 20:32:46.327180 whitebox-adversarial-toolbox-0.1.2/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3221 2023-06-09 16:17:26.000000 whitebox-adversarial-toolbox-0.1.2/README.md
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.599179 whitebox-adversarial-toolbox-0.1.2/examples/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.623179 whitebox-adversarial-toolbox-0.1.2/examples/.ipynb_checkpoints/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   584485 2022-08-13 20:41:55.000000 whitebox-adversarial-toolbox-0.1.2/examples/.ipynb_checkpoints/MinM-Attack-ICRA-checkpoint.ipynb
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.647179 whitebox-adversarial-toolbox-0.1.2/examples/__pycache__/
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2640 2022-06-30 13:26:59.000000 whitebox-adversarial-toolbox-0.1.2/examples/__pycache__/logger.cpython-37.pyc
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.779179 whitebox-adversarial-toolbox-0.1.2/examples/attack/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       44 2023-06-06 18:51:35.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/.gitignore
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      705 2022-06-20 17:20:47.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/coco_classes.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    63235 2022-08-11 09:36:40.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/demo.jpg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  1185437 2023-06-09 16:34:39.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/demo.mp4
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  4153472 2023-06-09 15:43:26.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/noise.npy
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4831 2023-06-08 18:41:08.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_evaluation.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3098 2023-06-08 18:41:12.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_image.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3778 2023-06-09 15:44:21.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_universal_video.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4963 2023-06-08 18:43:35.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_universal_voc2012.py
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5441 2023-06-09 20:29:26.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_video.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4888 2023-06-08 18:44:02.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_tog_attack_evaluation.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3192 2023-06-08 18:45:28.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_tog_attack_image.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5429 2023-06-09 20:29:30.000000 whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_tog_attack_video.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.831179 whitebox-adversarial-toolbox-0.1.2/examples/inference/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2449 2023-06-08 16:19:14.000000 whitebox-adversarial-toolbox-0.1.2/examples/inference/faster_rcnn_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1807 2023-06-08 16:19:50.000000 whitebox-adversarial-toolbox-0.1.2/examples/inference/mobilenet_v1_ssd_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1796 2023-06-08 16:19:55.000000 whitebox-adversarial-toolbox-0.1.2/examples/inference/mobilenet_v2_ssd_lite_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1909 2023-06-08 16:13:45.000000 whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov3_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1985 2023-06-08 16:13:57.000000 whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov3_tiny_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1822 2023-06-08 16:14:06.000000 whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov4_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1852 2023-06-08 16:14:17.000000 whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov4_tiny_demo.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.899179 whitebox-adversarial-toolbox-0.1.2/examples/train/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       18 2023-06-06 18:52:43.000000 whitebox-adversarial-toolbox-0.1.2/examples/train/.gitignore
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.919179 whitebox-adversarial-toolbox-0.1.2/examples/train/checkpoint/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       71 2023-06-09 16:42:39.000000 whitebox-adversarial-toolbox-0.1.2/examples/train/checkpoint/.gitignore
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4346 2023-06-06 18:50:41.000000 whitebox-adversarial-toolbox-0.1.2/examples/train/faster_rcnn_train.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4172 2023-06-06 18:49:31.000000 whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v1_ssd_train.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3372 2022-07-04 16:24:25.000000 whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v1_ssd_train_fast.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4199 2023-06-06 18:49:53.000000 whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v2_ssd_lite_train.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3390 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v2_ssd_lite_train_fast.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1476 2023-06-09 16:53:56.000000 whitebox-adversarial-toolbox-0.1.2/pyproject.toml
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-06-09 20:32:46.327180 whitebox-adversarial-toolbox-0.1.2/setup.cfg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2007 2023-06-08 20:03:33.000000 whitebox-adversarial-toolbox-0.1.2/setup.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.943179 whitebox-adversarial-toolbox-0.1.2/tests/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:45.987179 whitebox-adversarial-toolbox-0.1.2/tests/__pycache__/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      163 2023-06-01 14:20:34.000000 whitebox-adversarial-toolbox-0.1.2/tests/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      793 2023-06-01 14:20:36.000000 whitebox-adversarial-toolbox-0.1.2/tests/__pycache__/test_what.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      161 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/tests/test_what.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.011180 whitebox-adversarial-toolbox-0.1.2/what/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4966 2023-06-09 20:00:43.000000 whitebox-adversarial-toolbox-0.1.2/what/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       31 2023-06-01 14:11:31.000000 whitebox-adversarial-toolbox-0.1.2/what/__main__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4345 2023-06-09 13:01:43.000000 whitebox-adversarial-toolbox-0.1.2/what/_main.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.011180 whitebox-adversarial-toolbox-0.1.2/what/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      634 2023-06-09 14:08:02.000000 whitebox-adversarial-toolbox-0.1.2/what/attacks/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.011180 whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      119 2023-06-09 14:09:29.000000 whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.011180 whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/yolo/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3467 2023-06-09 19:39:34.000000 whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/yolo/PCB.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3515 2023-06-09 19:39:30.000000 whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/yolo/TOG.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      399 2023-06-09 14:10:17.000000 whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/yolo/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.035179 whitebox-adversarial-toolbox-0.1.2/what/cli/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      190 2023-06-09 19:59:11.000000 whitebox-adversarial-toolbox-0.1.2/what/cli/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      308 2023-06-06 15:06:36.000000 whitebox-adversarial-toolbox-0.1.2/what/cli/attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1231 2023-06-09 19:57:45.000000 whitebox-adversarial-toolbox-0.1.2/what/cli/example.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2874 2023-06-08 19:49:22.000000 whitebox-adversarial-toolbox-0.1.2/what/cli/model.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.039179 whitebox-adversarial-toolbox-0.1.2/what/examples/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1562 2023-06-09 14:14:25.000000 whitebox-adversarial-toolbox-0.1.2/what/examples/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2723 2023-06-08 16:13:19.000000 whitebox-adversarial-toolbox-0.1.2/what/examples/faster_rcnn_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3237 2023-06-08 16:20:25.000000 whitebox-adversarial-toolbox-0.1.2/what/examples/mobilenet_ssd_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3027 2023-06-08 15:58:16.000000 whitebox-adversarial-toolbox-0.1.2/what/examples/yolov3_demo.py
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4346 2023-06-09 20:28:53.000000 whitebox-adversarial-toolbox-0.1.2/what/examples/yolov3_pcb_attack_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4226 2023-06-09 20:28:59.000000 whitebox-adversarial-toolbox-0.1.2/what/examples/yolov3_tog_attack_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2999 2023-06-08 19:48:12.000000 whitebox-adversarial-toolbox-0.1.2/what/examples/yolov4_demo.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.039179 whitebox-adversarial-toolbox-0.1.2/what/models/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1298 2023-06-09 14:03:33.000000 whitebox-adversarial-toolbox-0.1.2/what/models/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.039179 whitebox-adversarial-toolbox-0.1.2/what/models/detection/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      310 2023-06-09 14:15:42.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.039179 whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2466 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/coco.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2664 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/fiftyone.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4823 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/open_images.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5154 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/voc.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.043180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      213 2023-06-09 19:28:40.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.075179 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:10:38.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3936 2023-06-09 18:42:48.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/dataset.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9989 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/util.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5592 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/voc_dataset.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10716 2023-06-09 18:48:38.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/faster_rcnn.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.111180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/meter/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1188 2023-06-09 18:49:26.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/meter/averagevalue_meter.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3353 2023-06-09 18:49:40.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/meter/confusion_meter.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      544 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/meter/meter.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.151180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:03:08.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12038 2023-06-09 18:40:50.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/faster_rcnn_model.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5507 2023-06-09 18:41:40.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/faster_rcnn_vgg16.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7975 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/region_proposal_network.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.171180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8810 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/utils/bbox_tools.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    16788 2023-06-09 18:41:58.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/utils/creator_tool.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.211180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:30:17.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1712 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/utils/config.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12665 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/utils/eval_tool.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.219180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      374 2023-06-09 19:29:20.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8043 2023-06-09 18:38:37.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/mobilenet_v1_ssd.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8113 2023-06-09 18:38:44.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/mobilenet_v2_ssd_lite.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.227180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1673 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/mobilenet_v1.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6607 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/mobilenet_v2.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8233 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/mobilenet_v3.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4876 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/squeezenet.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.291180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      624 2023-06-09 18:43:13.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_ssd_config.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3183 2023-06-09 18:43:24.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3607 2023-06-09 18:43:33.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3500 2023-06-09 18:46:50.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5319 2023-06-01 14:09:32.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1966 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/multibox_loss.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3150 2022-06-20 18:22:30.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/predictor.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1773 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/preprocessing.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      617 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/squeezenet_ssd_config.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3817 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7027 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/ssd.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.307180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/transforms/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    13325 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/transforms/transforms.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.311180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10937 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/utils/box_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      535 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/utils/misc.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.311180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      153 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      589 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/utils/array_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1233 2022-06-20 17:46:01.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/utils/box_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      403 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/utils/time_utils.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.315180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      525 2023-06-09 19:29:57.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.315180 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3470 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/utils/yolo_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      896 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov3.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      911 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov3_tiny.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1040 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov4.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1101 2023-06-06 15:51:49.000000 whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov4_tiny.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.323180 whitebox-adversarial-toolbox-0.1.2/what/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      267 2023-06-09 20:09:37.000000 whitebox-adversarial-toolbox-0.1.2/what/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2397 2023-06-09 20:08:01.000000 whitebox-adversarial-toolbox-0.1.2/what/utils/file.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3522 2022-06-30 13:51:17.000000 whitebox-adversarial-toolbox-0.1.2/what/utils/logger.py
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      477 2022-06-21 20:00:37.000000 whitebox-adversarial-toolbox-0.1.2/what/utils/proj.py
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1054 2022-06-21 19:32:15.000000 whitebox-adversarial-toolbox-0.1.2/what/utils/resize.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:32:46.327180 whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4259 2023-06-09 20:32:45.000000 whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4952 2023-06-09 20:32:45.000000 whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-06-09 20:32:45.000000 whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       41 2023-06-09 20:32:45.000000 whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      126 2023-06-09 20:32:45.000000 whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/requires.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        5 2023-06-09 20:32:45.000000 whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/top_level.txt
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/LICENSE
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       66 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/MANIFEST.in
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4257 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3219 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/README.md
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.369785 whitebox-adversarial-toolbox-0.2.0/docs/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       19 2023-06-09 20:43:02.000000 whitebox-adversarial-toolbox-0.2.0/docs/CNAME
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.457785 whitebox-adversarial-toolbox-0.2.0/docs/images/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  5657169 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/demo.gif
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   124402 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what.eps
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  1070518 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what.png
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    77237 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what.psd
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   187801 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what_logo.psd
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      135 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    84252 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/search.js
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    76595 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/_main.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   113391 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo/PCB.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   118219 2023-06-21 10:07:54.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo/TOG.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37957 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36618 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39361 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37675 2023-06-21 10:07:54.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/cli.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    72344 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/faster_rcnn_demo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79798 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/mobilenet_ssd_demo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    75940 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov3_demo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    92781 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov3_pcb_attack_demo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    90861 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov3_tog_attack_demo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    75508 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov4_demo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    44796 2023-06-21 10:07:54.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    48520 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/coco.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    82238 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/fiftyone.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   120100 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/open_images.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   121756 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/voc.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    35417 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/frcnn/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241300 2023-06-21 10:07:57.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/frcnn/faster_rcnn.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37384 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/frcnn.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   190796 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd/mobilenet_v1_ssd.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   194634 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd/mobilenet_v2_ssd_lite.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38242 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    48496 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/array_utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    58750 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/box_utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    47979 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/time_utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36304 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    55703 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov3.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    56188 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov3_tiny.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    59301 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov4.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    60668 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov4_tiny.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39565 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38012 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    40578 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    69669 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/file.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   110443 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/logger.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43089 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/proj.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    56657 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/resize.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38053 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57945 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.337786 whitebox-adversarial-toolbox-0.2.0/examples/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/examples/.ipynb_checkpoints/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   584485 2022-08-13 20:41:55.000000 whitebox-adversarial-toolbox-0.2.0/examples/.ipynb_checkpoints/MinM-Attack-ICRA-checkpoint.ipynb
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.489784 whitebox-adversarial-toolbox-0.2.0/examples/__pycache__/
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2640 2022-06-30 13:26:59.000000 whitebox-adversarial-toolbox-0.2.0/examples/__pycache__/logger.cpython-37.pyc
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.741782 whitebox-adversarial-toolbox-0.2.0/examples/attack/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       44 2023-06-06 18:51:35.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/.gitignore
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      705 2022-06-20 17:20:47.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/coco_classes.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    63235 2022-08-11 09:36:40.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/demo.jpg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  1185437 2023-06-09 16:34:39.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/demo.mp4
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  4153472 2023-06-09 15:43:26.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/noise.npy
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4831 2023-06-08 18:41:08.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_evaluation.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3098 2023-06-08 18:41:12.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_image.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3778 2023-06-09 15:44:21.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_universal_video.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4963 2023-06-08 18:43:35.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_universal_voc2012.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5441 2023-06-09 20:43:07.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_video.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4888 2023-06-08 18:44:02.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_evaluation.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3192 2023-06-08 18:45:28.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_image.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5429 2023-06-09 20:43:07.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_video.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.777782 whitebox-adversarial-toolbox-0.2.0/examples/inference/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2449 2023-06-08 16:19:14.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/faster_rcnn_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1910 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/mobilenet_v1_ssd_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1903 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/mobilenet_v2_ssd_lite_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1909 2023-06-08 16:13:45.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1985 2023-06-08 16:13:57.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_tiny_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1822 2023-06-08 16:14:06.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov4_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1852 2023-06-08 16:14:17.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov4_tiny_demo.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.845781 whitebox-adversarial-toolbox-0.2.0/examples/train/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       18 2023-06-06 18:52:43.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/.gitignore
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.865781 whitebox-adversarial-toolbox-0.2.0/examples/train/checkpoint/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       71 2023-06-09 16:42:39.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/checkpoint/.gitignore
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4346 2023-06-06 18:50:41.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/faster_rcnn_train.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4172 2023-06-06 18:49:31.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v1_ssd_train.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3372 2022-07-04 16:24:25.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v1_ssd_train_fast.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4199 2023-06-06 18:49:53.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v2_ssd_lite_train.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3390 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v2_ssd_lite_train_fast.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1476 2023-06-21 10:06:15.000000 whitebox-adversarial-toolbox-0.2.0/pyproject.toml
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/setup.cfg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2007 2023-06-08 20:03:33.000000 whitebox-adversarial-toolbox-0.2.0/setup.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.865781 whitebox-adversarial-toolbox-0.2.0/tests/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.905780 whitebox-adversarial-toolbox-0.2.0/tests/__pycache__/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      163 2023-06-01 14:20:34.000000 whitebox-adversarial-toolbox-0.2.0/tests/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      793 2023-06-01 14:20:36.000000 whitebox-adversarial-toolbox-0.2.0/tests/__pycache__/test_what.cpython-38-pytest-7.3.1.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      161 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/tests/test_what.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.937780 whitebox-adversarial-toolbox-0.2.0/what/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4966 2023-06-21 10:06:21.000000 whitebox-adversarial-toolbox-0.2.0/what/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       31 2023-06-01 14:11:31.000000 whitebox-adversarial-toolbox-0.2.0/what/__main__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4345 2023-06-09 13:01:43.000000 whitebox-adversarial-toolbox-0.2.0/what/_main.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.941780 whitebox-adversarial-toolbox-0.2.0/what/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      634 2023-06-09 14:08:02.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.941780 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      119 2023-06-09 14:09:29.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.941780 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3467 2023-06-09 19:39:34.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/PCB.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3515 2023-06-09 19:39:30.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/TOG.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      399 2023-06-09 14:10:17.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.965780 whitebox-adversarial-toolbox-0.2.0/what/cli/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      190 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      308 2023-06-06 15:06:36.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1231 2023-06-09 19:57:45.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/example.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2874 2023-06-08 19:49:22.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/model.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/examples/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1562 2023-06-09 14:14:25.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2723 2023-06-08 16:13:19.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/faster_rcnn_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3416 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/mobilenet_ssd_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3027 2023-06-08 15:58:16.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4346 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_pcb_attack_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4226 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_tog_attack_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2999 2023-06-08 19:48:12.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov4_demo.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1298 2023-06-09 14:03:33.000000 whitebox-adversarial-toolbox-0.2.0/what/models/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      310 2023-06-09 14:15:42.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2466 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/coco.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2664 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/fiftyone.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4823 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/open_images.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5154 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/voc.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      213 2023-06-09 19:28:40.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.033779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:10:38.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3936 2023-06-09 18:42:48.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/dataset.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9989 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/util.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5592 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/voc_dataset.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10716 2023-06-09 18:48:38.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/faster_rcnn.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.105778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1188 2023-06-09 18:49:26.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/averagevalue_meter.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3353 2023-06-09 18:49:40.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/confusion_meter.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      544 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/meter.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.129778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:03:08.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12038 2023-06-09 18:40:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_model.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5507 2023-06-09 18:41:40.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_vgg16.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7975 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/region_proposal_network.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.145778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8810 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/bbox_tools.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    16788 2023-06-09 18:41:58.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/creator_tool.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.189777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:30:17.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1712 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/config.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12665 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/eval_tool.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.197777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      374 2023-06-09 19:29:20.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7597 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v1_ssd.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7730 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v2_ssd_lite.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.205778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1673 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v1.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6607 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v2.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8233 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v3.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4876 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/squeezenet.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.261777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      624 2023-06-09 18:43:13.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_ssd_config.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3183 2023-06-09 18:43:24.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3607 2023-06-09 18:43:33.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3500 2023-06-09 18:46:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5319 2023-06-01 14:09:32.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1966 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/multibox_loss.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3150 2022-06-20 18:22:30.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/predictor.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1773 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/preprocessing.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      617 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_config.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3817 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7027 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/ssd.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.277777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/transforms/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    13325 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/transforms/transforms.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.277777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10937 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/box_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      535 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/misc.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.281777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      153 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      589 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/array_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1233 2022-06-20 17:46:01.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/box_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      403 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/time_utils.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.281777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      525 2023-06-09 19:29:57.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.281777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3470 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/utils/yolo_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      896 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      911 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3_tiny.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1040 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1101 2023-06-06 15:51:49.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4_tiny.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/what/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      267 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2397 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/file.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3522 2022-06-30 13:51:17.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/logger.py
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      477 2022-06-21 20:00:37.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/proj.py
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1054 2022-06-21 19:32:15.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/resize.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4257 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6718 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       41 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      126 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        5 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/top_level.txt
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/LICENSE` & `whitebox-adversarial-toolbox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/PKG-INFO` & `whitebox-adversarial-toolbox-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitebox-adversarial-toolbox
-Version: 0.1.2
+Version: 0.2.0
 Summary: WHite-box Adversarial Toolbox (WHAT) - Python Library for Deep Learning Security
 Home-page: https://github.com/wuhanstudio/whitebox-adversarial-toolbox
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
@@ -26,15 +26,15 @@
 # WHite-box Adversarial Toolbox (WHAT)
 
 <!-- [![CircleCI](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox.svg?style=svg)](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox) -->
 [![Build Status](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox.svg?branch=master)](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox)
 [![PyPI version](https://badge.fury.io/py/whitebox-adversarial-toolbox.svg)](https://badge.fury.io/py/whitebox-adversarial-toolbox)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whitebox-adversarial-toolbox)](https://pypi.org/project/whitebox-adversarial-toolbox/)
-[![](https://img.shields.io/badge/Documentation-infromational)](https://what.wuhanstudio.uk/)
+[![](https://img.shields.io/badge/Documentation-brightgreen)](https://what.wuhanstudio.uk/)
 
 A Python Library for Deep Learning Security that focuses on Real-time White-box Attacks.
 
 ![](docs/images/demo.gif)
 
 ## Installation
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/README.md` & `whitebox-adversarial-toolbox-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # WHite-box Adversarial Toolbox (WHAT)
 
 <!-- [![CircleCI](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox.svg?style=svg)](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox) -->
 [![Build Status](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox.svg?branch=master)](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox)
 [![PyPI version](https://badge.fury.io/py/whitebox-adversarial-toolbox.svg)](https://badge.fury.io/py/whitebox-adversarial-toolbox)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whitebox-adversarial-toolbox)](https://pypi.org/project/whitebox-adversarial-toolbox/)
-[![](https://img.shields.io/badge/Documentation-infromational)](https://what.wuhanstudio.uk/)
+[![](https://img.shields.io/badge/Documentation-brightgreen)](https://what.wuhanstudio.uk/)
 
 A Python Library for Deep Learning Security that focuses on Real-time White-box Attacks.
 
 ![](docs/images/demo.gif)
 
 ## Installation
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/.ipynb_checkpoints/MinM-Attack-ICRA-checkpoint.ipynb` & `whitebox-adversarial-toolbox-0.2.0/examples/.ipynb_checkpoints/MinM-Attack-ICRA-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/__pycache__/logger.cpython-37.pyc` & `whitebox-adversarial-toolbox-0.2.0/examples/__pycache__/logger.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/coco_classes.txt` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/coco_classes.txt`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/demo.jpg` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/demo.jpg`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/demo.mp4` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/demo.mp4`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/noise.npy` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/noise.npy`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_evaluation.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_evaluation.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_image.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_image.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_universal_video.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_universal_video.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_universal_voc2012.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_universal_voc2012.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_pcb_attack_video.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_video.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_tog_attack_evaluation.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_evaluation.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_tog_attack_image.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_image.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/attack/yolov3_tog_attack_video.py` & `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_video.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/inference/faster_rcnn_demo.py` & `whitebox-adversarial-toolbox-0.2.0/examples/inference/faster_rcnn_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/inference/mobilenet_v1_ssd_demo.py` & `whitebox-adversarial-toolbox-0.2.0/examples/inference/mobilenet_v1_ssd_demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import torch
 
 from what.cli.model import *
 from what.utils.file import get_file
 
 from what.models.detection.ssd.mobilenet_v1_ssd import MobileNetV1SSD
 from what.models.detection.utils.box_utils import draw_bounding_boxes
+from what.models.detection.datasets.voc import VOC_CLASS_NAMES
 
 device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
 
 video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
 while not video.isdigit():
     video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
@@ -26,14 +27,15 @@
     get_file(what_model_list[index][WHAT_MODEL_FILE_INDEX],
                 WHAT_MODEL_PATH,
                 what_model_list[index][WHAT_MODEL_URL_INDEX],
                 what_model_list[index][WHAT_MODEL_HASH_INDEX])
 
 # Initialize the model
 model = MobileNetV1SSD(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX]),
+                       VOC_CLASS_NAMES,
                        is_test=True,
                        device=device)
 
 while True:
     _, orig_image = cap.read()
     if orig_image is None:
         continue
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/inference/mobilenet_v2_ssd_lite_demo.py` & `whitebox-adversarial-toolbox-0.2.0/examples/inference/mobilenet_v2_ssd_lite_demo.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import torch
 
 from what.cli.model import *
 from what.utils.file import get_file
 
 from what.models.detection.ssd.mobilenet_v2_ssd_lite import MobileNetV2SSDLite
 from what.models.detection.utils.box_utils import draw_bounding_boxes
+from what.models.detection.datasets.voc import VOC_CLASS_NAMES
 
 device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
 
 video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
 while not video.isdigit():
     video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
@@ -26,14 +27,15 @@
     get_file(what_model_list[index][WHAT_MODEL_FILE_INDEX],
                 WHAT_MODEL_PATH,
                 what_model_list[index][WHAT_MODEL_URL_INDEX],
                 what_model_list[index][WHAT_MODEL_HASH_INDEX])
 
 # Initialize the model
 model = MobileNetV2SSDLite(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX]),
+                           VOC_CLASS_NAMES,
                            is_test=True,
                            device=device)
 
 while True:
     _, orig_image = cap.read()
     if orig_image is None:
         continue
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov3_demo.py` & `whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov3_tiny_demo.py` & `whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_tiny_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov4_demo.py` & `whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov4_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/inference/yolov4_tiny_demo.py` & `whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov4_tiny_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/train/faster_rcnn_train.py` & `whitebox-adversarial-toolbox-0.2.0/examples/train/faster_rcnn_train.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v1_ssd_train.py` & `whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v1_ssd_train.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v1_ssd_train_fast.py` & `whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v1_ssd_train_fast.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v2_ssd_lite_train.py` & `whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v2_ssd_lite_train.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/examples/train/mobilenet_v2_ssd_lite_train_fast.py` & `whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v2_ssd_lite_train_fast.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/pyproject.toml` & `whitebox-adversarial-toolbox-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "click",
     "progressbar",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitebox-adversarial-toolbox"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 maintainers = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 description = "WHite-box Adversarial Toolbox (WHAT) - Python Library for Deep Learning Security"
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/setup.py` & `whitebox-adversarial-toolbox-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/tests/__pycache__/test_what.cpython-38-pytest-7.3.1.pyc` & `whitebox-adversarial-toolbox-0.2.0/tests/__pycache__/test_what.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/__init__.py` & `whitebox-adversarial-toolbox-0.2.0/what/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 
 # Project Imports
 from what import models
 from what import attacks
 from what import utils
 
 # Semantic Version
-__version__ = "0.1.2"
+__version__ = "0.2.0"
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/_main.py` & `whitebox-adversarial-toolbox-0.2.0/what/_main.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/attacks/__init__.py` & `whitebox-adversarial-toolbox-0.2.0/what/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/yolo/PCB.py` & `whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/PCB.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/attacks/detection/yolo/TOG.py` & `whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/TOG.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/cli/example.py` & `whitebox-adversarial-toolbox-0.2.0/what/cli/example.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/cli/model.py` & `whitebox-adversarial-toolbox-0.2.0/what/cli/model.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/examples/__init__.py` & `whitebox-adversarial-toolbox-0.2.0/what/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/examples/faster_rcnn_demo.py` & `whitebox-adversarial-toolbox-0.2.0/what/examples/faster_rcnn_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/examples/mobilenet_ssd_demo.py` & `whitebox-adversarial-toolbox-0.2.0/what/examples/mobilenet_ssd_demo.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import torch
 
 from what.cli.model import *
 from what.utils.file import get_file
 
 from what.models.detection.ssd.mobilenet_v1_ssd import MobileNetV1SSD
 from what.models.detection.ssd.mobilenet_v2_ssd_lite import MobileNetV2SSDLite
+from what.models.detection.datasets.voc import VOC_CLASS_NAMES
 
 from what.models.detection.utils.box_utils import draw_bounding_boxes
 
 device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
 
 what_ssd_model_list = what_model_list[6:8]
 
@@ -36,22 +37,24 @@
                     WHAT_MODEL_PATH,
                     what_ssd_model_list[index][WHAT_MODEL_URL_INDEX],
                     what_ssd_model_list[index][WHAT_MODEL_HASH_INDEX])
 
     if index == 0:
         # Initialize the model
         model = MobileNetV1SSD(os.path.join(WHAT_MODEL_PATH, what_ssd_model_list[index][WHAT_MODEL_FILE_INDEX]),
-                            is_test=True,
-                            device=device)
+                               VOC_CLASS_NAMES,
+                               is_test=True,
+                               device=device)
 
     if index == 1:
         # Initialize the model
-        model = MobileNetV2SSDLite(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX]),
-                                is_test=True,
-                                device=device)
+        model = MobileNetV2SSDLite(os.path.join(WHAT_MODEL_PATH, what_ssd_model_list[index][WHAT_MODEL_FILE_INDEX]),
+                                   VOC_CLASS_NAMES,
+                                   is_test=True,
+                                   device=device)
 
     video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
     while not video.isdigit():
         video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
     # Capture from camera
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/examples/yolov3_demo.py` & `whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/examples/yolov3_pcb_attack_demo.py` & `whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_pcb_attack_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/examples/yolov3_tog_attack_demo.py` & `whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_tog_attack_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/examples/yolov4_demo.py` & `whitebox-adversarial-toolbox-0.2.0/what/examples/yolov4_demo.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/__init__.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/__init__.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/coco.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/fiftyone.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/fiftyone.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/open_images.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/open_images.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/datasets/voc.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/dataset.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/util.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/util.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/datasets/voc_dataset.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/voc_dataset.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/faster_rcnn.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/meter/averagevalue_meter.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/averagevalue_meter.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/meter/confusion_meter.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/confusion_meter.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/meter/meter.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/meter.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/faster_rcnn_model.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_model.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/faster_rcnn_vgg16.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_vgg16.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/region_proposal_network.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/region_proposal_network.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/utils/bbox_tools.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/bbox_tools.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/model/utils/creator_tool.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/creator_tool.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/utils/config.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/config.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/frcnn/utils/eval_tool.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/eval_tool.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/mobilenet_v1_ssd.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v1_ssd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 import os
 import itertools
 
 import torch
 from torch.optim.lr_scheduler import CosineAnnealingLR
 
-from what.models.detection.datasets.voc import VOC_CLASS_NAMES
 import what.utils.logger as log
 
 from .ssd.mobilenet_v1_ssd_create import create_mobilenet_v1_ssd, create_mobilenet_v1_ssd_predictor
 from .ssd.multibox_loss import MultiboxLoss
 from .ssd import mobilenet_ssd_config
 
 from .utils.misc import freeze_net_layers
 
 logger = log.get_logger(__name__)
 
 class MobileNetV1SSD:
-    def __init__(self, class_names = None, model_path=None, pretrained=None, is_test=False, device=None):
+    def __init__(self, model_path, class_names, is_test=False, device=None):
 
-        if class_names is None:
-            self.class_names = VOC_CLASS_NAMES
-        else:
-            self.class_names = class_names
+        self.class_names = class_names
 
         self.net = create_mobilenet_v1_ssd(len(self.class_names), is_test=is_test)
 
-        if model_path is not None:
-            pretrained = False
-
         self.predictor = None;
         self.device = device;
 
-        if pretrained is True:
-            self.net.load("https://storage.googleapis.com/models-hao/mobilenet-v1-ssd-mp-0_675.pth", pretrained=True)
-        elif model_path is not None:
-            self.net.load(model_path)
+        self.net.load(model_path)
 
     def predict(self, image, top_k=-1, prob_threshold=None):
         if self.predictor is None:
             self.predictor = create_mobilenet_v1_ssd_predictor(self.net, device=self.device, candidate_size=200)
 
         return self.predictor.predict(image, top_k, prob_threshold)
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/mobilenet_v2_ssd_lite.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v2_ssd_lite.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,33 +13,24 @@
 from .utils.misc import freeze_net_layers
 
 logger = log.get_logger(__name__)
 
 from what.models.detection.datasets.voc import VOC_CLASS_NAMES
 
 class MobileNetV2SSDLite:
-    def __init__(self, class_names = None, model_path = None, pretrained = None, width_mult = 1.0, is_test=False, device=None):
+    def __init__(self, model_path, class_names, width_mult = 1.0, is_test=False, device=None):
 
-        if class_names is None:
-            self.class_names = VOC_CLASS_NAMES
-        else:
-            self.class_names = class_names
+        self.class_names = class_names
 
         self.net = create_mobilenet_v2_ssd_lite(len(self.class_names), is_test=is_test, width_mult=width_mult)
 
-        if model_path is not None:
-            pretrained = False
-
         self.predictor = None;
         self.device = device;
 
-        if pretrained is True:
-            self.net.load("https://storage.googleapis.com/models-hao/mb2-ssd-lite-mp-0_686.pth", pretrained=True)
-        elif model_path is not None:
-            self.net.load(model_path)
+        self.net.load(model_path)
 
     def predict(self, image, top_k=-1, prob_threshold=None):
         if self.predictor is None:
             self.predictor = create_mobilenet_v2_ssd_lite_predictor(self.net, candidate_size=200, device=self.device)
 
         return self.predictor.predict(image, top_k, prob_threshold)
```

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/mobilenet_v1.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/mobilenet_v2.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/mobilenet_v3.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/nn/squeezenet.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/squeezenet.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_ssd_config.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_ssd_config.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/multibox_loss.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/multibox_loss.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/predictor.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/predictor.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/preprocessing.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/squeezenet_ssd_config.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_config.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/ssd/ssd.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/ssd.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/transforms/transforms.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/utils/box_utils.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/ssd/utils/misc.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/misc.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/utils/array_utils.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/utils/box_utils.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/__init__.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/__init__.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/utils/yolo_utils.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/utils/yolo_utils.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov3.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov3_tiny.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3_tiny.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov4.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/models/detection/yolo/yolov4_tiny.py` & `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4_tiny.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/utils/file.py` & `whitebox-adversarial-toolbox-0.2.0/what/utils/file.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/utils/logger.py` & `whitebox-adversarial-toolbox-0.2.0/what/utils/logger.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/what/utils/resize.py` & `whitebox-adversarial-toolbox-0.2.0/what/utils/resize.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.1.2/whitebox_adversarial_toolbox.egg-info/PKG-INFO` & `whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitebox-adversarial-toolbox
-Version: 0.1.2
+Version: 0.2.0
 Summary: WHite-box Adversarial Toolbox (WHAT) - Python Library for Deep Learning Security
 Home-page: https://github.com/wuhanstudio/whitebox-adversarial-toolbox
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
@@ -26,15 +26,15 @@
 # WHite-box Adversarial Toolbox (WHAT)
 
 <!-- [![CircleCI](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox.svg?style=svg)](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox) -->
 [![Build Status](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox.svg?branch=master)](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox)
 [![PyPI version](https://badge.fury.io/py/whitebox-adversarial-toolbox.svg)](https://badge.fury.io/py/whitebox-adversarial-toolbox)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whitebox-adversarial-toolbox)](https://pypi.org/project/whitebox-adversarial-toolbox/)
-[![](https://img.shields.io/badge/Documentation-infromational)](https://what.wuhanstudio.uk/)
+[![](https://img.shields.io/badge/Documentation-brightgreen)](https://what.wuhanstudio.uk/)
 
 A Python Library for Deep Learning Security that focuses on Real-time White-box Attacks.
 
 ![](docs/images/demo.gif)
 
 ## Installation
```

