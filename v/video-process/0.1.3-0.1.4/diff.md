# Comparing `tmp/video_process-0.1.3.tar.gz` & `tmp/video_process-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.1.3.tar", max compression
+gzip compressed data, was "video_process-0.1.4.tar", max compression
```

## Comparing `video_process-0.1.3.tar` & `video_process-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      357 2023-06-21 04:25:52.186815 video_process-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-20 07:17:23.855346 video_process-0.1.3/video_process/__init__.py
--rw-r--r--   0        0        0     5606 2023-06-20 06:39:07.757764 video_process-0.1.3/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1290 2023-06-20 07:28:56.534270 video_process-0.1.3/video_process/index.py
--rw-r--r--   0        0        0     4061 2023-06-20 10:46:59.013491 video_process-0.1.3/video_process/lib.py
--rw-r--r--   0        0        0      585 2023-06-19 09:26:44.831078 video_process-0.1.3/video_process/subtitle.py
--rw-r--r--   0        0        0     1206 2023-06-19 09:01:27.560964 video_process-0.1.3/video_process/test_graph.py
--rw-r--r--   0        0        0     3005 2023-06-20 09:57:33.787485 video_process-0.1.3/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      357 2023-06-21 06:42:12.881622 video_process-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-20 07:17:23.855346 video_process-0.1.4/video_process/__init__.py
+-rw-r--r--   0        0        0     5606 2023-06-20 06:39:07.757764 video_process-0.1.4/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1290 2023-06-20 07:28:56.534270 video_process-0.1.4/video_process/index.py
+-rw-r--r--   0        0        0     4061 2023-06-20 10:46:59.013491 video_process-0.1.4/video_process/lib.py
+-rw-r--r--   0        0        0     1941 2023-06-21 06:40:11.174245 video_process-0.1.4/video_process/subtitle.py
+-rw-r--r--   0        0        0     1206 2023-06-19 09:01:27.560964 video_process-0.1.4/video_process/test_graph.py
+-rw-r--r--   0        0        0     2944 2023-06-21 06:40:24.748946 video_process-0.1.4/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.4/PKG-INFO
```

### Comparing `video_process-0.1.3/video_process/graph_builder.py` & `video_process-0.1.4/video_process/graph_builder.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.3/video_process/index.py` & `video_process-0.1.4/video_process/index.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.3/video_process/lib.py` & `video_process-0.1.4/video_process/lib.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.3/video_process/test_graph.py` & `video_process-0.1.4/video_process/test_graph.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.3/video_process/utils.py` & `video_process-0.1.4/video_process/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,16 +49,15 @@
             subtitle_path = os.path.join(base_dir, "subtitle.srt")
             download_file(subtitle_url, subtitle_path)
             subtitle["subtitle_path"] = subtitle_path
 
             # 转换SRT字幕为ASS字幕
             style = subtitle["subtitle_style"]
             output_ass_path = os.path.join(base_dir, "subtitle.ass")
-            convert_to_ass(subtitle_path, output_ass_path)
-            change_style(output_ass_path, output_ass_path, style)
+            change_style(subtitle_path, output_ass_path, style)
             subtitle["subtitle_path"] = output_ass_path
 
     # 处理图层字段
     if data.get("enable_layers"):
         layers = data["layers"]
         for layer in layers:
             if layer.get("url"):
```

