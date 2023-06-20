# Comparing `tmp/remotecv-5.1.2.tar.gz` & `tmp/remotecv-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotecv-5.1.2.tar", last modified: Thu Jun 15 17:25:07 2023, max compression
+gzip compressed data, was "remotecv-5.1.3.tar", last modified: Tue Jun 20 22:13:34 2023, max compression
```

## Comparing `remotecv-5.1.2.tar` & `remotecv-5.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.399847 remotecv-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 17:24:55.000000 remotecv-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 17:24:55.000000 remotecv-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-15 17:25:07.399847 remotecv-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-15 17:24:55.000000 remotecv-5.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 17:24:55.000000 remotecv-5.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.387847 remotecv-5.1.2/remotecv/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/celery_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.387847 remotecv-5.1.2/remotecv/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.387847 remotecv-5.1.2/remotecv/detectors/complete_detector/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/complete_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.391847 remotecv-5.1.2/remotecv/detectors/face_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   676709 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml
--rw-r--r--   0 runner    (1001) docker     (123)   540616 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml
--rw-r--r--   0 runner    (1001) docker     (123)  2689040 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml
--rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/detectors/feature_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/feature_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/detectors/glasses_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/glasses_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   601661 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/detectors/profile_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/profile_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   828514 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/profile_detector/haarcascade_profileface.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/http_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/image_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/metrics/logger_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/pyres_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/result_store/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/result_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/result_store/memcache_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/result_store/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/unique_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.399847 remotecv-5.1.2/remotecv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 17:25:07.399847 remotecv-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-15 17:24:55.000000 remotecv-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.129892 remotecv-5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 22:13:23.000000 remotecv-5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 22:13:23.000000 remotecv-5.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-20 22:13:34.129892 remotecv-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-20 22:13:23.000000 remotecv-5.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-20 22:13:23.000000 remotecv-5.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.121892 remotecv-5.1.3/remotecv/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/celery_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.121892 remotecv-5.1.3/remotecv/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.121892 remotecv-5.1.3/remotecv/detectors/complete_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/complete_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.125892 remotecv-5.1.3/remotecv/detectors/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   676709 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   540616 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  2689040 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.129892 remotecv-5.1.3/remotecv/detectors/feature_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/feature_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.129892 remotecv-5.1.3/remotecv/detectors/glasses_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/glasses_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   601661 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.129892 remotecv-5.1.3/remotecv/detectors/profile_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/profile_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   828514 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/detectors/profile_detector/haarcascade_profileface.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/http_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/image_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.129892 remotecv-5.1.3/remotecv/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/metrics/logger_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/pyres_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.129892 remotecv-5.1.3/remotecv/result_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/result_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/result_store/memcache_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/result_store/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/unique_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-20 22:13:23.000000 remotecv-5.1.3/remotecv/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:13:34.129892 remotecv-5.1.3/remotecv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-20 22:13:34.000000 remotecv-5.1.3/remotecv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-20 22:13:34.000000 remotecv-5.1.3/remotecv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:13:34.000000 remotecv-5.1.3/remotecv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 22:13:34.000000 remotecv-5.1.3/remotecv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-20 22:13:34.000000 remotecv-5.1.3/remotecv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 22:13:34.000000 remotecv-5.1.3/remotecv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 22:13:34.133892 remotecv-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-20 22:13:23.000000 remotecv-5.1.3/setup.py
```

### Comparing `remotecv-5.1.2/LICENSE` & `remotecv-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/PKG-INFO` & `remotecv-5.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: remotecv
-Version: 5.1.2
+Version: 5.1.3
 Summary: remotecv is an OpenCV worker for facial and feature recognition
+Home-page: https://github.com/thumbor/remotecv
 Author: Bernardo Heynemann
 Author-email: heynemann@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `remotecv-5.1.2/README.md` & `remotecv-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/celery_tasks.py` & `remotecv-5.1.3/remotecv/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/__init__.py` & `remotecv-5.1.3/remotecv/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/complete_detector/__init__.py` & `remotecv-5.1.3/remotecv/detectors/complete_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/face_detector/__init__.py` & `remotecv-5.1.3/remotecv/detectors/face_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml` & `remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml` & `remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml` & `remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml` & `remotecv-5.1.3/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/feature_detector/__init__.py` & `remotecv-5.1.3/remotecv/detectors/feature_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml` & `remotecv-5.1.3/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/detectors/profile_detector/haarcascade_profileface.xml` & `remotecv-5.1.3/remotecv/detectors/profile_detector/haarcascade_profileface.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/error_handler.py` & `remotecv-5.1.3/remotecv/error_handler.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/http_loader.py` & `remotecv-5.1.3/remotecv/http_loader.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/image.py` & `remotecv-5.1.3/remotecv/image.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/image_processor.py` & `remotecv-5.1.3/remotecv/image_processor.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/metrics/logger_metrics.py` & `remotecv-5.1.3/remotecv/metrics/logger_metrics.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/pyres_tasks.py` & `remotecv-5.1.3/remotecv/pyres_tasks.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/result_store/__init__.py` & `remotecv-5.1.3/remotecv/result_store/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/result_store/memcache_store.py` & `remotecv-5.1.3/remotecv/result_store/memcache_store.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv/unique_queue.py` & `remotecv-5.1.3/remotecv/unique_queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from pyres import ResQ
 from pyres.worker import Worker
 
-from remotecv.utils import logger
+from remotecv.timing import get_time, get_interval
+from remotecv.utils import context, logger
 
 
 class UniqueQueue(ResQ):
     def _escape_for_key(self, value):
         return value.replace(" ", "").replace("\n", "")
 
     def _create_unique_key(self, queue, key):
         return f"resque:unique:queue:{queue}:{self._escape_for_key(str(key))}"
 
     def add_unique_key(self, queue, key):
         unique_key = self._create_unique_key(queue, key)
         if self.redis.get(unique_key) == b"1":
             # Do nothing as this message is already enqueued
             return False
-
         self.redis.set(unique_key, "1")
+
         return True
 
     def del_unique_key(self, queue, key):
+        start_time = get_time()
         unique_key = self._create_unique_key(queue, key)
         self.redis.delete(unique_key)
+        context.metrics.timing(
+            "worker.del_unique_key.time",
+            get_interval(start_time, get_time()),
+        )
 
     def enqueue_unique_from_string(
         self, klass_as_string, queue, args=None, key=None
     ):
         if not self.add_unique_key(queue, key):
             logger.debug("key %s already enqueued", key)
             return
@@ -65,7 +71,16 @@
             self.after_fork_fn(job)
 
     def before_process(self, job):
         self.resq.del_unique_key(
             job._queue, job._payload["key"]  # pylint: disable=protected-access
         )
         return job
+
+    def reserve(self, timeout=10):
+        start_time = get_time()
+        job = super().reserve(timeout=timeout)
+        context.metrics.timing(
+            "worker.read_queue.time",
+            get_interval(start_time, get_time()),
+        )
+        return job
```

### Comparing `remotecv-5.1.2/remotecv/utils.py` & `remotecv-5.1.3/remotecv/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # http://www.opensource.org/licenses/mit-license
 # Copyright (c) 2011 globo.com timehome@corp.globo.com
 
 import logging
 
 from redis import Redis, Sentinel
 
+from remotecv.timing import get_time, get_interval
+
 
 class Config:
     pass
 
 
 class Context:
     pass
@@ -26,24 +28,30 @@
 context = Context()
 
 SINGLE_NODE = "single_node"
 SENTINEL = "sentinel"
 
 
 def redis_client():
+    start_time = get_time()
     if config.redis_mode == SINGLE_NODE:
-        return __redis_single_node_client()
-
-    if config.redis_mode == SENTINEL:
-        return __redis_sentinel_client()
+        client = __redis_single_node_client()
+    elif config.redis_mode == SENTINEL:
+        client = __redis_sentinel_client()
+    else:
+        raise AttributeError(
+            f"redis-mode must be either {SINGLE_NODE} or {SENTINEL}"
+        )
 
-    raise AttributeError(
-        f"redis-mode must be either {SINGLE_NODE} or {SENTINEL}"
+    context.metrics.timing(
+        "worker.redis_connection.time", get_interval(start_time, get_time()),
     )
 
+    return client
+
 
 def __redis_sentinel_client():
     instances_split = config.redis_sentinel_instances.split(",")
     instances = [instance.split(":") for instance in instances_split]
 
     if config.redis_sentinel_password:
         sentinel_instance = Sentinel(
```

### Comparing `remotecv-5.1.2/remotecv/worker.py` & `remotecv-5.1.3/remotecv/worker.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv.egg-info/PKG-INFO` & `remotecv-5.1.3/remotecv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: remotecv
-Version: 5.1.2
+Version: 5.1.3
 Summary: remotecv is an OpenCV worker for facial and feature recognition
+Home-page: https://github.com/thumbor/remotecv
 Author: Bernardo Heynemann
 Author-email: heynemann@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `remotecv-5.1.2/remotecv.egg-info/SOURCES.txt` & `remotecv-5.1.3/remotecv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/remotecv.egg-info/requires.txt` & `remotecv-5.1.3/remotecv.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.2/setup.py` & `remotecv-5.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "click-option-group==0.5.*",
 ]
 
 setup(
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="remotecv",
+    url="https://github.com/thumbor/remotecv",
     version=version,
     description="remotecv is an OpenCV worker for facial and feature recognition",
     python_requires="==3.*,>=3.7.0",
     author="Bernardo Heynemann",
     author_email="heynemann@gmail.com",
     license="MIT",
     entry_points={"console_scripts": ["remotecv = remotecv.worker:main"]},
```

