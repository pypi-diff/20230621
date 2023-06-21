# Comparing `tmp/p-ttauto-crawler-0.1.4.tar.gz` & `tmp/p-ttauto-crawler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.1.4.tar", last modified: Wed Jun 21 11:00:45 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.1.5.tar", last modified: Wed Jun 21 11:06:54 2023, max compression
```

## Comparing `p-ttauto-crawler-0.1.4.tar` & `p-ttauto-crawler-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 11:00:45.247198 p-ttauto-crawler-0.1.4/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      397 2023-06-21 11:00:45.246198 p-ttauto-crawler-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 11:00:45.225197 p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-21 11:00:45.000000 p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-06-21 11:00:45.000000 p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 11:00:45.000000 p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-21 11:00:45.000000 p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-21 11:00:45.000000 p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 11:00:45.000000 p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 11:00:45.247198 p-ttauto-crawler-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-06-21 11:00:11.000000 p-ttauto-crawler-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:00:45.243198 p-ttauto-crawler-0.1.4/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/__init__.py
--rw-rw-rw-   0        0        0     9460 2023-06-21 10:59:50.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/auto_crawler.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:00:45.244197 p-ttauto-crawler-0.1.4/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/bin/print_md5.py
--rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/binary.py
--rw-rw-rw-   0        0        0    10986 2023-06-21 10:59:45.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/downloader.py
--rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/mecord_downloader.py
--rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/processing.py
--rw-rw-rw-   0        0        0     3934 2023-06-20 07:22:50.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/task.py
--rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/ttsUtils.py
--rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/txt2proj.py
--rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/uploading.py
--rw-rw-rw-   0        0        0    10914 2023-06-20 08:47:18.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/utils.py
--rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/video_merge.py
--rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/video_random_cutter.py
--rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.4/ttauto_crawler/ytdlp_downloader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:06:54.288608 p-ttauto-crawler-0.1.5/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-06-21 11:06:54.288608 p-ttauto-crawler-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 11:06:54.262609 p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-21 11:06:54.000000 p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-21 11:06:54.000000 p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 11:06:54.000000 p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-21 11:06:54.000000 p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-21 11:06:54.000000 p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 11:06:54.000000 p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 11:06:54.289609 p-ttauto-crawler-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-06-21 11:06:49.000000 p-ttauto-crawler-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:06:54.283612 p-ttauto-crawler-0.1.5/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/__init__.py
+-rw-rw-rw-   0        0        0     9460 2023-06-21 10:59:50.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/auto_crawler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:06:54.286610 p-ttauto-crawler-0.1.5/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/bin/print_md5.py
+-rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/binary.py
+-rw-rw-rw-   0        0        0    10986 2023-06-21 10:59:45.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/downloader.py
+-rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/mecord_downloader.py
+-rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/processing.py
+-rw-rw-rw-   0        0        0     3934 2023-06-21 11:06:32.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/task.py
+-rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/ttsUtils.py
+-rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/txt2proj.py
+-rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/uploading.py
+-rw-rw-rw-   0        0        0    10914 2023-06-21 11:06:41.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/utils.py
+-rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/video_merge.py
+-rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/video_random_cutter.py
+-rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.5/ttauto_crawler/ytdlp_downloader.py
```

### Comparing `p-ttauto-crawler-0.1.4/LICENSE` & `p-ttauto-crawler-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/p_ttauto_crawler.egg-info/SOURCES.txt` & `p-ttauto-crawler-0.1.5/p_ttauto_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/setup.py` & `p-ttauto-crawler-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.1.4",
+    version="0.1.5",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/auto_crawler.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/auto_crawler.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/bin/print_md5.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/bin/print_md5.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/binary.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/binary.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/downloader.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/main.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/main.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/mecord_downloader.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/mecord_downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/processing.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/processing.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/task.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     DOWNLOADING = 1
     WAIT_TEMPLATE = 2
     TEMPLATEING = 3
     WAIT_UPLOAD = 4
     UPLOADING = 5
     END = 6
     
-MAX_DOWNLOADING_COUNT = 5
+MAX_DOWNLOADING_COUNT = 2
 MAX_PROCESSING_COUNT = 2
 MAX_UPLOADING_COUNT = 5
 
 def _configFile():
     thisFileDir = os.path.dirname(os.path.abspath(__file__))
     file = os.path.join(thisFileDir, "task.config")
     if os.path.exists(file) == False:
```

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/ttsUtils.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/ttsUtils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/txt2proj.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/txt2proj.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/uploading.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/uploading.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
             free = 0
             try:
                 total, used, free = shutil.disk_usage(d)
             except:
                 continue
             if free > 0:
                 freeGB = free / 1024.0 / 1024.0 / 1024.0
-                if freeGB > 400:
+                if freeGB > 300:
                     path = d
                     break
         if len(path) <= 0:
             path = os.path.dirname(os.path.abspath(__file__))
     elif sys.platform == "linux":
         return "/home"
     elif sys.platform == "darwin":
```

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/video_merge.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/video_merge.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/video_random_cutter.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/video_random_cutter.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.4/ttauto_crawler/ytdlp_downloader.py` & `p-ttauto-crawler-0.1.5/ttauto_crawler/ytdlp_downloader.py`

 * *Files identical despite different names*

