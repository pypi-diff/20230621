# Comparing `tmp/p-ttauto-crawler-0.1.6.tar.gz` & `tmp/p-ttauto-crawler-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.1.6.tar", last modified: Wed Jun 21 11:15:37 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.1.7.tar", last modified: Wed Jun 21 11:20:36 2023, max compression
```

## Comparing `p-ttauto-crawler-0.1.6.tar` & `p-ttauto-crawler-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 11:15:37.432669 p-ttauto-crawler-0.1.6/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      397 2023-06-21 11:15:37.432669 p-ttauto-crawler-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 11:15:37.402669 p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-21 11:15:37.000000 p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-06-21 11:15:37.000000 p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 11:15:37.000000 p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-21 11:15:37.000000 p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-21 11:15:37.000000 p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 11:15:37.000000 p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 11:15:37.433669 p-ttauto-crawler-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-06-21 11:15:31.000000 p-ttauto-crawler-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:15:37.428669 p-ttauto-crawler-0.1.6/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/__init__.py
--rw-rw-rw-   0        0        0     9460 2023-06-21 11:15:15.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/auto_crawler.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:15:37.430670 p-ttauto-crawler-0.1.6/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/bin/print_md5.py
--rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/binary.py
--rw-rw-rw-   0        0        0    10986 2023-06-21 10:59:45.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/downloader.py
--rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/mecord_downloader.py
--rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/processing.py
--rw-rw-rw-   0        0        0     3934 2023-06-21 11:15:21.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/task.py
--rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/ttsUtils.py
--rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/txt2proj.py
--rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/uploading.py
--rw-rw-rw-   0        0        0    10914 2023-06-21 11:06:41.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/utils.py
--rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/video_merge.py
--rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/video_random_cutter.py
--rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.6/ttauto_crawler/ytdlp_downloader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:20:36.924141 p-ttauto-crawler-0.1.7/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-06-21 11:20:36.924141 p-ttauto-crawler-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 11:20:36.905142 p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-21 11:20:36.000000 p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-21 11:20:36.000000 p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 11:20:36.000000 p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-21 11:20:36.000000 p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-21 11:20:36.000000 p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 11:20:36.000000 p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 11:20:36.924141 p-ttauto-crawler-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-06-21 11:20:32.000000 p-ttauto-crawler-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:20:36.921141 p-ttauto-crawler-0.1.7/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/__init__.py
+-rw-rw-rw-   0        0        0     9460 2023-06-21 11:15:15.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/auto_crawler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:20:36.923141 p-ttauto-crawler-0.1.7/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/bin/print_md5.py
+-rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/binary.py
+-rw-rw-rw-   0        0        0    10986 2023-06-21 10:59:45.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/downloader.py
+-rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/mecord_downloader.py
+-rw-rw-rw-   0        0        0     9074 2023-06-21 11:20:25.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/processing.py
+-rw-rw-rw-   0        0        0     3934 2023-06-21 11:15:21.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/task.py
+-rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/ttsUtils.py
+-rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/txt2proj.py
+-rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/uploading.py
+-rw-rw-rw-   0        0        0    10914 2023-06-21 11:06:41.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/utils.py
+-rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/video_merge.py
+-rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/video_random_cutter.py
+-rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.7/ttauto_crawler/ytdlp_downloader.py
```

### Comparing `p-ttauto-crawler-0.1.6/LICENSE` & `p-ttauto-crawler-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/p_ttauto_crawler.egg-info/SOURCES.txt` & `p-ttauto-crawler-0.1.7/p_ttauto_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/setup.py` & `p-ttauto-crawler-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.1.6",
+    version="0.1.7",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -18,15 +18,15 @@
     ],
     py_modules=[],
     install_requires=[
         'requests',
         'oss2',
         'Image',
         'Pillow',
-        'p-template-generator>=0.1.67',
+        'p-template-generator>=0.1.77',
         'fake_useragent',
         'mutagen',
         'yt-dlp==2023.3.4',
         'moviepy',
         'urlparser'
     ],
     dependency_links=[],
```

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/auto_crawler.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/auto_crawler.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/bin/print_md5.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/bin/print_md5.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/binary.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/binary.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/downloader.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/main.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/main.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/mecord_downloader.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/mecord_downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/processing.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,17 @@
     data = []
     official_template_list = []
     #videos
     if len(crawler_template_name) > 0:
         for tpname in crawler_template_name:
             templateDir = os.path.join(genertor_binary.randomEffectPath(""), tpname)
             official_template_list.append(templateDir)
-            videoToTemplate(curGroupId, data, curDownloadDir, tpname, addRandomText, splitDuration, verticalScreen)
+            videoToTemplate(curGroupId, data, curDownloadDir, tpname, addRandomText, splitDuration, verticalScreen, tag)
     else:
-        videoToTemplate(curGroupId, data, curDownloadDir, "", addRandomText, splitDuration, verticalScreen)
+        videoToTemplate(curGroupId, data, curDownloadDir, "", addRandomText, splitDuration, verticalScreen, tag)
     #imgs
     if img_to_video > 0:
         if len(crawler_template_name) > 0:
             for tpname in crawler_template_name:
                 templateDir = os.path.join(genertor_binary.randomEffectPath(""), tpname)
                 official_template_list.append(templateDir)
                 processAllImage(curGroupId, data, curDownloadDir, tpname, addRandomText, img_to_video, tag)
```

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/task.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/task.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/ttsUtils.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/ttsUtils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/txt2proj.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/txt2proj.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/uploading.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/uploading.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/video_merge.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/video_merge.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/video_random_cutter.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/video_random_cutter.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.6/ttauto_crawler/ytdlp_downloader.py` & `p-ttauto-crawler-0.1.7/ttauto_crawler/ytdlp_downloader.py`

 * *Files identical despite different names*

