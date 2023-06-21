# Comparing `tmp/y2mate-api-0.0.4.tar.gz` & `tmp/y2mate-api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.4.tar", last modified: Tue Jun 20 11:15:14 2023, max compression
+gzip compressed data, was "y2mate-api-0.0.5.tar", last modified: Wed Jun 21 11:50:21 2023, max compression
```

## Comparing `y2mate-api-0.0.4.tar` & `y2mate-api-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:14.210421 y2mate-api-0.0.4/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.4/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    10845 2023-06-20 11:15:14.190421 y2mate-api-0.0.4/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     9750 2023-06-20 11:11:01.000000 y2mate-api-0.0.4/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-20 11:15:14.214421 y2mate-api-0.0.4/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.4/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:13.774421 y2mate-api-0.0.4/tests/
--rw-rw----   0 root         (0) everybody  (9997)      255 2023-06-15 19:45:34.000000 y2mate-api-0.0.4/tests/test.py
--rw-rw----   0 root         (0) everybody  (9997)      267 2023-06-15 19:39:07.000000 y2mate-api-0.0.4/tests/test_1.py
--rw-rw----   0 root         (0) everybody  (9997)      261 2023-06-15 20:21:38.000000 y2mate-api-0.0.4/tests/test_3.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:13.974421 y2mate-api-0.0.4/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-19 17:39:27.000000 y2mate-api-0.0.4/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.4/y2mate_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     5333 2023-06-19 18:27:02.000000 y2mate-api-0.0.4/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    13935 2023-06-19 18:39:05.000000 y2mate-api-0.0.4/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14849 2023-06-19 13:09:05.000000 y2mate-api-0.0.4/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:14.174421 y2mate-api-0.0.4/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    10845 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      390 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.966188 y2mate-api-0.0.5/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.5/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-21 11:50:20.946188 y2mate-api-0.0.5/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     9751 2023-06-21 11:45:37.000000 y2mate-api-0.0.5/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-21 11:50:20.966188 y2mate-api-0.0.5/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.5/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.510188 y2mate-api-0.0.5/tests/
+-rw-rw----   0 root         (0) everybody  (9997)     1565 2023-06-20 21:34:48.000000 y2mate-api-0.0.5/tests/test_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.5/tests/test_queries.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.662188 y2mate-api-0.0.5/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-21 11:46:18.000000 y2mate-api-0.0.5/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.5/y2mate_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5333 2023-06-19 18:27:02.000000 y2mate-api-0.0.5/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    14001 2023-06-20 16:45:31.000000 y2mate-api-0.0.5/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14438 2023-06-21 11:48:19.000000 y2mate-api-0.0.5/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-21 11:50:20.862188 y2mate-api-0.0.5/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    10846 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-21 11:50:19.000000 y2mate-api-0.0.5/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.4/LICENSE` & `y2mate-api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.4/PKG-INFO` & `y2mate-api-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.5&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -159,15 +159,15 @@
   * timeout : http requests timeout
   * ask : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
   * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
-  * quality : Media qualiy such as 720p/128kbps
+  * quality : Media quality such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
   * limit : Total videos to be retrieved
   * keyword : Phrase(s) that must be in media title
   * author : Video author i.e Youtube Channel
 
 - `Handler.auto_save`
   * dir : Path to Directory for saving the media files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.4 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.5 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -54,15 +54,15 @@
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
 requests timeout * ask : Confirm before downloading media * unique : Auto-
 ignore previously downloaded media * thread : Download (x) value of file at a
-time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media qualiy
+time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media quality
 such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
```

### Comparing `y2mate-api-0.0.4/README.md` & `y2mate-api-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.5&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -131,15 +131,15 @@
   * timeout : http requests timeout
   * ask : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
   * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
-  * quality : Media qualiy such as 720p/128kbps
+  * quality : Media quality such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
   * limit : Total videos to be retrieved
   * keyword : Phrase(s) that must be in media title
   * author : Video author i.e Youtube Channel
 
 - `Handler.auto_save`
   * dir : Path to Directory for saving the media files
```

#### html2text {}

```diff
@@ -40,15 +40,15 @@
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
 requests timeout * ask : Confirm before downloading media * unique : Auto-
 ignore previously downloaded media * thread : Download (x) value of file at a
-time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media qualiy
+time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media quality
 such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
```

### Comparing `y2mate-api-0.0.4/setup.py` & `y2mate-api-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.4/y2mate_api/console.py` & `y2mate-api-0.0.5/y2mate_api/console.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.4/y2mate_api/downloader.py` & `y2mate-api-0.0.5/y2mate_api/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,15 +352,17 @@
                     % (Fore.GREEN, size_in_mb, Fore.CYAN, Fore.YELLOW, Fore.RESET),
                 ) as p_bar:
                     with open(save_to, "wb") as fh:
                         for chunks in resp.iter_content(chunk_size=chunk_size):
                             fh.write(chunks)
                             p_bar.update(chunk_size)
                     utils.add_history(third_dict)
+                    return save_to
             else:
                 with open(save_to, "wb") as fh:
                     for chunks in resp.iter_content(chunk_size=chunk_size):
                         fh.write(chunks)
                 utils.add_history(third_dict)
                 logging.info(f"{filename} - {size_in_mb}MB ✅")
+                return save_to
         else:
             logging.error(f"Empty `third_dict` parameter parsed : {third_dict}")
```

### Comparing `y2mate-api-0.0.4/y2mate_api/main.py` & `y2mate-api-0.0.5/y2mate_api/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -190,17 +190,16 @@
     def __init__(self, query_one: object, item_no: int = 0):
         r"""Initializes second_query class
         :param query_one: Query_one class
         :type query_one: object
         :param item_no: (Optional) Query_one.vitems index
         :type item_no: int
         """
-        if not query_one.processed:
+        assert query_one.processed, "First query failed"
 
-            raise Exception("First query failed")
         self.query_one = query_one
         self.item_no = item_no
         self.processed = False
         self.video_dict = None
         self.url = "https://www.y2mate.com/mates/analyzeV2/ajax"
         # self.payload  = self.__get_payload()
 
@@ -312,16 +311,15 @@
             logging.error(f"Second query failed - [{resp.status_code} : {resp.reason}")
         return self
 
 
 class third_query:
     def __init__(self, query_two: object):
 
-        if not query_two.processed:
-            raise Execption("Unprocessed second_query object parsed")
+        assert query_two.processed, "Unprocessed second_query object parsed"
         self.query_two = query_two
         self.url = "https://www.y2mate.com/mates/convertV2/index"
         self.formats = ["mp4", "mp3"]
         self.qualities = {
             self.formats[0]: [
                 "4k",
                 "1080p",
@@ -384,15 +382,15 @@
         if not format in self.formats:
 
             raise Exception(f"'{format}' is not in supported formats - {self.formats}")
 
         if not quality in self.qualities[format]:
 
             raise Exception(
-                "'{quality}' is not in supported qualities - {self.qualities[format]}"
+                f"'{quality}' is not in supported qualities - {self.qualities[format]}"
             )
         items = self.query_two.video if format == "mp4" else self.query_two.audio
         hunted = []
         for key in items.keys():
             if items[key].get("q") == quality:
                 hunted.append(items[key])
         if len(hunted) > 1:
@@ -432,24 +430,8 @@
                     f"Third query failed - [{resp.status_code} : {resp.reason}"
                 )
                 return {}
         else:
             logging.error(
                 f"Zero media hunted with params : {{quality : {quality}, format : {format}  }}"
             )
-            return {}
-
-
-def main_():
-    # from sys import exit
-    y2 = first_query("Alan walker lonely")  # "https://youtu.be/q88kDdMRVAQ")
-    run1 = y2()
-    run2 = second_query(run1())
-    # print(dir(run2))
-    run3 = third_query(run2()).main(format="mp4", quality="360p")
-    import json
-
-    print(json.dumps(run3, indent=4))
-
-
-if __name__ == "__main__":
-    main_()
+            return {}
```

### Comparing `y2mate-api-0.0.4/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-0.0.5/y2mate_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.5&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -159,15 +159,15 @@
   * timeout : http requests timeout
   * ask : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
   * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
-  * quality : Media qualiy such as 720p/128kbps
+  * quality : Media quality such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
   * limit : Total videos to be retrieved
   * keyword : Phrase(s) that must be in media title
   * author : Video author i.e Youtube Channel
 
 - `Handler.auto_save`
   * dir : Path to Directory for saving the media files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.4 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.5 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -54,15 +54,15 @@
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
 requests timeout * ask : Confirm before downloading media * unique : Auto-
 ignore previously downloaded media * thread : Download (x) value of file at a
-time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media qualiy
+time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media quality
 such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
```

