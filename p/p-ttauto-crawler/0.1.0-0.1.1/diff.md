# Comparing `tmp/p-ttauto-crawler-0.1.0.tar.gz` & `tmp/p-ttauto-crawler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.1.0.tar", last modified: Wed Jun 21 05:12:29 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.1.1.tar", last modified: Wed Jun 21 05:26:25 2023, max compression
```

## Comparing `p-ttauto-crawler-0.1.0.tar` & `p-ttauto-crawler-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.742390 p-ttauto-crawler-0.1.0/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      397 2023-06-21 05:12:29.742390 p-ttauto-crawler-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.726390 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 05:12:29.743391 p-ttauto-crawler-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-06-20 10:32:11.000000 p-ttauto-crawler-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.740391 p-ttauto-crawler-0.1.0/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/__init__.py
--rw-rw-rw-   0        0        0     9462 2023-06-21 05:10:39.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/auto_crawler.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.741390 p-ttauto-crawler-0.1.0/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/bin/print_md5.py
--rw-rw-rw-   0        0        0     4084 2023-06-21 05:12:20.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/binary.py
--rw-rw-rw-   0        0        0    10986 2023-06-20 10:58:46.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/downloader.py
--rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/mecord_downloader.py
--rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/processing.py
--rw-rw-rw-   0        0        0     3934 2023-06-20 07:22:50.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/task.py
--rw-rw-rw-   0        0        0     2208 2023-06-21 04:26:09.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/ttsUtils.py
--rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/txt2proj.py
--rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/uploading.py
--rw-rw-rw-   0        0        0    10914 2023-06-20 08:47:18.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/utils.py
--rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/video_merge.py
--rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/video_random_cutter.py
--rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/ytdlp_downloader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:26:25.051229 p-ttauto-crawler-0.1.1/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-06-21 05:26:25.050230 p-ttauto-crawler-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 05:26:25.027232 p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-21 05:26:24.000000 p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-21 05:26:24.000000 p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:26:24.000000 p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-21 05:26:24.000000 p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-21 05:26:24.000000 p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 05:26:24.000000 p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:26:25.051229 p-ttauto-crawler-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-06-21 05:25:30.000000 p-ttauto-crawler-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:26:25.047229 p-ttauto-crawler-0.1.1/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/__init__.py
+-rw-rw-rw-   0        0        0     9462 2023-06-21 05:25:47.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/auto_crawler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:26:25.049233 p-ttauto-crawler-0.1.1/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/bin/print_md5.py
+-rw-rw-rw-   0        0        0     4084 2023-06-21 05:12:20.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/binary.py
+-rw-rw-rw-   0        0        0    10986 2023-06-20 10:58:46.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/downloader.py
+-rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/mecord_downloader.py
+-rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/processing.py
+-rw-rw-rw-   0        0        0     3934 2023-06-20 07:22:50.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/task.py
+-rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/ttsUtils.py
+-rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/txt2proj.py
+-rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/uploading.py
+-rw-rw-rw-   0        0        0    10914 2023-06-20 08:47:18.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/utils.py
+-rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/video_merge.py
+-rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/video_random_cutter.py
+-rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.1/ttauto_crawler/ytdlp_downloader.py
```

### Comparing `p-ttauto-crawler-0.1.0/LICENSE` & `p-ttauto-crawler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/SOURCES.txt` & `p-ttauto-crawler-0.1.1/p_ttauto_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/setup.py` & `p-ttauto-crawler-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.1.0",
+    version="0.1.1",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/auto_crawler.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/auto_crawler.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/bin/print_md5.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/bin/print_md5.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/binary.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/binary.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/downloader.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/main.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/main.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/mecord_downloader.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/mecord_downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/processing.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/processing.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/task.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/task.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/ttsUtils.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/ttsUtils.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,15 +54,17 @@
                             "lyric": lyricFile(root, name),
                             "audio": audio,
                             "duration": f.info.length
                         })
                     
     return txt
     
-def randomTTS(label = "bag", duration = 0):
+def randomTTS(label = "all", duration = 0):
+    if len(label) <= 0:
+        label = "all"
     tts_list = allTTSKey(label, duration)
     tts_list_len = len(tts_list)
     if tts_list_len > 0:
         rd_idx = random.randint(0, tts_list_len-1)
         k = tts_list[rd_idx]
         with open(k["lyric"], "r", encoding="UTF-8") as f:
             s = f.read()
```

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/txt2proj.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/txt2proj.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/uploading.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/uploading.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/video_merge.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/video_merge.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/video_random_cutter.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/video_random_cutter.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.0/ttauto_crawler/ytdlp_downloader.py` & `p-ttauto-crawler-0.1.1/ttauto_crawler/ytdlp_downloader.py`

 * *Files identical despite different names*

