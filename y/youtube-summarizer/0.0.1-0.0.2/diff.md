# Comparing `tmp/youtube_summarizer-0.0.1.tar.gz` & `tmp/youtube_summarizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_summarizer-0.0.1.tar", last modified: Wed Jun 21 19:15:04 2023, max compression
+gzip compressed data, was "youtube_summarizer-0.0.2.tar", last modified: Wed Jun 21 19:26:27 2023, max compression
```

## Comparing `youtube_summarizer-0.0.1.tar` & `youtube_summarizer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:15:04.651100 youtube_summarizer-0.0.1/
--rw-r--r--   0 isaacduong   (501) staff       (20)      252 2023-06-21 19:15:04.650931 youtube_summarizer-0.0.1/PKG-INFO
--rw-r--r--   0 isaacduong   (501) staff       (20)     3152 2023-06-21 17:47:12.000000 youtube_summarizer-0.0.1/README.md
--rw-r--r--   0 isaacduong   (501) staff       (20)       38 2023-06-21 19:15:04.651158 youtube_summarizer-0.0.1/setup.cfg
--rw-r--r--   0 isaacduong   (501) staff       (20)      373 2023-06-21 19:14:55.000000 youtube_summarizer-0.0.1/setup.py
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:15:04.649768 youtube_summarizer-0.0.1/src/
--rw-r--r--   0 isaacduong   (501) staff       (20)        0 2023-06-21 18:29:06.000000 youtube_summarizer-0.0.1/src/__init__.py
--rw-r--r--   0 isaacduong   (501) staff       (20)    10617 2023-06-21 19:10:55.000000 youtube_summarizer-0.0.1/src/youtube_video_summary.py
-drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:15:04.650661 youtube_summarizer-0.0.1/youtube_summarizer.egg-info/
--rw-r--r--   0 isaacduong   (501) staff       (20)      252 2023-06-21 19:15:04.000000 youtube_summarizer-0.0.1/youtube_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 isaacduong   (501) staff       (20)      231 2023-06-21 19:15:04.000000 youtube_summarizer-0.0.1/youtube_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)        1 2023-06-21 19:15:04.000000 youtube_summarizer-0.0.1/youtube_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 isaacduong   (501) staff       (20)        4 2023-06-21 19:15:04.000000 youtube_summarizer-0.0.1/youtube_summarizer.egg-info/top_level.txt
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:26:27.085346 youtube_summarizer-0.0.2/
+-rw-r--r--   0 isaacduong   (501) staff       (20)      252 2023-06-21 19:26:27.085185 youtube_summarizer-0.0.2/PKG-INFO
+-rw-r--r--   0 isaacduong   (501) staff       (20)     3152 2023-06-21 17:47:12.000000 youtube_summarizer-0.0.2/README.md
+-rw-r--r--   0 isaacduong   (501) staff       (20)       38 2023-06-21 19:26:27.085400 youtube_summarizer-0.0.2/setup.cfg
+-rw-r--r--   0 isaacduong   (501) staff       (20)      383 2023-06-21 19:26:23.000000 youtube_summarizer-0.0.2/setup.py
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:26:27.083609 youtube_summarizer-0.0.2/src/
+-rw-r--r--   0 isaacduong   (501) staff       (20)        0 2023-06-21 18:29:06.000000 youtube_summarizer-0.0.2/src/__init__.py
+-rw-r--r--   0 isaacduong   (501) staff       (20)    10617 2023-06-21 19:10:55.000000 youtube_summarizer-0.0.2/src/youtube_video_summary.py
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:26:27.084480 youtube_summarizer-0.0.2/youtube_summarizer.egg-info/
+-rw-r--r--   0 isaacduong   (501) staff       (20)      252 2023-06-21 19:26:27.000000 youtube_summarizer-0.0.2/youtube_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 isaacduong   (501) staff       (20)      296 2023-06-21 19:26:27.000000 youtube_summarizer-0.0.2/youtube_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)        1 2023-06-21 19:26:27.000000 youtube_summarizer-0.0.2/youtube_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 isaacduong   (501) staff       (20)       14 2023-06-21 19:26:27.000000 youtube_summarizer-0.0.2/youtube_summarizer.egg-info/top_level.txt
+drwxr-xr-x   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:26:27.084814 youtube_summarizer-0.0.2/yt_summarizer/
+-rw-r--r--   0 isaacduong   (501) staff       (20)        0 2023-06-21 19:25:30.000000 youtube_summarizer-0.0.2/yt_summarizer/__init__.py
+-rw-r--r--   0 isaacduong   (501) staff       (20)    10617 2023-06-21 19:25:17.000000 youtube_summarizer-0.0.2/yt_summarizer/youtube_video_summary.py
```

### Comparing `youtube_summarizer-0.0.1/README.md` & `youtube_summarizer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `youtube_summarizer-0.0.1/src/youtube_video_summary.py` & `youtube_summarizer-0.0.2/src/youtube_video_summary.py`

 * *Files identical despite different names*

