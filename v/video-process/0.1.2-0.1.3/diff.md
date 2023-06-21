# Comparing `tmp/video_process-0.1.2.tar.gz` & `tmp/video_process-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.1.2.tar", max compression
+gzip compressed data, was "video_process-0.1.3.tar", max compression
```

## Comparing `video_process-0.1.2.tar` & `video_process-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      357 2023-06-21 03:53:11.551449 video_process-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-20 07:17:23.855346 video_process-0.1.2/video_process/__init__.py
--rw-r--r--   0        0        0     5606 2023-06-20 06:39:07.757764 video_process-0.1.2/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1290 2023-06-20 07:28:56.534270 video_process-0.1.2/video_process/index.py
--rw-r--r--   0        0        0     4061 2023-06-20 10:46:59.013491 video_process-0.1.2/video_process/lib.py
--rw-r--r--   0        0        0      585 2023-06-19 09:26:44.831078 video_process-0.1.2/video_process/subtitle.py
--rw-r--r--   0        0        0     1206 2023-06-19 09:01:27.560964 video_process-0.1.2/video_process/test_graph.py
--rw-r--r--   0        0        0     3005 2023-06-20 09:57:33.787485 video_process-0.1.2/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      357 2023-06-21 04:25:52.186815 video_process-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-20 07:17:23.855346 video_process-0.1.3/video_process/__init__.py
+-rw-r--r--   0        0        0     5606 2023-06-20 06:39:07.757764 video_process-0.1.3/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1290 2023-06-20 07:28:56.534270 video_process-0.1.3/video_process/index.py
+-rw-r--r--   0        0        0     4061 2023-06-20 10:46:59.013491 video_process-0.1.3/video_process/lib.py
+-rw-r--r--   0        0        0      585 2023-06-19 09:26:44.831078 video_process-0.1.3/video_process/subtitle.py
+-rw-r--r--   0        0        0     1206 2023-06-19 09:01:27.560964 video_process-0.1.3/video_process/test_graph.py
+-rw-r--r--   0        0        0     3005 2023-06-20 09:57:33.787485 video_process-0.1.3/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.3/PKG-INFO
```

### Comparing `video_process-0.1.2/video_process/graph_builder.py` & `video_process-0.1.3/video_process/graph_builder.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.2/video_process/index.py` & `video_process-0.1.3/video_process/index.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.2/video_process/lib.py` & `video_process-0.1.3/video_process/lib.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.2/video_process/subtitle.py` & `video_process-0.1.3/video_process/subtitle.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.2/video_process/test_graph.py` & `video_process-0.1.3/video_process/test_graph.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.2/video_process/utils.py` & `video_process-0.1.3/video_process/utils.py`

 * *Files identical despite different names*

