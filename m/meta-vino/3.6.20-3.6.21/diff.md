# Comparing `tmp/meta-vino-3.6.20.tar.gz` & `tmp/meta-vino-3.6.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-vino-3.6.20.tar", last modified: Tue Jun 20 10:31:06 2023, max compression
+gzip compressed data, was "dist/meta-vino-3.6.21.tar", last modified: Wed Jun 21 03:43:59 2023, max compression
```

## Comparing `meta-vino-3.6.20.tar` & `meta-vino-3.6.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/
--rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-20 10:31:06.000000 meta-vino-3.6.20/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       40 2022-11-09 06:00:33.000000 meta-vino-3.6.20/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      560 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       47 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/
--rw-rw-r--   0 cash      (1000) cash      (1000)      139 2023-06-09 09:59:52.000000 meta-vino-3.6.20/metavino/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)      313 2023-06-09 09:59:37.000000 meta-vino-3.6.20/metavino/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2549 2022-11-10 09:22:51.000000 meta-vino-3.6.20/metavino/app/instance_segment_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1679 2022-11-09 08:30:52.000000 meta-vino-3.6.20/metavino/app/object_classification_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      275 2022-11-08 11:30:35.000000 meta-vino-3.6.20/metavino/app/object_detection_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      990 2022-11-08 12:47:07.000000 meta-vino-3.6.20/metavino/app/onnx_to_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1889 2022-11-10 08:16:13.000000 meta-vino-3.6.20/metavino/app/saliency_segment_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4340 2023-06-20 10:24:32.000000 meta-vino-3.6.20/metavino/app/yolo_segment_vino.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)        0 2022-11-08 11:30:50.000000 meta-vino-3.6.20/metavino/model_zoo/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       23 2022-11-08 12:00:00.000000 meta-vino-3.6.20/metavino/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7238 2023-06-20 10:28:43.000000 meta-vino-3.6.20/metavino/utils/general.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-06-20 10:31:06.000000 meta-vino-3.6.20/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      674 2023-06-20 10:29:54.000000 meta-vino-3.6.20/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-21 03:43:59.000000 meta-vino-3.6.21/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-21 03:43:59.000000 meta-vino-3.6.21/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       40 2022-11-09 06:00:33.000000 meta-vino-3.6.21/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-21 03:43:59.000000 meta-vino-3.6.21/meta_vino.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-21 03:43:58.000000 meta-vino-3.6.21/meta_vino.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      560 2023-06-21 03:43:58.000000 meta-vino-3.6.21/meta_vino.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-21 03:43:58.000000 meta-vino-3.6.21/meta_vino.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       47 2023-06-21 03:43:58.000000 meta-vino-3.6.21/meta_vino.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-06-21 03:43:58.000000 meta-vino-3.6.21/meta_vino.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-21 03:43:58.000000 meta-vino-3.6.21/meta_vino.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-21 03:43:59.000000 meta-vino-3.6.21/metavino/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      139 2023-06-09 09:59:52.000000 meta-vino-3.6.21/metavino/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-21 03:43:59.000000 meta-vino-3.6.21/metavino/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      313 2023-06-09 09:59:37.000000 meta-vino-3.6.21/metavino/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2549 2022-11-10 09:22:51.000000 meta-vino-3.6.21/metavino/app/instance_segment_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1679 2022-11-09 08:30:52.000000 meta-vino-3.6.21/metavino/app/object_classification_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      275 2022-11-08 11:30:35.000000 meta-vino-3.6.21/metavino/app/object_detection_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      990 2022-11-08 12:47:07.000000 meta-vino-3.6.21/metavino/app/onnx_to_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1889 2022-11-10 08:16:13.000000 meta-vino-3.6.21/metavino/app/saliency_segment_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4340 2023-06-20 10:24:32.000000 meta-vino-3.6.21/metavino/app/yolo_segment_vino.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-21 03:43:59.000000 meta-vino-3.6.21/metavino/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)        0 2022-11-08 11:30:50.000000 meta-vino-3.6.21/metavino/model_zoo/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-21 03:43:59.000000 meta-vino-3.6.21/metavino/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       23 2022-11-08 12:00:00.000000 meta-vino-3.6.21/metavino/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7369 2023-06-21 03:43:17.000000 meta-vino-3.6.21/metavino/utils/general.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-06-21 03:43:59.000000 meta-vino-3.6.21/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      674 2023-06-21 03:43:32.000000 meta-vino-3.6.21/setup.py
```

### Comparing `meta-vino-3.6.20/meta_vino.egg-info/SOURCES.txt` & `meta-vino-3.6.21/meta_vino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.20/metavino/app/instance_segment_vino.py` & `meta-vino-3.6.21/metavino/app/instance_segment_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.20/metavino/app/object_classification_vino.py` & `meta-vino-3.6.21/metavino/app/object_classification_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.20/metavino/app/onnx_to_vino.py` & `meta-vino-3.6.21/metavino/app/onnx_to_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.20/metavino/app/saliency_segment_vino.py` & `meta-vino-3.6.21/metavino/app/saliency_segment_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.20/metavino/app/yolo_segment_vino.py` & `meta-vino-3.6.21/metavino/app/yolo_segment_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.20/metavino/utils/general.py` & `meta-vino-3.6.21/metavino/utils/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,28 +147,31 @@
         inds = np.where(ovr <= nms_thr)[0]
         order = order[inds + 1]
 
     return keep
 
 
 def preproc(image, input_size, mean, std, swap=(2, 0, 1)):
-    if len(image.shape) == 3:
-        padded_img = np.ones((input_size[0], input_size[1], 3)) * 114.0
-    else:
-        padded_img = np.ones(input_size) * 114.0
     img = np.array(image)
     r = min(input_size[0] / img.shape[0], input_size[1] / img.shape[1])
-    resized_img = cv2.resize(
-        img,
-        (int(img.shape[1] * r), int(img.shape[0] * r)),
-        interpolation=cv2.INTER_LINEAR,
-    ).astype(np.float32)
-    padded_img[: int(img.shape[0] * r), : int(img.shape[1] * r)] = resized_img
-    # if use yolox set
-    padded_img = padded_img[:, :, ::-1]
+
+    if img.shape[:2] == input_size:
+        padded_img = img.astype(np.float32)
+    else:
+        # 传入图像默认为RGB
+        if len(image.shape) == 3:
+            padded_img = np.ones((input_size[0], input_size[1], 3)) * 114.0
+        else:
+            padded_img = np.ones(input_size) * 114.0
+        resized_img = cv2.resize(
+            img,
+            (int(round(img.shape[1] * r)), int(round(img.shape[0] * r))),
+            interpolation=cv2.INTER_LINEAR,
+        ).astype(np.float32)
+        padded_img[: int(round(img.shape[0] * r)), : int(round(img.shape[1] * r))] = resized_img
     padded_img /= 255.0
     if mean is not None:
         padded_img -= mean
     if std is not None:
         padded_img /= std
     padded_img = padded_img.transpose(swap)
     padded_img = np.ascontiguousarray(padded_img, dtype=np.float32)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `meta-vino-3.6.20/setup.py` & `meta-vino-3.6.21/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     'opencv-python',
     'setuptools',
     'openvino',
     'numpy',
     'pillow',
 ]
 
-__version__ = 'V3.06.20'
+__version__ = 'V3.06.21'
 
 setup(
     name='meta-vino',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvopenvino',
```

