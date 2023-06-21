# Comparing `tmp/rpsbot-1.0.0.tar.gz` & `tmp/rpsbot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpsbot-1.0.0.tar", last modified: Sat Jun 17 17:00:11 2023, max compression
+gzip compressed data, was "rpsbot-1.0.1.tar", last modified: Wed Jun 21 18:13:27 2023, max compression
```

## Comparing `rpsbot-1.0.0.tar` & `rpsbot-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-17 17:00:11.297598 rpsbot-1.0.0/
--rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-17 17:00:11.300598 rpsbot-1.0.0/PKG-INFO
-drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-17 17:00:11.236610 rpsbot-1.0.0/rpsbot.egg-info/
--rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/PKG-INFO
--rwxrwxrwx   0 elia      (1000) elia      (1000)      181 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/SOURCES.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)        1 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/dependency_links.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)       40 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/entry_points.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)        7 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/top_level.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)     1684 2023-06-17 16:58:55.000000 rpsbot-1.0.0/rpsbot.py
--rwxrwxrwx   0 elia      (1000) elia      (1000)      286 2023-06-17 17:00:11.316794 rpsbot-1.0.0/setup.cfg
--rwxrwxrwx   0 elia      (1000) elia      (1000)      270 2023-06-17 16:24:19.000000 rpsbot-1.0.0/setup.py
+drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-21 18:13:27.843587 rpsbot-1.0.1/
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-21 18:13:27.846585 rpsbot-1.0.1/PKG-INFO
+drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-21 18:13:27.495858 rpsbot-1.0.1/rpsbot/
+-rwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-21 18:10:33.000000 rpsbot-1.0.1/rpsbot/__init__.py
+-rwxrwxrwx   0 elia      (1000) elia      (1000)       44 2023-06-21 18:11:47.000000 rpsbot-1.0.1/rpsbot/__main__.py
+-rwxrwxrwx   0 elia      (1000) elia      (1000)     1684 2023-06-17 16:58:55.000000 rpsbot-1.0.1/rpsbot/rpsbot.py
+drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-21 18:13:27.782970 rpsbot-1.0.1/rpsbot.egg-info/
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-21 18:13:26.000000 rpsbot-1.0.1/rpsbot.egg-info/PKG-INFO
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      226 2023-06-21 18:13:27.000000 rpsbot-1.0.1/rpsbot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)        1 2023-06-21 18:13:26.000000 rpsbot-1.0.1/rpsbot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)       47 2023-06-21 18:13:26.000000 rpsbot-1.0.1/rpsbot.egg-info/entry_points.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)        7 2023-06-21 18:13:26.000000 rpsbot-1.0.1/rpsbot.egg-info/top_level.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      286 2023-06-21 18:13:27.860604 rpsbot-1.0.1/setup.cfg
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      275 2023-06-21 18:10:55.000000 rpsbot-1.0.1/setup.py
```

### Comparing `rpsbot-1.0.0/rpsbot.py` & `rpsbot-1.0.1/rpsbot/rpsbot.py`

 * *Files identical despite different names*

