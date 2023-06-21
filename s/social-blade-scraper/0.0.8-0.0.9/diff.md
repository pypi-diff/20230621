# Comparing `tmp/social-blade-scraper-0.0.8.tar.gz` & `tmp/social-blade-scraper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-blade-scraper-0.0.8.tar", last modified: Wed Jun 21 10:14:14 2023, max compression
+gzip compressed data, was "social-blade-scraper-0.0.9.tar", last modified: Wed Jun 21 10:49:25 2023, max compression
```

## Comparing `social-blade-scraper-0.0.8.tar` & `social-blade-scraper-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:14:14.770053 social-blade-scraper-0.0.8/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 10:14:14.770053 social-blade-scraper-0.0.8/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.0.8/README.md
--rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-21 10:14:14.770053 social-blade-scraper-0.0.8/setup.cfg
--rw-rw-r--   0 tej       (1000) tej       (1000)      717 2023-06-21 10:13:43.000000 social-blade-scraper-0.0.8/setup.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:14:14.766053 social-blade-scraper-0.0.8/src/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.0.8/src/__init__.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:14:14.766053 social-blade-scraper-0.0.8/src/social_blade_scraper/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.0.8/src/social_blade_scraper/__init__.py
--rw-rw-r--   0 tej       (1000) tej       (1000)     1284 2023-06-21 10:13:05.000000 social-blade-scraper-0.0.8/src/social_blade_scraper/fetch.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:14:14.770053 social-blade-scraper-0.0.8/src/social_blade_scraper/stats/
--rw-rw-r--   0 tej       (1000) tej       (1000)    12316 2023-06-21 09:24:07.000000 social-blade-scraper-0.0.8/src/social_blade_scraper/stats/youtube.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:14:14.770053 social-blade-scraper-0.0.8/src/social_blade_scraper.egg-info/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 10:14:14.000000 social-blade-scraper-0.0.8/src/social_blade_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)      408 2023-06-21 10:14:14.000000 social-blade-scraper-0.0.8/src/social_blade_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-21 10:14:14.000000 social-blade-scraper-0.0.8/src/social_blade_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       36 2023-06-21 10:14:14.000000 social-blade-scraper-0.0.8/src/social_blade_scraper.egg-info/requires.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-21 10:14:14.000000 social-blade-scraper-0.0.8/src/social_blade_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:14:14.770053 social-blade-scraper-0.0.8/tests/
--rw-rw-r--   0 tej       (1000) tej       (1000)     1923 2023-06-21 09:08:45.000000 social-blade-scraper-0.0.8/tests/test_youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:49:25.299029 social-blade-scraper-0.0.9/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 10:49:25.299029 social-blade-scraper-0.0.9/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.0.9/README.md
+-rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-21 10:49:25.299029 social-blade-scraper-0.0.9/setup.cfg
+-rw-rw-r--   0 tej       (1000) tej       (1000)      717 2023-06-21 10:49:12.000000 social-blade-scraper-0.0.9/setup.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:49:25.295029 social-blade-scraper-0.0.9/src/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.0.9/src/__init__.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:49:25.295029 social-blade-scraper-0.0.9/src/social_blade_scraper/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.0.9/src/social_blade_scraper/__init__.py
+-rw-rw-r--   0 tej       (1000) tej       (1000)      995 2023-06-21 10:48:46.000000 social-blade-scraper-0.0.9/src/social_blade_scraper/fetch.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:49:25.295029 social-blade-scraper-0.0.9/src/social_blade_scraper/stats/
+-rw-rw-r--   0 tej       (1000) tej       (1000)    12316 2023-06-21 09:24:07.000000 social-blade-scraper-0.0.9/src/social_blade_scraper/stats/youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:49:25.295029 social-blade-scraper-0.0.9/src/social_blade_scraper.egg-info/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 10:49:25.000000 social-blade-scraper-0.0.9/src/social_blade_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)      408 2023-06-21 10:49:25.000000 social-blade-scraper-0.0.9/src/social_blade_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-21 10:49:25.000000 social-blade-scraper-0.0.9/src/social_blade_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       36 2023-06-21 10:49:25.000000 social-blade-scraper-0.0.9/src/social_blade_scraper.egg-info/requires.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-21 10:49:25.000000 social-blade-scraper-0.0.9/src/social_blade_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 10:49:25.295029 social-blade-scraper-0.0.9/tests/
+-rw-rw-r--   0 tej       (1000) tej       (1000)     1923 2023-06-21 09:08:45.000000 social-blade-scraper-0.0.9/tests/test_youtube.py
```

### Comparing `social-blade-scraper-0.0.8/setup.py` & `social-blade-scraper-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="social-blade-scraper",
-    version="0.0.8",
+    version="0.0.9",
     description="Social blade scraper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/tejmagar/social-blade-scraper",
     install_requires=[
         "beautifulsoup4",
```

### Comparing `social-blade-scraper-0.0.8/src/social_blade_scraper/stats/youtube.py` & `social-blade-scraper-0.0.9/src/social_blade_scraper/stats/youtube.py`

 * *Files identical despite different names*

### Comparing `social-blade-scraper-0.0.8/tests/test_youtube.py` & `social-blade-scraper-0.0.9/tests/test_youtube.py`

 * *Files identical despite different names*

