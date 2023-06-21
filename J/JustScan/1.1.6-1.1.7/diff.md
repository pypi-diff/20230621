# Comparing `tmp/JustScan-1.1.6.tar.gz` & `tmp/JustScan-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustScan-1.1.6.tar", last modified: Wed Jun 21 02:52:12 2023, max compression
+gzip compressed data, was "JustScan-1.1.7.tar", last modified: Wed Jun 21 02:53:56 2023, max compression
```

## Comparing `JustScan-1.1.6.tar` & `JustScan-1.1.7.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.502341 JustScan-1.1.6/
--rw-r--r--   0 macbook    (501) staff       (20)     2638 2023-06-21 02:52:12.502157 JustScan-1.1.6/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-1.1.6/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.471528 JustScan-1.1.6/app/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.476414 JustScan-1.1.6/app/JustScan/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 17:20:30.000000 JustScan-1.1.6/app/JustScan/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.478174 JustScan-1.1.6/app/JustScan/api/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-1.1.6/app/JustScan/api/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-20 10:57:02.000000 JustScan-1.1.6/app/JustScan/api/itc_cli.py
--rw-r--r--   0 macbook    (501) staff       (20)     5520 2023-06-20 17:06:38.000000 JustScan-1.1.6/app/JustScan/api/just_scan_api.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.479092 JustScan-1.1.6/app/JustScan/config/
--rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-1.1.6/app/JustScan/config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-1.1.6/app/JustScan/config/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-1.1.6/app/JustScan/config/config_db.py
--rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-1.1.6/app/JustScan/config/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-1.1.6/app/JustScan/config/pydantic_models.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.480035 JustScan-1.1.6/app/JustScan/database/
--rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-1.1.6/app/JustScan/database/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     4411 2023-06-21 02:51:05.000000 JustScan-1.1.6/app/JustScan/database/crud.py
--rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-1.1.6/app/JustScan/database/data_models.py
--rw-r--r--   0 macbook    (501) staff       (20)      570 2023-06-20 17:06:38.000000 JustScan-1.1.6/app/JustScan/database/database.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.480291 JustScan-1.1.6/app/JustScan/face_id/
--rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-1.1.6/app/JustScan/face_id/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.480590 JustScan-1.1.6/app/JustScan/face_id/commons/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.481518 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/
--rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.482032 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/data_io/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)    11469 2023-06-21 02:49:42.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
--rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
--rw-r--r--   0 macbook    (501) staff       (20)     1402 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.482494 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/model_lib/
--rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
--rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/utility.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.482818 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/
--rw-r--r--   0 macbook    (501) staff       (20)     3004 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)      983 2023-06-21 02:52:02.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.483495 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/
--rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/layers.py
--rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/models.py
--rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.484000 JustScan-1.1.6/app/JustScan/face_id/commons/CloseEyes/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/CloseEyes/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1104 2023-06-20 17:27:59.000000 JustScan-1.1.6/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
--rw-r--r--   0 macbook    (501) staff       (20)     1315 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/face_id/commons/CloseEyes/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.484348 JustScan-1.1.6/app/JustScan/face_id/commons/FaceMask/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/FaceMask/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      812 2023-06-20 17:27:59.000000 JustScan-1.1.6/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.484831 JustScan-1.1.6/app/JustScan/face_id/commons/FaceQuality/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/FaceQuality/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-1.1.6/app/JustScan/face_id/commons/FaceQuality/dom.py
--rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-1.1.6/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.488316 JustScan-1.1.6/app/JustScan/face_id/commons/ScrFd/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ScrFd/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 JustScan-1.1.6/app/JustScan/face_id/commons/ScrFd/scrfd.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.6/app/JustScan/face_id/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-1.1.6/app/JustScan/face_id/commons/config.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.489184 JustScan-1.1.6/app/JustScan/face_id/libraries/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.6/app/JustScan/face_id/libraries/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7235 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/face_id/libraries/face_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     5325 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/face_id/libraries/face_id.py
--rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-1.1.6/app/JustScan/face_id/libraries/face_recognition.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.489544 JustScan-1.1.6/app/JustScan/face_id/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.6/app/JustScan/face_id/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3955 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/face_id/tools/modules.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.489709 JustScan-1.1.6/app/JustScan/ocr/
--rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-1.1.6/app/JustScan/ocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.489872 JustScan-1.1.6/app/JustScan/ocr/core/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.490835 JustScan-1.1.6/app/JustScan/ocr/core/commons/
--rw-r--r--   0 macbook    (501) staff       (20)      814 2023-06-20 08:24:37.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/SpoofingNID.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5592 2023-06-20 08:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/id_card_classification.py
--rw-r--r--   0 macbook    (501) staff       (20)     5675 2023-06-20 10:04:38.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/id_card_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     1761 2023-06-20 08:22:16.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/merge_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.491133 JustScan-1.1.6/app/JustScan/ocr/core/commons/utils/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/utils/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2513 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/commons/utils/utils_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.491301 JustScan-1.1.6/app/JustScan/ocr/core/modules/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.491733 JustScan-1.1.6/app/JustScan/ocr/core/modules/corner_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/corner_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
--rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/corner_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.492042 JustScan-1.1.6/app/JustScan/ocr/core/modules/id_card_classification/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      923 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/id_card_classification/classify.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.492488 JustScan-1.1.6/app/JustScan/ocr/core/modules/mrc/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/mrc/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2938 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/mrc/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.493084 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9072 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/passport.py
--rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/passport_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.493642 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_align_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.494016 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9668 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.494335 JustScan-1.1.6/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2927 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.494667 JustScan-1.1.6/app/JustScan/ocr/core/modules/spell_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/spell_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.494954 JustScan-1.1.6/app/JustScan/ocr/core/modules/spoofing_nid/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      935 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.495450 JustScan-1.1.6/app/JustScan/ocr/core/modules/text_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/text_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7020 2023-06-20 08:33:20.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/text_detection/dictionary.py
--rw-r--r--   0 macbook    (501) staff       (20)    11602 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/text_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.495798 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2511 2023-06-20 08:34:11.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.496314 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.496974 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.497882 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.498741 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.499394 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.499860 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.500155 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.501276 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     7313 2023-06-20 08:38:07.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.501899 JustScan-1.1.6/app/JustScan/ocr/core/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.6/app/JustScan/ocr/core/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-1.1.6/app/JustScan/ocr/core/tools/api_json.py
--rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/tools/dictionaries.py
--rw-r--r--   0 macbook    (501) staff       (20)     2518 2023-06-20 17:16:54.000000 JustScan-1.1.6/app/JustScan/ocr/core/tools/functional.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:52:12.477469 JustScan-1.1.6/app/JustScan.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2638 2023-06-21 02:52:12.000000 JustScan-1.1.6/app/JustScan.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     7220 2023-06-21 02:52:12.000000 JustScan-1.1.6/app/JustScan.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-21 02:52:12.000000 JustScan-1.1.6/app/JustScan.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       58 2023-06-21 02:52:12.000000 JustScan-1.1.6/app/JustScan.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-21 02:52:12.000000 JustScan-1.1.6/app/JustScan.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-21 02:52:12.000000 JustScan-1.1.6/app/JustScan.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-21 02:52:12.502403 JustScan-1.1.6/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1158 2023-06-21 02:52:11.000000 JustScan-1.1.6/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.413237 JustScan-1.1.7/
+-rw-r--r--   0 macbook    (501) staff       (20)     2638 2023-06-21 02:53:56.413066 JustScan-1.1.7/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-1.1.7/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.385427 JustScan-1.1.7/app/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.389925 JustScan-1.1.7/app/JustScan/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 17:20:30.000000 JustScan-1.1.7/app/JustScan/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.391708 JustScan-1.1.7/app/JustScan/api/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-1.1.7/app/JustScan/api/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-20 10:57:02.000000 JustScan-1.1.7/app/JustScan/api/itc_cli.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5520 2023-06-20 17:06:38.000000 JustScan-1.1.7/app/JustScan/api/just_scan_api.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.392598 JustScan-1.1.7/app/JustScan/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-1.1.7/app/JustScan/config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-1.1.7/app/JustScan/config/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-1.1.7/app/JustScan/config/config_db.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-1.1.7/app/JustScan/config/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-1.1.7/app/JustScan/config/pydantic_models.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.393308 JustScan-1.1.7/app/JustScan/database/
+-rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-1.1.7/app/JustScan/database/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4411 2023-06-21 02:51:05.000000 JustScan-1.1.7/app/JustScan/database/crud.py
+-rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-1.1.7/app/JustScan/database/data_models.py
+-rw-r--r--   0 macbook    (501) staff       (20)      570 2023-06-20 17:06:38.000000 JustScan-1.1.7/app/JustScan/database/database.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.393484 JustScan-1.1.7/app/JustScan/face_id/
+-rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-1.1.7/app/JustScan/face_id/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.393816 JustScan-1.1.7/app/JustScan/face_id/commons/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.394965 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/
+-rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.395523 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/data_io/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11469 2023-06-21 02:49:42.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
+-rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1402 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.396090 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/model_lib/
+-rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/utility.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.396403 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/
+-rw-r--r--   0 macbook    (501) staff       (20)     3004 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)      983 2023-06-21 02:52:02.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.397171 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/layers.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.397639 JustScan-1.1.7/app/JustScan/face_id/commons/CloseEyes/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/CloseEyes/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1104 2023-06-20 17:27:59.000000 JustScan-1.1.7/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1315 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/face_id/commons/CloseEyes/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.397928 JustScan-1.1.7/app/JustScan/face_id/commons/FaceMask/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/FaceMask/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      812 2023-06-20 17:27:59.000000 JustScan-1.1.7/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.398356 JustScan-1.1.7/app/JustScan/face_id/commons/FaceQuality/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/FaceQuality/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-1.1.7/app/JustScan/face_id/commons/FaceQuality/dom.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-1.1.7/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.398659 JustScan-1.1.7/app/JustScan/face_id/commons/ScrFd/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ScrFd/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 JustScan-1.1.7/app/JustScan/face_id/commons/ScrFd/scrfd.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.7/app/JustScan/face_id/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-1.1.7/app/JustScan/face_id/commons/config.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.399242 JustScan-1.1.7/app/JustScan/face_id/libraries/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.7/app/JustScan/face_id/libraries/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7235 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/face_id/libraries/face_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5325 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/face_id/libraries/face_id.py
+-rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-1.1.7/app/JustScan/face_id/libraries/face_recognition.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.399521 JustScan-1.1.7/app/JustScan/face_id/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.7/app/JustScan/face_id/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3955 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/face_id/tools/modules.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.399686 JustScan-1.1.7/app/JustScan/ocr/
+-rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-1.1.7/app/JustScan/ocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.399852 JustScan-1.1.7/app/JustScan/ocr/core/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.400700 JustScan-1.1.7/app/JustScan/ocr/core/commons/
+-rw-r--r--   0 macbook    (501) staff       (20)      814 2023-06-20 08:24:37.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/SpoofingNID.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5592 2023-06-20 08:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/id_card_classification.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5675 2023-06-20 10:04:38.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/id_card_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1761 2023-06-20 08:22:16.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/merge_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.401025 JustScan-1.1.7/app/JustScan/ocr/core/commons/utils/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/utils/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2513 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/commons/utils/utils_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.401194 JustScan-1.1.7/app/JustScan/ocr/core/modules/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.401685 JustScan-1.1.7/app/JustScan/ocr/core/modules/corner_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/corner_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/corner_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.402335 JustScan-1.1.7/app/JustScan/ocr/core/modules/id_card_classification/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      923 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/id_card_classification/classify.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.402960 JustScan-1.1.7/app/JustScan/ocr/core/modules/mrc/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/mrc/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2938 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/mrc/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.403774 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9072 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/passport.py
+-rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/passport_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.404538 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_align_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.404956 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9668 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.405346 JustScan-1.1.7/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2936 2023-06-21 02:53:49.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.405728 JustScan-1.1.7/app/JustScan/ocr/core/modules/spell_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/spell_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.406151 JustScan-1.1.7/app/JustScan/ocr/core/modules/spoofing_nid/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      935 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.406778 JustScan-1.1.7/app/JustScan/ocr/core/modules/text_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/text_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7020 2023-06-20 08:33:20.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/text_detection/dictionary.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11602 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/text_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.407128 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2511 2023-06-20 08:34:11.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.407629 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.408241 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.409014 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.409680 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.410358 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.410821 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.411125 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.412235 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7313 2023-06-20 08:38:07.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.412833 JustScan-1.1.7/app/JustScan/ocr/core/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.7/app/JustScan/ocr/core/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-1.1.7/app/JustScan/ocr/core/tools/api_json.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/tools/dictionaries.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2518 2023-06-20 17:16:54.000000 JustScan-1.1.7/app/JustScan/ocr/core/tools/functional.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-21 02:53:56.391188 JustScan-1.1.7/app/JustScan.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2638 2023-06-21 02:53:56.000000 JustScan-1.1.7/app/JustScan.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     7220 2023-06-21 02:53:56.000000 JustScan-1.1.7/app/JustScan.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-21 02:53:56.000000 JustScan-1.1.7/app/JustScan.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       58 2023-06-21 02:53:56.000000 JustScan-1.1.7/app/JustScan.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-21 02:53:56.000000 JustScan-1.1.7/app/JustScan.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-21 02:53:56.000000 JustScan-1.1.7/app/JustScan.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-21 02:53:56.413294 JustScan-1.1.7/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1158 2023-06-21 02:53:49.000000 JustScan-1.1.7/setup.py
```

### Comparing `JustScan-1.1.6/PKG-INFO` & `JustScan-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 1.1.6
+Version: 1.1.7
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JustScan-1.1.6/README.md` & `JustScan-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/api/just_scan_api.py` & `JustScan-1.1.7/app/JustScan/api/just_scan_api.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/config/config.py` & `JustScan-1.1.7/app/JustScan/config/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/config/config_db.py` & `JustScan-1.1.7/app/JustScan/config/config_db.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/config/logger.py` & `JustScan-1.1.7/app/JustScan/config/logger.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/config/pydantic_models.py` & `JustScan-1.1.7/app/JustScan/config/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/database/crud.py` & `JustScan-1.1.7/app/JustScan/database/crud.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/database/data_models.py` & `JustScan-1.1.7/app/JustScan/database/data_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/database/database.py` & `JustScan-1.1.7/app/JustScan/database/database.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/AntiSpoof/utility.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/AntiSpoof/utility.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/__init__.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/__init__.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/layers.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/layers.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/models.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/models.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/ArcFace/lib/utils.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/ArcFace/lib/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/CloseEyes/utils.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/CloseEyes/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/FaceQuality/dom.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/FaceQuality/dom.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/ScrFd/scrfd.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/ScrFd/scrfd.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/commons/config.py` & `JustScan-1.1.7/app/JustScan/face_id/commons/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/libraries/face_detection.py` & `JustScan-1.1.7/app/JustScan/face_id/libraries/face_detection.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/libraries/face_id.py` & `JustScan-1.1.7/app/JustScan/face_id/libraries/face_id.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/face_id/tools/modules.py` & `JustScan-1.1.7/app/JustScan/face_id/tools/modules.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/commons/SpoofingNID.py` & `JustScan-1.1.7/app/JustScan/ocr/core/commons/SpoofingNID.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/commons/config.py` & `JustScan-1.1.7/app/JustScan/ocr/core/commons/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/commons/id_card_classification.py` & `JustScan-1.1.7/app/JustScan/ocr/core/commons/id_card_classification.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/commons/id_card_onnx.py` & `JustScan-1.1.7/app/JustScan/ocr/core/commons/id_card_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/commons/merge_model.py` & `JustScan-1.1.7/app/JustScan/ocr/core/commons/merge_model.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/commons/utils/utils_onnx.py` & `JustScan-1.1.7/app/JustScan/ocr/core/commons/utils/utils_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/corner_detection/utils.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/corner_detection/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/id_card_classification/classify.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/id_card_classification/classify.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/mrc/mrc_detection.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/mrc/mrc_detection.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/mrc/utils.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/mrc/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/passport.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/passport.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import cv2
 import numpy as np
 import math
-from face_id.commons.FaceQuality.dom import DOM
+from JustScan.face_id.commons.FaceQuality.dom import DOM
 from ...commons.SpoofingNID import SpoofingNIDModel
 from fastapi import HTTPException
 from JustScan.config.logger import setup_logger
 
 logging = setup_logger(__name__)
 
 MIN_SHARPNESS = 0.46
```

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/text_detection/dictionary.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/text_detection/dictionary.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/text_detection/utils.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/text_detection/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py` & `JustScan-1.1.7/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/tools/api_json.py` & `JustScan-1.1.7/app/JustScan/ocr/core/tools/api_json.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/tools/dictionaries.py` & `JustScan-1.1.7/app/JustScan/ocr/core/tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan/ocr/core/tools/functional.py` & `JustScan-1.1.7/app/JustScan/ocr/core/tools/functional.py`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan.egg-info/PKG-INFO` & `JustScan-1.1.7/app/JustScan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 1.1.6
+Version: 1.1.7
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JustScan-1.1.6/app/JustScan.egg-info/SOURCES.txt` & `JustScan-1.1.7/app/JustScan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/app/JustScan.egg-info/requires.txt` & `JustScan-1.1.7/app/JustScan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `JustScan-1.1.6/setup.py` & `JustScan-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 with open("README.md", "r") as f:
     long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="JustScan",
-    version="1.1.6",
+    version="1.1.7",
     description="E-kyc for Industries application",
     package_dir={"": "app"},
     packages=find_packages(where="./app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aihackervn",
     author="Theodore",
```

