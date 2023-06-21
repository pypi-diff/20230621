# Comparing `tmp/twtr-nuuuwan-1.0.6.tar.gz` & `tmp/twtr-nuuuwan-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtr-nuuuwan-1.0.6.tar", last modified: Thu Jun 15 12:12:07 2023, max compression
+gzip compressed data, was "twtr-nuuuwan-1.0.7.tar", last modified: Wed Jun 21 08:29:06 2023, max compression
```

## Comparing `twtr-nuuuwan-1.0.6.tar` & `twtr-nuuuwan-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.194621 twtr-nuuuwan-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.194621 twtr-nuuuwan-1.0.6/src/twtr/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.194621 twtr-nuuuwan-1.0.6/src/twtr/core/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/core/Tweet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/core/Twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/tests/test_twitter_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/src/twtr/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/src/twtr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/src/twtr/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/src/twtr/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/src/twtr/core/Tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/src/twtr/core/Twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/src/twtr/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/src/twtr_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-21 08:29:06.000000 twtr-nuuuwan-1.0.7/src/twtr_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 08:29:06.000000 twtr-nuuuwan-1.0.7/src/twtr_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:29:06.000000 twtr-nuuuwan-1.0.7/src/twtr_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:29:06.000000 twtr-nuuuwan-1.0.7/src/twtr_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 08:29:06.000000 twtr-nuuuwan-1.0.7/src/twtr_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:29:06.743819 twtr-nuuuwan-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-21 08:28:16.000000 twtr-nuuuwan-1.0.7/tests/test_twitter_basic.py
```

### Comparing `twtr-nuuuwan-1.0.6/LICENSE` & `twtr-nuuuwan-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twtr-nuuuwan-1.0.6/setup.py` & `twtr-nuuuwan-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'twtr'
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 DESCRIPTION = "Wrapper library for the Twitter API and tweepy"
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
```

### Comparing `twtr-nuuuwan-1.0.6/src/twtr/core/Twitter.py` & `twtr-nuuuwan-1.0.7/src/twtr/core/Twitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import argparse
 import os
+import random
+import time
 
 import tweepy
 
 from twtr.common import log
 from twtr.core.Tweet import Tweet
 
 MIN_TOKEN_LEN = 8
@@ -71,27 +73,33 @@
             consumer_key=consumer_key,
             consumer_secret=consumer_secret,
             access_token=access_token,
             access_token_secret=access_token_secret,
         )
         self.__api__ = tweepy.API(auth)
 
+    def sleep_random(self):
+        t = random.randint(10, 30)
+        log.debug(f'Sleeping for {t} seconds...')
+        time.sleep(t)
+
     def check_api_and_client(self):
         if self.__client__ is None:
             raise ValueError('Client is not valid')
 
     def __media_upload__(self, image_path: str) -> int:
         if not os.path.exists(image_path):
             raise FileNotFoundError(f'Image not found: {image_path}')
 
         self.check_api_and_client()
         media = self.__api__.media_upload(image_path)
         log.debug(f'{media=}')
         media_id = media.media_id
         log.debug(f'Uploaded media {image_path} to {media_id}.')
+        self.sleep_random()
         return media_id
 
     def __media_upload_all__(self, image_path_list: list[str]) -> list[int]:
         media_ids = []
         for image_path in image_path_list:
             media_id = self.__media_upload__(image_path)
             media_ids.append(media_id)
@@ -116,14 +124,15 @@
             response = self.__client__.create_tweet(
                 text=tweet.text,
             )
 
         log.debug(f'{response=}')
         tweet_id = response.data['id']
         log.debug(f'Sent tweet ({tweet_id}).')
+        self.sleep_random()
         return tweet_id
 
     def send(self, tweet: Tweet):
         try:
             return self.__create_tweet__(tweet)
         except Exception as e:
             log.error(f'Failed to send tweet: {e}')
```

### Comparing `twtr-nuuuwan-1.0.6/tests/test_twitter_basic.py` & `twtr-nuuuwan-1.0.7/tests/test_twitter_basic.py`

 * *Files identical despite different names*

