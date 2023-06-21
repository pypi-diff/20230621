# Comparing `tmp/etm-dgraham-5.1.4.tar.gz` & `tmp/etm-dgraham-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.1.4.tar", last modified: Mon Jun 19 17:40:24 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.5.tar", last modified: Wed Jun 21 13:13:52 2023, max compression
```

## Comparing `etm-dgraham-5.1.4.tar` & `etm-dgraham-5.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.970517 etm-dgraham-5.1.4/
--rw-r--r--   0 dag        (501) staff       (20)     2491 2023-06-19 17:40:17.000000 etm-dgraham-5.1.4/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-19 17:40:24.970365 etm-dgraham-5.1.4/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.4/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.4/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.4/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.962495 etm-dgraham-5.1.4/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.966120 etm-dgraham-5.1.4/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.4/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-19 17:40:17.000000 etm-dgraham-5.1.4/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.4/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.4/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.4/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   285975 2023-06-19 17:40:17.000000 etm-dgraham-5.1.4/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.4/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.4/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   100087 2023-06-19 09:51:43.000000 etm-dgraham-5.1.4/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.968675 etm-dgraham-5.1.4/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-19 17:40:24.000000 etm-dgraham-5.1.4/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.4/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.4/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.4/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-19 17:40:24.970552 etm-dgraham-5.1.4/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.4/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.968784 etm-dgraham-5.1.4/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.4/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-19 17:40:24.969838 etm-dgraham-5.1.4/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.4/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.4/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.4/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.4/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 13:13:52.754186 etm-dgraham-5.1.5/
+-rw-r--r--   0 dag        (501) staff       (20)     2481 2023-06-21 13:13:42.000000 etm-dgraham-5.1.5/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.5/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132192 2023-06-21 13:13:52.754043 etm-dgraham-5.1.5/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131280 2023-06-21 13:13:42.000000 etm-dgraham-5.1.5/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.5/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.5/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 13:13:52.746526 etm-dgraham-5.1.5/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.5/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.5/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.5/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 13:13:52.749729 etm-dgraham-5.1.5/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.5/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.5/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-21 13:13:42.000000 etm-dgraham-5.1.5/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.5/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.5/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.5/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   286845 2023-06-21 13:13:42.000000 etm-dgraham-5.1.5/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.5/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.5/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100697 2023-06-21 13:13:42.000000 etm-dgraham-5.1.5/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 13:13:52.751980 etm-dgraham-5.1.5/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132192 2023-06-21 13:13:52.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-21 13:13:52.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-21 13:13:52.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-21 13:13:52.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-21 13:13:52.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-21 13:13:52.000000 etm-dgraham-5.1.5/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.5/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.5/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.5/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.5/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.5/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.5/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-21 13:13:52.754224 etm-dgraham-5.1.5/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.5/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 13:13:52.752112 etm-dgraham-5.1.5/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.5/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 13:13:52.753509 etm-dgraham-5.1.5/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.5/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.5/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.5/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.5/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.1.4/CHANGES.txt` & `etm-dgraham-5.1.5/CHANGES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-Recent tagged changes as of 2023-06-19T13:40:16.377730-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.1.4) Daniel Graham
+Recent tagged changes as of 2023-06-21T09:13:39.987856-04:00:
+- 1 second ago (HEAD -> working, tag: 5.1.5) Daniel Graham
+    17d91e2 2023-06-21 09:13:39 -0400
+    Tagged version 5.1.5.
+
+- 2 days ago (tag: 5.1.4) Daniel Graham
     84421ec 2023-06-19 13:40:16 -0400
     Tagged version 5.1.4.
 
-- 2 hours ago (tag: 5.1.3) Daniel Graham
+- 2 days ago (tag: 5.1.3) Daniel Graham
     c776097 2023-06-19 11:40:16 -0400
     Tagged version 5.1.3.
 
-- 8 hours ago (tag: 5.1.2) Daniel Graham
+- 2 days ago (tag: 5.1.2) Daniel Graham
     3483b69 2023-06-19 05:51:42 -0400
     Tagged version 5.1.2.
 
-- 29 hours ago (tag: 5.1.1) Daniel Graham
+- 3 days ago (tag: 5.1.1) Daniel Graham
     d0c733f 2023-06-18 08:29:16 -0400
     Tagged version 5.1.1.
 
-- 30 hours ago (tag: 5.1.0) Daniel Graham
+- 3 days ago (tag: 5.1.0) Daniel Graham
     ece86e8 2023-06-18 07:28:25 -0400
     Tagged version 5.1.0. Added ability to display completion history
     for tasks including skipped instead of finished instances.
 
-- 2 days ago (tag: 5.0.12) Daniel Graham
+- 4 days ago (tag: 5.0.12) Daniel Graham
     c42576c 2023-06-17 08:57:03 -0400
     Tagged version 5.0.12.
 
-- 2 days ago (tag: 5.0.11) Daniel Graham
+- 4 days ago (tag: 5.0.11) Daniel Graham
     e9228d2 2023-06-17 05:19:31 -0400
     Tagged version 5.0.11.
 
-- 2 days ago (tag: 5.0.10) Daniel Graham
+- 4 days ago (tag: 5.0.10) Daniel Graham
     2e1f579 2023-06-17 05:05:32 -0400
     Tagged version 5.0.10.
 
-- 4 days ago (tag: 5.0.9) Daniel Graham
+- 6 days ago (tag: 5.0.9) Daniel Graham
     7f30e8b 2023-06-15 10:14:19 -0400
     Tagged version 5.0.9.
 
-- 6 days ago (tag: 5.0.8) Daniel Graham
+- 8 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
-- 11 days ago (tag: 5.0.7) Daniel Graham
+- 13 days ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
 
 - 2 weeks ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
@@ -65,19 +69,15 @@
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
 - 2 weeks ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
-- 2 weeks ago (tag: 5.0.0) Daniel Graham
+- 3 weeks ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
 
-- 3 weeks ago (tag: 4.12.9) Daniel Graham
+- 4 weeks ago (tag: 4.12.9) Daniel Graham
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
-
-- 3 weeks ago (tag: 4.12.8) Daniel Graham
-    b0316d5 2023-05-26 13:50:15 -0400
-    Tagged version 4.12.8.
```

### Comparing `etm-dgraham-5.1.4/PKG-INFO` & `etm-dgraham-5.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.4
+Version: 5.1.5
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -57,16 +57,16 @@
     -   [Menus](#menus)
         -   [etm menu notes](#etm-menu-notes)
         -   [view menu notes](#view-menu-notes)
         -   [editor menu notes](#editor-menu-notes)
         -   [selected menu notes](#selected-menu-notes)
     -   [Installation](#installation)
         -   [For personal use](#for-personal-use)
-        -   [for use in an isolated environment](#for-use-in-an-isolated-environment)
-        -   [for use system wide](#for-use-system-wide)
+        -   [For use in an isolated environment](#for-use-in-an-isolated-environment)
+        -   [For use system wide](#for-use-system-wide)
     -   [Usage](#usage)
         -   [Terminal size and color](#terminal-size-and-color)
         -   [Home directory](#home-directory)
         -   [Timers](#timers)
         -   [lorem examples](#loremexamples)
         -   [Using etm+](#etmplus)
     -   [Deinstallation](#deinstallation)
@@ -1528,37 +1528,38 @@
 
 [↺ contents](#contents)
 
 ## Deinstallation {#deinstallation}
 
 ### From a personal installation {#from-a-personal-installation}
 
-To remove *etm* installed into, say, python3, run
+To remove *etm* run
 
-    $ python3 -m pip uninstall etm-dgraham
+    $ pip uninstall etm-dgraham
 
 This will remove *etm* from the python site-packages directory and the *etm* and *etm+* executables from the python bin directory. Then remove any *etm home* directories that you have created.
 
 [↺ contents](#contents)
 
 ### From a virtual environment {#from-a-virtual-environment}
 
-If you should ever want to deinstall etm, first deactivate the virtual environment, if necessary, by changing to the virtual environment directory and entering
+Use *pipx* instead of *pip*:
 
-        (env) $ deactivate
+    $ pipx uninstall etm-dgraham
 
-You can now simply delete the virtual environment directory and, if you have additional *home* directories, delete each of them. One of the many advantages of the virtual environment is that these steps remove every trace.
+You can now remove any *home* directories you may have created.
 
 [↺ contents](#contents)
 
 ### From a system wide installation {#from-a-system-wide-installation}
 
 To remove *etm* installed into, say, python3.7, run
 
-    $ sudo -H python3.7 -m pip uninstall etm-dgraham
+    $ sudo -H pip uninstall etm-dgraham
+
 This will remove *etm* from the python site-packages directory and the *etm* and *etm+* executables from the python bin directory. Then remove any *etm home* directories that you have created.
 
 [↺ contents](#contents)
 
 # Details {#details}
 
 ## Item Types {#item-types}
```

### Comparing `etm-dgraham-5.1.4/README.md` & `etm-dgraham-5.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     -   [Menus](#menus)
         -   [etm menu notes](#etm-menu-notes)
         -   [view menu notes](#view-menu-notes)
         -   [editor menu notes](#editor-menu-notes)
         -   [selected menu notes](#selected-menu-notes)
     -   [Installation](#installation)
         -   [For personal use](#for-personal-use)
-        -   [for use in an isolated environment](#for-use-in-an-isolated-environment)
-        -   [for use system wide](#for-use-system-wide)
+        -   [For use in an isolated environment](#for-use-in-an-isolated-environment)
+        -   [For use system wide](#for-use-system-wide)
     -   [Usage](#usage)
         -   [Terminal size and color](#terminal-size-and-color)
         -   [Home directory](#home-directory)
         -   [Timers](#timers)
         -   [lorem examples](#loremexamples)
         -   [Using etm+](#etmplus)
     -   [Deinstallation](#deinstallation)
@@ -1504,37 +1504,38 @@
 
 [↺ contents](#contents)
 
 ## Deinstallation {#deinstallation}
 
 ### From a personal installation {#from-a-personal-installation}
 
-To remove *etm* installed into, say, python3, run
+To remove *etm* run
 
-    $ python3 -m pip uninstall etm-dgraham
+    $ pip uninstall etm-dgraham
 
 This will remove *etm* from the python site-packages directory and the *etm* and *etm+* executables from the python bin directory. Then remove any *etm home* directories that you have created.
 
 [↺ contents](#contents)
 
 ### From a virtual environment {#from-a-virtual-environment}
 
-If you should ever want to deinstall etm, first deactivate the virtual environment, if necessary, by changing to the virtual environment directory and entering
+Use *pipx* instead of *pip*:
 
-        (env) $ deactivate
+    $ pipx uninstall etm-dgraham
 
-You can now simply delete the virtual environment directory and, if you have additional *home* directories, delete each of them. One of the many advantages of the virtual environment is that these steps remove every trace.
+You can now remove any *home* directories you may have created.
 
 [↺ contents](#contents)
 
 ### From a system wide installation {#from-a-system-wide-installation}
 
 To remove *etm* installed into, say, python3.7, run
 
-    $ sudo -H python3.7 -m pip uninstall etm-dgraham
+    $ sudo -H pip uninstall etm-dgraham
+
 This will remove *etm* from the python site-packages directory and the *etm* and *etm+* executables from the python bin directory. Then remove any *etm home* directories that you have created.
 
 [↺ contents](#contents)
 
 # Details {#details}
 
 ## Item Types {#item-types}
```

### Comparing `etm-dgraham-5.1.4/bump.py` & `etm-dgraham-5.1.5/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/docs/index_konnections.md` & `etm-dgraham-5.1.5/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/docs/index_usedtime.md` & `etm-dgraham-5.1.5/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/docs/multiple_timers.md` & `etm-dgraham-5.1.5/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm/__main__.py` & `etm-dgraham-5.1.5/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm/data.py` & `etm-dgraham-5.1.5/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm/ical.py` & `etm-dgraham-5.1.5/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm/make_examples.py` & `etm-dgraham-5.1.5/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm/model.py` & `etm-dgraham-5.1.5/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3891,15 +3891,15 @@
 {{ nowrap(location) }} \
 {% endif -%}\
 {%- if 'r' in h -%}\
 {%- for x in h['r'] -%}\
 {%- if 'r' in x and x['r'] -%}\
 {%- set rrule %}\
 {{ x['r'] }}\
-{%- for k in ['i', 's', 'M', 'm', 'n', 'w', 'E', 'c'] -%}
+{%- for k in ['i', 's', 'M', 'm', 'n', 'h', 'w', 'E', 'c'] -%}
 {%- if k in x %} {{ "&{} {}".format(k, one_or_more(x[k])) }}{%- endif %}\
 {%- endfor %}
 {% if isinstance(x, dict) and 'u' in x %}{{ " &u {} ".format(dt2str(x['u'])[1]) }}{% endif %}\
 {%- endset %}
 @r {{ nowrap(rrule) }} \
 {% endif -%}\
 {%- endfor %}\
@@ -3998,15 +3998,15 @@
 {{ wrap(location) }} \
 {% endif -%}\
 {%- if 'r' in h -%}\
 {%- for x in h['r'] -%}\
 {%- if 'r' in x and x['r'] -%}\
 {%- set rrule %}\
 {{ x['r'] }}\
-{%- for k in ['i', 's', 'M', 'm', 'n', 'w', 'E', 'c'] -%}
+{%- for k in ['i', 's', 'M', 'm', 'n', 'h', 'w', 'E', 'c'] -%}
 {%- if k in x %} {{ "&{} {}".format(k, one_or_more(x[k])) }}{%- endif %}\
 {%- endfor %}
 {% if isinstance(x, dict) and 'u' in x %}{{ " &u {} ".format(dt2str(x['u'])[1]) }}{% endif %}\
 {%- endset %}
 @r {{ wrap(rrule) }} \
 {% endif -%}\
 {%- endfor %}\
@@ -4248,18 +4248,18 @@
             else:
                 # we have 2 good periods since none were bad
                 obj = obj_periods
     return obj, rep
 
 
 def do_overdue(arg):
-    ovrstr = "overdue: character from (r)estart, (s)kip, (k)eep or (p)reserve"
+    ovrstr = "overdue: character from (r)estart, (s)kip or (k)eep"
 
     if arg:
-        ok = arg in ('k', 'r', 's', 'p')
+        ok = arg in ('k', 'r', 's')
         if ok:
             return arg, f"overdue: {arg}"
         else:
             return None, f"invalid overdue: '{arg}'. {ovrstr}"
     else:
         return None, ovrstr
 
@@ -5758,22 +5758,32 @@
                 if '+' in item:
                     for dt in item['+']:
                         dt = date_to_datetime(dt)
                         rset.rdate(dt)
 
                 if item['itemtype'] == '-':
                     switch = item.get('o', 'k')
-                    relevant = rset.after(today, inc=True)
                     if switch == 's':
-                        if relevant and date_to_datetime(item['s']) < today:
-                            cur = date_to_datetime(item['s'])
-                            while cur < today:
+                        now = pendulum.now('local')
+                        relevant = rset.after(today, inc=True)
+                        cur = date_to_datetime(item['s'])
+                        # make 'all day' tasks not pastdue until one minute before midnight
+                        isdate = (isinstance(item['s'], pendulum.Date) and not isinstance(item['s'], pendulum.DateTime))
+                        isdate = cur.hour == 0 and cur.minute == 0
+                        delta = pendulum.duration(hours=23, minutes=59) if isdate else ZERO
+                        # logger.debug(f"{item['summary']} isdate: {isdate}, delta: {delta}, relevant: {relevant}, cur: {cur}")
+                        if relevant and date_to_datetime(item['s']) + delta < now:
+                            while cur + delta < now:
                                 item.setdefault('h', []).append(pendulum.period(cur+ONEMIN, cur))
                                 cur = rset.after(cur, inc=False)
-
+                            num_finished = settings.get('num_finished', 0)
+                            if num_finished and len(item['h']) > num_finished:
+                                h = item['h']
+                                h.sort(key=sortprd)
+                                item['h'] = h[-num_finished:]
                             item['s'] = pendulum.instance(cur)
                             update_db(db, item.doc_id, item)
                     else: # k or p
                         relevant = rset.after(today, inc=True)
                         already_done = [x.end for x in item.get('h', [])]
                         # relevant will be the first instance after 12am today
                         # it will be the @s entry for the updated repeating item
```

### Comparing `etm-dgraham-5.1.4/etm/options.py` & `etm-dgraham-5.1.5/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm/report.py` & `etm-dgraham-5.1.5/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm/view.py` & `etm-dgraham-5.1.5/etm/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -833,18 +833,29 @@
             res = f"the installed version, {etm_version}, is the latest available"
 
     return status_char, res
 
 
 update_status = UpdateStatus()
 
-async def auto_check_loop(loop):
+async def updates_loop(loop):
+    logger.debug("XXX update_loop XXX")
     status, res = check_update()
     update_status.set_status(status)
 
+async def refresh_loop(loop):
+    logger.debug("XXX refresh_loop XXX")
+    dataview.refreshRelevant()  # sets now, currentYrWk, current
+    dataview.refreshAgenda()
+    dataview.refreshCurrent()
+    set_text(dataview.show_active_view())
+    get_app().invalidate()
+
+
+
 @bindings.add('f3')
 def do_system(*event):
     show_message('system information', about(22)[1], 20)
 
 
 @bindings.add('f6')
 def dt_calculator(*event):
@@ -1390,36 +1401,40 @@
     if bad:
         logger.error(f"unrecognized alert commands: {bad}")
 
 
 async def event_handler():
     global current_datetime
     # check for updates every interval minutes
-    interval = settings.get('updates_interval', 0)
-    refresh_interval = settings.get('refresh_interval', 60)
-    minutes = 0
+    updates_interval = settings.get('updates_interval', 0)
+    refresh_interval = settings.get('refresh_interval', 60) # seconds to wait between loops
+    # minutes = pendulum.now().minute
+    # minutes = minutes % interval if interval else minutes % 5
+
     try:
         while True:
             now = pendulum.now('local')
             current_datetime = status_time(now)
             wait = refresh_interval - now.second % refresh_interval # residual
             if now.second < 6:
+                # minutes = now.minute % interval if interval else now.minute % 5
+                minutes = now.minute
                 current_today = dataview.now.format("YYYYMMDD")
                 asyncio.ensure_future(maybe_alerts(now))
                 current_datetime = status_time(now)
                 today = now.format("YYYYMMDD")
+                logger.debug(f"now: {now}, minutes: {minutes}")
 
-                if interval:
-                    if minutes == 0:
-                        minutes = 1
-                        loop = asyncio.get_event_loop()
-                        asyncio.ensure_future(auto_check_loop(loop))
-                    else:
-                        minutes += 1
-                        minutes = minutes % interval
+                if updates_interval and minutes % updates_interval == 0:
+                    loop = asyncio.get_event_loop()
+                    asyncio.ensure_future(updates_loop(loop))
+
+                if minutes % 5 == 0:
+                    loop = asyncio.get_event_loop()
+                    asyncio.ensure_future(refresh_loop(loop))
 
                 if today != current_today:
                     loop = asyncio.get_event_loop()
                     asyncio.ensure_future(new_day(loop))
 
             asyncio.ensure_future(save_timers())
             if dataview.active_view == 'timers':
```

### Comparing `etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.5/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.4
+Version: 5.1.5
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -57,16 +57,16 @@
     -   [Menus](#menus)
         -   [etm menu notes](#etm-menu-notes)
         -   [view menu notes](#view-menu-notes)
         -   [editor menu notes](#editor-menu-notes)
         -   [selected menu notes](#selected-menu-notes)
     -   [Installation](#installation)
         -   [For personal use](#for-personal-use)
-        -   [for use in an isolated environment](#for-use-in-an-isolated-environment)
-        -   [for use system wide](#for-use-system-wide)
+        -   [For use in an isolated environment](#for-use-in-an-isolated-environment)
+        -   [For use system wide](#for-use-system-wide)
     -   [Usage](#usage)
         -   [Terminal size and color](#terminal-size-and-color)
         -   [Home directory](#home-directory)
         -   [Timers](#timers)
         -   [lorem examples](#loremexamples)
         -   [Using etm+](#etmplus)
     -   [Deinstallation](#deinstallation)
@@ -1528,37 +1528,38 @@
 
 [↺ contents](#contents)
 
 ## Deinstallation {#deinstallation}
 
 ### From a personal installation {#from-a-personal-installation}
 
-To remove *etm* installed into, say, python3, run
+To remove *etm* run
 
-    $ python3 -m pip uninstall etm-dgraham
+    $ pip uninstall etm-dgraham
 
 This will remove *etm* from the python site-packages directory and the *etm* and *etm+* executables from the python bin directory. Then remove any *etm home* directories that you have created.
 
 [↺ contents](#contents)
 
 ### From a virtual environment {#from-a-virtual-environment}
 
-If you should ever want to deinstall etm, first deactivate the virtual environment, if necessary, by changing to the virtual environment directory and entering
+Use *pipx* instead of *pip*:
 
-        (env) $ deactivate
+    $ pipx uninstall etm-dgraham
 
-You can now simply delete the virtual environment directory and, if you have additional *home* directories, delete each of them. One of the many advantages of the virtual environment is that these steps remove every trace.
+You can now remove any *home* directories you may have created.
 
 [↺ contents](#contents)
 
 ### From a system wide installation {#from-a-system-wide-installation}
 
 To remove *etm* installed into, say, python3.7, run
 
-    $ sudo -H python3.7 -m pip uninstall etm-dgraham
+    $ sudo -H pip uninstall etm-dgraham
+
 This will remove *etm* from the python site-packages directory and the *etm* and *etm+* executables from the python bin directory. Then remove any *etm home* directories that you have created.
 
 [↺ contents](#contents)
 
 # Details {#details}
 
 ## Item Types {#item-types}
```

### Comparing `etm-dgraham-5.1.4/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.5/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.5/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etmlogo.png` & `etm-dgraham-5.1.5/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etmlogo_small.png` & `etm-dgraham-5.1.5/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/etmview_agenda.png` & `etm-dgraham-5.1.5/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/namedcolors.py` & `etm-dgraham-5.1.5/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/new.png` & `etm-dgraham-5.1.5/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/setup.py` & `etm-dgraham-5.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/test/test_parser.py` & `etm-dgraham-5.1.5/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.5/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/utilities/etm_in` & `etm-dgraham-5.1.5/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/utilities/inbasket` & `etm-dgraham-5.1.5/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.4/utilities/open_in_mutt` & `etm-dgraham-5.1.5/utilities/open_in_mutt`

 * *Files identical despite different names*

