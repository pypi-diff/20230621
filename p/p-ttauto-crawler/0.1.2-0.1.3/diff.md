# Comparing `tmp/p-ttauto-crawler-0.1.2.tar.gz` & `tmp/p-ttauto-crawler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.1.2.tar", last modified: Wed Jun 21 07:12:53 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.1.3.tar", last modified: Wed Jun 21 10:52:56 2023, max compression
```

## Comparing `p-ttauto-crawler-0.1.2.tar` & `p-ttauto-crawler-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 07:12:53.414997 p-ttauto-crawler-0.1.2/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      397 2023-06-21 07:12:53.414997 p-ttauto-crawler-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 07:12:53.398998 p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-21 07:12:53.000000 p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-06-21 07:12:53.000000 p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 07:12:53.000000 p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-21 07:12:53.000000 p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-21 07:12:53.000000 p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 07:12:53.000000 p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 07:12:53.414997 p-ttauto-crawler-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-06-21 07:12:45.000000 p-ttauto-crawler-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:12:53.411997 p-ttauto-crawler-0.1.2/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/__init__.py
--rw-rw-rw-   0        0        0     9462 2023-06-21 05:25:47.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/auto_crawler.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:12:53.413998 p-ttauto-crawler-0.1.2/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/bin/print_md5.py
--rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/binary.py
--rw-rw-rw-   0        0        0    10986 2023-06-20 10:58:46.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/downloader.py
--rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/mecord_downloader.py
--rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/processing.py
--rw-rw-rw-   0        0        0     3934 2023-06-20 07:22:50.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/task.py
--rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/ttsUtils.py
--rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/txt2proj.py
--rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/uploading.py
--rw-rw-rw-   0        0        0    10914 2023-06-20 08:47:18.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/utils.py
--rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/video_merge.py
--rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/video_random_cutter.py
--rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.2/ttauto_crawler/ytdlp_downloader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:52:56.811818 p-ttauto-crawler-0.1.3/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-06-21 10:52:56.810819 p-ttauto-crawler-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 10:52:56.794819 p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-21 10:52:56.000000 p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-21 10:52:56.000000 p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 10:52:56.000000 p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-21 10:52:56.000000 p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-21 10:52:56.000000 p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 10:52:56.000000 p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 10:52:56.811818 p-ttauto-crawler-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-06-21 10:52:45.000000 p-ttauto-crawler-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:52:56.808818 p-ttauto-crawler-0.1.3/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/__init__.py
+-rw-rw-rw-   0        0        0     9464 2023-06-21 10:52:38.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/auto_crawler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:52:56.810819 p-ttauto-crawler-0.1.3/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/bin/print_md5.py
+-rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/binary.py
+-rw-rw-rw-   0        0        0    10986 2023-06-20 10:58:46.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/downloader.py
+-rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/mecord_downloader.py
+-rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/processing.py
+-rw-rw-rw-   0        0        0     3934 2023-06-20 07:22:50.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/task.py
+-rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/ttsUtils.py
+-rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/txt2proj.py
+-rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/uploading.py
+-rw-rw-rw-   0        0        0    10914 2023-06-20 08:47:18.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/utils.py
+-rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/video_merge.py
+-rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/video_random_cutter.py
+-rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.3/ttauto_crawler/ytdlp_downloader.py
```

### Comparing `p-ttauto-crawler-0.1.2/LICENSE` & `p-ttauto-crawler-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/p_ttauto_crawler.egg-info/SOURCES.txt` & `p-ttauto-crawler-0.1.3/p_ttauto_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/setup.py` & `p-ttauto-crawler-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.1.2",
+    version="0.1.3",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/auto_crawler.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/auto_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,54 +109,54 @@
                 url = url.replace("VerticalScreen=true","")
             return curGroupId, url, template_name_list, video_merge_num, video_merge_second, img_to_video, split_video, add_text, verticalScreen, tag
     return None, None, None, None, None, None, None, None, None, None
 
 def autoCrawler():    
     thisFileDir = os.path.dirname(os.path.abspath(__file__))
     global THEADING_LIST
-    for i in range(0, 5):
+    for i in range(0, 2):
         THEADING_LIST.append(CralwerThread(t=task.C_STATE.DOWNLOADING))
     for i in range(0, 2):
         THEADING_LIST.append(CralwerThread(t=task.C_STATE.TEMPLATEING))
-    for i in range(0, 5):
+    for i in range(0, 2):
         THEADING_LIST.append(CralwerThread(t=task.C_STATE.UPLOADING))
     while (os.path.exists(os.path.join(thisFileDir, "stop.now")) == False):
         if task.canAddDownload(lock):
             try:
-                # task.push(lock, {
-                #     "curGroupId":0, 
-                #     "url":"ftp://192.168.3.220/1TB01/data/test/",
-                #     "crawler_template_name":[], 
-                #     "addRandomText":True, 
-                #     "splitDuration":0, 
-                #     "img_to_video":5,
-                #     "video_merge_num":0,
-                #     "video_merge_second":0, 
-                #     "verticalScreen":False, 
-                #     "tag":"bag"
-                # })
-                curGroupId, url, template_name_list, video_merge_num, video_merge_second, img_to_video, split_video, add_text, verticalScreen, tag = getTask()
-                if curGroupId:    
-                    task.push(lock, {
-                        "curGroupId":curGroupId, 
-                        "url":url,
-                        "crawler_template_name":template_name_list, 
-                        "addRandomText":add_text, 
-                        "splitDuration":split_video, 
-                        "img_to_video":img_to_video,
-                        "video_merge_num":video_merge_num,
-                        "video_merge_second":video_merge_second, 
-                        "verticalScreen":verticalScreen, 
-                        "tag":tag
-                    })
+                task.push(lock, {
+                    "curGroupId":0, 
+                    "url":"ftp://192.168.3.220/1TB01/data/test/",
+                    "crawler_template_name":[], 
+                    "addRandomText":True, 
+                    "splitDuration":0, 
+                    "img_to_video":5,
+                    "video_merge_num":0,
+                    "video_merge_second":0, 
+                    "verticalScreen":False, 
+                    "tag":"bag"
+                })
+                # curGroupId, url, template_name_list, video_merge_num, video_merge_second, img_to_video, split_video, add_text, verticalScreen, tag = getTask()
+                # if curGroupId:    
+                #     task.push(lock, {
+                #         "curGroupId":curGroupId, 
+                #         "url":url,
+                #         "crawler_template_name":template_name_list, 
+                #         "addRandomText":add_text, 
+                #         "splitDuration":split_video, 
+                #         "img_to_video":img_to_video,
+                #         "video_merge_num":video_merge_num,
+                #         "video_merge_second":video_merge_second, 
+                #         "verticalScreen":verticalScreen, 
+                #         "tag":tag
+                #     })
             except Exception as e:
                 utils.logInfo("====================== uncatch Exception ======================", False)
                 utils.logInfo(e, False)
                 utils.logInfo("======================      end      ======================", False)
-        time.sleep(600)
+        time.sleep(6)
     utils.logInfo(f"prepare stop !", False)
     for t in THEADING_LIST:
         t.markStop()
     for t in THEADING_LIST:
         t.join()
     os.remove(os.path.join(thisFileDir, "stop.now"))
     utils.logInfo(f"stoped !", False)
```

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/bin/print_md5.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/bin/print_md5.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/binary.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/binary.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/downloader.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/main.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/main.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/mecord_downloader.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/mecord_downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/processing.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/processing.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/task.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/task.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/ttsUtils.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/ttsUtils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/txt2proj.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/txt2proj.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/uploading.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/uploading.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/video_merge.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/video_merge.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/video_random_cutter.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/video_random_cutter.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.2/ttauto_crawler/ytdlp_downloader.py` & `p-ttauto-crawler-0.1.3/ttauto_crawler/ytdlp_downloader.py`

 * *Files identical despite different names*

