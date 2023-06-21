# Comparing `tmp/lino_react-23.6.1.tar.gz` & `tmp/lino_react-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.6.1.tar", last modified: Tue Jun 13 10:44:16 2023, max compression
+gzip compressed data, was "lino_react-23.6.2.tar", last modified: Wed Jun 21 08:42:00 2023, max compression
```

## Comparing `lino_react-23.6.1.tar` & `lino_react-23.6.2.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.616160 lino_react-23.6.1/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.6.1/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.6.1/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-06-13 10:44:16.616160 lino_react-23.6.1/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.6.1/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.6.1/lino_react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)     4628 2023-06-13 10:30:58.000000 lino_react-23.6.1/lino_react/react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/__pycache__/
--rw-rw-r--   0 luc       (1000) www-data    (33)     3362 2023-06-13 10:37:43.000000 lino_react-23.6.1/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)     3993 2023-05-02 09:01:06.000000 lino_react-23.6.1/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-05-02 09:01:04.000000 lino_react-23.6.1/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    18321 2023-06-08 14:52:20.000000 lino_react-23.6.1/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-05-02 13:45:04.000000 lino_react-23.6.1/lino_react/react/__pycache__/views.cpython-310.pyc
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/config/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.6.1/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 luc       (1000) www-data    (33)     1910 2023-06-11 12:10:21.000000 lino_react-23.6.1/lino_react/react/config/react/main.html
--rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.6.1/lino_react/react/config/react/service-worker.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3893 2023-04-24 18:09:52.000000 lino_react-23.6.1/lino_react/react/icons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.6.1/lino_react/react/index.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.6.1/lino_react/react/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    29204 2023-06-13 10:43:27.000000 lino_react-23.6.1/lino_react/react/renderer.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/static/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.616160 lino_react-23.6.1/lino_react/react/static/media/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/color.6441e63a.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/color.c7a33805.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.6.1/lino_react/react/static/media/line.567f5738.gif
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.616160 lino_react-23.6.1/lino_react/react/static/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)  1776853 2023-06-13 09:28:20.000000 lino_react-23.6.1/lino_react/react/static/react/main.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.6.1/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.6.1/lino_react/react/views.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-06-13 10:43:55.000000 lino_react-23.6.1/lino_react/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.6.1/lino_react.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-06-13 10:44:16.616160 lino_react-23.6.1/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.6.1/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.6.1/tasks.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:42:00.007061 lino_react-23.6.2/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:19.000000 lino_react-23.6.2/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      157 2023-02-28 05:23:19.000000 lino_react-23.6.2/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-06-21 08:42:00.007061 lino_react-23.6.2/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      178 2023-02-28 05:23:19.000000 lino_react-23.6.2/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      283 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.999061 lino_react-23.6.2/lino_react/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4628 2023-06-13 10:46:31.000000 lino_react-23.6.2/lino_react/react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.999061 lino_react-23.6.2/lino_react/react/__pycache__/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3382 2023-06-15 05:49:26.000000 lino_react-23.6.2/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2980 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4013 2023-04-27 06:42:41.000000 lino_react-23.6.2/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/icons.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      160 2023-03-30 05:54:52.000000 lino_react-23.6.2/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1412 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/models.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18341 2023-05-03 06:16:14.000000 lino_react-23.6.2/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/renderer.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20615 2023-06-12 10:17:24.000000 lino_react-23.6.2/lino_react/react/__pycache__/views.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20473 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/views.cpython-38.pyc
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react/react/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.999061 lino_react-23.6.2/lino_react/react/config/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1910 2023-06-11 06:54:48.000000 lino_react-23.6.2/lino_react/react/config/react/main.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    16246 2023-06-21 07:51:55.000000 lino_react-23.6.2/lino_react/react/config/react/service-worker.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3893 2023-04-27 06:29:15.000000 lino_react-23.6.2/lino_react/react/icons.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       36 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/index.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-03-30 05:51:42.000000 lino_react-23.6.2/lino_react/react/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    29204 2023-05-03 06:10:54.000000 lino_react-23.6.2/lino_react/react/renderer.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react/react/static/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:42:00.003061 lino_react-23.6.2/lino_react/react/static/media/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13112 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39748 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57384 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39648 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   234640 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39572 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57560 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   163568 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57460 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:42:00.007061 lino_react-23.6.2/lino_react/react/static/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)  1777129 2023-06-21 07:51:55.000000 lino_react-23.6.2/lino_react/react/static/react/main.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2437 2023-06-21 07:51:55.000000 lino_react-23.6.2/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    28705 2023-06-11 15:16:59.000000 lino_react-23.6.2/lino_react/react/views.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1431 2023-06-21 08:41:02.000000 lino_react-23.6.2/lino_react/setup_info.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1770 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:26.000000 lino_react-23.6.2/lino_react.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        5 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       11 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-06-21 08:42:00.007061 lino_react-23.6.2/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:19.000000 lino_react-23.6.2/setup.py
```

### Comparing `lino_react-23.6.1/COPYING` & `lino_react-23.6.2/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/PKG-INFO` & `lino_react-23.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino_react
-Version: 23.6.1
+Version: 23.6.2
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
 Classifier:   Environment :: Web Environment
 Classifier:   Framework :: Django
 Classifier:   Intended Audience :: Developers
 Classifier:   Intended Audience :: System Administrators
@@ -25,9 +23,7 @@
 
 
 The React front end for Lino
 
 Project homepage is https://gitlab.com/lino-framework/react
 
 
-
-
```

### Comparing `lino_react-23.6.1/lino_react/react/__init__.py` & `lino_react-23.6.2/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/__pycache__/__init__.cpython-310.pyc` & `lino_react-23.6.2/lino_react/react/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 13 10:30:58 2023 UTC, .py size: 4628 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6245 8864 1412 0000  o.......bE.d....
+00000000: 6f0d 0d0a 0000 0000 0749 8864 1412 0000  o........I.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6506 8303 5a06 6407 5300 2908 7a93 0a41  e...Z.d.S.).z..A
 00000070: 2075 7365 7220 696e 7465 7266 6163 6520   user interface 
@@ -31,181 +31,182 @@
 000001e0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
 000001f0: 0043 0000 0073 1a00 0000 6401 6402 6c00  .C...s....d.d.l.
 00000200: 6d01 7d02 0100 7c02 7c00 8301 7c00 5f00  m.}...|.|...|._.
 00000210: 6400 5300 2903 4ee9 0100 0000 2901 da08  d.S.).N.....)...
 00000220: 5265 6e64 6572 6572 2902 da08 7265 6e64  Renderer)...rend
 00000230: 6572 6572 7208 0000 0029 03da 0473 656c  ererr....)...sel
 00000240: 66da 066b 6572 6e65 6c72 0800 0000 a900  f..kernelr......
-00000250: 720c 0000 00fa 312f 686f 6d65 2f6c 7563  r.....1/home/luc
-00000260: 2f77 6f72 6b2f 7265 6163 742f 6c69 6e6f  /work/react/lino
-00000270: 5f72 6561 6374 2f72 6561 6374 2f5f 5f69  _react/react/__i
-00000280: 6e69 745f 5f2e 7079 da0a 6f6e 5f75 695f  nit__.py..on_ui_
-00000290: 696e 6974 2500 0000 7304 0000 000c 010e  init%...s.......
-000002a0: 017a 1150 6c75 6769 6e2e 6f6e 5f75 695f  .z.Plugin.on_ui_
-000002b0: 696e 6974 6302 0000 0000 0000 0000 0000  initc...........
-000002c0: 0008 0000 0009 0000 0043 0000 0073 7a00  .........C...sz.
-000002d0: 0000 7400 7c00 6a01 7c00 6a02 7c01 7c00  ..t.|.j.|.j.|.|.
-000002e0: 6a02 6a03 6a04 7405 a006 a100 7407 6400  j.j.j.t.....t.d.
-000002f0: 6401 8d07 7d02 6402 7d03 7c00 6a02 6a03  d...}.d.}.|.j.j.
-00000300: 6a08 6a01 6a09 7d04 7c00 6a02 6a0a 4400  j.j.j.}.|.j.j.D.
-00000310: 5d1b 7d05 7c05 6a0b 4400 5d15 7d06 7c04  ].}.|.j.D.].}.|.
-00000320: a00c 7c06 a101 7d07 7c03 6403 7c07 6a0d  ..|...}.|.d.|.j.
-00000330: 6405 6900 7c02 a401 8e01 9b00 6404 9d03  d.i.|.......d...
-00000340: 3700 7d03 7124 711f 7c03 5300 2906 4e29  7.}.q$q.|.S.).N)
-00000350: 07da 0e65 7874 6a73 5f72 656e 6465 7265  ...extjs_rendere
-00000360: 72da 0473 6974 65da 0873 6574 7469 6e67  r..site..setting
-00000370: 73da 046c 696e 6fda 086c 616e 6775 6167  s..lino..languag
-00000380: 6572 0300 0000 da05 6578 746a 73da 007a  er......extjs..z
-00000390: 083c 7363 7269 7074 3e7a 093c 2f73 6372  .<script>z.</scr
-000003a0: 6970 743e 720c 0000 0029 0eda 0464 6963  ipt>r....)...dic
-000003b0: 7472 0900 0000 7210 0000 00da 0770 6c75  tr....r......plu
-000003c0: 6769 6e73 7212 0000 0072 0200 0000 da0c  ginsr....r......
-000003d0: 6765 745f 6c61 6e67 7561 6765 7203 0000  get_languager...
-000003e0: 00da 056a 696e 6a61 da09 6a69 6e6a 615f  ...jinja..jinja_
-000003f0: 656e 76da 0e73 6f72 7465 645f 706c 7567  env..sorted_plug
-00000400: 696e 73da 1073 6974 655f 6a73 5f73 6e69  ins..site_js_sni
-00000410: 7070 6574 73da 0c67 6574 5f74 656d 706c  ppets..get_templ
-00000420: 6174 65da 0672 656e 6465 7229 0872 0a00  ate..render).r..
-00000430: 0000 7211 0000 00da 0763 6f6e 7465 7874  ..r......context
-00000440: da02 6a73 da03 656e 76da 0170 da07 736e  ..js..env..p..sn
-00000450: 6970 7065 74da 0874 656d 706c 6174 6572  ippet..templater
-00000460: 0c00 0000 720c 0000 0072 0d00 0000 da15  ....r....r......
-00000470: 6c6f 6164 5f73 6974 655f 6a73 5f73 6e69  load_site_js_sni
-00000480: 7070 6574 732b 0000 0073 2200 0000 0201  ppets+...s".....
-00000490: 0401 0401 0201 0801 0601 0201 0201 06f9  ................
-000004a0: 040a 0e01 0c02 0a01 0a01 1e01 02fe 0404  ................
-000004b0: 7a1c 506c 7567 696e 2e6c 6f61 645f 7369  z.Plugin.load_si
-000004c0: 7465 5f6a 735f 736e 6970 7065 7473 6301  te_js_snippetsc.
-000004d0: 0000 0000 0000 0000 0000 0006 0000 0014  ................
-000004e0: 0000 0043 0000 0073 5a01 0000 6401 6402  ...C...sZ...d.d.
-000004f0: 6c00 6d01 7d01 0100 6401 6403 6c00 6d02  l.m.}...d.d.l.m.
-00000500: 7d02 0100 6404 6405 6c03 6d04 7d03 0100  }...d.d.l.m.}...
-00000510: 6406 7d04 7c01 7c04 6407 1700 7c03 6a05  d.}.|.|.d...|.j.
-00000520: a006 a100 8302 7c01 7c04 6408 1700 7c03  ......|.|.d...|.
-00000530: 6a07 a006 a100 8302 7c01 7c04 6409 1700  j.......|.|.d...
-00000540: 7c03 6a08 a006 a100 8302 7c01 7c04 640a  |.j.......|.|.d.
-00000550: 1700 7c03 6a09 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
-00000560: 640b 1700 7c03 6a0a a006 a100 8302 7c01  d...|.j.......|.
-00000570: 640c 7c03 6a0b a006 a100 8302 7c01 7c04  d.|.j.......|.|.
-00000580: 640d 1700 7c03 6a0c a006 a100 8302 7c02  d...|.j.......|.
-00000590: 640e 7c03 6a0d a006 a100 8302 7c01 7c04  d.|.j.......|.|.
-000005a0: 640f 1700 7c03 6a0e a006 a100 8302 7c01  d...|.j.......|.
-000005b0: 7c04 6410 1700 7c03 6a0f a006 a100 8302  |.d...|.j.......
-000005c0: 7c01 7c04 6411 1700 7c03 6a0e a006 a100  |.|.d...|.j.....
-000005d0: 8302 7c01 7c04 6412 1700 7c03 6a0f a006  ..|.|.d...|.j...
-000005e0: a100 8302 7c01 7c04 6413 1700 7c03 6a10  ....|.|.d...|.j.
-000005f0: a006 a100 8302 7c01 7c04 6414 1700 7c03  ......|.|.d...|.
-00000600: 6a11 a006 a100 8302 7c01 7c04 6415 1700  j.......|.|.d...
-00000610: 7c03 6a11 a006 a100 8302 7c01 7c04 6416  |.j.......|.|.d.
-00000620: 1700 7c03 6a12 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
-00000630: 6417 1700 7c03 6a13 a006 a100 8302 6711  d...|.j.......g.
-00000640: 7d05 7c05 5300 2918 4e72 0100 0000 2901  }.|.S.).Nr....).
-00000650: da07 7265 5f70 6174 6829 01da 0470 6174  ..re_path)...pat
-00000660: 6872 0700 0000 2901 da05 7669 6577 73fa  hr....)...views.
-00000670: 015e fa01 247a 0d75 7365 722f 7365 7474  .^..$z.user/sett
-00000680: 696e 6773 7a05 6175 7468 247a 056e 756c  ingsz.auth$z.nul
-00000690: 6c2f 7a25 283f 503c 776f 726b 626f 783e  l/z%(?P<workbox>
-000006a0: 776f 726b 626f 782d 5b61 2d7a 412d 5a30  workbox-[a-zA-Z0
-000006b0: 2d39 5d2a 2e6a 7329 247a 1173 6572 7669  -9]*.js)$z.servi
-000006c0: 6365 2d77 6f72 6b65 722e 6a73 7a0e 6170  ce-worker.jsz.ap
-000006d0: 692f 6d61 696e 5f68 746d 6c24 7a15 6461  i/main_html$z.da
-000006e0: 7368 626f 6172 642f 3c69 6e74 3a69 6e64  shboard/<int:ind
-000006f0: 6578 3e7a 2a72 6573 7466 756c 2f28 3f50  ex>z*restful/(?P
-00000700: 3c61 7070 5f6c 6162 656c 3e5c 772b 292f  <app_label>\w+)/
-00000710: 283f 503c 6163 746f 723e 5c77 2b29 247a  (?P<actor>\w+)$z
-00000720: 3572 6573 7466 756c 2f28 3f50 3c61 7070  5restful/(?P<app
-00000730: 5f6c 6162 656c 3e5c 772b 292f 283f 503c  _label>\w+)/(?P<
-00000740: 6163 746f 723e 5c77 2b29 2f28 3f50 3c70  actor>\w+)/(?P<p
-00000750: 6b3e 2e2b 2924 7a26 6170 692f 283f 503c  k>.+)$z&api/(?P<
-00000760: 6170 705f 6c61 6265 6c3e 5c77 2b29 2f28  app_label>\w+)/(
-00000770: 3f50 3c61 6374 6f72 3e5c 772b 2924 7a34  ?P<actor>\w+)$z4
-00000780: 6170 692f 283f 503c 6170 705f 6c61 6265  api/(?P<app_labe
-00000790: 6c3e 5c77 2b29 2f28 3f50 3c61 6374 6f72  l>\w+)/(?P<actor
-000007a0: 3e5c 772b 292f 283f 503c 706b 3e5b 5e2f  >\w+)/(?P<pk>[^/
-000007b0: 5d2b 2924 7a42 7661 6c75 6573 2f28 3f50  ]+)$zBvalues/(?P
-000007c0: 3c61 7070 5f6c 6162 656c 3e5c 772b 292f  <app_label>\w+)/
-000007d0: 283f 503c 6163 746f 723e 5c77 2b29 2f28  (?P<actor>\w+)/(
-000007e0: 3f50 3c70 6b3e 2e2b 292f 283f 503c 6669  ?P<pk>.+)/(?P<fi
-000007f0: 656c 643e 2e2b 2924 7a2a 6368 6f69 6365  eld>.+)$z*choice
-00000800: 732f 283f 503c 6170 705f 6c61 6265 6c3e  s/(?P<app_label>
-00000810: 5c77 2b29 2f28 3f50 3c61 6374 6f72 3e5c  \w+)/(?P<actor>\
-00000820: 772b 2924 7a39 6368 6f69 6365 732f 283f  w+)$z9choices/(?
-00000830: 503c 6170 705f 6c61 6265 6c3e 5c77 2b29  P<app_label>\w+)
-00000840: 2f28 3f50 3c61 6374 6f72 3e5c 772b 292f  /(?P<actor>\w+)/
-00000850: 283f 503c 6669 656c 643e 5c77 2b29 247a  (?P<field>\w+)$z
-00000860: 4761 7063 686f 6963 6573 2f28 3f50 3c61  Gapchoices/(?P<a
-00000870: 7070 5f6c 6162 656c 3e5c 772b 292f 283f  pp_label>\w+)/(?
-00000880: 503c 6163 746f 723e 5c77 2b29 2f28 3f50  P<actor>\w+)/(?P
-00000890: 3c61 6e3e 5c77 2b29 2f28 3f50 3c66 6965  <an>\w+)/(?P<fie
-000008a0: 6c64 3e5c 772b 2924 7a0c 6368 6f69 6365  ld>\w+)$z.choice
-000008b0: 6c69 7374 732f 2914 da0b 646a 616e 676f  lists/)...django
-000008c0: 2e75 726c 7372 2600 0000 7227 0000 0072  .urlsr&...r'...r
-000008d0: 1500 0000 7228 0000 00da 0549 6e64 6578  ....r(.....Index
-000008e0: da07 6173 5f76 6965 77da 0c55 7365 7253  ..as_view..UserS
-000008f0: 6574 7469 6e67 73da 0c41 7574 6865 6e74  ettings..Authent
-00000900: 6963 6174 65da 044e 756c 6cda 0657 4256  icate..Null..WBV
-00000910: 6965 77da 0653 5756 6965 77da 084d 6169  iew..SWView..Mai
-00000920: 6e48 746d 6cda 0d44 6173 6862 6f61 7264  nHtml..Dashboard
-00000930: 4974 656d da07 4170 694c 6973 74da 0a41  Item..ApiList..A
-00000940: 7069 456c 656d 656e 74da 0c44 656c 6179  piElement..Delay
-00000950: 6564 5661 6c75 65da 0743 686f 6963 6573  edValue..Choices
-00000960: da12 4163 7469 6f6e 5061 7261 6d43 686f  ..ActionParamCho
-00000970: 6963 6573 da0f 4368 6f69 6365 4c69 7374  ices..ChoiceList
-00000980: 4d6f 6465 6c29 0672 0a00 0000 da03 7572  Model).r......ur
-00000990: 6c72 2700 0000 7228 0000 00da 0272 78da  lr'...r(.....rx.
-000009a0: 0475 726c 7372 0c00 0000 720c 0000 0072  .urlsr....r....r
-000009b0: 0d00 0000 da0c 6765 745f 7061 7474 6572  ......get_patter
-000009c0: 6e73 4000 0000 7356 0000 000c 030c 010c  ns@...sV........
-000009d0: 0104 0212 0612 0112 0112 0108 0208 0102  ................
-000009e0: ff0e 0212 020e 0208 0308 0102 ff08 0208  ................
-000009f0: 0102 ff08 0308 0102 ff08 0208 0102 ff08  ................
-00000a00: 0408 0102 ff08 0208 0102 ff08 0208 0202  ................
-00000a10: fe08 0308 0202 fe08 0808 0102 ff04 d704  ................
-00000a20: 2d7a 1350 6c75 6769 6e2e 6765 745f 7061  -z.Plugin.get_pa
-00000a30: 7474 6572 6e73 6304 0000 0000 0000 0000  tternsc.........
-00000a40: 0000 0006 0000 0007 0000 004f 0000 0073  ...........O...s
-00000a50: 2c00 0000 7c00 6a00 6401 6402 7c02 6a01  ,...|.j.d.d.|.j.
-00000a60: a002 6403 6404 a102 7403 7c03 8301 6704  ..d.d...t.|...g.
-00000a70: 7c04 a201 5200 6900 7c05 a401 8e01 5300  |...R.i.|.....S.
-00000a80: 2905 4efa 0123 da03 6170 69da 012e fa01  ).N..#..api.....
-00000a90: 2f29 04da 0f62 7569 6c64 5f70 6c61 696e  /)...build_plain
-00000aa0: 5f75 726c da08 6163 746f 725f 6964 da07  _url..actor_id..
-00000ab0: 7265 706c 6163 65da 0373 7472 2906 720a  replace..str).r.
-00000ac0: 0000 00da 0261 72da 0561 6374 6f72 da02  .....ar..actor..
-00000ad0: 706b da04 6172 6773 da02 6b77 720c 0000  pk..args..kwr...
-00000ae0: 0072 0c00 0000 720d 0000 00da 0e67 6574  .r....r......get
-00000af0: 5f64 6574 6169 6c5f 7572 6c7b 0000 0073  _detail_url{...s
-00000b00: 1400 0000 0401 0201 0201 0c01 0601 02fc  ................
-00000b10: 0204 06fc 0204 06fc 7a15 506c 7567 696e  ........z.Plugin
-00000b20: 2e67 6574 5f64 6574 6169 6c5f 7572 6c46  .get_detail_urlF
-00000b30: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b40: 0002 0000 0063 0000 0073 1800 0000 8100  .....c...s......
-00000b50: 7c01 6400 7501 720a 6401 5600 0100 6400  |.d.u.r.d.V...d.
-00000b60: 5300 6400 5300 2902 4e29 03da 0552 6561  S.d.S.).N)...Rea
-00000b70: 6374 7a04 3136 2e36 7a14 6874 7470 733a  ctz.16.6z.https:
-00000b80: 2f2f 7265 6163 746a 732e 6f72 672f 720c  //reactjs.org/r.
-00000b90: 0000 0029 0272 0a00 0000 da04 6874 6d6c  ...).r......html
-00000ba0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000bb0: 0d67 6574 5f75 7365 645f 6c69 6273 8200  .get_used_libs..
-00000bc0: 0000 7308 0000 0002 8008 010a 0104 ff7a  ..s............z
-00000bd0: 1450 6c75 6769 6e2e 6765 745f 7573 6564  .Plugin.get_used
-00000be0: 5f6c 6962 734e 2901 4629 0dda 085f 5f6e  _libsN).F)...__n
-00000bf0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000c00: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000c10: 1375 695f 6861 6e64 6c65 5f61 7474 725f  .ui_handle_attr_
-00000c20: 6e61 6d65 da0d 6e65 6564 735f 706c 7567  name..needs_plug
-00000c30: 696e 73da 0a75 726c 5f70 7265 6669 78da  ins..url_prefix.
-00000c40: 0a6d 6564 6961 5f6e 616d 65da 0d73 7570  .media_name..sup
-00000c50: 706f 7274 5f61 7379 6e63 720e 0000 0072  port_asyncr....r
-00000c60: 2500 0000 723e 0000 0072 4c00 0000 724f  %...r>...rL...rO
-00000c70: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000c80: 0000 720d 0000 0072 0400 0000 1600 0000  ..r....r........
-00000c90: 7316 0000 0008 0004 0208 0304 0304 0204  s...............
-00000ca0: 0108 0408 0608 1508 3b0e 0772 0400 0000  ........;..r....
-00000cb0: 4e29 07da 075f 5f64 6f63 5f5f da0c 646a  N)...__doc__..dj
-00000cc0: 616e 676f 2e75 7469 6c73 7202 0000 00da  ango.utilsr.....
-00000cd0: 096c 696e 6f2e 636f 7265 7203 0000 00da  .lino.corer.....
-00000ce0: 0b6c 696e 6f2e 6170 692e 6164 7204 0000  .lino.api.adr...
-00000cf0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000d00: 720d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000d10: 0000 0073 0a00 0000 0404 0c0c 0c01 0c01  ...s............
-00000d20: 1403                                     ..
+00000250: 720c 0000 00fa 452f 686f 6d65 2f62 6c75  r.....E/home/blu
+00000260: 7272 792f 6c69 6e6f 2f65 6e76 2f72 6570  rry/lino/env/rep
+00000270: 6f73 6974 6f72 6965 732f 7265 6163 742f  ositories/react/
+00000280: 6c69 6e6f 5f72 6561 6374 2f72 6561 6374  lino_react/react
+00000290: 2f5f 5f69 6e69 745f 5f2e 7079 da0a 6f6e  /__init__.py..on
+000002a0: 5f75 695f 696e 6974 2500 0000 7304 0000  _ui_init%...s...
+000002b0: 000c 010e 017a 1150 6c75 6769 6e2e 6f6e  .....z.Plugin.on
+000002c0: 5f75 695f 696e 6974 6302 0000 0000 0000  _ui_initc.......
+000002d0: 0000 0000 0008 0000 0009 0000 0043 0000  .............C..
+000002e0: 0073 7a00 0000 7400 7c00 6a01 7c00 6a02  .sz...t.|.j.|.j.
+000002f0: 7c01 7c00 6a02 6a03 6a04 7405 a006 a100  |.|.j.j.j.t.....
+00000300: 7407 6400 6401 8d07 7d02 6402 7d03 7c00  t.d.d...}.d.}.|.
+00000310: 6a02 6a03 6a08 6a01 6a09 7d04 7c00 6a02  j.j.j.j.j.}.|.j.
+00000320: 6a0a 4400 5d1b 7d05 7c05 6a0b 4400 5d15  j.D.].}.|.j.D.].
+00000330: 7d06 7c04 a00c 7c06 a101 7d07 7c03 6403  }.|...|...}.|.d.
+00000340: 7c07 6a0d 6405 6900 7c02 a401 8e01 9b00  |.j.d.i.|.......
+00000350: 6404 9d03 3700 7d03 7124 711f 7c03 5300  d...7.}.q$q.|.S.
+00000360: 2906 4e29 07da 0e65 7874 6a73 5f72 656e  ).N)...extjs_ren
+00000370: 6465 7265 72da 0473 6974 65da 0873 6574  derer..site..set
+00000380: 7469 6e67 73da 046c 696e 6fda 086c 616e  tings..lino..lan
+00000390: 6775 6167 6572 0300 0000 da05 6578 746a  guager......extj
+000003a0: 73da 007a 083c 7363 7269 7074 3e7a 093c  s..z.<script>z.<
+000003b0: 2f73 6372 6970 743e 720c 0000 0029 0eda  /script>r....)..
+000003c0: 0464 6963 7472 0900 0000 7210 0000 00da  .dictr....r.....
+000003d0: 0770 6c75 6769 6e73 7212 0000 0072 0200  .pluginsr....r..
+000003e0: 0000 da0c 6765 745f 6c61 6e67 7561 6765  ....get_language
+000003f0: 7203 0000 00da 056a 696e 6a61 da09 6a69  r......jinja..ji
+00000400: 6e6a 615f 656e 76da 0e73 6f72 7465 645f  nja_env..sorted_
+00000410: 706c 7567 696e 73da 1073 6974 655f 6a73  plugins..site_js
+00000420: 5f73 6e69 7070 6574 73da 0c67 6574 5f74  _snippets..get_t
+00000430: 656d 706c 6174 65da 0672 656e 6465 7229  emplate..render)
+00000440: 0872 0a00 0000 7211 0000 00da 0763 6f6e  .r....r......con
+00000450: 7465 7874 da02 6a73 da03 656e 76da 0170  text..js..env..p
+00000460: da07 736e 6970 7065 74da 0874 656d 706c  ..snippet..templ
+00000470: 6174 6572 0c00 0000 720c 0000 0072 0d00  ater....r....r..
+00000480: 0000 da15 6c6f 6164 5f73 6974 655f 6a73  ....load_site_js
+00000490: 5f73 6e69 7070 6574 732b 0000 0073 2200  _snippets+...s".
+000004a0: 0000 0201 0401 0401 0201 0801 0601 0201  ................
+000004b0: 0201 06f9 040a 0e01 0c02 0a01 0a01 1e01  ................
+000004c0: 02fe 0404 7a1c 506c 7567 696e 2e6c 6f61  ....z.Plugin.loa
+000004d0: 645f 7369 7465 5f6a 735f 736e 6970 7065  d_site_js_snippe
+000004e0: 7473 6301 0000 0000 0000 0000 0000 0006  tsc.............
+000004f0: 0000 0014 0000 0043 0000 0073 5a01 0000  .......C...sZ...
+00000500: 6401 6402 6c00 6d01 7d01 0100 6401 6403  d.d.l.m.}...d.d.
+00000510: 6c00 6d02 7d02 0100 6404 6405 6c03 6d04  l.m.}...d.d.l.m.
+00000520: 7d03 0100 6406 7d04 7c01 7c04 6407 1700  }...d.}.|.|.d...
+00000530: 7c03 6a05 a006 a100 8302 7c01 7c04 6408  |.j.......|.|.d.
+00000540: 1700 7c03 6a07 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
+00000550: 6409 1700 7c03 6a08 a006 a100 8302 7c01  d...|.j.......|.
+00000560: 7c04 640a 1700 7c03 6a09 a006 a100 8302  |.d...|.j.......
+00000570: 7c01 7c04 640b 1700 7c03 6a0a a006 a100  |.|.d...|.j.....
+00000580: 8302 7c01 640c 7c03 6a0b a006 a100 8302  ..|.d.|.j.......
+00000590: 7c01 7c04 640d 1700 7c03 6a0c a006 a100  |.|.d...|.j.....
+000005a0: 8302 7c02 640e 7c03 6a0d a006 a100 8302  ..|.d.|.j.......
+000005b0: 7c01 7c04 640f 1700 7c03 6a0e a006 a100  |.|.d...|.j.....
+000005c0: 8302 7c01 7c04 6410 1700 7c03 6a0f a006  ..|.|.d...|.j...
+000005d0: a100 8302 7c01 7c04 6411 1700 7c03 6a0e  ....|.|.d...|.j.
+000005e0: a006 a100 8302 7c01 7c04 6412 1700 7c03  ......|.|.d...|.
+000005f0: 6a0f a006 a100 8302 7c01 7c04 6413 1700  j.......|.|.d...
+00000600: 7c03 6a10 a006 a100 8302 7c01 7c04 6414  |.j.......|.|.d.
+00000610: 1700 7c03 6a11 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
+00000620: 6415 1700 7c03 6a11 a006 a100 8302 7c01  d...|.j.......|.
+00000630: 7c04 6416 1700 7c03 6a12 a006 a100 8302  |.d...|.j.......
+00000640: 7c01 7c04 6417 1700 7c03 6a13 a006 a100  |.|.d...|.j.....
+00000650: 8302 6711 7d05 7c05 5300 2918 4e72 0100  ..g.}.|.S.).Nr..
+00000660: 0000 2901 da07 7265 5f70 6174 6829 01da  ..)...re_path)..
+00000670: 0470 6174 6872 0700 0000 2901 da05 7669  .pathr....)...vi
+00000680: 6577 73fa 015e fa01 247a 0d75 7365 722f  ews..^..$z.user/
+00000690: 7365 7474 696e 6773 7a05 6175 7468 247a  settingsz.auth$z
+000006a0: 056e 756c 6c2f 7a25 283f 503c 776f 726b  .null/z%(?P<work
+000006b0: 626f 783e 776f 726b 626f 782d 5b61 2d7a  box>workbox-[a-z
+000006c0: 412d 5a30 2d39 5d2a 2e6a 7329 247a 1173  A-Z0-9]*.js)$z.s
+000006d0: 6572 7669 6365 2d77 6f72 6b65 722e 6a73  ervice-worker.js
+000006e0: 7a0e 6170 692f 6d61 696e 5f68 746d 6c24  z.api/main_html$
+000006f0: 7a15 6461 7368 626f 6172 642f 3c69 6e74  z.dashboard/<int
+00000700: 3a69 6e64 6578 3e7a 2a72 6573 7466 756c  :index>z*restful
+00000710: 2f28 3f50 3c61 7070 5f6c 6162 656c 3e5c  /(?P<app_label>\
+00000720: 772b 292f 283f 503c 6163 746f 723e 5c77  w+)/(?P<actor>\w
+00000730: 2b29 247a 3572 6573 7466 756c 2f28 3f50  +)$z5restful/(?P
+00000740: 3c61 7070 5f6c 6162 656c 3e5c 772b 292f  <app_label>\w+)/
+00000750: 283f 503c 6163 746f 723e 5c77 2b29 2f28  (?P<actor>\w+)/(
+00000760: 3f50 3c70 6b3e 2e2b 2924 7a26 6170 692f  ?P<pk>.+)$z&api/
+00000770: 283f 503c 6170 705f 6c61 6265 6c3e 5c77  (?P<app_label>\w
+00000780: 2b29 2f28 3f50 3c61 6374 6f72 3e5c 772b  +)/(?P<actor>\w+
+00000790: 2924 7a34 6170 692f 283f 503c 6170 705f  )$z4api/(?P<app_
+000007a0: 6c61 6265 6c3e 5c77 2b29 2f28 3f50 3c61  label>\w+)/(?P<a
+000007b0: 6374 6f72 3e5c 772b 292f 283f 503c 706b  ctor>\w+)/(?P<pk
+000007c0: 3e5b 5e2f 5d2b 2924 7a42 7661 6c75 6573  >[^/]+)$zBvalues
+000007d0: 2f28 3f50 3c61 7070 5f6c 6162 656c 3e5c  /(?P<app_label>\
+000007e0: 772b 292f 283f 503c 6163 746f 723e 5c77  w+)/(?P<actor>\w
+000007f0: 2b29 2f28 3f50 3c70 6b3e 2e2b 292f 283f  +)/(?P<pk>.+)/(?
+00000800: 503c 6669 656c 643e 2e2b 2924 7a2a 6368  P<field>.+)$z*ch
+00000810: 6f69 6365 732f 283f 503c 6170 705f 6c61  oices/(?P<app_la
+00000820: 6265 6c3e 5c77 2b29 2f28 3f50 3c61 6374  bel>\w+)/(?P<act
+00000830: 6f72 3e5c 772b 2924 7a39 6368 6f69 6365  or>\w+)$z9choice
+00000840: 732f 283f 503c 6170 705f 6c61 6265 6c3e  s/(?P<app_label>
+00000850: 5c77 2b29 2f28 3f50 3c61 6374 6f72 3e5c  \w+)/(?P<actor>\
+00000860: 772b 292f 283f 503c 6669 656c 643e 5c77  w+)/(?P<field>\w
+00000870: 2b29 247a 4761 7063 686f 6963 6573 2f28  +)$zGapchoices/(
+00000880: 3f50 3c61 7070 5f6c 6162 656c 3e5c 772b  ?P<app_label>\w+
+00000890: 292f 283f 503c 6163 746f 723e 5c77 2b29  )/(?P<actor>\w+)
+000008a0: 2f28 3f50 3c61 6e3e 5c77 2b29 2f28 3f50  /(?P<an>\w+)/(?P
+000008b0: 3c66 6965 6c64 3e5c 772b 2924 7a0c 6368  <field>\w+)$z.ch
+000008c0: 6f69 6365 6c69 7374 732f 2914 da0b 646a  oicelists/)...dj
+000008d0: 616e 676f 2e75 726c 7372 2600 0000 7227  ango.urlsr&...r'
+000008e0: 0000 0072 1500 0000 7228 0000 00da 0549  ...r....r(.....I
+000008f0: 6e64 6578 da07 6173 5f76 6965 77da 0c55  ndex..as_view..U
+00000900: 7365 7253 6574 7469 6e67 73da 0c41 7574  serSettings..Aut
+00000910: 6865 6e74 6963 6174 65da 044e 756c 6cda  henticate..Null.
+00000920: 0657 4256 6965 77da 0653 5756 6965 77da  .WBView..SWView.
+00000930: 084d 6169 6e48 746d 6cda 0d44 6173 6862  .MainHtml..Dashb
+00000940: 6f61 7264 4974 656d da07 4170 694c 6973  oardItem..ApiLis
+00000950: 74da 0a41 7069 456c 656d 656e 74da 0c44  t..ApiElement..D
+00000960: 656c 6179 6564 5661 6c75 65da 0743 686f  elayedValue..Cho
+00000970: 6963 6573 da12 4163 7469 6f6e 5061 7261  ices..ActionPara
+00000980: 6d43 686f 6963 6573 da0f 4368 6f69 6365  mChoices..Choice
+00000990: 4c69 7374 4d6f 6465 6c29 0672 0a00 0000  ListModel).r....
+000009a0: da03 7572 6c72 2700 0000 7228 0000 00da  ..urlr'...r(....
+000009b0: 0272 78da 0475 726c 7372 0c00 0000 720c  .rx..urlsr....r.
+000009c0: 0000 0072 0d00 0000 da0c 6765 745f 7061  ...r......get_pa
+000009d0: 7474 6572 6e73 4000 0000 7356 0000 000c  tterns@...sV....
+000009e0: 030c 010c 0104 0212 0612 0112 0112 0108  ................
+000009f0: 0208 0102 ff0e 0212 020e 0208 0308 0102  ................
+00000a00: ff08 0208 0102 ff08 0308 0102 ff08 0208  ................
+00000a10: 0102 ff08 0408 0102 ff08 0208 0102 ff08  ................
+00000a20: 0208 0202 fe08 0308 0202 fe08 0808 0102  ................
+00000a30: ff04 d704 2d7a 1350 6c75 6769 6e2e 6765  ....-z.Plugin.ge
+00000a40: 745f 7061 7474 6572 6e73 6304 0000 0000  t_patternsc.....
+00000a50: 0000 0000 0000 0006 0000 0007 0000 004f  ...............O
+00000a60: 0000 0073 2c00 0000 7c00 6a00 6401 6402  ...s,...|.j.d.d.
+00000a70: 7c02 6a01 a002 6403 6404 a102 7403 7c03  |.j...d.d...t.|.
+00000a80: 8301 6704 7c04 a201 5200 6900 7c05 a401  ..g.|...R.i.|...
+00000a90: 8e01 5300 2905 4efa 0123 da03 6170 69da  ..S.).N..#..api.
+00000aa0: 012e fa01 2f29 04da 0f62 7569 6c64 5f70  ..../)...build_p
+00000ab0: 6c61 696e 5f75 726c da08 6163 746f 725f  lain_url..actor_
+00000ac0: 6964 da07 7265 706c 6163 65da 0373 7472  id..replace..str
+00000ad0: 2906 720a 0000 00da 0261 72da 0561 6374  ).r......ar..act
+00000ae0: 6f72 da02 706b da04 6172 6773 da02 6b77  or..pk..args..kw
+00000af0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000b00: 0e67 6574 5f64 6574 6169 6c5f 7572 6c7b  .get_detail_url{
+00000b10: 0000 0073 1400 0000 0401 0201 0201 0c01  ...s............
+00000b20: 0601 02fc 0204 06fc 0204 06fc 7a15 506c  ............z.Pl
+00000b30: 7567 696e 2e67 6574 5f64 6574 6169 6c5f  ugin.get_detail_
+00000b40: 7572 6c46 6302 0000 0000 0000 0000 0000  urlFc...........
+00000b50: 0002 0000 0002 0000 0063 0000 0073 1800  .........c...s..
+00000b60: 0000 8100 7c01 6400 7501 720a 6401 5600  ....|.d.u.r.d.V.
+00000b70: 0100 6400 5300 6400 5300 2902 4e29 03da  ..d.S.d.S.).N)..
+00000b80: 0552 6561 6374 7a04 3136 2e36 7a14 6874  .Reactz.16.6z.ht
+00000b90: 7470 733a 2f2f 7265 6163 746a 732e 6f72  tps://reactjs.or
+00000ba0: 672f 720c 0000 0029 0272 0a00 0000 da04  g/r....).r......
+00000bb0: 6874 6d6c 720c 0000 0072 0c00 0000 720d  htmlr....r....r.
+00000bc0: 0000 00da 0d67 6574 5f75 7365 645f 6c69  .....get_used_li
+00000bd0: 6273 8200 0000 7308 0000 0002 8008 010a  bs....s.........
+00000be0: 0104 ff7a 1450 6c75 6769 6e2e 6765 745f  ...z.Plugin.get_
+00000bf0: 7573 6564 5f6c 6962 734e 2901 4629 0dda  used_libsN).F)..
+00000c00: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000c10: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000c20: 655f 5fda 1375 695f 6861 6e64 6c65 5f61  e__..ui_handle_a
+00000c30: 7474 725f 6e61 6d65 da0d 6e65 6564 735f  ttr_name..needs_
+00000c40: 706c 7567 696e 73da 0a75 726c 5f70 7265  plugins..url_pre
+00000c50: 6669 78da 0a6d 6564 6961 5f6e 616d 65da  fix..media_name.
+00000c60: 0d73 7570 706f 7274 5f61 7379 6e63 720e  .support_asyncr.
+00000c70: 0000 0072 2500 0000 723e 0000 0072 4c00  ...r%...r>...rL.
+00000c80: 0000 724f 0000 0072 0c00 0000 720c 0000  ..rO...r....r...
+00000c90: 0072 0c00 0000 720d 0000 0072 0400 0000  .r....r....r....
+00000ca0: 1600 0000 7316 0000 0008 0004 0208 0304  ....s...........
+00000cb0: 0304 0204 0108 0408 0608 1508 3b0e 0772  ............;..r
+00000cc0: 0400 0000 4e29 07da 075f 5f64 6f63 5f5f  ....N)...__doc__
+00000cd0: da0c 646a 616e 676f 2e75 7469 6c73 7202  ..django.utilsr.
+00000ce0: 0000 00da 096c 696e 6f2e 636f 7265 7203  .....lino.corer.
+00000cf0: 0000 00da 0b6c 696e 6f2e 6170 692e 6164  .....lino.api.ad
+00000d00: 7204 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000d10: 0c00 0000 720d 0000 00da 083c 6d6f 6475  ....r......<modu
+00000d20: 6c65 3e01 0000 0073 0a00 0000 0404 0c0c  le>....s........
+00000d30: 0c01 0c01 1403                           ......
```

### Comparing `lino_react-23.6.1/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.6.2/lino_react/react/__pycache__/icons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 24 18:09:52 2023 UTC, .py size: 3893 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f0c5 4664 350f 0000  o.........Fd5...
+00000000: 6f0d 0d0a 0000 0000 3b16 4a64 350f 0000  o.......;.Jd5...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 a002 a100  d.l.m.Z...d.....
 00000040: 5a03 6900 6403 6404 9301 6405 6406 9301  Z.i.d.d...d.d...
 00000050: 6407 6408 9301 6409 640a 9301 640b 640c  d.d...d.d...d.d.
 00000060: 9301 640d 640e 9301 640f 6410 9301 6411  ..d.d...d.d...d.
 00000070: 6412 9301 6413 6404 9301 6414 6415 9301  d...d.d...d.d...
@@ -220,31 +220,32 @@
 00000db0: 7074 da0d 6461 7461 6261 7365 5f67 6561  pt..database_gea
 00000dc0: 72da 0663 616e 6365 6cda 0a66 6c61 675f  r..cancel..flag_
 00000dd0: 6772 6565 6eda 0964 6174 655f 6e65 7874  green..date_next
 00000de0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00000df0: 0004 0000 0043 0000 0073 1200 0000 6900  .....C...s....i.
 00000e00: 7c00 5d05 7d01 7c01 7c01 9302 7102 5300  |.].}.|.|...q.S.
 00000e10: a900 722b 0000 0029 02da 022e 30da 0469  ..r+...)....0..i
-00000e20: 636f 6e72 2b00 0000 722b 0000 00fa 2e2f  conr+...r+...../
-00000e30: 686f 6d65 2f6c 7563 2f77 6f72 6b2f 7265  home/luc/work/re
-00000e40: 6163 742f 6c69 6e6f 5f72 6561 6374 2f72  act/lino_react/r
-00000e50: 6561 6374 2f69 636f 6e73 2e70 79da 0a3c  eact/icons.py..<
-00000e60: 6469 6374 636f 6d70 3ee4 0000 0073 0200  dictcomp>....s..
-00000e70: 0000 1200 722f 0000 0029 06da 136c 696e  ....r/...)...lin
-00000e80: 6f2e 636f 7265 2e63 6f6e 7374 616e 7473  o.core.constants
-00000e90: 7202 0000 00da 0573 706c 6974 da10 5245  r......split..RE
-00000ea0: 4143 545f 4943 4f4e 5f4e 414d 4553 da12  ACT_ICON_NAMES..
-00000eb0: 5245 4143 545f 4943 4f4e 5f4d 4150 5049  REACT_ICON_MAPPI
-00000ec0: 4e47 da06 7570 6461 7465 722b 0000 0072  NG..updater+...r
-00000ed0: 2b00 0000 722b 0000 0072 2e00 0000 da08  +...r+...r......
-00000ee0: 3c6d 6f64 756c 653e 0100 0000 73a8 0000  <module>....s...
-00000ef0: 000c 0002 0200 7f04 3400 8102 cc00 7f02  ........4.......
-00000f00: 3604 0102 ff04 0202 fe04 0302 fd04 0402  6...............
-00000f10: fc04 0502 fb04 0602 fa04 0702 f904 0802  ................
-00000f20: f804 0902 f704 0a02 f604 0b02 f504 0c02  ................
-00000f30: f404 0d02 f304 0e02 f204 0f02 f104 1002  ................
-00000f40: f004 1104 ef04 1202 ee04 1302 ed04 1402  ................
-00000f50: ec04 1502 eb04 1602 ea04 1702 e904 1802  ................
-00000f60: e804 1902 e704 1a02 e604 1b02 e504 1c02  ................
-00000f70: e404 1d02 e304 1e02 e204 1f02 e104 2002  .............. .
-00000f80: e004 2102 df04 2204 de02 2302 0102 0102  ..!..."...#.....
-00000f90: 0102 0102 0108 d818 2c                   ........,
+00000e20: 636f 6e72 2b00 0000 722b 0000 00fa 422f  conr+...r+....B/
+00000e30: 686f 6d65 2f62 6c75 7272 792f 6c69 6e6f  home/blurry/lino
+00000e40: 2f65 6e76 2f72 6570 6f73 6974 6f72 6965  /env/repositorie
+00000e50: 732f 7265 6163 742f 6c69 6e6f 5f72 6561  s/react/lino_rea
+00000e60: 6374 2f72 6561 6374 2f69 636f 6e73 2e70  ct/react/icons.p
+00000e70: 79da 0a3c 6469 6374 636f 6d70 3ee4 0000  y..<dictcomp>...
+00000e80: 0073 0200 0000 1200 722f 0000 0029 06da  .s......r/...)..
+00000e90: 136c 696e 6f2e 636f 7265 2e63 6f6e 7374  .lino.core.const
+00000ea0: 616e 7473 7202 0000 00da 0573 706c 6974  antsr......split
+00000eb0: da10 5245 4143 545f 4943 4f4e 5f4e 414d  ..REACT_ICON_NAM
+00000ec0: 4553 da12 5245 4143 545f 4943 4f4e 5f4d  ES..REACT_ICON_M
+00000ed0: 4150 5049 4e47 da06 7570 6461 7465 722b  APPING..updater+
+00000ee0: 0000 0072 2b00 0000 722b 0000 0072 2e00  ...r+...r+...r..
+00000ef0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000f00: 73a8 0000 000c 0002 0200 7f04 3400 8102  s...........4...
+00000f10: cc00 7f02 3604 0102 ff04 0202 fe04 0302  ....6...........
+00000f20: fd04 0402 fc04 0502 fb04 0602 fa04 0702  ................
+00000f30: f904 0802 f804 0902 f704 0a02 f604 0b02  ................
+00000f40: f504 0c02 f404 0d02 f304 0e02 f204 0f02  ................
+00000f50: f104 1002 f004 1104 ef04 1202 ee04 1302  ................
+00000f60: ed04 1402 ec04 1502 eb04 1602 ea04 1702  ................
+00000f70: e904 1802 e804 1902 e704 1a02 e604 1b02  ................
+00000f80: e504 1c02 e404 1d02 e304 1e02 e204 1f02  ................
+00000f90: e104 2002 e004 2102 df04 2204 de02 2302  .. ...!..."...#.
+00000fa0: 0102 0102 0102 0102 0108 d818 2c         ............,
```

### Comparing `lino_react-23.6.1/lino_react/react/__pycache__/renderer.cpython-310.pyc` & `lino_react-23.6.2/lino_react/react/__pycache__/renderer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 14:52:17 2023 UTC, .py size: 29268 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 21eb 8164 5472 0000  o.......!..dTr..
+00000000: 6f0d 0d0a 0000 0000 eefa 5164 1472 0000  o.........Qd.r..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -83,1064 +83,1065 @@
 00000520: 6974 7465 7227 7320 6974 656d 2061 6e64  itter's item and
 00000530: 2072 6574 7572 6e73 2074 6861 7420 7761   returns that wa
 00000540: 6e74 6564 206d 6174 6368 6564 2069 7465  nted matched ite
 00000550: 6de9 ffff ffff 2902 da08 6361 6c6c 6162  m.....)...callab
 00000560: 6c65 da09 656e 756d 6572 6174 6529 05da  le..enumerate)..
 00000570: 0569 7474 6572 da06 7461 7267 6574 da03  .itter..target..
 00000580: 6b65 79da 0169 da01 78a9 0072 3600 0000  key..i..x..r6...
-00000590: fa31 2f68 6f6d 652f 6c75 632f 776f 726b  .1/home/luc/work
-000005a0: 2f72 6561 6374 2f6c 696e 6f5f 7265 6163  /react/lino_reac
-000005b0: 742f 7265 6163 742f 7265 6e64 6572 6572  t/react/renderer
-000005c0: 2e70 79da 0466 696e 642d 0000 0073 1000  .py..find-...s..
-000005d0: 0000 1802 1002 0401 0801 0801 0801 02ff  ................
-000005e0: 0403 7238 0000 0063 0000 0000 0000 0000  ..r8...c........
-000005f0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00000600: 73e6 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000610: 0364 025a 0464 025a 0564 035a 0664 045a  .d.Z.d.Z.d.Z.d.Z
-00000620: 0764 025a 0887 0066 0164 0564 0684 085a  .d.Z...f.d.d...Z
-00000630: 0964 0764 0884 005a 0a64 0964 0a84 005a  .d.d...Z.d.d...Z
-00000640: 0b64 0b64 0c84 005a 0c64 0d64 0e84 005a  .d.d...Z.d.d...Z
-00000650: 0d64 0f64 1084 005a 0e64 1164 1284 005a  .d.d...Z.d.d...Z
-00000660: 0f64 3264 1464 1584 015a 1069 0066 0164  .d2d.d...Z.i.f.d
-00000670: 1664 1784 015a 1164 1864 1984 005a 1264  .d...Z.d.d...Z.d
-00000680: 1a64 1b84 005a 1364 1c64 1d84 005a 1464  .d...Z.d.d...Z.d
-00000690: 1e64 1f84 005a 1564 2064 2184 005a 1664  .d...Z.d d!..Z.d
-000006a0: 2264 2384 005a 1764 2464 2584 005a 1864  "d#..Z.d$d%..Z.d
-000006b0: 2664 2784 005a 1964 2864 2984 005a 1a64  &d'..Z.d(d)..Z.d
-000006c0: 2a64 2b84 005a 1b64 2c64 2d84 005a 1c64  *d+..Z.d,d-..Z.d
-000006d0: 2e64 2f84 005a 1d87 0066 0164 3064 3184  .d/..Z...f.d0d1.
-000006e0: 085a 1e87 0004 005a 1f53 0029 33da 0852  .Z.....Z.S.)3..R
-000006f0: 656e 6465 7265 727a 480a 2020 2020 4120  endererzH.    A 
-00000700: 6672 6f6e 742d 656e 6420 7265 6e64 6572  front-end render
-00000710: 6572 2074 6861 7420 7573 6573 2074 6865  er that uses the
-00000720: 2052 6561 6374 204a 6176 6173 6372 6970   React Javascrip
-00000730: 7420 6672 616d 6577 6f72 6b2e 0a20 2020  t framework..   
-00000740: 2054 7a12 7265 6163 742f 6c69 6e6f 7765   Tz.react/linowe
-00000750: 622e 6a73 6f6e 7a05 2e6a 736f 6e63 0200  b.jsonz..jsonc..
-00000760: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000770: 0000 0300 0000 731c 0000 0074 0083 00a0  ......s....t....
-00000780: 017c 01a1 0101 0074 02a0 037c 006a 04a1  .|.....t...|.j..
-00000790: 0101 0064 0053 00a9 014e 2905 da05 7375  ...d.S...N)...su
-000007a0: 7065 72da 085f 5f69 6e69 745f 5f72 2500  per..__init__r%.
-000007b0: 0000 da12 7265 6769 7374 6572 5f63 6f6e  ....register_con
-000007c0: 7665 7274 6572 da0f 7079 326a 735f 636f  verter..py2js_co
-000007d0: 6e76 6572 7465 7229 02da 0473 656c 66da  nverter)...self.
-000007e0: 0966 726f 6e74 5f65 6e64 a901 da09 5f5f  .front_end....__
-000007f0: 636c 6173 735f 5f72 3600 0000 7237 0000  class__r6...r7..
-00000800: 0072 3c00 0000 4500 0000 7304 0000 000c  .r<...E...s.....
-00000810: 0110 017a 1152 656e 6465 7265 722e 5f5f  ...z.Renderer.__
-00000820: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
-00000830: 0000 000c 0000 0008 0000 0003 0000 0073  ...............s
-00000840: 7202 0000 6401 6402 8400 7400 6a01 a002  r...d.d...t.j...
-00000850: a100 4400 8301 7d02 7403 8300 7d03 8800  ..D...}.t...}...
-00000860: 6a04 4400 5d14 7d04 7c04 a005 a100 4400  j.D.].}.|.....D.
-00000870: 5d0d 7d05 7c05 6a06 7c03 7601 7223 7c03  ].}.|.j.|.v.r#|.
-00000880: a007 7c05 6a06 a101 0100 7116 7110 6403  ..|.j.....q.q.d.
-00000890: 8800 5f08 7409 6a0a 6a0b 7d06 740c 8700  .._.t.j.j.}.t...
-000008a0: 6601 6404 6402 8408 7c03 4400 8301 7409  f.d.d...|.D...t.
-000008b0: 6a0a a00d 740e 8300 a101 7c06 6a0f 6a10  j...t.....|.j.j.
-000008c0: 7409 6a0a 6a11 8800 6a12 6a13 6405 7501  t.j.j...j.j.d.u.
-000008d0: 6406 6402 8400 7409 6a0a 6a14 4400 8301  d.d...t.j.j.D...
-000008e0: 6407 8d06 7d07 7409 6a0a a015 6408 a101  d...}.t.j...d...
-000008f0: 7264 7c07 6a16 7417 7c06 6a18 6a19 6a1a  rd|.j.t.|.j.j.j.
-00000900: a01b a100 8301 6409 8d01 0100 7c07 6a16  ......d.....|.j.
-00000910: 7409 6a0a 6a00 6a1c 640a 8d01 0100 7a13  t.j.j.j.d.....z.
-00000920: 7c07 6a16 741d a01e 741f 7409 6a20 8301  |.j.t...t.t.j ..
-00000930: 640b 1b00 640c 1b00 a101 6a21 640d 8d01  d...d.....j!d...
-00000940: 0100 5700 6e09 0400 7422 7989 0100 0100  ..W.n...t"y.....
-00000950: 0100 5900 6e01 7700 7423 7409 6a0a 640e  ..Y.n.w.t#t.j.d.
-00000960: 8302 7298 7c07 6a16 7409 6a0a 6a24 640f  ..r.|.j.t.j.j$d.
-00000970: 8d01 0100 7409 6a0a 6a25 6405 6b02 72a5  ....t.j.j%d.k.r.
-00000980: 7c07 6a16 6403 6410 8d01 0100 6e0e 7423  |.j.d.d.....n.t#
-00000990: 7c06 6a26 6411 8302 72b3 7c07 6a16 7c06  |.j&d...r.|.j.|.
-000009a0: 6a26 6a27 6412 8d01 0100 7409 6a0a a015  j&j'd.....t.j...
-000009b0: 6413 a101 72c5 7c07 6a16 7c06 6a28 6a29  d...r.|.j.|.j(j)
-000009c0: 6fc2 7409 6a0a 6a2a 6414 8d01 0100 6900  o.t.j.j*d.....i.
-000009d0: 7d08 8800 6a2b 4400 5d2f 7d09 8800 a02c  }...j+D.]/}....,
-000009e0: 7c09 a101 7c08 7c09 6a2d 3c00 7423 7c09  |...|.|.j-<.t#|.
-000009f0: 6415 8302 72f9 6416 7c09 6a2d 7600 72f9  d...r.d.|.j-v.r.
-00000a00: 742e 7c02 6417 1900 8301 4400 5d14 5c02  t.|.d.....D.].\.
-00000a10: 7d0a 7d0b 7c0b 6418 1900 7c09 6a2f 6b02  }.}.|.d...|.j/k.
-00000a20: 72f8 7c09 6a2d 7c02 6417 1900 7c0a 1900  r.|.j-|.d...|...
-00000a30: 6419 3c00 71e4 71ca 8800 6a30 4400 5d0a  d.<.q.q...j0D.].
-00000a40: 7d09 8800 a02c 7c09 a101 7c08 7c09 6a2d  }....,|...|.|.j-
-00000a50: 3c00 71fd 8800 6a31 4400 5d0b 7d09 8800  <.q...j1D.].}...
-00000a60: a02c 7c09 a101 7c08 7c09 6a2d 3c00 9001  .,|...|.|.j-<...
-00000a70: 710b 8800 6a32 4400 5d0b 7d09 8800 a02c  q...j2D.].}....,
-00000a80: 7c09 a101 7c08 7c09 6a2d 3c00 9001 711a  |...|.|.j-<...q.
-00000a90: 7c07 6a16 7c08 7c02 641a 8d02 0100 7c01  |.j.|.|.d.....|.
-00000aa0: a033 7434 7c07 8301 a101 0100 641b 8800  .3t4|.......d...
-00000ab0: 5f08 641c 5300 291d 7a86 0a20 2020 2020  _.d.S.).z..     
-00000ac0: 2020 2043 7265 6174 6573 2077 6861 7420     Creates what 
-00000ad0: 6973 206b 6e6f 776e 2061 7320 7769 6e64  is known as wind
-00000ae0: 6f77 2e41 7070 2e73 7461 7465 2e73 6974  ow.App.state.sit
-00000af0: 655f 6461 7461 2069 6e20 5265 6163 7420  e_data in React 
-00000b00: 636f 6465 2e0a 0a20 2020 2020 2020 203a  code...        :
-00000b10: 7061 7261 6d20 663a 2046 696c 6520 6f62  param f: File ob
-00000b20: 6a65 6374 0a20 2020 2020 2020 203a 7265  ject.        :re
-00000b30: 7475 726e 3a20 310a 2020 2020 2020 2020  turn: 1.        
-00000b40: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000b50: 0006 0000 0053 0000 0073 2400 0000 6900  .....S...s$...i.
-00000b60: 7c00 5d0e 5c02 7d01 7d02 7c01 6400 6401  |.].\.}.}.|.d.d.
-00000b70: 8400 7c02 a000 a100 4400 8301 9302 7102  ..|.....D.....q.
-00000b80: 5300 2902 6301 0000 0000 0000 0000 0000  S.).c...........
-00000b90: 0002 0000 0006 0000 0053 0000 0073 2400  .........S...s$.
-00000ba0: 0000 6700 7c00 5d0e 7d01 7c01 6400 1900  ..g.|.].}.|.d...
-00000bb0: 6a00 7401 7c01 6401 1900 8301 6402 9c02  j.t.|.d.....d...
-00000bc0: 9102 7102 5300 2903 7201 0000 0072 2c00  ..q.S.).r....r,.
-00000bd0: 0000 2902 da05 7661 6c75 65da 0474 6578  ..)...value..tex
-00000be0: 7429 0272 4300 0000 da03 7374 7229 02da  t).rC.....str)..
-00000bf0: 022e 30da 0163 7236 0000 0072 3600 0000  ..0..cr6...r6...
-00000c00: 7237 0000 00da 0a3c 6c69 7374 636f 6d70  r7.....<listcomp
-00000c10: 3e52 0000 0073 0200 0000 2400 7a35 5265  >R...s....$.z5Re
-00000c20: 6e64 6572 6572 2e77 7269 7465 5f6c 696e  nderer.write_lin
-00000c30: 6f5f 6a73 2e3c 6c6f 6361 6c73 3e2e 3c64  o_js.<locals>.<d
-00000c40: 6963 7463 6f6d 703e 2e3c 6c69 7374 636f  ictcomp>.<listco
-00000c50: 6d70 3e29 01da 0b67 6574 5f63 686f 6963  mp>)...get_choic
-00000c60: 6573 2903 7246 0000 00da 0249 44da 0263  es).rF.....ID..c
-00000c70: 6c72 3600 0000 7236 0000 0072 3700 0000  lr6...r6...r7...
-00000c80: da0a 3c64 6963 7463 6f6d 703e 5000 0000  ..<dictcomp>P...
-00000c90: 7308 0000 0006 0006 0312 ff06 fe7a 2a52  s............z*R
-00000ca0: 656e 6465 7265 722e 7772 6974 655f 6c69  enderer.write_li
-00000cb0: 6e6f 5f6a 732e 3c6c 6f63 616c 733e 2e3c  no_js.<locals>.<
-00000cc0: 6469 6374 636f 6d70 3e54 6301 0000 0000  dictcomp>Tc.....
-00000cd0: 0000 0000 0000 0002 0000 0006 0000 0013  ................
-00000ce0: 0000 0073 1a00 0000 6900 7c00 5d09 7d01  ...s....i.|.].}.
-00000cf0: 7c01 6a00 8800 a001 7c01 a101 9302 7102  |.j.....|.....q.
-00000d00: 5300 7236 0000 0029 02da 0b61 6374 696f  S.r6...)...actio
-00000d10: 6e5f 6e61 6d65 da0b 6163 7469 6f6e 326a  n_name..action2j
-00000d20: 736f 6e29 0272 4600 0000 da01 61a9 0172  son).rF.....a..r
-00000d30: 3f00 0000 7236 0000 0072 3700 0000 724c  ?...r6...r7...rL
-00000d40: 0000 005f 0000 0073 0200 0000 1a00 4e63  ..._...s......Nc
-00000d50: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000d60: 0400 0000 5300 0000 7316 0000 0069 007c  ....S...s....i.|
-00000d70: 005d 077d 017c 016a 007c 016a 0193 0271  .].}.|.j.|.j...q
-00000d80: 0253 0072 3600 0000 2902 da0b 646a 616e  .S.r6...)...djan
-00000d90: 676f 5f63 6f64 65da 046e 616d 6529 0272  go_code..name).r
-00000da0: 4600 0000 da04 6c61 6e67 7236 0000 0072  F.....langr6...r
-00000db0: 3600 0000 7237 0000 0072 4c00 0000 6500  6...r7...rL...e.
-00000dc0: 0000 7302 0000 0016 0029 06da 0761 6374  ..s......)...act
-00000dd0: 696f 6e73 da04 6d65 6e75 da15 7573 655f  ions..menu..use_
-00000de0: 6461 7368 626f 6172 645f 6c61 796f 7574  dashboard_layout
-00000df0: 73da 0a73 6974 655f 7469 746c 65da 1065  s..site_title..e
-00000e00: 6469 7469 6e67 5f66 726f 6e74 656e 64da  diting_frontend.
-00000e10: 096c 616e 6775 6167 6573 da04 6d65 6d6f  .languages..memo
-00000e20: 2901 da0a 7375 6767 6573 746f 7273 2901  )...suggestors).
-00000e30: da0f 7265 7669 7369 6f6e 5f6e 756d 6265  ..revision_numbe
-00000e40: 72da 0572 6561 6374 7a07 6d61 696e 2e6a  r..reactz.main.j
-00000e50: 7329 01da 0d6d 6a73 5f74 696d 6573 7461  s)...mjs_timesta
-00000e60: 6d70 da0a 7468 656d 655f 6e61 6d65 2901  mp..theme_name).
-00000e70: 725f 0000 0029 01da 0d6e 6f5f 7573 6572  r_...)...no_user
-00000e80: 5f6d 6f64 656c da19 616c 6c6f 775f 6f6e  _model..allow_on
-00000e90: 6c69 6e65 5f72 6567 6973 7472 6174 696f  line_registratio
-00000ea0: 6e29 0172 6100 0000 da06 6e6f 7469 6679  n).ra.....notify
-00000eb0: 2901 da0c 7573 655f 7075 7368 5f61 7069  )...use_push_api
-00000ec0: da0b 6368 6f69 6365 5f6e 616d 657a 1073  ..choice_namez.s
-00000ed0: 7973 7465 6d2e 4461 7368 626f 6172 647a  ystem.Dashboardz
-00000ee0: 1773 7973 7465 6d2e 4461 7368 626f 6172  .system.Dashboar
-00000ef0: 644c 6179 6f75 7473 7243 0000 00da 0d77  dLayoutsrC.....w
-00000f00: 696e 646f 775f 6c61 796f 7574 2902 da0b  indow_layout)...
-00000f10: 666f 726d 5f70 616e 656c 7372 0d00 0000  form_panelsr....
-00000f20: 4672 2c00 0000 2935 7223 0000 00da 0b43  Fr,...)5r#.....C
-00000f30: 484f 4943 454c 4953 5453 da05 6974 656d  HOICELISTS..item
-00000f40: 73da 0373 6574 da0b 6163 746f 7273 5f6c  s..set..actors_l
-00000f50: 6973 74da 0b67 6574 5f61 6374 696f 6e73  ist..get_actions
-00000f60: da06 6163 7469 6f6e da03 6164 64da 1173  ..action..add..s
-00000f70: 6572 6961 6c69 7365 5f6a 735f 636f 6465  erialise_js_code
-00000f80: 7204 0000 00da 0453 4954 45da 0770 6c75  r......SITE..plu
-00000f90: 6769 6e73 da04 6469 6374 da0d 6765 745f  gins..dict..get_
-00000fa0: 7369 7465 5f6d 656e 7572 2900 0000 da06  site_menur).....
-00000fb0: 7379 7374 656d 7256 0000 00da 0574 6974  systemrV.....tit
-00000fc0: 6c65 7240 0000 00da 0a75 726c 5f70 7265  ler@.....url_pre
-00000fd0: 6669 7872 5900 0000 da0c 6973 5f69 6e73  fixrY.....is_ins
-00000fe0: 7461 6c6c 6564 da06 7570 6461 7465 da04  talled..update..
-00000ff0: 6c69 7374 725a 0000 00da 0670 6172 7365  listrZ.....parse
-00001000: 72da 0a73 7567 6765 7374 6572 73da 046b  r..suggesters..k
-00001010: 6579 73da 0a63 6f64 655f 6d74 696d 65da  eys..code_mtime.
-00001020: 026f 73da 0473 7461 7472 0200 0000 da0b  .os..statr......
-00001030: 5354 4154 4943 5f52 4f4f 54da 0873 745f  STATIC_ROOT..st_
-00001040: 6d74 696d 65da 1146 696c 654e 6f74 466f  mtime..FileNotFo
-00001050: 756e 6445 7272 6f72 da07 6861 7361 7474  undError..hasatt
-00001060: 7272 5f00 0000 da0a 7573 6572 5f6d 6f64  rr_.....user_mod
-00001070: 656c da05 7573 6572 7372 6100 0000 7262  el..usersra...rb
-00001080: 0000 0072 6300 0000 da09 7573 655f 6c69  ...rc.....use_li
-00001090: 6e6f 6472 6600 0000 da0a 7061 6e65 6c32  nodrf.....panel2
-000010a0: 6a73 6f6e da0f 5f66 6f72 6d70 616e 656c  json.._formpanel
-000010b0: 5f6e 616d 6572 3000 0000 7264 0000 00da  _namer0...rd....
-000010c0: 0c70 6172 616d 5f70 616e 656c 73da 1361  .param_panels..a
-000010d0: 6374 696f 6e5f 7061 7261 6d5f 7061 6e65  ction_param_pane
-000010e0: 6c73 da0c 6f74 6865 725f 7061 6e65 6c73  ls..other_panels
-000010f0: da05 7772 6974 6572 2600 0000 290c 723f  ..writer&...).r?
-00001100: 0000 00da 0166 da10 6368 6f69 6365 6c69  .....f..choiceli
-00001110: 7374 735f 6461 7461 7254 0000 00da 0372  sts_datarT.....r
-00001120: 7074 da02 6261 7270 0000 00da 0464 6174  pt..barp.....dat
-00001130: 6172 6600 0000 da01 7072 3400 0000 da04  arf.....pr4.....
-00001140: 6974 656d 7236 0000 0072 5000 0000 7237  itemr6...rP...r7
-00001150: 0000 00da 0d77 7269 7465 5f6c 696e 6f5f  .....write_lino_
-00001160: 6a73 4900 0000 7370 0000 0006 0708 0306  jsI...sp........
-00001170: fd06 050a 010c 020a 010c 0102 8002 fe06  ................
-00001180: 0408 0102 0110 010c 0206 0106 010a 0110  ................
-00001190: 0106 f90c 0904 0210 0106 ff12 0602 0126  ...............&
-000011a0: 010c 0104 0102 ff0c 0310 010c 020e 010c  ................
-000011b0: 0110 010c 0218 0104 090a 0110 0114 0114  ................
-000011c0: 010e 0112 0104 800a 0112 010a 0114 010a  ................
-000011d0: 0114 010e 010e 0506 0204 017a 1652 656e  ...........z.Ren
-000011e0: 6465 7265 722e 7772 6974 655f 6c69 6e6f  derer.write_lino
-000011f0: 5f6a 7363 0200 0000 0000 0000 0000 0000  _jsc............
-00001200: 0400 0000 0600 0000 4300 0000 73c6 0000  ........C...s...
-00001210: 0074 007c 0174 0183 0273 074a 0082 0174  .t.|.t...s.J...t
-00001220: 027c 016a 037c 01a0 04a1 007c 01a0 05a1  .|.j.|.....|....
-00001230: 007c 016a 0664 018d 047d 0274 007c 0174  .|.j.d...}.t.|.t
-00001240: 0783 0272 297c 016a 086a 096a 037c 0264  ...r)|.j.j.j.|.d
-00001250: 023c 0074 0a7c 016a 086a 0b83 017c 0264  .<.t.|.j.j...|.d
-00001260: 033c 007c 016a 0c72 317c 016a 0c7c 0264  .<.|.j.r1|.j.|.d
-00001270: 043c 007c 016a 0d72 397c 016a 0d7c 0264  .<.|.j.r9|.j.|.d
-00001280: 053c 007c 016a 0e72 4064 067c 0264 073c  .<.|.j.r@d.|.d.<
-00001290: 007c 016a 0f72 487c 016a 0f7c 0264 083c  .|.j.rH|.j.|.d.<
-000012a0: 007c 016a 1072 4f64 067c 0264 093c 007c  .|.j.rOd.|.d.<.|
-000012b0: 016a 1172 5664 067c 0264 0a3c 007c 00a0  .j.rVd.|.d.<.|..
-000012c0: 127c 01a1 017d 037c 0372 617c 037c 0264  .|...}.|.ra|.|.d
-000012d0: 0b3c 007c 0253 0029 0c7a 3343 6f6e 7665  .<.|.S.).z3Conve
-000012e0: 7274 7320 676c 6f62 616c 206c 6973 7420  rts global list 
-000012f0: 6f66 2061 6c6c 2061 6374 696f 6e73 2074  of all actions t
-00001300: 6f20 6a73 6f6e 2066 6f72 6d61 742e 2904  o json format.).
-00001310: da02 616e da05 6c61 6265 6cda 0d77 696e  ..an..label..win
-00001320: 646f 775f 6163 7469 6f6e da0b 6874 7470  dow_action..http
-00001330: 5f6d 6574 686f 6472 9400 0000 da05 6163  _methodr......ac
-00001340: 746f 72da 0c70 7265 7072 6f63 6573 736f  tor..preprocesso
-00001350: 72da 0b73 656c 6563 745f 726f 7773 54da  r..select_rowsT.
-00001360: 1073 7562 6d69 745f 666f 726d 5f64 6174  .submit_form_dat
-00001370: 61da 0b62 7574 746f 6e5f 7465 7874 da14  a..button_text..
-00001380: 7368 6f77 5f69 6e5f 7369 6465 5f74 6f6f  show_in_side_too
-00001390: 6c62 6172 da0e 6e65 7665 725f 636f 6c6c  lbar..never_coll
-000013a0: 6170 7365 da04 6963 6f6e 2913 da0a 6973  apse..icon)...is
-000013b0: 696e 7374 616e 6365 7217 0000 0072 7100  instancer....rq.
-000013c0: 0000 724d 0000 00da 0967 6574 5f6c 6162  ..rM.....get_lab
-000013d0: 656c da10 6973 5f77 696e 646f 775f 6163  el..is_window_ac
-000013e0: 7469 6f6e 7297 0000 0072 1200 0000 da0c  tionr....r......
-000013f0: 626f 756e 645f 6163 7469 6f6e 726c 0000  bound_actionrl..
-00001400: 0072 4500 0000 7298 0000 0072 9900 0000  .rE...r....r....
-00001410: 729a 0000 0072 9b00 0000 729c 0000 0072  r....r....r....r
-00001420: 9d00 0000 729e 0000 00da 0f67 6574 5f61  ....r......get_a
-00001430: 6374 696f 6e5f 6963 6f6e 2904 723f 0000  ction_icon).r?..
-00001440: 00da 0176 da06 7265 7375 6c74 729f 0000  ...v..resultr...
-00001450: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-00001460: 724e 0000 009e 0000 0073 2400 0000 0e02  rN.......s$.....
-00001470: 0604 0601 0601 0401 06fd 0a06 0e01 1001  ................
-00001480: 1002 1002 0e01 1001 0e01 0e01 0a02 0c01  ................
-00001490: 0402 7a14 5265 6e64 6572 6572 2e61 6374  ..z.Renderer.act
-000014a0: 696f 6e32 6a73 6f6e 6302 0000 0000 0000  ion2jsonc.......
-000014b0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-000014c0: 0073 2e00 0000 7400 7c01 7401 8302 7307  .s....t.|.t...s.
-000014d0: 4a00 8201 7c01 a002 a100 7d02 7403 7c00  J...|.....}.t.|.
-000014e0: a004 7c02 6a05 a101 7c02 6a06 6a07 6401  ..|.j...|.j.j.d.
-000014f0: 8d02 5300 2902 4e29 02da 046d 6169 6eda  ..S.).N)...main.
-00001500: 0b77 696e 646f 775f 7369 7a65 2908 72a0  .window_size).r.
-00001510: 0000 0072 1d00 0000 da11 6765 745f 6c61  ...r......get_la
-00001520: 796f 7574 5f68 616e 646c 6572 7100 0000  yout_handlerq...
-00001530: da09 656c 656d 326a 736f 6e72 a700 0000  ..elem2jsonr....
-00001540: da06 6c61 796f 7574 72a8 0000 0029 0372  ..layoutr....).r
-00001550: 3f00 0000 7291 0000 0072 a500 0000 7236  ?...r....r....r6
-00001560: 0000 0072 3600 0000 7237 0000 0072 8600  ...r6...r7...r..
-00001570: 0000 bb00 0000 730a 0000 000e 0108 030c  ......s.........
-00001580: 0106 0106 ff7a 1352 656e 6465 7265 722e  .....z.Renderer.
-00001590: 7061 6e65 6c32 6a73 6f6e 6302 0000 0000  panel2jsonc.....
-000015a0: 0000 0000 0000 0004 0000 0005 0000 0003  ................
-000015b0: 0000 0073 d600 0000 7400 7c01 7401 8302  ...s....t.|.t...
-000015c0: 7307 4a00 8201 7402 7c01 a003 a100 7c01  s.J...t.|.....|.
-000015d0: 6a04 6a05 6401 8d02 7d02 7406 7c01 6402  j.j.d...}.t.|.d.
-000015e0: 8302 7222 8700 6601 6403 6404 8408 7c01  ..r"..f.d.d...|.
-000015f0: 6a07 4400 8301 7c02 6405 3c00 7c02 a008  j.D...|.d.<.|...
-00001600: 7409 7c01 6406 8302 a101 0100 7406 7c01  t.|.d.......t.|.
-00001610: 6407 8302 7253 7c02 a008 7409 7c01 6a0a  d...rS|...t.|.j.
-00001620: 6408 8302 a101 0100 7406 7c01 6409 8302  d.......t.|.d...
-00001630: 7253 7c01 6a0b 6400 7501 7253 7c01 6a0b  rS|.j.d.u.rS|.j.
-00001640: a00c a100 4400 5d0b 5c02 7d03 7d01 8800  ....D.].\.}.}...
-00001650: a00d 7c01 a101 7c02 7c03 3c00 7147 740e  ..|...|.|.<.qGt.
-00001660: 7c01 6a04 740f 8302 7269 7c02 6a08 7c01  |.j.t...ri|.j.|.
-00001670: a010 a100 640a 8d01 0100 7c02 6a08 7c01  ....d.....|.j.|.
-00001680: 6a11 6a12 640b 8d01 0100 7c02 5300 290c  j.j.d.....|.S.).
-00001690: 4e29 0272 9500 0000 da0a 7265 6163 745f  N).r......react_
-000016a0: 6e61 6d65 da08 656c 656d 656e 7473 6301  name..elementsc.
-000016b0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000016c0: 0000 0013 0000 0073 1e00 0000 6700 7c00  .......s....g.|.
-000016d0: 5d0b 7d01 7c01 a000 a100 7202 8800 a001  ].}.|.....r.....
-000016e0: 7c01 a101 9102 7102 5300 7236 0000 0029  |.....q.S.r6...)
-000016f0: 02da 0a69 735f 7669 7369 626c 6572 aa00  ...is_visibler..
-00001700: 0000 2902 7246 0000 00da 0165 7250 0000  ..).rF.....erP..
-00001710: 0072 3600 0000 7237 0000 0072 4800 0000  .r6...r7...rH...
-00001720: ca00 0000 7302 0000 001e 007a 2652 656e  ....s......z&Ren
-00001730: 6465 7265 722e 656c 656d 326a 736f 6e2e  derer.elem2json.
-00001740: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00001750: 6d70 3e72 6800 0000 7a98 6669 656c 6473  mp>rh...z.fields
-00001760: 5f69 6e64 6578 2066 6965 6c64 735f 696e  _index fields_in
-00001770: 6465 785f 6869 6464 656e 2065 6469 7461  dex_hidden edita
-00001780: 626c 6520 7665 7274 6963 616c 2068 7061  ble vertical hpa
-00001790: 6420 6973 5f66 6965 6c64 7365 7420 6e61  d is_fieldset na
-000017a0: 6d65 2077 6964 7468 2070 7265 6665 7272  me width preferr
-000017b0: 6564 5f77 6964 7468 2020 2020 2020 2020  ed_width        
-000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017d0: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
-000017e0: 2076 616c 7565 2068 666c 6578 2076 666c   value hflex vfl
-000017f0: 6578 7298 0000 007a 1561 6374 6f72 5f69  exr....z.actor_i
-00001800: 6420 6469 7370 6c61 795f 6d6f 6465 da06  d display_mode..
-00001810: 736c 6176 6573 2901 da0d 6669 656c 645f  slaves)...field_
-00001820: 6f70 7469 6f6e 7329 01da 0968 656c 705f  options)...help_
-00001830: 7465 7874 2913 72a0 0000 0072 1e00 0000  text).r....r....
-00001840: 7271 0000 0072 a100 0000 7242 0000 00da  rq...r....rB....
-00001850: 085f 5f6e 616d 655f 5f72 8200 0000 72ad  .__name__r....r.
-00001860: 0000 0072 7700 0000 7228 0000 0072 9800  ...rw...r(...r..
-00001870: 0000 72b0 0000 0072 6800 0000 72aa 0000  ..r....rh...r...
-00001880: 00da 0a69 7373 7562 636c 6173 7372 2100  ...issubclassr!.
-00001890: 0000 da11 6765 745f 6669 656c 645f 6f70  ....get_field_op
-000018a0: 7469 6f6e 73da 0566 6965 6c64 72b2 0000  tions..fieldr...
-000018b0: 0029 0472 3f00 0000 72a5 0000 0072 a600  .).r?...r....r..
-000018c0: 0000 da01 6b72 3600 0000 7250 0000 0072  ....kr6...rP...r
-000018d0: 3700 0000 72aa 0000 00c3 0000 0073 2000  7...r........s .
-000018e0: 0000 0e01 0802 0602 06fe 0a03 1801 1002  ................
-000018f0: 0a04 1202 1403 1201 1001 0c03 1001 1001  ................
-00001900: 0402 7a12 5265 6e64 6572 6572 2e65 6c65  ..z.Renderer.ele
-00001910: 6d32 6a73 6f6e 6301 0000 0000 0000 0000  m2jsonc.........
-00001920: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00001930: 0400 0000 6401 5300 2902 4e7a 1e77 696e  ....d.S.).Nz.win
-00001940: 646f 772e 4170 702e 6461 7368 626f 6172  dow.App.dashboar
-00001950: 642e 7265 6c6f 6164 2829 3b72 3600 0000  d.reload();r6...
-00001960: 7250 0000 0072 3600 0000 7236 0000 0072  rP...r6...r6...r
-00001970: 3700 0000 da09 7265 6c6f 6164 5f6a 73e2  7.....reload_js.
-00001980: 0000 0073 0200 0000 0401 7a12 5265 6e64  ...s......z.Rend
-00001990: 6572 6572 2e72 656c 6f61 645f 6a73 6302  erer.reload_jsc.
-000019a0: 0000 0000 0000 0000 0000 0006 0000 0004  ................
-000019b0: 0000 004f 0000 0073 dc00 0000 7c01 6a00  ...O...s....|.j.
-000019c0: 6a01 6401 6b02 720f 7c00 6a02 6a03 7c02  j.d.k.r.|.j.j.|.
-000019d0: 6900 7c03 a401 8e01 5300 7c01 a004 a100  i.|.....S.|.....
-000019e0: 7d04 7c03 a005 7c04 6402 1900 a101 0100  }.|...|.d.......
-000019f0: 7406 7c03 7c01 8302 0100 7c01 6a07 6403  t.|.|.....|.j.d.
-00001a00: 7501 722c 7c03 a008 7409 6a0a 7c01 6a07  u.r,|...t.j.|.j.
-00001a10: a102 0100 7c01 6a0b 6403 7501 7239 7c03  ....|.j.d.u.r9|.
-00001a20: a008 7409 6a0c 7c01 6a0b a102 0100 7c01  ..t.j.|.j.....|.
-00001a30: 6a0d 6403 7501 725c 7c01 6a0d 6404 1900  j.d.u.r\|.j.d...
-00001a40: 7d05 7c05 a00e 6405 a101 7255 7c05 6406  }.|...d...rU|.d.
-00001a50: 6403 8502 1900 7d05 7c03 a008 7409 6a0f  d.....}.|...t.j.
-00001a60: 6407 a102 0100 7c03 a008 7409 6a10 7c05  d.....|...t.j.|.
-00001a70: a102 0100 7c00 6a02 6a03 7c01 6a00 6a11  ....|.j.j.|.j.j.
-00001a80: 7c01 6a00 6a01 6702 7c02 a201 5200 6900  |.j.j.g.|...R.i.
-00001a90: 7c03 a401 8e01 5300 2908 7a20 5573 6564  |.....S.).z Used
-00001aa0: 2066 6f72 2074 7572 6e20 7265 7175 6573   for turn reques
-00001ab0: 7473 2069 6e74 6f20 7572 6c73 da04 4d61  ts into urls..Ma
-00001ac0: 696e da0b 6261 7365 5f70 6172 616d 734e  in..base_paramsN
-00001ad0: 7201 0000 00fa 012d 722c 0000 00da 0444  r......-r,.....D
-00001ae0: 4553 4329 1272 9800 0000 72b3 0000 0072  ESC).r....r....r
-00001af0: 4000 0000 da0f 6275 696c 645f 706c 6169  @.....build_plai
-00001b00: 6e5f 7572 6cda 0a67 6574 5f73 7461 7475  n_url..get_statu
-00001b10: 7372 7700 0000 7208 0000 00da 066f 6666  srw...r......off
-00001b20: 7365 74da 0a73 6574 6465 6661 756c 7472  set..setdefaultr
-00001b30: 0c00 0000 da0f 5552 4c5f 5041 5241 4d5f  ......URL_PARAM_
-00001b40: 5354 4152 54da 056c 696d 6974 da0f 5552  START..limit..UR
-00001b50: 4c5f 5041 5241 4d5f 4c49 4d49 54da 086f  L_PARAM_LIMIT..o
-00001b60: 7264 6572 5f62 79da 0a73 7461 7274 7377  rder_by..startsw
-00001b70: 6974 68da 1155 524c 5f50 4152 414d 5f53  ith..URL_PARAM_S
-00001b80: 4f52 5444 4952 da0e 5552 4c5f 5041 5241  ORTDIR..URL_PARA
-00001b90: 4d5f 534f 5254 da09 6170 705f 6c61 6265  M_SORT..app_labe
-00001ba0: 6c29 0672 3f00 0000 da02 6172 da04 6172  l).r?.....ar..ar
-00001bb0: 6773 da02 6b77 da02 7374 da02 7363 7236  gs..kw..st..scr6
-00001bc0: 0000 0072 3600 0000 7237 0000 00da 0f67  ...r6...r7.....g
-00001bd0: 6574 5f72 6571 7565 7374 5f75 726c e500  et_request_url..
-00001be0: 0000 732c 0000 000c 0212 0108 020e 010a  ..s,............
-00001bf0: 010a 0110 010a 0110 010a 010a 010a 010c  ................
-00001c00: 010e 010e 0106 030c 0102 ff02 0106 ff02  ................
-00001c10: 0106 ff7a 1852 656e 6465 7265 722e 6765  ...z.Renderer.ge
-00001c20: 745f 7265 7175 6573 745f 7572 6c4e 6305  t_request_urlNc.
-00001c30: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-00001c40: 0000 004b 0000 0073 ae00 0000 7c04 7005  ...K...s....|.p.
-00001c50: 7c03 a000 a100 7d04 7401 7c04 8301 6401  |.....}.t.|...d.
-00001c60: 6b02 7211 6402 a002 7c04 a101 7d04 7c03  k.r.d...|...}.|.
-00001c70: 6a03 6a04 722c 7c03 6a03 6a05 732c 7c00  j.j.r,|.j.j.s,|.
-00001c80: a006 7c02 7c03 7c01 a103 7d06 7c00 6a07  ..|.|.|...}.|.j.
-00001c90: 7c02 7c03 7c06 7c04 6604 6900 7c05 a401  |.|.|.|.f.i.|...
-00001ca0: 8e01 5300 7c03 6a03 6a08 724b 7c02 a009  ..S.|.j.j.rK|...
-00001cb0: a100 7d06 7c01 6400 7501 723f 7c06 6a0a  ..}.|.d.u.r?|.j.
-00001cc0: 7c01 6a0b 6403 8d01 0100 7c00 6a07 7c02  |.j.d.....|.j.|.
-00001cd0: 7c03 7c06 7c04 6604 6900 7c05 a401 8e01  |.|.|.f.i.|.....
-00001ce0: 5300 7c00 6a0c 7c01 7c02 7c03 7c04 6604  S.|.j.|.|.|.|.f.
-00001cf0: 6900 7c05 a401 8e01 5300 2904 4e72 2c00  i.|.....S.).Nr,.
-00001d00: 0000 7506 0000 00c2 a07b 7dc2 a029 01da  ..u......{}..)..
-00001d10: 0972 6563 6f72 645f 6964 290d da10 6765  .record_id)...ge
-00001d20: 745f 6275 7474 6f6e 5f6c 6162 656c da03  t_button_label..
-00001d30: 6c65 6eda 0666 6f72 6d61 7472 6c00 0000  len..formatrl...
-00001d40: da0a 7061 7261 6d65 7465 7273 da10 6e6f  ..parameters..no
-00001d50: 5f70 6172 616d 735f 7769 6e64 6f77 da11  _params_window..
-00001d60: 6765 745f 6163 7469 6f6e 5f73 7461 7475  get_action_statu
-00001d70: 73da 1477 696e 646f 775f 6163 7469 6f6e  s..window_action
-00001d80: 5f62 7574 746f 6eda 0e6f 7065 6e73 5f61  _button..opens_a
-00001d90: 5f77 696e 646f 7772 be00 0000 7277 0000  _windowr....rw..
-00001da0: 00da 0270 6bda 1172 6f77 5f61 6374 696f  ...pk..row_actio
-00001db0: 6e5f 6275 7474 6f6e 2907 723f 0000 00da  n_button).r?....
-00001dc0: 036f 626a 72c9 0000 0072 8f00 0000 7295  .objr....r....r.
-00001dd0: 0000 0072 cb00 0000 72cc 0000 0072 3600  ...r....r....r6.
-00001de0: 0000 7236 0000 0072 3700 0000 da0d 6163  ..r6...r7.....ac
-00001df0: 7469 6f6e 5f62 7574 746f 6efd 0000 0073  tion_button....s
-00001e00: 2000 0000 0c01 0c01 0a01 1002 0e01 0401   ...............
-00001e10: 0801 04ff 0201 06ff 0802 0801 0801 0e01  ................
-00001e20: 1801 1801 7a16 5265 6e64 6572 6572 2e61  ....z.Renderer.a
-00001e30: 6374 696f 6e5f 6275 7474 6f6e 6305 0000  ction_buttonc...
-00001e40: 0000 0000 0000 0000 0007 0000 0004 0000  ................
-00001e50: 004b 0000 0073 4000 0000 7c02 6401 7500  .K...s@...|.d.u.
-00001e60: 720d 7c03 6a00 6402 6900 7c04 a401 8e01  r.|.j.d.i.|.....
-00001e70: 7d06 6e09 7c02 6a01 7c03 6601 6900 7c04  }.n.|.j.|.f.i.|.
-00001e80: a401 8e01 7d06 7c00 6a02 7c06 7c01 6602  ....}.|.j.|.|.f.
-00001e90: 6900 7c05 a401 8e01 5300 2903 61cf 0100  i.|.....S.).a...
-00001ea0: 004e 6f74 6520 7468 6174 2060 6261 2e61  .Note that `ba.a
-00001eb0: 6374 6f72 6020 6d61 7920 6469 6666 6572  ctor` may differ
-00001ec0: 2066 726f 6d20 6061 722e 6163 746f 7260   from `ar.actor`
-00001ed0: 2077 6865 6e20 6465 6669 6e65 6420 6f6e   when defined on
-00001ee0: 2061 0a20 2020 2020 2020 2064 6966 6665   a.        diffe
-00001ef0: 7265 6e74 2061 6374 6f72 2e20 5265 6d65  rent actor. Reme
-00001f00: 6d62 6572 2065 2e67 2e20 7468 6520 224d  mber e.g. the "M
-00001f10: 7573 7420 7265 6164 2065 4944 2063 6172  ust read eID car
-00001f20: 6422 2061 6374 696f 6e0a 2020 2020 2020  d" action.      
-00001f30: 2020 6275 7474 6f6e 2069 6e20 6569 645f    button in eid_
-00001f40: 696e 666f 206f 6620 6e65 7763 6f6d 6572  info of newcomer
-00001f50: 732e 4e65 7743 6c69 656e 7473 2028 3230  s.NewClients (20
-00001f60: 3134 3034 3232 292e 0a0a 2020 2020 2020  140422)...      
-00001f70: 2020 3a6f 626a 3a20 2054 6865 2064 6174    :obj:  The dat
-00001f80: 6162 6173 6520 6f62 6a65 6374 0a20 2020  abase object.   
-00001f90: 2020 2020 203a 6172 3a20 2020 5468 6520       :ar:   The 
-00001fa0: 6163 7469 6f6e 2072 6571 7565 7374 0a20  action request. 
-00001fb0: 2020 2020 2020 203a 6261 3a20 2054 6865         :ba:  The
-00001fc0: 2062 6f75 6e64 2061 6374 696f 6e0a 2020   bound action.  
-00001fd0: 2020 2020 2020 3a72 6571 7565 7374 5f6b        :request_k
-00001fe0: 7761 7267 733a 206b 6579 776f 7264 2061  wargs: keyword a
-00001ff0: 7267 756d 656e 7473 2074 6f20 666f 7277  rguments to forw
-00002000: 6172 6465 6420 746f 2074 6865 2063 6869  arded to the chi
-00002010: 6c64 2061 6374 696f 6e20 7265 7175 6573  ld action reques
-00002020: 740a 0a20 2020 2020 2020 2041 6e79 206b  t..        Any k
-00002030: 6579 776f 7264 206f 7468 6572 2061 7267  eyword other arg
-00002040: 756d 656e 7473 2061 7265 2066 6f72 7761  uments are forwa
-00002050: 7264 6564 2074 6f20 3a6d 6574 683a 6061  rded to :meth:`a
-00002060: 7232 6a73 602e 0a0a 2020 2020 2020 2020  r2js`...        
-00002070: 4e72 3600 0000 2903 da07 7265 7175 6573  Nr6...)...reques
-00002080: 74da 0573 7061 776e da05 6172 326a 7329  t..spawn..ar2js)
-00002090: 0772 3f00 0000 72da 0000 0072 c900 0000  .r?...r....r....
-000020a0: 728f 0000 00da 0e72 6571 7565 7374 5f6b  r......request_k
-000020b0: 7761 7267 73da 0673 7461 7475 73da 0373  wargs..status..s
-000020c0: 6172 7236 0000 0072 3600 0000 7237 0000  arr6...r6...r7..
-000020d0: 00da 1761 6374 696f 6e5f 6361 6c6c 5f6f  ...action_call_o
-000020e0: 6e5f 696e 7374 616e 6365 0e01 0000 7308  n_instance....s.
-000020f0: 0000 0008 0e12 0112 0314 017a 2052 656e  ...........z Ren
-00002100: 6465 7265 722e 6163 7469 6f6e 5f63 616c  derer.action_cal
-00002110: 6c5f 6f6e 5f69 6e73 7461 6e63 6563 0200  l_on_instancec..
-00002120: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00002130: 0000 4300 0000 732c 0000 007c 016a 0070  ..C...s,...|.j.p
-00002140: 057c 016a 017d 0274 02a0 037c 0264 01a1  .|.j.}.t...|.d..
-00002150: 027d 037c 0364 0175 0072 1264 0153 0064  .}.|.d.u.r.d.S.d
-00002160: 027c 0316 0053 0029 037a bf0a 2020 2020  .|...S.).z..    
-00002170: 2020 2020 5573 6573 2061 6e20 696e 7465      Uses an inte
-00002180: 726e 616c 206d 6170 7069 6e67 2066 6f72  rnal mapping for
-00002190: 2069 636f 6e20 6e61 6d65 7320 746f 2063   icon names to c
-000021a0: 6f6e 7665 7274 2065 7869 7374 696e 6720  onvert existing 
-000021b0: 6963 6f6e 7320 696e 746f 2072 6561 6374  icons into react
-000021c0: 2d75 7361 626c 652e 0a20 2020 2020 2020  -usable..       
-000021d0: 203a 7061 7261 6d20 6163 7469 6f6e 3a0a   :param action:.
-000021e0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-000021f0: 2073 7472 3a20 6120 6963 6f6e 206e 616d   str: a icon nam
-00002200: 6520 666f 7220 6569 7468 6572 2070 7269  e for either pri
-00002210: 6d65 2d72 6561 6374 206f 7220 6963 6f6e  me-react or icon
-00002220: 380a 2020 2020 2020 2020 4e7a 0570 6920  8.        Nz.pi 
-00002230: 2573 2904 da0f 7265 6163 745f 6963 6f6e  %s)...react_icon
-00002240: 5f6e 616d 65da 0969 636f 6e5f 6e61 6d65  _name..icon_name
-00002250: 722d 0000 00da 0367 6574 2904 723f 0000  r-.....get).r?..
-00002260: 0072 6c00 0000 729f 0000 00da 0a72 6561  .rl...r......rea
-00002270: 6374 5f69 636f 6e72 3600 0000 7236 0000  ct_iconr6...r6..
-00002280: 0072 3700 0000 72a4 0000 0023 0100 0073  .r7...r....#...s
-00002290: 0a00 0000 0c07 0c01 0801 0401 0802 7a18  ..............z.
-000022a0: 5265 6e64 6572 6572 2e67 6574 5f61 6374  Renderer.get_act
-000022b0: 696f 6e5f 6963 6f6e 6303 0000 0000 0000  ion_iconc.......
-000022c0: 0000 0000 0008 0000 0007 0000 004b 0000  .............K..
-000022d0: 0073 a400 0000 7c01 6a00 7d04 7c01 6a01  .s....|.j.}.|.j.
-000022e0: 7d05 6900 7d06 7c05 6a02 a003 a100 721c  }.i.}.|.j.....r.
-000022f0: 7c03 a004 7c00 a005 7c01 7c05 7c02 a103  |...|...|.|.|...
-00002300: a101 0100 7c06 a004 7c03 a101 0100 7c06  ....|...|.....|.
-00002310: a004 7c00 a006 7c01 7c05 7c02 a103 a101  ..|...|.|.|.....
-00002320: 0100 7c06 a004 7c03 a101 0100 7c04 7c05  ..|...|.....|.|.
-00002330: 6a02 6a07 7c01 6a08 7c05 6a09 6a0a 7c06  j.j.|.j.|.j.j.|.
-00002340: 6401 9c05 7d07 740b 7c02 6402 8302 7243  d...}.t.|.d...rC
-00002350: 7c02 6a0c 7c07 6403 3c00 6e09 740d 7c02  |.j.|.d.<.n.t.|.
-00002360: 740e 8302 724c 7c02 7c07 6403 3c00 6404  t...rL|.|.d.<.d.
-00002370: 740f 7c07 8301 1600 5300 2905 7a43 496d  t.|.....S.).zCIm
-00002380: 706c 656d 656e 7473 203a 6d65 7468 3a60  plements :meth:`
-00002390: 6c69 6e6f 2e63 6f72 652e 7265 6e64 6572  lino.core.render
-000023a0: 6572 2e48 746d 6c52 656e 6465 7265 722e  er.HtmlRenderer.
-000023b0: 6172 326a 7360 2e0a 0a20 2020 2020 2020  ar2js`...       
-000023c0: 2029 05da 0272 7072 9400 0000 da06 6f6e   )...rpr......on
-000023d0: 4d61 696e da07 6163 746f 7249 6472 e000  Main..actorIdr..
-000023e0: 0000 72d8 0000 00da 0273 72fa 1877 696e  ..r......sr..win
-000023f0: 646f 772e 4170 702e 7275 6e41 6374 696f  dow.App.runActio
-00002400: 6e28 2573 2929 10da 1072 6571 7565 7374  n(%s))...request
-00002410: 696e 675f 7061 6e65 6c72 a300 0000 726c  ing_panelr....rl
-00002420: 0000 0072 a200 0000 7277 0000 0072 d500  ...r....rw...r..
-00002430: 0000 da11 6765 745f 6163 7469 6f6e 5f70  ....get_action_p
-00002440: 6172 616d 7372 4d00 0000 da10 6973 5f6f  aramsrM.....is_o
-00002450: 6e5f 6d61 696e 5f61 6374 6f72 7298 0000  n_main_actorr...
-00002460: 00da 0861 6374 6f72 5f69 6472 8200 0000  ...actor_idr....
-00002470: 72d8 0000 0072 a000 0000 7278 0000 0072  r....r....rx...r
-00002480: 2600 0000 2908 723f 0000 0072 c900 0000  &...).r?...r....
-00002490: 72da 0000 0072 e000 0000 72e7 0000 0072  r....r....r....r
-000024a0: 8f00 0000 da06 7061 7261 6d73 da06 6a73  ......params..js
-000024b0: 5f6f 626a 7236 0000 0072 3600 0000 7237  _objr6...r6...r7
-000024c0: 0000 0072 de00 0000 3101 0000 732a 0000  ...r....1...s*..
-000024d0: 0006 0406 0104 010a 0114 040a 0114 010a  ................
-000024e0: 0102 0306 0104 0106 0102 0106 fb0a 070c  ................
-000024f0: 010a 0208 0102 0206 0104 ff7a 0e52 656e  ...........z.Ren
-00002500: 6465 7265 722e 6172 326a 7363 0200 0000  derer.ar2jsc....
-00002510: 0000 0000 0000 0000 0600 0000 0600 0000  ................
-00002520: 4300 0000 73bc 0100 007c 0174 006a 016a  C...s....|.t.j.j
-00002530: 0275 0072 0a74 0364 0183 0153 0074 047c  .u.r.t.d...S.t.|
-00002540: 0174 0583 0272 1674 0664 02a0 077c 01a1  .t...r.t.d...|..
-00002550: 0183 0182 0174 047c 0174 086a 0983 0272  .....t.|.t.j...r
-00002560: 2009 007c 016a 0a53 0074 047c 0174 0b6a   ..|.j.S.t.|.t.j
-00002570: 0c83 0272 297c 016a 0d53 0074 047c 0174  ...r)|.j.S.t.|.t
-00002580: 0683 0272 3274 0e7c 0183 0153 0074 047c  ...r2t.|...S.t.|
-00002590: 0174 0f83 0272 4a7c 016a 1064 0375 0072  .t...rJ|.j.d.u.r
-000025a0: 3f7c 016a 1153 0074 127c 016a 1374 127c  ?|.j.S.t.|.j.t.|
-000025b0: 016a 1164 048d 0164 058d 0253 0074 047c  .j.d...d...S.t.|
-000025c0: 0174 1483 0272 cc7c 016a 1564 0375 0172  .t...r.|.j.d.u.r
-000025d0: 6d7c 00a0 1664 037c 016a 1564 03a1 037d  m|...d.|.j.d...}
-000025e0: 027c 0264 0375 0173 624a 0082 0164 067c  .|.d.u.sbJ...d.|
-000025f0: 0216 007d 037c 00a0 177c 017c 0264 03a1  ...}.|...|.|.d..
-00002600: 0353 007c 016a 1864 0375 0172 957c 016a  .S.|.j.d.u.r.|.j
-00002610: 1972 857c 016a 186a 1a64 0d69 007c 016a  .r.|.j.j.d.i.|.j
-00002620: 19a4 018e 017d 047c 00a0 1b7c 04a1 017d  .....}.|...|...}
-00002630: 036e 087c 00a0 1c64 037c 016a 1869 00a1  .n.|...d.|.j.i..
-00002640: 037d 037c 00a0 177c 017c 037c 016a 1da1  .}.|...|.|.|.j..
-00002650: 0353 007c 016a 1e64 0375 0172 a764 067c  .S.|.j.d.u.r.d.|
-00002660: 016a 1e16 007d 037c 00a0 177c 017c 037c  .j...}.|...|.|.|
-00002670: 016a 1da1 0353 007c 016a 1f64 0375 0172  .j...S.|.j.d.u.r
-00002680: b07c 016a 1f7d 056e 037c 016a 1353 007c  .|.j.}.n.|.j.S.|
-00002690: 016a 106a 1064 0375 0072 c574 1264 077c  .j.j.d.u.r.t.d.|
-000026a0: 016a 1374 0364 087c 0516 0083 0164 098d  .j.t.d.|.....d..
-000026b0: 0353 0074 127c 016a 137c 0564 0a8d 0253  .S.t.|.j.|.d...S
-000026c0: 0074 047c 0174 0383 0272 dc74 207c 0064  .t.|.t...r.t |.d
-000026d0: 0b64 0c83 0372 dc74 0e7c 016a 2183 0153  .d...r.t.|.j!..S
-000026e0: 007c 0153 0029 0e7a 540a 2020 2020 2020  .|.S.).zT.      
-000026f0: 2020 4164 6469 7469 6f6e 616c 2063 6f6e    Additional con
-00002700: 7665 7274 696e 6720 6c6f 6769 6320 666f  verting logic fo
-00002710: 7220 7365 7269 616c 697a 696e 6720 5079  r serializing Py
-00002720: 7468 6f6e 2076 616c 7565 7320 746f 206a  thon values to j
-00002730: 736f 6e2e 0a20 2020 2020 2020 20da 104c  son..        ..L
-00002740: 414e 4755 4147 455f 4348 4f49 4345 537a  ANGUAGE_CHOICESz
-00002750: 0b32 3032 3130 3531 3720 7b7d 4e29 0172  .20210517 {}N).r
-00002760: 6800 0000 2902 7244 0000 0072 5500 0000  h...).rD...rU...
-00002770: 7a02 2573 da06 6275 7474 6f6e 7a23 6675  z.%s..buttonz#fu
-00002780: 6e63 7469 6f6e 2829 207b 204c 696e 6f2e  nction() { Lino.
-00002790: 6c6f 6164 5f75 726c 2827 2573 2729 3b20  load_url('%s'); 
-000027a0: 7d29 03da 0578 7479 7065 7244 0000 00da  })...xtyperD....
-000027b0: 0768 616e 646c 6572 2902 7244 0000 00da  .handler).rD....
-000027c0: 0468 7265 6672 6e00 0000 4672 3600 0000  .hrefrn...Fr6...
-000027d0: 2922 7204 0000 0072 6f00 0000 72f2 0000  )"r....ro...r...
-000027e0: 0072 2700 0000 72a0 0000 0072 1c00 0000  .r'...r....r....
-000027f0: da09 4578 6365 7074 696f 6e72 d200 0000  ..Exceptionr....
-00002800: 720d 0000 00da 0643 686f 6963 6572 4300  r......ChoicerC.
-00002810: 0000 7205 0000 00da 054d 6f64 656c 72d8  ..r......Modelr.
-00002820: 0000 0072 4500 0000 720a 0000 00da 0670  ...rE...r......p
-00002830: 6172 656e 7472 6800 0000 7271 0000 0072  arentrh...rq...r
-00002840: 9500 0000 720b 0000 00da 0869 6e73 7461  ....r......insta
-00002850: 6e63 65da 1069 6e73 7461 6e63 655f 6861  nce..instance_ha
-00002860: 6e64 6c65 72da 0c68 616e 646c 6572 5f69  ndler..handler_i
-00002870: 7465 6d72 a300 0000 72f0 0000 0072 dc00  temr....r....r..
-00002880: 0000 da0f 7265 7175 6573 745f 6861 6e64  ....request_hand
-00002890: 6c65 72da 0b61 6374 696f 6e5f 6361 6c6c  ler..action_call
-000028a0: 72b2 0000 00da 0a6a 6176 6173 6372 6970  r......javascrip
-000028b0: 7472 f600 0000 da07 6765 7461 7474 72da  tr......getattr.
-000028c0: 0173 2906 723f 0000 0072 a500 0000 da01  .s).r?...r......
-000028d0: 68da 026a 7372 c900 0000 da03 7572 6c72  h..jsr......urlr
-000028e0: 3600 0000 7236 0000 0072 3700 0000 723e  6...r6...r7...r>
-000028f0: 0000 0052 0100 0073 5400 0000 0c04 0801  ...R...sT.......
-00002900: 0a01 0e01 0c01 0201 0603 0c01 0601 0a01  ................
-00002910: 0801 0a01 0a01 0601 1603 0a02 0a02 1001  ................
-00002920: 0c01 0801 0e01 0a01 0601 1401 0c01 1004  ................
-00002930: 1001 0a02 0a01 1001 0a01 0801 0607 0c02  ................
-00002940: 0202 0601 0a02 06fd 0e04 1602 0a02 0402  ................
-00002950: 7a18 5265 6e64 6572 6572 2e70 7932 6a73  z.Renderer.py2js
-00002960: 5f63 6f6e 7665 7274 6572 6304 0000 0000  _converterc.....
-00002970: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-00002980: 0000 0073 5000 0000 7400 7c01 6a01 7c02  ...sP...t.|.j.|.
-00002990: 6401 8d02 7d04 7c01 6a02 721a 7c01 6a02  d...}.|.j.r.|.j.
-000029a0: 6a03 6a04 721a 7c04 6a05 6402 7c01 6a02  j.j.r.|.j.d.|.j.
-000029b0: 6a03 6a04 1700 6403 8d01 0100 7406 6a07  j.j...d.....t.j.
-000029c0: 6a08 7226 7c03 7226 7c04 6a05 7c03 6404  j.r&|.r&|.j.|.d.
-000029d0: 8d01 0100 7c04 5300 2905 da00 2902 7244  ....|.S.)...).rD
-000029e0: 0000 0072 f500 0000 7a07 782d 7462 6172  ...r....z.x-tbar
-000029f0: 2d29 01da 0769 636f 6e43 6c73 2901 da07  -)...iconCls)...
-00002a00: 746f 6f6c 5469 7029 0972 7100 0000 7295  toolTip).rq...r.
-00002a10: 0000 0072 a300 0000 726c 0000 0072 e400  ...r....rl...r..
-00002a20: 0000 7277 0000 0072 0400 0000 726f 0000  ..rw...r....ro..
-00002a30: 00da 0d75 7365 5f71 7569 636b 7469 7073  ...use_quicktips
-00002a40: 2905 723f 0000 00da 026d 6972 f500 0000  ).r?.....mir....
-00002a50: 72b2 0000 00da 0164 7236 0000 0072 3600  r......dr6...r6.
-00002a60: 0000 7237 0000 0072 fd00 0000 a301 0000  ..r7...r........
-00002a70: 730c 0000 000e 0410 0116 010c 010c 0304  s...............
-00002a80: 017a 1552 656e 6465 7265 722e 6861 6e64  .z.Renderer.hand
-00002a90: 6c65 725f 6974 656d 6302 0000 0000 0000  ler_itemc.......
-00002aa0: 0000 0000 0005 0000 0005 0000 004f 0000  .............O..
-00002ab0: 0073 2000 0000 7c01 6a00 6402 6900 7c03  .s ...|.j.d.i.|.
-00002ac0: a401 8e01 7d04 7c00 a001 7c01 7c01 6a02  ....}.|...|.|.j.
-00002ad0: 7c04 a103 5300 2903 7a36 2047 656e 6572  |...S.).z6 Gener
-00002ae0: 6174 6573 206a 7320 7374 7269 6e67 2066  ates js string f
-00002af0: 6f72 2061 6374 696f 6e20 6275 7474 6f6e  or action button
-00002b00: 2063 616c 6c73 2e0a 2020 2020 2020 2020   calls..        
-00002b10: 4e72 3600 0000 2903 72be 0000 0072 ff00  Nr6...).r....r..
-00002b20: 0000 72a3 0000 0029 0572 3f00 0000 72c9  ..r....).r?...r.
-00002b30: 0000 0072 ca00 0000 72cb 0000 0072 cc00  ...r....r....r..
-00002b40: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
-00002b50: 0072 fe00 0000 b101 0000 7304 0000 0010  .r........s.....
-00002b60: 0410 017a 1852 656e 6465 7265 722e 7265  ...z.Renderer.re
-00002b70: 7175 6573 745f 6861 6e64 6c65 7263 0400  quest_handlerc..
-00002b80: 0000 0000 0000 0000 0000 0800 0000 0800  ................
-00002b90: 0000 4300 0000 739c 0000 007c 026a 007d  ..C...s....|.j.}
-00002ba0: 047c 02a0 01a1 00a0 0264 0164 02a1 025c  .|.......d.d...\
-00002bb0: 027d 057d 067c 0373 1169 007d 037c 0164  .}.}.|.s.i.}.|.d
-00002bc0: 0075 0172 2274 037c 0164 0383 0272 227c  .u.r"t.|.d...r"|
-00002bd0: 016a 0464 0869 007c 03a4 018e 017d 037c  .j.d.i.|.....}.|
-00002be0: 0172 2d7c 016a 0572 2d7c 016a 057c 0374  .r-|.j.r-|.j.|.t
-00002bf0: 066a 073c 007c 0664 046b 0272 3974 037c  .j.<.|.d.k.r9t.|
-00002c00: 0364 0583 0272 397c 0364 053d 007c 0164  .d...r9|.d.=.|.d
-00002c10: 0075 0072 3f64 006e 027c 016a 087d 0764  .u.r?d.n.|.j.}.d
-00002c20: 0674 0974 0a7c 067c 057c 037c 0764 078d  .t.t.|.|.|.|.d..
-00002c30: 0483 0116 0053 0029 094e da01 2e72 2c00  .....S.).N...r,.
-00002c40: 0000 72be 0000 00da 0467 7269 6472 cf00  ..r......gridr..
-00002c50: 0000 72eb 0000 0029 0472 9400 0000 72e9  ..r....).r....r.
-00002c60: 0000 0072 e000 0000 72e7 0000 0072 3600  ...r....r....r6.
-00002c70: 0000 290b 726c 0000 00da 0966 756c 6c5f  ..).rl.....full_
-00002c80: 6e61 6d65 da06 7273 706c 6974 7282 0000  name..rsplitr...
-00002c90: 0072 be00 0000 da0a 7375 6273 745f 7573  .r......subst_us
-00002ca0: 6572 720c 0000 00da 1455 524c 5f50 4152  err......URL_PAR
-00002cb0: 414d 5f53 5542 5354 5f55 5345 5272 ec00  AM_SUBST_USERr..
-00002cc0: 0000 7226 0000 0072 7100 0000 2908 723f  ..r&...rq...).r?
-00002cd0: 0000 0072 c900 0000 72a3 0000 0072 e000  ...r....r....r..
-00002ce0: 0000 724f 0000 0072 e900 0000 7294 0000  ..rO...r....r...
-00002cf0: 0072 e700 0000 7236 0000 0072 3600 0000  .r....r6...r6...
-00002d00: 7237 0000 0072 ff00 0000 bb01 0000 7322  r7...r........s"
-00002d10: 0000 0006 0214 0204 0204 0112 0210 010a  ................
-00002d20: 020c 0112 1106 0112 0206 0202 0102 0102  ................
-00002d30: 0102 010a fc7a 1452 656e 6465 7265 722e  .....z.Renderer.
-00002d40: 6163 7469 6f6e 5f63 616c 6c63 0200 0000  action_callc....
-00002d50: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00002d60: 4300 0000 732e 0000 007c 0173 0464 0053  C...s....|.s.d.S
-00002d70: 0074 007c 0174 0183 0273 0d74 017c 0183  .t.|.t...s.t.|..
-00002d80: 017d 0174 027c 0164 0164 028d 027d 0164  .}.t.|.d.d...}.d
-00002d90: 037c 0117 0053 0029 044e 4629 01da 0571  .|...S.).NF)...q
-00002da0: 756f 7465 7a0b 6a61 7661 7363 7269 7074  uotez.javascript
-00002db0: 3a29 0372 a000 0000 7245 0000 0072 0300  :).r....rE...r..
-00002dc0: 0000 2902 723f 0000 0072 0401 0000 7236  ..).r?...r....r6
-00002dd0: 0000 0072 3600 0000 7237 0000 00da 066a  ...r6...r7.....j
-00002de0: 7332 7572 6ce4 0100 0073 0c00 0000 0401  s2url....s......
-00002df0: 0401 0a02 0801 0c01 0801 7a0f 5265 6e64  ..........z.Rend
-00002e00: 6572 6572 2e6a 7332 7572 6c63 0600 0000  erer.js2urlc....
-00002e10: 0000 0000 0000 0000 0700 0000 0400 0000  ................
-00002e20: 4300 0000 7356 0000 0074 006a 016a 0272  C...sV...t.j.j.r
-00002e30: 2774 006a 016a 0372 0f64 017c 047c 0566  't.j.j.r.d.|.|.f
-00002e40: 0216 007d 066e 0264 027d 067c 0272 1974  ...}.n.d.}.|.r.t
-00002e50: 0464 037c 067c 0283 037d 067c 0672 297c  .d.|.|...}.|.r)|
-00002e60: 016a 0564 047c 037c 0666 0216 0064 058d  .j.d.|.|.f...d..
-00002e70: 0101 0064 0053 0064 0053 0064 0053 0029  ...d.S.d.S.d.S.)
-00002e80: 064e 7a08 2825 732e 2573 2920 7206 0100  .Nz.(%s.%s) r...
-00002e90: 007a 047b 7d7b 7d7a 0728 2573 2c25 7329  .z.{}{}z.(%s,%s)
-00002ea0: 2901 da08 7175 6963 6b74 6970 2906 7204  )...quicktip).r.
-00002eb0: 0000 0072 6f00 0000 7209 0100 00da 1973  ...ro...r......s
-00002ec0: 686f 775f 696e 7465 726e 616c 5f66 6965  how_internal_fie
-00002ed0: 6c64 5f6e 616d 6573 7206 0000 0072 7700  ld_namesr....rw.
-00002ee0: 0000 2907 723f 0000 0072 cb00 0000 72b2  ..).r?...r....r.
-00002ef0: 0000 0072 7400 0000 da0a 6461 7461 736f  ...rt.....dataso
-00002f00: 7572 6365 da09 6669 656c 646e 616d 65da  urce..fieldname.
-00002f10: 0374 7474 7236 0000 0072 3600 0000 7237  .tttr6...r6...r7
-00002f20: 0000 00da 0d61 6464 5f68 656c 705f 7465  .....add_help_te
-00002f30: 7874 ed01 0000 7318 0000 0008 0108 010e  xt....s.........
-00002f40: 0104 0204 010c 0104 0108 0402 010e ff04  ................
-00002f50: f504 077a 1652 656e 6465 7265 722e 6164  ...z.Renderer.ad
-00002f60: 645f 6865 6c70 5f74 6578 7463 0200 0000  d_help_textc....
-00002f70: 0000 0000 0000 0000 0500 0000 0300 0000  ................
-00002f80: 4300 0000 7356 0000 0074 0083 007d 0264  C...sV...t...}.d
-00002f90: 017c 0117 0064 0217 007d 037c 006a 01a0  .|...d...}.|.j..
-00002fa0: 0264 03a1 0164 0419 007d 047c 0264 0575  .d...d...}.|.d.u
-00002fb0: 0172 1c7c 037c 026a 0364 0217 0037 007d  .r.|.|.j.d...7.}
-00002fc0: 037c 0374 04a0 05a1 0064 0317 007c 0417  .|.t.....d...|..
-00002fd0: 0037 007d 0364 067c 047c 0366 0353 0029  .7.}.d.|.|.f.S.)
-00002fe0: 077a 2c4c 696b 6520 6c69 6e6f 5f6a 735f  .z,Like lino_js_
-00002ff0: 7061 7274 732c 2062 7574 2066 6f72 2061  parts, but for a
-00003000: 6374 6f72 5f6c 6576 656c 2064 6174 61da  ctor_level data.
-00003010: 054c 696e 6f5f da01 5f72 0c01 0000 722e  .Lino_.._r....r.
-00003020: 0000 004e da05 6361 6368 6529 0672 2900  ...N..cache).r).
-00003030: 0000 da11 6c69 6e6f 5f77 6562 5f74 656d  ....lino_web_tem
-00003040: 706c 6174 6572 0f01 0000 7243 0000 0072  plater....rC...r
-00003050: 0700 0000 da0c 6765 745f 6c61 6e67 7561  ......get_langua
-00003060: 6765 2905 723f 0000 0072 e900 0000 da09  ge).r?...r......
-00003070: 7573 6572 5f74 7970 65da 0866 696c 656e  user_type..filen
-00003080: 616d 65da 0966 696c 655f 7479 7065 7236  ame..file_typer6
-00003090: 0000 0072 3600 0000 7237 0000 00da 156c  ...r6...r7.....l
-000030a0: 696e 6f5f 6a73 5f70 6172 7473 5f63 6875  ino_js_parts_chu
-000030b0: 6e6b 6564 fc01 0000 730e 0000 0006 020c  nked....s.......
-000030c0: 0110 0108 010e 0114 010a 017a 1e52 656e  ...........z.Ren
-000030d0: 6465 7265 722e 6c69 6e6f 5f6a 735f 7061  derer.lino_js_pa
-000030e0: 7274 735f 6368 756e 6b65 6463 0200 0000  rts_chunkedc....
-000030f0: 0000 0000 0000 0000 1100 0000 0600 0000  ................
-00003100: 4300 0000 73de 0100 0067 007d 0267 007d  C...s....g.}.g.}
-00003110: 037c 0144 005d e47d 047c 04a0 00a1 007d  .|.D.].}.|.....}
-00003120: 057c 0573 127c 046a 016a 0272 cc74 036a  .|.s.|.j.j.r.t.j
-00003130: 047c 046a 016a 0569 017d 067c 0572 237c  .|.j.j.i.}.|.r#|
-00003140: 066a 067c 056a 076a 0864 018d 0101 007c  .j.|.j.j.d.....|
-00003150: 046a 016a 0272 c767 007d 0774 0983 007d  .j.j.r.g.}.t...}
-00003160: 087c 046a 0aa0 0b7c 046a 0174 0c83 00a1  .|.j...|.j.t....
-00003170: 0244 005d 727d 0974 097c 096a 016a 0564  .D.]r}.t.|.j.j.d
-00003180: 028d 017d 0a7c 096a 016a 0d7d 0b7c 0b72  ...}.|.j.j.}.|.r
-00003190: 487c 0b7c 0a64 033c 007c 096a 016a 0e7d  H|.|.d.<.|.j.j.}
-000031a0: 0c7c 0c72 5e74 0f7c 0c83 0172 5a7c 0c7c  .|.r^t.|...rZ|.|
-000031b0: 096a 0a83 017c 0a64 043c 006e 047c 0c7c  .j...|.d.<.n.|.|
-000031c0: 0a64 043c 007c 096a 016a 1064 0575 0172  .d.<.|.j.j.d.u.r
-000031d0: 847c 096a 016a 107d 0d7c 0d7c 0876 0072  .|.j.j.}.|.|.v.r
-000031e0: 747c 087c 0d19 00a0 117c 0aa1 0101 006e  t|.|.....|.....n
-000031f0: 1574 097c 0d64 068d 017d 0e7c 0a67 017c  .t.|.d...}.|.g.|
-00003200: 087c 0d3c 007c 07a0 117c 0ea1 0101 006e  .|.<.|...|.....n
-00003210: 057c 07a0 117c 0aa1 0101 007c 096a 016a  .|...|.....|.j.j
-00003220: 1272 a774 137c 096a 016a 1283 017d 0f74  .r.t.|.j.j...}.t
-00003230: 147c 0f64 0783 0273 9e7c 096a 016a 057c  .|.d...s.|.j.j.|
-00003240: 0f64 073c 007c 0f7c 0376 0172 a77c 03a0  .d.<.|.|.v.r.|..
-00003250: 117c 0fa1 0101 0071 357c 0872 c374 157c  .|.....q5|.r.t.|
-00003260: 0783 0144 005d 145c 027d 107d 0a7c 0aa0  ...D.].\.}.}.|..
-00003270: 1664 0864 09a1 0272 c27c 087c 0a64 0819  .d.d...r.|.|.d..
-00003280: 0019 007c 077c 1019 0064 0a3c 0071 ae7c  ...|.|...d.<.q.|
-00003290: 077c 0664 0b3c 007c 02a0 117c 06a1 0101  .|.d.<.|...|....
-000032a0: 007c 046a 016a 1272 ea74 137c 046a 016a  .|.j.j.r.t.|.j.j
-000032b0: 1283 017d 0f74 147c 0f64 0783 0273 e17c  ...}.t.|.d...s.|
-000032c0: 046a 016a 057c 0f64 073c 007c 0f7c 0376  .j.j.|.d.<.|.|.v
-000032d0: 0172 ea7c 03a0 117c 0fa1 0101 0071 067c  .r.|...|.....q.|
-000032e0: 027c 0366 0253 0029 0c7a 4543 6f6e 7665  .|.f.S.).zEConve
-000032f0: 7274 7320 6f66 2061 6c6c 2074 6865 2062  rts of all the b
-00003300: 6f75 6e64 6163 7469 6f6e 7320 6f66 2061  oundactions of a
-00003310: 6e20 6163 746f 7220 746f 206a 736f 6e20  n actor to json 
-00003320: 666f 726d 6174 2e0a 2020 2020 2020 2020  format..        
-00003330: a901 7265 0000 0029 0172 9400 0000 72b2  ..re...).r....r.
-00003340: 0000 00da 0a6a 735f 6861 6e64 6c65 724e  .....js_handlerN
-00003350: 2901 da05 636f 6d62 6f72 8f00 0000 7225  )...combor....r%
-00003360: 0100 0046 7255 0000 00da 0e74 6f6f 6c62  ...FrU.....toolb
-00003370: 6172 4163 7469 6f6e 7329 17da 1167 6574  arActions)...get
-00003380: 5f6c 6179 6f75 745f 6861 6e64 656c 726c  _layout_handelrl
-00003390: 0000 00da 0b77 696e 646f 775f 7479 7065  .....window_type
-000033a0: 720c 0000 00da 1555 524c 5f50 4152 414d  r......URL_PARAM
-000033b0: 5f41 4354 494f 4e5f 4e41 4d45 724d 0000  _ACTION_NAMErM..
-000033c0: 0072 7700 0000 72ab 0000 0072 8700 0000  .rw...r....r....
-000033d0: 7271 0000 0072 9800 0000 da13 6765 745f  rq...r......get_
-000033e0: 746f 6f6c 6261 725f 6163 7469 6f6e 7372  toolbar_actionsr
-000033f0: 2900 0000 72b2 0000 0072 2401 0000 722f  )...r....r$...r/
-00003400: 0000 00da 0b63 6f6d 626f 5f67 726f 7570  .....combo_group
-00003410: da06 6170 7065 6e64 da06 686f 746b 6579  ..append..hotkey
-00003420: da04 7661 7273 7282 0000 0072 3000 0000  ..varsr....r0...
-00003430: 72e5 0000 0029 1172 3f00 0000 da0c 6163  r....).r?.....ac
-00003440: 7469 6f6e 735f 6c69 7374 72a6 0000 00da  tions_listr.....
-00003450: 0768 6f74 6b65 7973 728f 0000 00da 026c  .hotkeysr......l
-00003460: 68da 1161 6374 696f 6e5f 6465 7363 7269  h..action_descri
-00003470: 7074 6f72 da04 7462 6173 da09 636f 6d62  ptor..tbas..comb
-00003480: 6f5f 6d61 7072 4f00 0000 da03 7462 6172  o_maprO.....tbar
-00003490: b200 0000 7224 0100 0072 2b01 0000 7225  ....r$...r+...r%
-000034a0: 0100 0072 2d01 0000 7234 0000 0072 3600  ...r-...r4...r6.
-000034b0: 0000 7236 0000 0072 3700 0000 da0c 6163  ..r6...r7.....ac
-000034c0: 7469 6f6e 7332 6a73 6f6e 0602 0000 7368  tions2json....sh
-000034d0: 0000 0004 0404 0108 0208 010c 010e 0204  ................
-000034e0: 0110 0108 0104 0106 0106 0208 0108 ff0e  ................
-000034f0: 0308 010c 0108 0104 0108 0110 0108 020c  ................
-00003500: 0208 0108 0210 010a 020a 010c 010a 0208  ................
-00003510: 020c 010a 010c 0108 010a 0102 8004 0210  ................
-00003520: 010c 0114 0102 8008 020a 0208 020c 010a  ................
-00003530: 010c 0108 010a 0102 8008 027a 1552 656e  ...........z.Ren
-00003540: 6465 7265 722e 6163 7469 6f6e 7332 6a73  derer.actions2js
-00003550: 6f6e 6302 0000 0000 0000 0000 0000 0005  onc.............
-00003560: 0000 0005 0000 0043 0000 0073 5800 0000  .......C...sX...
-00003570: 6700 7d02 6400 7d03 7c01 4400 5d14 7d04  g.}.d.}.|.D.].}.
-00003580: 7c04 6401 1900 6400 7500 7213 7c04 6402  |.d...d.u.r.|.d.
-00003590: 1900 7d03 7106 7c02 a000 7401 7c04 8301  ..}.q.|...t.|...
-000035a0: a101 0100 7106 7402 7c02 6403 6404 8400  ....q.t.|.d.d...
-000035b0: 6405 8d02 7d02 7c02 a000 6400 7c03 6702  d...}.|...d.|.g.
-000035c0: a101 0100 7c02 5300 2906 4e72 0100 0000  ....|.S.).Nr....
-000035d0: 722c 0000 0063 0100 0000 0000 0000 0000  r,...c..........
-000035e0: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-000035f0: 0000 007c 0064 0119 0053 0029 024e 7201  ...|.d...S.).Nr.
-00003600: 0000 0072 3600 0000 2901 7235 0000 0072  ...r6...).r5...r
-00003610: 3600 0000 7236 0000 0072 3700 0000 da08  6...r6...r7.....
-00003620: 3c6c 616d 6264 613e 5202 0000 7302 0000  <lambda>R...s...
-00003630: 0008 007a 2c52 656e 6465 7265 722e 6469  ...z,Renderer.di
-00003640: 7370 6c61 795f 6d6f 6465 326a 736f 6e2e  splay_mode2json.
-00003650: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00003660: 3ea9 0172 3300 0000 2903 722c 0100 0072  >..r3...).r,...r
-00003670: 7800 0000 da06 736f 7274 6564 2905 723f  x.....sorted).r?
-00003680: 0000 00da 0c64 6973 706c 6179 5f6d 6f64  .....display_mod
-00003690: 65da 0364 6d73 da03 646d 6472 9200 0000  e..dms..dmdr....
-000036a0: 7236 0000 0072 3600 0000 7237 0000 00da  r6...r6...r7....
-000036b0: 1164 6973 706c 6179 5f6d 6f64 6532 6a73  .display_mode2js
-000036c0: 6f6e 4a02 0000 7312 0000 0004 0104 0108  onJ...s.........
-000036d0: 010c 010a 0110 0210 010e 0104 017a 1a52  .............z.R
-000036e0: 656e 6465 7265 722e 6469 7370 6c61 795f  enderer.display_
-000036f0: 6d6f 6465 326a 736f 6e63 0200 0000 0000  mode2jsonc......
-00003700: 0000 0000 0000 1100 0000 0800 0000 4300  ..............C.
-00003710: 0000 73fe 0200 0074 007c 0183 0172 0974  ..s....t.|...r.t
-00003720: 017c 0174 0283 0273 0b4a 0082 017c 00a0  .|.t...s.J...|..
-00003730: 037c 016a 04a1 015c 027d 027d 0374 057c  .|.j...\.}.}.t.|
-00003740: 016a 067c 027c 01a0 07a1 0074 087c 016a  .j.|.|.....t.|.j
-00003750: 0983 017c 01a0 0a74 0b83 00a1 010c 0064  ...|...t.......d
-00003760: 018d 057d 0474 0c7c 0383 0172 317c 046a  ...}.t.|...r1|.j
-00003770: 0d7c 0364 028d 0101 007c 01a0 0ea1 007d  .|.d.....|.....}
-00003780: 057c 056a 0f64 0075 0072 4374 106a 116a  .|.j.d.u.rCt.j.j
-00003790: 12a0 1364 037c 01a1 0201 006e 5d74 147c  ...d.|.....n]t.|
-000037a0: 0564 0483 0272 9767 007d 0664 057d 077c  .d...r.g.}.d.}.|
-000037b0: 05a0 15a1 007d 087c 0844 005d 407d 097c  .....}.|.D.]@}.|
-000037c0: 00a0 167c 09a1 017d 0a7c 0a6a 0d74 177c  ...|...}.|.j.t.|
-000037d0: 056a 0f6a 187c 096a 196a 1a64 0664 0784  .j.j.|.j.j.d.d..
-000037e0: 0064 088d 037c 0717 0064 098d 0101 0074  .d...|...d.....t
-000037f0: 1b7c 0974 1c83 0272 8474 1b7c 0974 1d83  .|.t...r.t.|.t..
-00003800: 0273 847c 0a6a 0d7c 0a64 0a19 0064 0b17  .s.|.j.|.d...d..
-00003810: 0064 0c8d 0101 007c 0764 0b37 007d 0774  .d.....|.d.7.}.t
-00003820: 1b7c 0974 1e83 0272 8d7c 0764 0d37 007d  .|.t...r.|.d.7.}
-00003830: 077c 06a0 1f7c 0aa1 0101 0071 527c 067c  .|...|.....qR|.|
-00003840: 0464 0e3c 007c 04a0 0d74 207c 056a 0f64  .d.<.|...t |.j.d
-00003850: 0f83 02a1 0101 007c 04a0 0d74 207c 0164  .......|...t |.d
-00003860: 1083 02a1 0101 0074 147c 016a 2164 1183  .......t.|.j!d..
-00003870: 0272 b47c 046a 0d64 1264 138d 0101 007c  .r.|.j.d.d.....|
-00003880: 016a 2264 0075 0172 c17c 00a0 237c 016a  .j"d.u.r.|..#|.j
-00003890: 22a1 017c 0464 143c 007c 016a 2464 0075  "..|.d.<.|.j$d.u
-000038a0: 0172 d67c 016a 24a0 25a1 007d 0b7c 0b64  .r.|.j$.%..}.|.d
-000038b0: 0075 0172 d67c 046a 0d7c 0b6a 2664 158d  .u.r.|.j.|.j&d..
-000038c0: 0101 007c 016a 2772 e27c 046a 0d74 287c  ...|.j'r.|.j.t(|
-000038d0: 016a 2783 0164 168d 0101 0074 297c 0164  .j'..d.....t)|.d
-000038e0: 1764 0083 037d 0c7c 0c64 0075 0172 f37c  .d...}.|.d.u.r.|
-000038f0: 046a 0d7c 0c6a 2664 188d 0101 0074 297c  .j.|.j&d.....t)|
-00003900: 0164 1964 0083 037d 0d7c 0d64 0075 0190  .d.d...}.|.d.u..
-00003910: 0172 057c 046a 0d7c 0d6a 2664 1a8d 0101  .r.|.j.|.j&d....
-00003920: 0074 297c 016a 2164 1b69 0083 037d 0e7c  .t)|.j!d.i...}.|
-00003930: 0e90 0172 1c7c 046a 0d64 1c64 1d84 007c  ...r.|.j.d.d...|
-00003940: 0ea0 2aa1 0044 0083 0164 1e8d 0101 0074  ..*..D...d.....t
-00003950: 106a 11a0 2b64 1fa1 0190 0172 3f74 297c  .j..+d.....r?t)|
-00003960: 0164 2064 0083 0364 0075 0190 0172 3f74  .d d...d.u...r?t
-00003970: 147c 016a 2164 2183 0290 0172 3f7c 046a  .|.j!d!....r?|.j
-00003980: 0d74 2c6a 2da0 2e7c 016a 21a1 016a 2f64  .t,j-..|.j!..j/d
-00003990: 228d 0101 0064 2344 005d 177d 0f74 297c  "....d#D.].}.t)|
-000039a0: 017c 0f64 0083 037d 107c 1064 0075 0190  .|.d...}.|.d.u..
-000039b0: 0172 577c 04a0 0d7c 0f7c 106a 306a 3169  .rW|...|.|.j0j1i
-000039c0: 01a1 0101 0090 0171 417c 016a 3264 0075  .......qA|.j2d.u
-000039d0: 0190 0172 7d7c 046a 0d7c 016a 326a 2664  ...r}|.j.|.j2j&d
-000039e0: 2464 2584 007c 016a 326a 336a 3444 0083  $d%..|.j2j3j4D..
-000039f0: 0164 268d 0201 0074 147c 0164 2783 0290  .d&....t.|.d'...
-00003a00: 0172 7d7c 046a 0d7c 016a 3564 288d 0101  .r}|.j.|.j5d(...
-00003a10: 007c 0453 0029 294e 2905 da02 6964 722f  .|.S.))N)...idr/
-00003a20: 0100 0072 9500 0000 da05 736c 6176 65da  ...r......slave.
-00003a30: 0865 6469 7461 626c 6529 0172 3001 0000  .editable).r0...
-00003a40: 7a0f 2573 2068 6173 206e 6f20 7374 6f72  z.%s has no stor
-00003a50: 65da 0b67 6574 5f63 6f6c 756d 6e73 7201  e..get_columnsr.
-00003a60: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00003a70: 0100 0000 0100 0000 5300 0000 7306 0000  ........S...s...
-00003a80: 007c 006a 0053 0072 3a00 0000 a901 7252  .|.j.S.r:.....rR
-00003a90: 0000 00a9 0172 8c00 0000 7236 0000 0072  .....r....r6...r
-00003aa0: 3600 0000 7237 0000 0072 3701 0000 6f02  6...r7...r7...o.
-00003ab0: 0000 7302 0000 0006 007a 2552 656e 6465  ..s......z%Rende
-00003ac0: 7265 722e 6163 746f 7232 6a73 6f6e 2e3c  rer.actor2json.<
-00003ad0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00003ae0: 7238 0100 0029 01da 0c66 6965 6c64 735f  r8...)...fields_
-00003af0: 696e 6465 7872 4401 0000 722c 0000 0029  indexrD...r,...)
-00003b00: 01da 1366 6965 6c64 735f 696e 6465 785f  ...fields_index_
-00003b10: 6869 6464 656e e902 0000 00da 0363 6f6c  hidden.......col
-00003b20: da08 706b 5f69 6e64 6578 7ad0 7072 6576  ..pk_indexz.prev
-00003b30: 6965 775f 6c69 6d69 7420 7573 655f 6465  iew_limit use_de
-00003b40: 7461 696c 5f70 6172 616d 5f70 616e 656c  tail_param_panel
-00003b50: 2075 7365 5f64 6574 6169 6c5f 7061 7261   use_detail_para
-00003b60: 6d73 5f76 616c 7565 2068 6964 655f 6e61  ms_value hide_na
-00003b70: 7669 6761 746f 7220 7573 655f 6465 7461  vigator use_deta
-00003b80: 696c 5f70 6172 616d 735f 7661 6c75 6520  il_params_value 
-00003b90: 7265 6163 745f 7265 7370 6f6e 7369 7665  react_responsive
-00003ba0: 206d 6178 5f72 656e 6465 725f 6465 7074   max_render_dept
-00003bb0: 6820 7369 6d70 6c65 5f73 6c61 7665 6772  h simple_slavegr
-00003bc0: 6964 5f68 6561 6465 7220 7061 6769 6e61  id_header pagina
-00003bd0: 746f 725f 7465 6d70 6c61 7465 2068 6964  tor_template hid
-00003be0: 655f 746f 705f 746f 6f6c 6261 7220 6869  e_top_toolbar hi
-00003bf0: 6465 5f69 665f 656d 7074 7920 da04 6669  de_if_empty ..fi
-00003c00: 6c65 5429 01da 0d63 6f6e 7461 696e 5f6d  leT)...contain_m
-00003c10: 6564 6961 723a 0100 0072 2301 0000 2901  ediar:...r#...).
-00003c20: da0d 6163 7469 7665 5f66 6965 6c64 73da  ..active_fields.
-00003c30: 0b63 6172 645f 6c61 796f 7574 2901 724c  .card_layout).rL
-00003c40: 0100 00da 0b6c 6973 745f 6c61 796f 7574  .....list_layout
-00003c50: 2901 724d 0100 00da 0e5f 6368 6f6f 7365  ).rM....._choose
-00003c60: 7273 5f64 6963 7463 0100 0000 0000 0000  rs_dictc........
-00003c70: 0000 0000 0300 0000 0500 0000 5300 0000  ............S...
-00003c80: 7322 0000 0069 007c 005d 0d5c 027d 017d  s"...i.|.].\.}.}
-00003c90: 027c 0164 0064 0184 007c 026a 0044 0083  .|.d.d...|.j.D..
-00003ca0: 0193 0271 0253 0029 0263 0100 0000 0000  ...q.S.).c......
-00003cb0: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
-00003cc0: 0000 f312 0000 0067 007c 005d 057d 017c  .......g.|.].}.|
-00003cd0: 016a 0091 0271 0253 0072 3600 0000 7242  .j...q.S.r6...rB
-00003ce0: 0100 0029 0272 4600 0000 da02 6366 7236  ...).rF.....cfr6
-00003cf0: 0000 0072 3600 0000 7237 0000 0072 4800  ...r6...r7...rH.
-00003d00: 0000 a502 0000 f302 0000 0012 007a 3252  .............z2R
-00003d10: 656e 6465 7265 722e 6163 746f 7232 6a73  enderer.actor2js
-00003d20: 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  on.<locals>.<dic
-00003d30: 7463 6f6d 703e 2e3c 6c69 7374 636f 6d70  tcomp>.<listcomp
-00003d40: 3e29 01da 0e63 6f6e 7465 7874 5f66 6965  >)...context_fie
-00003d50: 6c64 7329 0372 4600 0000 da02 666e 7247  lds).rF.....fnrG
-00003d60: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00003d70: 0000 724c 0000 00a5 0200 0073 0600 0000  ..rL.......s....
-00003d80: 0600 0601 16ff 7a27 5265 6e64 6572 6572  ......z'Renderer
-00003d90: 2e61 6374 6f72 326a 736f 6e2e 3c6c 6f63  .actor2json.<loc
-00003da0: 616c 733e 2e3c 6469 6374 636f 6d70 3e29  als>.<dictcomp>)
-00003db0: 01da 0c63 686f 6f73 6572 5f64 6963 74da  ...chooser_dict.
-00003dc0: 0c63 6f6e 7465 6e74 7479 7065 73da 056d  .contenttypes..m
-00003dd0: 6f64 656c da05 5f6d 6574 6129 01da 0c63  odel.._meta)...c
-00003de0: 6f6e 7465 6e74 5f74 7970 6529 03da 0d64  ontent_type)...d
-00003df0: 6574 6169 6c5f 6163 7469 6f6e da0d 696e  etail_action..in
-00003e00: 7365 7274 5f61 6374 696f 6eda 0e64 6566  sert_action..def
-00003e10: 6175 6c74 5f61 6374 696f 6e63 0100 0000  ault_actionc....
-00003e20: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00003e30: 5300 0000 724f 0100 0072 3600 0000 7242  S...rO...r6...rB
-00003e40: 0100 0029 0272 4600 0000 728c 0000 0072  ...).rF...r....r
-00003e50: 3600 0000 7236 0000 0072 3700 0000 7248  6...r6...r7...rH
-00003e60: 0000 00b5 0200 0072 5101 0000 7a27 5265  .......rQ...z'Re
-00003e70: 6e64 6572 6572 2e61 6374 6f72 326a 736f  nderer.actor2jso
-00003e80: 6e2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  n.<locals>.<list
-00003e90: 636f 6d70 3e29 02da 0d70 6172 616d 735f  comp>)...params_
-00003ea0: 6c61 796f 7574 da0d 7061 7261 6d73 5f66  layout..params_f
-00003eb0: 6965 6c64 73da 1070 6172 616d 735f 7061  ields..params_pa
-00003ec0: 6e65 6c5f 706f 7329 0172 5e01 0000 2936  nel_pos).r^...)6
-00003ed0: 722b 0000 0072 b400 0000 721b 0000 0072  r+...r....r....r
-00003ee0: 3601 0000 da0d 5f61 6374 696f 6e73 5f6c  6....._actions_l
-00003ef0: 6973 7472 7100 0000 72ef 0000 00da 0f67  istrq...r......g
-00003f00: 6574 5f61 6374 6f72 5f6c 6162 656c da04  et_actor_label..
-00003f10: 626f 6f6c da06 6d61 7374 6572 da0c 6869  bool..master..hi
-00003f20: 6465 5f65 6469 7469 6e67 7229 0000 0072  de_editingr)...r
-00003f30: d100 0000 7277 0000 00da 0a67 6574 5f68  ....rw.....get_h
-00003f40: 616e 646c 65da 0573 746f 7265 7204 0000  andle..storer...
-00003f50: 0072 6f00 0000 da06 6c6f 6767 6572 da07  .ro.....logger..
-00003f60: 7761 726e 696e 6772 8200 0000 7241 0100  warningr....rA..
-00003f70: 0072 aa00 0000 7238 0000 00da 0b6c 6973  .r....r8.....lis
-00003f80: 745f 6669 656c 6473 72b6 0000 0072 5200  t_fieldsr....rR.
-00003f90: 0000 72a0 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00003fa0: 0072 2200 0000 722c 0100 0072 2800 0000  .r"...r,...r(...
-00003fb0: 7256 0100 0072 3a01 0000 723d 0100 0072  rV...r:...r=...r
-00003fc0: 5901 0000 da11 6765 745f 7769 6e64 6f77  Y.....get_window
-00003fd0: 5f6c 6179 6f75 7472 8700 0000 724b 0100  _layoutr....rK..
-00003fe0: 0072 7800 0000 7201 0100 0072 6800 0000  .rx...r....rh...
-00003ff0: 7276 0000 0072 0e00 0000 da07 6f62 6a65  rv...r......obje
-00004000: 6374 73da 0d67 6574 5f66 6f72 5f6d 6f64  cts..get_for_mod
-00004010: 656c 72d8 0000 0072 6c00 0000 724d 0000  elr....rl...rM..
-00004020: 0072 5c01 0000 da0c 7061 7261 6d73 5f73  .r\.....params_s
-00004030: 746f 7265 da0c 7061 7261 6d5f 6669 656c  tore..param_fiel
-00004040: 6473 725e 0100 0029 1172 3f00 0000 72a5  dsr^...).r?...r.
-00004050: 0000 00da 0261 6cda 0268 6b72 a600 0000  .....al..hkr....
-00004060: da02 6168 da07 636f 6c75 6d6e 73da 0969  ..ah..columns..i
-00004070: 6e64 6578 5f6d 6f64 da09 636f 6c5f 656c  ndex_mod..col_el
-00004080: 656d 7372 4701 0000 720b 0100 00da 0277  emsrG...r......w
-00004090: 6c72 4c01 0000 724d 0100 0072 5401 0000  lrL...rM...rT...
-000040a0: 72b7 0000 0072 8f00 0000 7236 0000 0072  r....r....r6...r
-000040b0: 3600 0000 7237 0000 00da 0a61 6374 6f72  6...r7.....actor
-000040c0: 326a 736f 6e56 0200 0073 8e00 0000 1601  2jsonV...s......
-000040d0: 1001 0601 0201 0601 0801 0c01 06fc 0807  ................
-000040e0: 0c01 0802 0a01 1201 0a03 0401 0401 0801  ................
-000040f0: 0801 0a01 1201 0601 04ff 0201 08ff 1402  ................
-00004100: 1403 0801 0a01 0801 0c01 0801 1205 1001  ................
-00004110: 0c0d 0c01 0a02 1001 0a02 0a01 0801 0e01  ................
-00004120: 0602 1201 0c02 0801 0e01 0c02 0a01 0e02  ................
-00004130: 0e03 0601 0a01 0601 0aff 2603 0201 06ff  ..........&.....
-00004140: 1803 0801 0c01 0a01 1201 0480 0c02 0402  ................
-00004150: 0601 1201 06fe 0c04 0e01 0401 7a13 5265  ............z.Re
-00004160: 6e64 6572 6572 2e61 6374 6f72 326a 736f  nderer.actor2jso
-00004170: 6e63 0200 0000 0000 0000 0000 0000 0400  nc..............
-00004180: 0000 0600 0000 0300 0000 7364 0000 0064  ..........sd...d
-00004190: 0188 015f 0088 016a 0144 005d 2289 0088  ..._...j.D.]"...
-000041a0: 006a 0264 0075 0172 0e71 0674 036a 046a  .j.d.u.r.q.t.j.j
-000041b0: 0588 01a0 0688 006a 07a1 018e 007d 0287  .......j.....}..
-000041c0: 0087 0166 0264 0264 0384 087d 0374 086a  ...f.d.d...}.t.j
-000041d0: 096a 0aa0 0b7c 027c 037c 01a1 0301 0071  .j...|.|.|.....q
-000041e0: 0664 0488 015f 0074 0c83 00a0 0d7c 01a1  .d..._.t.....|..
-000041f0: 0153 0029 054e 5463 0100 0000 0000 0000  .S.).NTc........
-00004200: 0000 0000 0100 0000 0600 0000 1300 0000  ................
-00004210: 7318 0000 007c 00a0 0074 0188 01a0 0288  s....|...t......
-00004220: 00a1 0183 01a1 0101 0064 0053 0072 3a00  .........d.S.r:.
-00004230: 0000 2903 728b 0000 0072 2600 0000 7275  ..).r....r&...ru
-00004240: 0100 0072 4301 0000 a902 7298 0000 0072  ...rC.....r....r
-00004250: 3f00 0000 7236 0000 0072 3700 0000 728b  ?...r6...r7...r.
-00004260: 0000 00c4 0200 0073 0200 0000 1801 7a26  .......s......z&
-00004270: 5265 6e64 6572 6572 2e62 7569 6c64 5f6a  Renderer.build_j
-00004280: 735f 6361 6368 652e 3c6c 6f63 616c 733e  s_cache.<locals>
-00004290: 2e77 7269 7465 4629 0e72 6e00 0000 726a  .writeF).rn...rj
-000042a0: 0000 00da 0f67 6574 5f68 616e 646c 655f  .....get_handle_
-000042b0: 6e61 6d65 727d 0000 00da 0470 6174 68da  namer}.....path.
-000042c0: 046a 6f69 6e72 2201 0000 72ef 0000 0072  .joinr"...r....r
-000042d0: 0400 0000 726f 0000 0072 2300 0000 da0f  ....ro...r#.....
-000042e0: 6d61 6b65 5f63 6163 6865 5f66 696c 6572  make_cache_filer
-000042f0: 3b00 0000 da0e 6275 696c 645f 6a73 5f63  ;.....build_js_c
-00004300: 6163 6865 2904 723f 0000 00da 0566 6f72  ache).r?.....for
-00004310: 6365 7253 0100 0072 8b00 0000 7241 0000  cerS...r....rA..
-00004320: 0072 7601 0000 7237 0000 0072 7b01 0000  .rv...r7...r{...
-00004330: bb02 0000 7312 0000 0006 020a 020a 0102  ....s...........
-00004340: 0114 010e 0214 0306 020c 017a 1752 656e  ...........z.Ren
-00004350: 6465 7265 722e 6275 696c 645f 6a73 5f63  derer.build_js_c
-00004360: 6163 6865 723a 0000 0029 2072 b300 0000  acher:...) r....
-00004370: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00004380: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00004390: 635f 5fda 0e69 735f 696e 7465 7261 6374  c__..is_interact
-000043a0: 6976 65da 0863 616e 5f61 7574 6872 1d01  ive..can_authr..
-000043b0: 0000 7221 0100 00da 1873 7570 706f 7274  ..r!.....support
-000043c0: 5f64 6173 6862 6f61 7264 5f6c 6179 6f75  _dashboard_layou
-000043d0: 7472 3c00 0000 7293 0000 0072 4e00 0000  tr<...r....rN...
-000043e0: 7286 0000 0072 aa00 0000 72b8 0000 0072  r....r....r....r
-000043f0: ce00 0000 72db 0000 0072 e200 0000 72a4  ....r....r....r.
-00004400: 0000 0072 de00 0000 723e 0000 0072 fd00  ...r....r>...r..
-00004410: 0000 72fe 0000 0072 ff00 0000 7213 0100  ..r....r....r...
-00004420: 0072 1901 0000 7222 0100 0072 3601 0000  .r....r"...r6...
-00004430: 723d 0100 0072 7501 0000 727b 0100 00da  r=...ru...r{....
-00004440: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7236  .__classcell__r6
-00004450: 0000 0072 3600 0000 7241 0000 0072 3700  ...r6...rA...r7.
-00004460: 0000 7239 0000 003a 0000 0073 3c00 0000  ..r9...:...s<...
-00004470: 0800 0401 0403 0401 0402 0401 0401 0c02  ................
-00004480: 0804 0855 081d 0808 081f 0803 0a18 0212  ...U............
-00004490: 0aff 0815 080e 0821 0851 080e 080a 0829  .......!.Q.....)
-000044a0: 0809 080f 080a 0844 080c 1465 7239 0000  .......D...er9..
-000044b0: 0072 3a00 0000 2946 727d 0000 00da 0770  .r:...)Fr}.....p
-000044c0: 6174 686c 6962 7202 0000 00da 0468 746d  athlibr......htm
-000044d0: 6c72 0300 0000 da0b 646a 616e 676f 2e63  lr......django.c
-000044e0: 6f6e 6672 0400 0000 da09 646a 616e 676f  onfr......django
-000044f0: 2e64 6272 0500 0000 da11 646a 616e 676f  .dbr......django
-00004500: 2e75 7469 6c73 2e74 6578 7472 0600 0000  .utils.textr....
-00004510: da0c 646a 616e 676f 2e75 7469 6c73 7207  ..django.utilsr.
-00004520: 0000 00da 126c 696e 6f2e 636f 7265 2e72  .....lino.core.r
-00004530: 656e 6465 7265 7272 0800 0000 7209 0000  endererr....r...
-00004540: 00da 0f6c 696e 6f2e 636f 7265 2e6d 656e  ...lino.core.men
-00004550: 7573 720a 0000 0072 0b00 0000 da09 6c69  usr....r......li
-00004560: 6e6f 2e63 6f72 6572 0c00 0000 720d 0000  no.corer....r...
-00004570: 00da 0e6c 696e 6f2e 636f 7265 2e67 666b  ...lino.core.gfk
-00004580: 7372 0e00 0000 da1e 6c69 6e6f 2e6d 6f64  sr......lino.mod
-00004590: 6c69 622e 6578 746a 732e 6578 745f 7265  lib.extjs.ext_re
-000045a0: 6e64 6572 6572 720f 0000 00da 116c 696e  ndererr......lin
-000045b0: 6f2e 636f 7265 2e61 6374 696f 6e73 7210  o.core.actionsr.
-000045c0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-000045d0: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000045e0: 0072 1700 0000 da15 6c69 6e6f 2e63 6f72  .r......lino.cor
-000045f0: 652e 626f 756e 6461 6374 696f 6e72 1800  e.boundactionr..
-00004600: 0000 da15 6c69 6e6f 2e63 6f72 652e 6368  ....lino.core.ch
-00004610: 6f69 6365 6c69 7374 7372 1900 0000 da1e  oicelistsr......
-00004620: 6c69 6e6f 2e6d 6f64 6c69 622e 7379 7374  lino.modlib.syst
-00004630: 656d 2e63 686f 6963 656c 6973 7473 721a  em.choicelistsr.
-00004640: 0000 00da 106c 696e 6f2e 636f 7265 2e61  .....lino.core.a
-00004650: 6374 6f72 7372 1b00 0000 da11 6c69 6e6f  ctorsr......lino
-00004660: 2e63 6f72 652e 6c61 796f 7574 7372 1c00  .core.layoutsr..
-00004670: 0000 721d 0000 00da 0f6c 696e 6f2e 636f  ..r......lino.co
-00004680: 7265 2e65 6c65 6d73 721e 0000 0072 1f00  re.elemsr....r..
-00004690: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-000046a0: 0072 2300 0000 da0a 6574 6765 6e2e 6874  .r#.....etgen.ht
-000046b0: 6d6c 7224 0000 00da 0a6c 696e 6f2e 7574  mlr$.....lino.ut
-000046c0: 696c 7372 2500 0000 da10 6c69 6e6f 2e75  ilsr%.....lino.u
-000046d0: 7469 6c73 2e6a 7367 656e 7226 0000 0072  tils.jsgenr&...r
-000046e0: 2700 0000 7228 0000 00da 176c 696e 6f2e  '...r(.....lino.
-000046f0: 6d6f 646c 6962 2e75 7365 7273 2e75 7469  modlib.users.uti
-00004700: 6c73 7229 0000 0072 2a00 0000 da07 696e  lsr)...r*.....in
-00004710: 7370 6563 7472 2b00 0000 da05 6963 6f6e  spectr+.....icon
-00004720: 7372 2d00 0000 7238 0000 0072 3900 0000  sr-...r8...r9...
-00004730: 7236 0000 0072 3600 0000 7236 0000 0072  r6...r6...r6...r
-00004740: 3700 0000 da08 3c6d 6f64 756c 653e 0100  7.....<module>..
-00004750: 0000 733a 0000 0008 040c 010c 010c 010c  ..s:............
-00004760: 010c 010c 0110 0210 020c 010c 010c 010c  ................
-00004770: 0128 020c 030c 010c 010c 0110 011c 010c  .(..............
-00004780: 020c 020c 0214 0110 020c 020c 020a 0314  ................
-00004790: 0d                                       .
+00000590: fa45 2f68 6f6d 652f 626c 7572 7279 2f6c  .E/home/blurry/l
+000005a0: 696e 6f2f 656e 762f 7265 706f 7369 746f  ino/env/reposito
+000005b0: 7269 6573 2f72 6561 6374 2f6c 696e 6f5f  ries/react/lino_
+000005c0: 7265 6163 742f 7265 6163 742f 7265 6e64  react/react/rend
+000005d0: 6572 6572 2e70 79da 0466 696e 642d 0000  erer.py..find-..
+000005e0: 0073 1000 0000 1802 1002 0401 0801 0801  .s..............
+000005f0: 0801 02ff 0403 7238 0000 0063 0000 0000  ......r8...c....
+00000600: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000610: 0000 0000 73e6 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00000620: 0264 015a 0364 025a 0464 025a 0564 035a  .d.Z.d.Z.d.Z.d.Z
+00000630: 0664 045a 0764 025a 0887 0066 0164 0564  .d.Z.d.Z...f.d.d
+00000640: 0684 085a 0964 0764 0884 005a 0a64 0964  ...Z.d.d...Z.d.d
+00000650: 0a84 005a 0b64 0b64 0c84 005a 0c64 0d64  ...Z.d.d...Z.d.d
+00000660: 0e84 005a 0d64 0f64 1084 005a 0e64 1164  ...Z.d.d...Z.d.d
+00000670: 1284 005a 0f64 3264 1464 1584 015a 1069  ...Z.d2d.d...Z.i
+00000680: 0066 0164 1664 1784 015a 1164 1864 1984  .f.d.d...Z.d.d..
+00000690: 005a 1264 1a64 1b84 005a 1364 1c64 1d84  .Z.d.d...Z.d.d..
+000006a0: 005a 1464 1e64 1f84 005a 1564 2064 2184  .Z.d.d...Z.d d!.
+000006b0: 005a 1664 2264 2384 005a 1764 2464 2584  .Z.d"d#..Z.d$d%.
+000006c0: 005a 1864 2664 2784 005a 1964 2864 2984  .Z.d&d'..Z.d(d).
+000006d0: 005a 1a64 2a64 2b84 005a 1b64 2c64 2d84  .Z.d*d+..Z.d,d-.
+000006e0: 005a 1c64 2e64 2f84 005a 1d87 0066 0164  .Z.d.d/..Z...f.d
+000006f0: 3064 3184 085a 1e87 0004 005a 1f53 0029  0d1..Z.....Z.S.)
+00000700: 33da 0852 656e 6465 7265 727a 480a 2020  3..RendererzH.  
+00000710: 2020 4120 6672 6f6e 742d 656e 6420 7265    A front-end re
+00000720: 6e64 6572 6572 2074 6861 7420 7573 6573  nderer that uses
+00000730: 2074 6865 2052 6561 6374 204a 6176 6173   the React Javas
+00000740: 6372 6970 7420 6672 616d 6577 6f72 6b2e  cript framework.
+00000750: 0a20 2020 2054 7a12 7265 6163 742f 6c69  .    Tz.react/li
+00000760: 6e6f 7765 622e 6a73 6f6e 7a05 2e6a 736f  noweb.jsonz..jso
+00000770: 6e63 0200 0000 0000 0000 0000 0000 0200  nc..............
+00000780: 0000 0300 0000 0300 0000 731c 0000 0074  ..........s....t
+00000790: 0083 00a0 017c 01a1 0101 0074 02a0 037c  .....|.....t...|
+000007a0: 006a 04a1 0101 0064 0053 00a9 014e 2905  .j.....d.S...N).
+000007b0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+000007c0: 5f72 2500 0000 da12 7265 6769 7374 6572  _r%.....register
+000007d0: 5f63 6f6e 7665 7274 6572 da0f 7079 326a  _converter..py2j
+000007e0: 735f 636f 6e76 6572 7465 7229 02da 0473  s_converter)...s
+000007f0: 656c 66da 0966 726f 6e74 5f65 6e64 a901  elf..front_end..
+00000800: da09 5f5f 636c 6173 735f 5f72 3600 0000  ..__class__r6...
+00000810: 7237 0000 0072 3c00 0000 4500 0000 7304  r7...r<...E...s.
+00000820: 0000 000c 0110 017a 1152 656e 6465 7265  .......z.Rendere
+00000830: 722e 5f5f 696e 6974 5f5f 6302 0000 0000  r.__init__c.....
+00000840: 0000 0000 0000 000c 0000 0008 0000 0003  ................
+00000850: 0000 0073 7202 0000 6401 6402 8400 7400  ...sr...d.d...t.
+00000860: 6a01 a002 a100 4400 8301 7d02 7403 8300  j.....D...}.t...
+00000870: 7d03 8800 6a04 4400 5d14 7d04 7c04 a005  }...j.D.].}.|...
+00000880: a100 4400 5d0d 7d05 7c05 6a06 7c03 7601  ..D.].}.|.j.|.v.
+00000890: 7223 7c03 a007 7c05 6a06 a101 0100 7116  r#|...|.j.....q.
+000008a0: 7110 6403 8800 5f08 7409 6a0a 6a0b 7d06  q.d..._.t.j.j.}.
+000008b0: 740c 8700 6601 6404 6402 8408 7c03 4400  t...f.d.d...|.D.
+000008c0: 8301 7409 6a0a a00d 740e 8300 a101 7c06  ..t.j...t.....|.
+000008d0: 6a0f 6a10 7409 6a0a 6a11 8800 6a12 6a13  j.j.t.j.j...j.j.
+000008e0: 6405 7501 6406 6402 8400 7409 6a0a 6a14  d.u.d.d...t.j.j.
+000008f0: 4400 8301 6407 8d06 7d07 7409 6a0a a015  D...d...}.t.j...
+00000900: 6408 a101 7264 7c07 6a16 7417 7c06 6a18  d...rd|.j.t.|.j.
+00000910: 6a19 6a1a a01b a100 8301 6409 8d01 0100  j.j.......d.....
+00000920: 7c07 6a16 7409 6a0a 6a00 6a1c 640a 8d01  |.j.t.j.j.j.d...
+00000930: 0100 7a13 7c07 6a16 741d a01e 741f 7409  ..z.|.j.t...t.t.
+00000940: 6a20 8301 640b 1b00 640c 1b00 a101 6a21  j ..d...d.....j!
+00000950: 640d 8d01 0100 5700 6e09 0400 7422 7989  d.....W.n...t"y.
+00000960: 0100 0100 0100 5900 6e01 7700 7423 7409  ......Y.n.w.t#t.
+00000970: 6a0a 640e 8302 7298 7c07 6a16 7409 6a0a  j.d...r.|.j.t.j.
+00000980: 6a24 640f 8d01 0100 7409 6a0a 6a25 6405  j$d.....t.j.j%d.
+00000990: 6b02 72a5 7c07 6a16 6403 6410 8d01 0100  k.r.|.j.d.d.....
+000009a0: 6e0e 7423 7c06 6a26 6411 8302 72b3 7c07  n.t#|.j&d...r.|.
+000009b0: 6a16 7c06 6a26 6a27 6412 8d01 0100 7409  j.|.j&j'd.....t.
+000009c0: 6a0a a015 6413 a101 72c5 7c07 6a16 7c06  j...d...r.|.j.|.
+000009d0: 6a28 6a29 6fc2 7409 6a0a 6a2a 6414 8d01  j(j)o.t.j.j*d...
+000009e0: 0100 6900 7d08 8800 6a2b 4400 5d2f 7d09  ..i.}...j+D.]/}.
+000009f0: 8800 a02c 7c09 a101 7c08 7c09 6a2d 3c00  ...,|...|.|.j-<.
+00000a00: 7423 7c09 6415 8302 72f9 6416 7c09 6a2d  t#|.d...r.d.|.j-
+00000a10: 7600 72f9 742e 7c02 6417 1900 8301 4400  v.r.t.|.d.....D.
+00000a20: 5d14 5c02 7d0a 7d0b 7c0b 6418 1900 7c09  ].\.}.}.|.d...|.
+00000a30: 6a2f 6b02 72f8 7c09 6a2d 7c02 6417 1900  j/k.r.|.j-|.d...
+00000a40: 7c0a 1900 6419 3c00 71e4 71ca 8800 6a30  |...d.<.q.q...j0
+00000a50: 4400 5d0a 7d09 8800 a02c 7c09 a101 7c08  D.].}....,|...|.
+00000a60: 7c09 6a2d 3c00 71fd 8800 6a31 4400 5d0b  |.j-<.q...j1D.].
+00000a70: 7d09 8800 a02c 7c09 a101 7c08 7c09 6a2d  }....,|...|.|.j-
+00000a80: 3c00 9001 710b 8800 6a32 4400 5d0b 7d09  <...q...j2D.].}.
+00000a90: 8800 a02c 7c09 a101 7c08 7c09 6a2d 3c00  ...,|...|.|.j-<.
+00000aa0: 9001 711a 7c07 6a16 7c08 7c02 641a 8d02  ..q.|.j.|.|.d...
+00000ab0: 0100 7c01 a033 7434 7c07 8301 a101 0100  ..|..3t4|.......
+00000ac0: 641b 8800 5f08 641c 5300 291d 7a86 0a20  d..._.d.S.).z.. 
+00000ad0: 2020 2020 2020 2043 7265 6174 6573 2077         Creates w
+00000ae0: 6861 7420 6973 206b 6e6f 776e 2061 7320  hat is known as 
+00000af0: 7769 6e64 6f77 2e41 7070 2e73 7461 7465  window.App.state
+00000b00: 2e73 6974 655f 6461 7461 2069 6e20 5265  .site_data in Re
+00000b10: 6163 7420 636f 6465 2e0a 0a20 2020 2020  act code...     
+00000b20: 2020 203a 7061 7261 6d20 663a 2046 696c     :param f: Fil
+00000b30: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00000b40: 203a 7265 7475 726e 3a20 310a 2020 2020   :return: 1.    
+00000b50: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+00000b60: 0003 0000 0006 0000 0053 0000 0073 2400  .........S...s$.
+00000b70: 0000 6900 7c00 5d0e 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+00000b80: 6400 6401 8400 7c02 a000 a100 4400 8301  d.d...|.....D...
+00000b90: 9302 7102 5300 2902 6301 0000 0000 0000  ..q.S.).c.......
+00000ba0: 0000 0000 0002 0000 0006 0000 0053 0000  .............S..
+00000bb0: 0073 2400 0000 6700 7c00 5d0e 7d01 7c01  .s$...g.|.].}.|.
+00000bc0: 6400 1900 6a00 7401 7c01 6401 1900 8301  d...j.t.|.d.....
+00000bd0: 6402 9c02 9102 7102 5300 2903 7201 0000  d.....q.S.).r...
+00000be0: 0072 2c00 0000 2902 da05 7661 6c75 65da  .r,...)...value.
+00000bf0: 0474 6578 7429 0272 4300 0000 da03 7374  .text).rC.....st
+00000c00: 7229 02da 022e 30da 0163 7236 0000 0072  r)....0..cr6...r
+00000c10: 3600 0000 7237 0000 00da 0a3c 6c69 7374  6...r7.....<list
+00000c20: 636f 6d70 3e52 0000 0073 0200 0000 2400  comp>R...s....$.
+00000c30: 7a35 5265 6e64 6572 6572 2e77 7269 7465  z5Renderer.write
+00000c40: 5f6c 696e 6f5f 6a73 2e3c 6c6f 6361 6c73  _lino_js.<locals
+00000c50: 3e2e 3c64 6963 7463 6f6d 703e 2e3c 6c69  >.<dictcomp>.<li
+00000c60: 7374 636f 6d70 3e29 01da 0b67 6574 5f63  stcomp>)...get_c
+00000c70: 686f 6963 6573 2903 7246 0000 00da 0249  hoices).rF.....I
+00000c80: 44da 0263 6c72 3600 0000 7236 0000 0072  D..clr6...r6...r
+00000c90: 3700 0000 da0a 3c64 6963 7463 6f6d 703e  7.....<dictcomp>
+00000ca0: 5000 0000 7308 0000 0006 0006 0312 ff06  P...s...........
+00000cb0: fe7a 2a52 656e 6465 7265 722e 7772 6974  .z*Renderer.writ
+00000cc0: 655f 6c69 6e6f 5f6a 732e 3c6c 6f63 616c  e_lino_js.<local
+00000cd0: 733e 2e3c 6469 6374 636f 6d70 3e54 6301  s>.<dictcomp>Tc.
+00000ce0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00000cf0: 0000 0013 0000 0073 1a00 0000 6900 7c00  .......s....i.|.
+00000d00: 5d09 7d01 7c01 6a00 8800 a001 7c01 a101  ].}.|.j.....|...
+00000d10: 9302 7102 5300 7236 0000 0029 02da 0b61  ..q.S.r6...)...a
+00000d20: 6374 696f 6e5f 6e61 6d65 da0b 6163 7469  ction_name..acti
+00000d30: 6f6e 326a 736f 6e29 0272 4600 0000 da01  on2json).rF.....
+00000d40: 61a9 0172 3f00 0000 7236 0000 0072 3700  a..r?...r6...r7.
+00000d50: 0000 724c 0000 005f 0000 0073 0200 0000  ..rL..._...s....
+00000d60: 1a00 4e63 0100 0000 0000 0000 0000 0000  ..Nc............
+00000d70: 0200 0000 0400 0000 5300 0000 7316 0000  ........S...s...
+00000d80: 0069 007c 005d 077d 017c 016a 007c 016a  .i.|.].}.|.j.|.j
+00000d90: 0193 0271 0253 0072 3600 0000 2902 da0b  ...q.S.r6...)...
+00000da0: 646a 616e 676f 5f63 6f64 65da 046e 616d  django_code..nam
+00000db0: 6529 0272 4600 0000 da04 6c61 6e67 7236  e).rF.....langr6
+00000dc0: 0000 0072 3600 0000 7237 0000 0072 4c00  ...r6...r7...rL.
+00000dd0: 0000 6500 0000 7302 0000 0016 0029 06da  ..e...s......)..
+00000de0: 0761 6374 696f 6e73 da04 6d65 6e75 da15  .actions..menu..
+00000df0: 7573 655f 6461 7368 626f 6172 645f 6c61  use_dashboard_la
+00000e00: 796f 7574 73da 0a73 6974 655f 7469 746c  youts..site_titl
+00000e10: 65da 1065 6469 7469 6e67 5f66 726f 6e74  e..editing_front
+00000e20: 656e 64da 096c 616e 6775 6167 6573 da04  end..languages..
+00000e30: 6d65 6d6f 2901 da0a 7375 6767 6573 746f  memo)...suggesto
+00000e40: 7273 2901 da0f 7265 7669 7369 6f6e 5f6e  rs)...revision_n
+00000e50: 756d 6265 72da 0572 6561 6374 7a07 6d61  umber..reactz.ma
+00000e60: 696e 2e6a 7329 01da 0d6d 6a73 5f74 696d  in.js)...mjs_tim
+00000e70: 6573 7461 6d70 da0a 7468 656d 655f 6e61  estamp..theme_na
+00000e80: 6d65 2901 725f 0000 0029 01da 0d6e 6f5f  me).r_...)...no_
+00000e90: 7573 6572 5f6d 6f64 656c da19 616c 6c6f  user_model..allo
+00000ea0: 775f 6f6e 6c69 6e65 5f72 6567 6973 7472  w_online_registr
+00000eb0: 6174 696f 6e29 0172 6100 0000 da06 6e6f  ation).ra.....no
+00000ec0: 7469 6679 2901 da0c 7573 655f 7075 7368  tify)...use_push
+00000ed0: 5f61 7069 da0b 6368 6f69 6365 5f6e 616d  _api..choice_nam
+00000ee0: 657a 1073 7973 7465 6d2e 4461 7368 626f  ez.system.Dashbo
+00000ef0: 6172 647a 1773 7973 7465 6d2e 4461 7368  ardz.system.Dash
+00000f00: 626f 6172 644c 6179 6f75 7473 7243 0000  boardLayoutsrC..
+00000f10: 00da 0d77 696e 646f 775f 6c61 796f 7574  ...window_layout
+00000f20: 2902 da0b 666f 726d 5f70 616e 656c 7372  )...form_panelsr
+00000f30: 0d00 0000 4672 2c00 0000 2935 7223 0000  ....Fr,...)5r#..
+00000f40: 00da 0b43 484f 4943 454c 4953 5453 da05  ...CHOICELISTS..
+00000f50: 6974 656d 73da 0373 6574 da0b 6163 746f  items..set..acto
+00000f60: 7273 5f6c 6973 74da 0b67 6574 5f61 6374  rs_list..get_act
+00000f70: 696f 6e73 da06 6163 7469 6f6e da03 6164  ions..action..ad
+00000f80: 64da 1173 6572 6961 6c69 7365 5f6a 735f  d..serialise_js_
+00000f90: 636f 6465 7204 0000 00da 0453 4954 45da  coder......SITE.
+00000fa0: 0770 6c75 6769 6e73 da04 6469 6374 da0d  .plugins..dict..
+00000fb0: 6765 745f 7369 7465 5f6d 656e 7572 2900  get_site_menur).
+00000fc0: 0000 da06 7379 7374 656d 7256 0000 00da  ....systemrV....
+00000fd0: 0574 6974 6c65 7240 0000 00da 0a75 726c  .titler@.....url
+00000fe0: 5f70 7265 6669 7872 5900 0000 da0c 6973  _prefixrY.....is
+00000ff0: 5f69 6e73 7461 6c6c 6564 da06 7570 6461  _installed..upda
+00001000: 7465 da04 6c69 7374 725a 0000 00da 0670  te..listrZ.....p
+00001010: 6172 7365 72da 0a73 7567 6765 7374 6572  arser..suggester
+00001020: 73da 046b 6579 73da 0a63 6f64 655f 6d74  s..keys..code_mt
+00001030: 696d 65da 026f 73da 0473 7461 7472 0200  ime..os..statr..
+00001040: 0000 da0b 5354 4154 4943 5f52 4f4f 54da  ....STATIC_ROOT.
+00001050: 0873 745f 6d74 696d 65da 1146 696c 654e  .st_mtime..FileN
+00001060: 6f74 466f 756e 6445 7272 6f72 da07 6861  otFoundError..ha
+00001070: 7361 7474 7272 5f00 0000 da0a 7573 6572  sattrr_.....user
+00001080: 5f6d 6f64 656c da05 7573 6572 7372 6100  _model..usersra.
+00001090: 0000 7262 0000 0072 6300 0000 da09 7573  ..rb...rc.....us
+000010a0: 655f 6c69 6e6f 6472 6600 0000 da0a 7061  e_linodrf.....pa
+000010b0: 6e65 6c32 6a73 6f6e da0f 5f66 6f72 6d70  nel2json.._formp
+000010c0: 616e 656c 5f6e 616d 6572 3000 0000 7264  anel_namer0...rd
+000010d0: 0000 00da 0c70 6172 616d 5f70 616e 656c  .....param_panel
+000010e0: 73da 1361 6374 696f 6e5f 7061 7261 6d5f  s..action_param_
+000010f0: 7061 6e65 6c73 da0c 6f74 6865 725f 7061  panels..other_pa
+00001100: 6e65 6c73 da05 7772 6974 6572 2600 0000  nels..writer&...
+00001110: 290c 723f 0000 00da 0166 da10 6368 6f69  ).r?.....f..choi
+00001120: 6365 6c69 7374 735f 6461 7461 7254 0000  celists_datarT..
+00001130: 00da 0372 7074 da02 6261 7270 0000 00da  ...rpt..barp....
+00001140: 0464 6174 6172 6600 0000 da01 7072 3400  .datarf.....pr4.
+00001150: 0000 da04 6974 656d 7236 0000 0072 5000  ....itemr6...rP.
+00001160: 0000 7237 0000 00da 0d77 7269 7465 5f6c  ..r7.....write_l
+00001170: 696e 6f5f 6a73 4900 0000 7370 0000 0006  ino_jsI...sp....
+00001180: 0708 0306 fd06 050a 010c 020a 010c 0102  ................
+00001190: 8002 fe06 0408 0102 0110 010c 0206 0106  ................
+000011a0: 010a 0110 0106 f90c 0904 0210 0106 ff12  ................
+000011b0: 0602 0126 010c 0104 0102 ff0c 0310 010c  ...&............
+000011c0: 020e 010c 0110 010c 0218 0104 090a 0110  ................
+000011d0: 0114 0114 010e 0112 0104 800a 0112 010a  ................
+000011e0: 0114 010a 0114 010e 010e 0506 0204 017a  ...............z
+000011f0: 1652 656e 6465 7265 722e 7772 6974 655f  .Renderer.write_
+00001200: 6c69 6e6f 5f6a 7363 0200 0000 0000 0000  lino_jsc........
+00001210: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00001220: 73c6 0000 0074 007c 0174 0183 0273 074a  s....t.|.t...s.J
+00001230: 0082 0174 027c 016a 037c 01a0 04a1 007c  ...t.|.j.|.....|
+00001240: 01a0 05a1 007c 016a 0664 018d 047d 0274  .....|.j.d...}.t
+00001250: 007c 0174 0783 0272 297c 016a 086a 096a  .|.t...r)|.j.j.j
+00001260: 037c 0264 023c 0074 0a7c 016a 086a 0b83  .|.d.<.t.|.j.j..
+00001270: 017c 0264 033c 007c 016a 0c72 317c 016a  .|.d.<.|.j.r1|.j
+00001280: 0c7c 0264 043c 007c 016a 0d72 397c 016a  .|.d.<.|.j.r9|.j
+00001290: 0d7c 0264 053c 007c 016a 0e72 4064 067c  .|.d.<.|.j.r@d.|
+000012a0: 0264 073c 007c 016a 0f72 487c 016a 0f7c  .d.<.|.j.rH|.j.|
+000012b0: 0264 083c 007c 016a 1072 4f64 067c 0264  .d.<.|.j.rOd.|.d
+000012c0: 093c 007c 016a 1172 5664 067c 0264 0a3c  .<.|.j.rVd.|.d.<
+000012d0: 007c 00a0 127c 01a1 017d 037c 0372 617c  .|...|...}.|.ra|
+000012e0: 037c 0264 0b3c 007c 0253 0029 0c7a 3343  .|.d.<.|.S.).z3C
+000012f0: 6f6e 7665 7274 7320 676c 6f62 616c 206c  onverts global l
+00001300: 6973 7420 6f66 2061 6c6c 2061 6374 696f  ist of all actio
+00001310: 6e73 2074 6f20 6a73 6f6e 2066 6f72 6d61  ns to json forma
+00001320: 742e 2904 da02 616e da05 6c61 6265 6cda  t.)...an..label.
+00001330: 0d77 696e 646f 775f 6163 7469 6f6e da0b  .window_action..
+00001340: 6874 7470 5f6d 6574 686f 6472 9400 0000  http_methodr....
+00001350: da05 6163 746f 72da 0c70 7265 7072 6f63  ..actor..preproc
+00001360: 6573 736f 72da 0b73 656c 6563 745f 726f  essor..select_ro
+00001370: 7773 54da 1073 7562 6d69 745f 666f 726d  wsT..submit_form
+00001380: 5f64 6174 61da 0b62 7574 746f 6e5f 7465  _data..button_te
+00001390: 7874 da14 7368 6f77 5f69 6e5f 7369 6465  xt..show_in_side
+000013a0: 5f74 6f6f 6c62 6172 da0e 6e65 7665 725f  _toolbar..never_
+000013b0: 636f 6c6c 6170 7365 da04 6963 6f6e 2913  collapse..icon).
+000013c0: da0a 6973 696e 7374 616e 6365 7217 0000  ..isinstancer...
+000013d0: 0072 7100 0000 724d 0000 00da 0967 6574  .rq...rM.....get
+000013e0: 5f6c 6162 656c da10 6973 5f77 696e 646f  _label..is_windo
+000013f0: 775f 6163 7469 6f6e 7297 0000 0072 1200  w_actionr....r..
+00001400: 0000 da0c 626f 756e 645f 6163 7469 6f6e  ....bound_action
+00001410: 726c 0000 0072 4500 0000 7298 0000 0072  rl...rE...r....r
+00001420: 9900 0000 729a 0000 0072 9b00 0000 729c  ....r....r....r.
+00001430: 0000 0072 9d00 0000 729e 0000 00da 0f67  ...r....r......g
+00001440: 6574 5f61 6374 696f 6e5f 6963 6f6e 2904  et_action_icon).
+00001450: 723f 0000 00da 0176 da06 7265 7375 6c74  r?.....v..result
+00001460: 729f 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
+00001470: 3700 0000 724e 0000 009e 0000 0073 2400  7...rN.......s$.
+00001480: 0000 0e02 0604 0601 0601 0401 06fd 0a06  ................
+00001490: 0e01 1001 1002 1002 0e01 1001 0e01 0e01  ................
+000014a0: 0a02 0c01 0402 7a14 5265 6e64 6572 6572  ......z.Renderer
+000014b0: 2e61 6374 696f 6e32 6a73 6f6e 6302 0000  .action2jsonc...
+000014c0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+000014d0: 0043 0000 0073 2e00 0000 7400 7c01 7401  .C...s....t.|.t.
+000014e0: 8302 7307 4a00 8201 7c01 a002 a100 7d02  ..s.J...|.....}.
+000014f0: 7403 7c00 a004 7c02 6a05 a101 7c02 6a06  t.|...|.j...|.j.
+00001500: 6a07 6401 8d02 5300 2902 4e29 02da 046d  j.d...S.).N)...m
+00001510: 6169 6eda 0b77 696e 646f 775f 7369 7a65  ain..window_size
+00001520: 2908 72a0 0000 0072 1d00 0000 da11 6765  ).r....r......ge
+00001530: 745f 6c61 796f 7574 5f68 616e 646c 6572  t_layout_handler
+00001540: 7100 0000 da09 656c 656d 326a 736f 6e72  q.....elem2jsonr
+00001550: a700 0000 da06 6c61 796f 7574 72a8 0000  ......layoutr...
+00001560: 0029 0372 3f00 0000 7291 0000 0072 a500  .).r?...r....r..
+00001570: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00001580: 0072 8600 0000 bb00 0000 730a 0000 000e  .r........s.....
+00001590: 0108 030c 0106 0106 ff7a 1352 656e 6465  .........z.Rende
+000015a0: 7265 722e 7061 6e65 6c32 6a73 6f6e 6302  rer.panel2jsonc.
+000015b0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+000015c0: 0000 0003 0000 0073 d600 0000 7400 7c01  .......s....t.|.
+000015d0: 7401 8302 7307 4a00 8201 7402 7c01 a003  t...s.J...t.|...
+000015e0: a100 7c01 6a04 6a05 6401 8d02 7d02 7406  ..|.j.j.d...}.t.
+000015f0: 7c01 6402 8302 7222 8700 6601 6403 6404  |.d...r"..f.d.d.
+00001600: 8408 7c01 6a07 4400 8301 7c02 6405 3c00  ..|.j.D...|.d.<.
+00001610: 7c02 a008 7409 7c01 6406 8302 a101 0100  |...t.|.d.......
+00001620: 7406 7c01 6407 8302 7253 7c02 a008 7409  t.|.d...rS|...t.
+00001630: 7c01 6a0a 6408 8302 a101 0100 7406 7c01  |.j.d.......t.|.
+00001640: 6409 8302 7253 7c01 6a0b 6400 7501 7253  d...rS|.j.d.u.rS
+00001650: 7c01 6a0b a00c a100 4400 5d0b 5c02 7d03  |.j.....D.].\.}.
+00001660: 7d01 8800 a00d 7c01 a101 7c02 7c03 3c00  }.....|...|.|.<.
+00001670: 7147 740e 7c01 6a04 740f 8302 7269 7c02  qGt.|.j.t...ri|.
+00001680: 6a08 7c01 a010 a100 640a 8d01 0100 7c02  j.|.....d.....|.
+00001690: 6a08 7c01 6a11 6a12 640b 8d01 0100 7c02  j.|.j.j.d.....|.
+000016a0: 5300 290c 4e29 0272 9500 0000 da0a 7265  S.).N).r......re
+000016b0: 6163 745f 6e61 6d65 da08 656c 656d 656e  act_name..elemen
+000016c0: 7473 6301 0000 0000 0000 0000 0000 0002  tsc.............
+000016d0: 0000 0005 0000 0013 0000 0073 1e00 0000  ...........s....
+000016e0: 6700 7c00 5d0b 7d01 7c01 a000 a100 7202  g.|.].}.|.....r.
+000016f0: 8800 a001 7c01 a101 9102 7102 5300 7236  ....|.....q.S.r6
+00001700: 0000 0029 02da 0a69 735f 7669 7369 626c  ...)...is_visibl
+00001710: 6572 aa00 0000 2902 7246 0000 00da 0165  er....).rF.....e
+00001720: 7250 0000 0072 3600 0000 7237 0000 0072  rP...r6...r7...r
+00001730: 4800 0000 ca00 0000 7302 0000 001e 007a  H.......s......z
+00001740: 2652 656e 6465 7265 722e 656c 656d 326a  &Renderer.elem2j
+00001750: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6c69  son.<locals>.<li
+00001760: 7374 636f 6d70 3e72 6800 0000 7a98 6669  stcomp>rh...z.fi
+00001770: 656c 6473 5f69 6e64 6578 2066 6965 6c64  elds_index field
+00001780: 735f 696e 6465 785f 6869 6464 656e 2065  s_index_hidden e
+00001790: 6469 7461 626c 6520 7665 7274 6963 616c  ditable vertical
+000017a0: 2068 7061 6420 6973 5f66 6965 6c64 7365   hpad is_fieldse
+000017b0: 7420 6e61 6d65 2077 6964 7468 2070 7265  t name width pre
+000017c0: 6665 7272 6564 5f77 6964 7468 2020 2020  ferred_width    
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017e0: 2020 2020 2020 2020 2020 2020 2020 6869                hi
+000017f0: 6464 656e 2076 616c 7565 2068 666c 6578  dden value hflex
+00001800: 2076 666c 6578 7298 0000 007a 1561 6374   vflexr....z.act
+00001810: 6f72 5f69 6420 6469 7370 6c61 795f 6d6f  or_id display_mo
+00001820: 6465 da06 736c 6176 6573 2901 da0d 6669  de..slaves)...fi
+00001830: 656c 645f 6f70 7469 6f6e 7329 01da 0968  eld_options)...h
+00001840: 656c 705f 7465 7874 2913 72a0 0000 0072  elp_text).r....r
+00001850: 1e00 0000 7271 0000 0072 a100 0000 7242  ....rq...r....rB
+00001860: 0000 00da 085f 5f6e 616d 655f 5f72 8200  .....__name__r..
+00001870: 0000 72ad 0000 0072 7700 0000 7228 0000  ..r....rw...r(..
+00001880: 0072 9800 0000 72b0 0000 0072 6800 0000  .r....r....rh...
+00001890: 72aa 0000 00da 0a69 7373 7562 636c 6173  r......issubclas
+000018a0: 7372 2100 0000 da11 6765 745f 6669 656c  sr!.....get_fiel
+000018b0: 645f 6f70 7469 6f6e 73da 0566 6965 6c64  d_options..field
+000018c0: 72b2 0000 0029 0472 3f00 0000 72a5 0000  r....).r?...r...
+000018d0: 0072 a600 0000 da01 6b72 3600 0000 7250  .r......kr6...rP
+000018e0: 0000 0072 3700 0000 72aa 0000 00c3 0000  ...r7...r.......
+000018f0: 0073 2000 0000 0e01 0802 0602 06fe 0a03  .s .............
+00001900: 1801 1002 0a04 1202 1403 1201 1001 0c03  ................
+00001910: 1001 1001 0402 7a12 5265 6e64 6572 6572  ......z.Renderer
+00001920: 2e65 6c65 6d32 6a73 6f6e 6301 0000 0000  .elem2jsonc.....
+00001930: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00001940: 0000 0073 0400 0000 6401 5300 2902 4e7a  ...s....d.S.).Nz
+00001950: 1e77 696e 646f 772e 4170 702e 6461 7368  .window.App.dash
+00001960: 626f 6172 642e 7265 6c6f 6164 2829 3b72  board.reload();r
+00001970: 3600 0000 7250 0000 0072 3600 0000 7236  6...rP...r6...r6
+00001980: 0000 0072 3700 0000 da09 7265 6c6f 6164  ...r7.....reload
+00001990: 5f6a 73e2 0000 0073 0200 0000 0401 7a12  _js....s......z.
+000019a0: 5265 6e64 6572 6572 2e72 656c 6f61 645f  Renderer.reload_
+000019b0: 6a73 6302 0000 0000 0000 0000 0000 0006  jsc.............
+000019c0: 0000 0004 0000 004f 0000 0073 dc00 0000  .......O...s....
+000019d0: 7c01 6a00 6a01 6401 6b02 720f 7c00 6a02  |.j.j.d.k.r.|.j.
+000019e0: 6a03 7c02 6900 7c03 a401 8e01 5300 7c01  j.|.i.|.....S.|.
+000019f0: a004 a100 7d04 7c03 a005 7c04 6402 1900  ....}.|...|.d...
+00001a00: a101 0100 7406 7c03 7c01 8302 0100 7c01  ....t.|.|.....|.
+00001a10: 6a07 6403 7501 722c 7c03 a008 7409 6a0a  j.d.u.r,|...t.j.
+00001a20: 7c01 6a07 a102 0100 7c01 6a0b 6403 7501  |.j.....|.j.d.u.
+00001a30: 7239 7c03 a008 7409 6a0c 7c01 6a0b a102  r9|...t.j.|.j...
+00001a40: 0100 7c01 6a0d 6403 7501 725c 7c01 6a0d  ..|.j.d.u.r\|.j.
+00001a50: 6404 1900 7d05 7c05 a00e 6405 a101 7255  d...}.|...d...rU
+00001a60: 7c05 6406 6403 8502 1900 7d05 7c03 a008  |.d.d.....}.|...
+00001a70: 7409 6a0f 6407 a102 0100 7c03 a008 7409  t.j.d.....|...t.
+00001a80: 6a10 7c05 a102 0100 7c00 6a02 6a03 7c01  j.|.....|.j.j.|.
+00001a90: 6a00 6a11 7c01 6a00 6a01 6702 7c02 a201  j.j.|.j.j.g.|...
+00001aa0: 5200 6900 7c03 a401 8e01 5300 2908 7a20  R.i.|.....S.).z 
+00001ab0: 5573 6564 2066 6f72 2074 7572 6e20 7265  Used for turn re
+00001ac0: 7175 6573 7473 2069 6e74 6f20 7572 6c73  quests into urls
+00001ad0: da04 4d61 696e da0b 6261 7365 5f70 6172  ..Main..base_par
+00001ae0: 616d 734e 7201 0000 00da 012d 722c 0000  amsNr......-r,..
+00001af0: 00da 0444 4553 4329 1272 9800 0000 72b3  ...DESC).r....r.
+00001b00: 0000 0072 4000 0000 da0f 6275 696c 645f  ...r@.....build_
+00001b10: 706c 6169 6e5f 7572 6cda 0a67 6574 5f73  plain_url..get_s
+00001b20: 7461 7475 7372 7700 0000 7208 0000 00da  tatusrw...r.....
+00001b30: 066f 6666 7365 74da 0a73 6574 6465 6661  .offset..setdefa
+00001b40: 756c 7472 0c00 0000 da0f 5552 4c5f 5041  ultr......URL_PA
+00001b50: 5241 4d5f 5354 4152 54da 056c 696d 6974  RAM_START..limit
+00001b60: da0f 5552 4c5f 5041 5241 4d5f 4c49 4d49  ..URL_PARAM_LIMI
+00001b70: 54da 086f 7264 6572 5f62 79da 0a73 7461  T..order_by..sta
+00001b80: 7274 7377 6974 68da 1155 524c 5f50 4152  rtswith..URL_PAR
+00001b90: 414d 5f53 4f52 5444 4952 da0e 5552 4c5f  AM_SORTDIR..URL_
+00001ba0: 5041 5241 4d5f 534f 5254 da09 6170 705f  PARAM_SORT..app_
+00001bb0: 6c61 6265 6c29 0672 3f00 0000 da02 6172  label).r?.....ar
+00001bc0: da04 6172 6773 da02 6b77 da02 7374 da02  ..args..kw..st..
+00001bd0: 7363 7236 0000 0072 3600 0000 7237 0000  scr6...r6...r7..
+00001be0: 00da 0f67 6574 5f72 6571 7565 7374 5f75  ...get_request_u
+00001bf0: 726c e500 0000 732c 0000 000c 0212 0108  rl....s,........
+00001c00: 020e 010a 010a 0110 010a 0110 010a 010a  ................
+00001c10: 010a 010c 010e 010e 0106 030c 0102 ff02  ................
+00001c20: 0106 ff02 0106 ff7a 1852 656e 6465 7265  .......z.Rendere
+00001c30: 722e 6765 745f 7265 7175 6573 745f 7572  r.get_request_ur
+00001c40: 6c4e 6305 0000 0000 0000 0000 0000 0007  lNc.............
+00001c50: 0000 0005 0000 004b 0000 0073 ae00 0000  .......K...s....
+00001c60: 7c04 7005 7c03 a000 a100 7d04 7401 7c04  |.p.|.....}.t.|.
+00001c70: 8301 6401 6b02 7211 6402 a002 7c04 a101  ..d.k.r.d...|...
+00001c80: 7d04 7c03 6a03 6a04 722c 7c03 6a03 6a05  }.|.j.j.r,|.j.j.
+00001c90: 732c 7c00 a006 7c02 7c03 7c01 a103 7d06  s,|...|.|.|...}.
+00001ca0: 7c00 6a07 7c02 7c03 7c06 7c04 6604 6900  |.j.|.|.|.|.f.i.
+00001cb0: 7c05 a401 8e01 5300 7c03 6a03 6a08 724b  |.....S.|.j.j.rK
+00001cc0: 7c02 a009 a100 7d06 7c01 6400 7501 723f  |.....}.|.d.u.r?
+00001cd0: 7c06 6a0a 7c01 6a0b 6403 8d01 0100 7c00  |.j.|.j.d.....|.
+00001ce0: 6a07 7c02 7c03 7c06 7c04 6604 6900 7c05  j.|.|.|.|.f.i.|.
+00001cf0: a401 8e01 5300 7c00 6a0c 7c01 7c02 7c03  ....S.|.j.|.|.|.
+00001d00: 7c04 6604 6900 7c05 a401 8e01 5300 2904  |.f.i.|.....S.).
+00001d10: 4e72 2c00 0000 7506 0000 00c2 a07b 7dc2  Nr,...u......{}.
+00001d20: a029 01da 0972 6563 6f72 645f 6964 290d  .)...record_id).
+00001d30: da10 6765 745f 6275 7474 6f6e 5f6c 6162  ..get_button_lab
+00001d40: 656c da03 6c65 6eda 0666 6f72 6d61 7472  el..len..formatr
+00001d50: 6c00 0000 da0a 7061 7261 6d65 7465 7273  l.....parameters
+00001d60: da10 6e6f 5f70 6172 616d 735f 7769 6e64  ..no_params_wind
+00001d70: 6f77 da11 6765 745f 6163 7469 6f6e 5f73  ow..get_action_s
+00001d80: 7461 7475 73da 1477 696e 646f 775f 6163  tatus..window_ac
+00001d90: 7469 6f6e 5f62 7574 746f 6eda 0e6f 7065  tion_button..ope
+00001da0: 6e73 5f61 5f77 696e 646f 7772 be00 0000  ns_a_windowr....
+00001db0: 7277 0000 00da 0270 6bda 1172 6f77 5f61  rw.....pk..row_a
+00001dc0: 6374 696f 6e5f 6275 7474 6f6e 2907 723f  ction_button).r?
+00001dd0: 0000 00da 036f 626a 72c9 0000 0072 8f00  .....objr....r..
+00001de0: 0000 7295 0000 0072 cb00 0000 72cc 0000  ..r....r....r...
+00001df0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+00001e00: da0d 6163 7469 6f6e 5f62 7574 746f 6efd  ..action_button.
+00001e10: 0000 0073 2000 0000 0c01 0c01 0a01 1002  ...s ...........
+00001e20: 0e01 0401 0801 04ff 0201 06ff 0802 0801  ................
+00001e30: 0801 0e01 1801 1801 7a16 5265 6e64 6572  ........z.Render
+00001e40: 6572 2e61 6374 696f 6e5f 6275 7474 6f6e  er.action_button
+00001e50: 6305 0000 0000 0000 0000 0000 0007 0000  c...............
+00001e60: 0004 0000 004b 0000 0073 4000 0000 7c02  .....K...s@...|.
+00001e70: 6401 7500 720d 7c03 6a00 6402 6900 7c04  d.u.r.|.j.d.i.|.
+00001e80: a401 8e01 7d06 6e09 7c02 6a01 7c03 6601  ....}.n.|.j.|.f.
+00001e90: 6900 7c04 a401 8e01 7d06 7c00 6a02 7c06  i.|.....}.|.j.|.
+00001ea0: 7c01 6602 6900 7c05 a401 8e01 5300 2903  |.f.i.|.....S.).
+00001eb0: 61cf 0100 004e 6f74 6520 7468 6174 2060  a....Note that `
+00001ec0: 6261 2e61 6374 6f72 6020 6d61 7920 6469  ba.actor` may di
+00001ed0: 6666 6572 2066 726f 6d20 6061 722e 6163  ffer from `ar.ac
+00001ee0: 746f 7260 2077 6865 6e20 6465 6669 6e65  tor` when define
+00001ef0: 6420 6f6e 2061 0a20 2020 2020 2020 2064  d on a.        d
+00001f00: 6966 6665 7265 6e74 2061 6374 6f72 2e20  ifferent actor. 
+00001f10: 5265 6d65 6d62 6572 2065 2e67 2e20 7468  Remember e.g. th
+00001f20: 6520 224d 7573 7420 7265 6164 2065 4944  e "Must read eID
+00001f30: 2063 6172 6422 2061 6374 696f 6e0a 2020   card" action.  
+00001f40: 2020 2020 2020 6275 7474 6f6e 2069 6e20        button in 
+00001f50: 6569 645f 696e 666f 206f 6620 6e65 7763  eid_info of newc
+00001f60: 6f6d 6572 732e 4e65 7743 6c69 656e 7473  omers.NewClients
+00001f70: 2028 3230 3134 3034 3232 292e 0a0a 2020   (20140422)...  
+00001f80: 2020 2020 2020 3a6f 626a 3a20 2054 6865        :obj:  The
+00001f90: 2064 6174 6162 6173 6520 6f62 6a65 6374   database object
+00001fa0: 0a20 2020 2020 2020 203a 6172 3a20 2020  .        :ar:   
+00001fb0: 5468 6520 6163 7469 6f6e 2072 6571 7565  The action reque
+00001fc0: 7374 0a20 2020 2020 2020 203a 6261 3a20  st.        :ba: 
+00001fd0: 2054 6865 2062 6f75 6e64 2061 6374 696f   The bound actio
+00001fe0: 6e0a 2020 2020 2020 2020 3a72 6571 7565  n.        :reque
+00001ff0: 7374 5f6b 7761 7267 733a 206b 6579 776f  st_kwargs: keywo
+00002000: 7264 2061 7267 756d 656e 7473 2074 6f20  rd arguments to 
+00002010: 666f 7277 6172 6465 6420 746f 2074 6865  forwarded to the
+00002020: 2063 6869 6c64 2061 6374 696f 6e20 7265   child action re
+00002030: 7175 6573 740a 0a20 2020 2020 2020 2041  quest..        A
+00002040: 6e79 206b 6579 776f 7264 206f 7468 6572  ny keyword other
+00002050: 2061 7267 756d 656e 7473 2061 7265 2066   arguments are f
+00002060: 6f72 7761 7264 6564 2074 6f20 3a6d 6574  orwarded to :met
+00002070: 683a 6061 7232 6a73 602e 0a0a 2020 2020  h:`ar2js`...    
+00002080: 2020 2020 4e72 3600 0000 2903 da07 7265      Nr6...)...re
+00002090: 7175 6573 74da 0573 7061 776e da05 6172  quest..spawn..ar
+000020a0: 326a 7329 0772 3f00 0000 72da 0000 0072  2js).r?...r....r
+000020b0: c900 0000 728f 0000 00da 0e72 6571 7565  ....r......reque
+000020c0: 7374 5f6b 7761 7267 73da 0673 7461 7475  st_kwargs..statu
+000020d0: 73da 0373 6172 7236 0000 0072 3600 0000  s..sarr6...r6...
+000020e0: 7237 0000 00da 1761 6374 696f 6e5f 6361  r7.....action_ca
+000020f0: 6c6c 5f6f 6e5f 696e 7374 616e 6365 0e01  ll_on_instance..
+00002100: 0000 7308 0000 0008 0e12 0112 0314 017a  ..s............z
+00002110: 2052 656e 6465 7265 722e 6163 7469 6f6e   Renderer.action
+00002120: 5f63 616c 6c5f 6f6e 5f69 6e73 7461 6e63  _call_on_instanc
+00002130: 6563 0200 0000 0000 0000 0000 0000 0400  ec..............
+00002140: 0000 0400 0000 4300 0000 732c 0000 007c  ......C...s,...|
+00002150: 016a 0070 057c 016a 017d 0274 02a0 037c  .j.p.|.j.}.t...|
+00002160: 0264 01a1 027d 037c 0364 0175 0072 1264  .d...}.|.d.u.r.d
+00002170: 0153 0064 027c 0316 0053 0029 037a bf0a  .S.d.|...S.).z..
+00002180: 2020 2020 2020 2020 5573 6573 2061 6e20          Uses an 
+00002190: 696e 7465 726e 616c 206d 6170 7069 6e67  internal mapping
+000021a0: 2066 6f72 2069 636f 6e20 6e61 6d65 7320   for icon names 
+000021b0: 746f 2063 6f6e 7665 7274 2065 7869 7374  to convert exist
+000021c0: 696e 6720 6963 6f6e 7320 696e 746f 2072  ing icons into r
+000021d0: 6561 6374 2d75 7361 626c 652e 0a20 2020  eact-usable..   
+000021e0: 2020 2020 203a 7061 7261 6d20 6163 7469       :param acti
+000021f0: 6f6e 3a0a 2020 2020 2020 2020 3a72 6574  on:.        :ret
+00002200: 7572 6e3a 2073 7472 3a20 6120 6963 6f6e  urn: str: a icon
+00002210: 206e 616d 6520 666f 7220 6569 7468 6572   name for either
+00002220: 2070 7269 6d65 2d72 6561 6374 206f 7220   prime-react or 
+00002230: 6963 6f6e 380a 2020 2020 2020 2020 4e7a  icon8.        Nz
+00002240: 0570 6920 2573 2904 da0f 7265 6163 745f  .pi %s)...react_
+00002250: 6963 6f6e 5f6e 616d 65da 0969 636f 6e5f  icon_name..icon_
+00002260: 6e61 6d65 722d 0000 00da 0367 6574 2904  namer-.....get).
+00002270: 723f 0000 0072 6c00 0000 729f 0000 00da  r?...rl...r.....
+00002280: 0a72 6561 6374 5f69 636f 6e72 3600 0000  .react_iconr6...
+00002290: 7236 0000 0072 3700 0000 72a4 0000 0023  r6...r7...r....#
+000022a0: 0100 0073 0a00 0000 0c07 0c01 0801 0401  ...s............
+000022b0: 0802 7a18 5265 6e64 6572 6572 2e67 6574  ..z.Renderer.get
+000022c0: 5f61 6374 696f 6e5f 6963 6f6e 6303 0000  _action_iconc...
+000022d0: 0000 0000 0000 0000 0008 0000 0007 0000  ................
+000022e0: 004b 0000 0073 a400 0000 7c01 6a00 7d04  .K...s....|.j.}.
+000022f0: 7c01 6a01 7d05 6900 7d06 7c05 6a02 a003  |.j.}.i.}.|.j...
+00002300: a100 721c 7c03 a004 7c00 a005 7c01 7c05  ..r.|...|...|.|.
+00002310: 7c02 a103 a101 0100 7c06 a004 7c03 a101  |.......|...|...
+00002320: 0100 7c06 a004 7c00 a006 7c01 7c05 7c02  ..|...|...|.|.|.
+00002330: a103 a101 0100 7c06 a004 7c03 a101 0100  ......|...|.....
+00002340: 7c04 7c05 6a02 6a07 7c01 6a08 7c05 6a09  |.|.j.j.|.j.|.j.
+00002350: 6a0a 7c06 6401 9c05 7d07 740b 7c02 6402  j.|.d...}.t.|.d.
+00002360: 8302 7243 7c02 6a0c 7c07 6403 3c00 6e09  ..rC|.j.|.d.<.n.
+00002370: 740d 7c02 740e 8302 724c 7c02 7c07 6403  t.|.t...rL|.|.d.
+00002380: 3c00 6404 740f 7c07 8301 1600 5300 2905  <.d.t.|.....S.).
+00002390: 7a43 496d 706c 656d 656e 7473 203a 6d65  zCImplements :me
+000023a0: 7468 3a60 6c69 6e6f 2e63 6f72 652e 7265  th:`lino.core.re
+000023b0: 6e64 6572 6572 2e48 746d 6c52 656e 6465  nderer.HtmlRende
+000023c0: 7265 722e 6172 326a 7360 2e0a 0a20 2020  rer.ar2js`...   
+000023d0: 2020 2020 2029 05da 0272 7072 9400 0000       )...rpr....
+000023e0: da06 6f6e 4d61 696e da07 6163 746f 7249  ..onMain..actorI
+000023f0: 6472 e000 0000 72d8 0000 00da 0273 72fa  dr....r......sr.
+00002400: 1877 696e 646f 772e 4170 702e 7275 6e41  .window.App.runA
+00002410: 6374 696f 6e28 2573 2929 10da 1072 6571  ction(%s))...req
+00002420: 7565 7374 696e 675f 7061 6e65 6c72 a300  uesting_panelr..
+00002430: 0000 726c 0000 0072 a200 0000 7277 0000  ..rl...r....rw..
+00002440: 0072 d500 0000 da11 6765 745f 6163 7469  .r......get_acti
+00002450: 6f6e 5f70 6172 616d 7372 4d00 0000 da10  on_paramsrM.....
+00002460: 6973 5f6f 6e5f 6d61 696e 5f61 6374 6f72  is_on_main_actor
+00002470: 7298 0000 00da 0861 6374 6f72 5f69 6472  r......actor_idr
+00002480: 8200 0000 72d8 0000 0072 a000 0000 7278  ....r....r....rx
+00002490: 0000 0072 2600 0000 2908 723f 0000 0072  ...r&...).r?...r
+000024a0: c900 0000 72da 0000 0072 e000 0000 72e7  ....r....r....r.
+000024b0: 0000 0072 8f00 0000 da06 7061 7261 6d73  ...r......params
+000024c0: da06 6a73 5f6f 626a 7236 0000 0072 3600  ..js_objr6...r6.
+000024d0: 0000 7237 0000 0072 de00 0000 3101 0000  ..r7...r....1...
+000024e0: 732a 0000 0006 0406 0104 010a 0114 040a  s*..............
+000024f0: 0114 010a 0102 0306 0104 0106 0102 0106  ................
+00002500: fb0a 070c 010a 0208 0102 0206 0104 ff7a  ...............z
+00002510: 0e52 656e 6465 7265 722e 6172 326a 7363  .Renderer.ar2jsc
+00002520: 0200 0000 0000 0000 0000 0000 0600 0000  ................
+00002530: 0600 0000 4300 0000 73bc 0100 007c 0174  ....C...s....|.t
+00002540: 006a 016a 0275 0072 0a74 0364 0183 0153  .j.j.u.r.t.d...S
+00002550: 0074 047c 0174 0583 0272 1674 0664 02a0  .t.|.t...r.t.d..
+00002560: 077c 01a1 0183 0182 0174 047c 0174 086a  .|.......t.|.t.j
+00002570: 0983 0272 2009 007c 016a 0a53 0074 047c  ...r ..|.j.S.t.|
+00002580: 0174 0b6a 0c83 0272 297c 016a 0d53 0074  .t.j...r)|.j.S.t
+00002590: 047c 0174 0683 0272 3274 0e7c 0183 0153  .|.t...r2t.|...S
+000025a0: 0074 047c 0174 0f83 0272 4a7c 016a 1064  .t.|.t...rJ|.j.d
+000025b0: 0375 0072 3f7c 016a 1153 0074 127c 016a  .u.r?|.j.S.t.|.j
+000025c0: 1374 127c 016a 1164 048d 0164 058d 0253  .t.|.j.d...d...S
+000025d0: 0074 047c 0174 1483 0272 cc7c 016a 1564  .t.|.t...r.|.j.d
+000025e0: 0375 0172 6d7c 00a0 1664 037c 016a 1564  .u.rm|...d.|.j.d
+000025f0: 03a1 037d 027c 0264 0375 0173 624a 0082  ...}.|.d.u.sbJ..
+00002600: 0164 067c 0216 007d 037c 00a0 177c 017c  .d.|...}.|...|.|
+00002610: 0264 03a1 0353 007c 016a 1864 0375 0172  .d...S.|.j.d.u.r
+00002620: 957c 016a 1972 857c 016a 186a 1a64 0d69  .|.j.r.|.j.j.d.i
+00002630: 007c 016a 19a4 018e 017d 047c 00a0 1b7c  .|.j.....}.|...|
+00002640: 04a1 017d 036e 087c 00a0 1c64 037c 016a  ...}.n.|...d.|.j
+00002650: 1869 00a1 037d 037c 00a0 177c 017c 037c  .i...}.|...|.|.|
+00002660: 016a 1da1 0353 007c 016a 1e64 0375 0172  .j...S.|.j.d.u.r
+00002670: a764 067c 016a 1e16 007d 037c 00a0 177c  .d.|.j...}.|...|
+00002680: 017c 037c 016a 1da1 0353 007c 016a 1f64  .|.|.j...S.|.j.d
+00002690: 0375 0172 b07c 016a 1f7d 056e 037c 016a  .u.r.|.j.}.n.|.j
+000026a0: 1353 007c 016a 106a 1064 0375 0072 c574  .S.|.j.j.d.u.r.t
+000026b0: 1264 077c 016a 1374 0364 087c 0516 0083  .d.|.j.t.d.|....
+000026c0: 0164 098d 0353 0074 127c 016a 137c 0564  .d...S.t.|.j.|.d
+000026d0: 0a8d 0253 0074 047c 0174 0383 0272 dc74  ...S.t.|.t...r.t
+000026e0: 207c 0064 0b64 0c83 0372 dc74 0e7c 016a   |.d.d...r.t.|.j
+000026f0: 2183 0153 007c 0153 0029 0e7a 540a 2020  !..S.|.S.).zT.  
+00002700: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+00002710: 2063 6f6e 7665 7274 696e 6720 6c6f 6769   converting logi
+00002720: 6320 666f 7220 7365 7269 616c 697a 696e  c for serializin
+00002730: 6720 5079 7468 6f6e 2076 616c 7565 7320  g Python values 
+00002740: 746f 206a 736f 6e2e 0a20 2020 2020 2020  to json..       
+00002750: 20da 104c 414e 4755 4147 455f 4348 4f49   ..LANGUAGE_CHOI
+00002760: 4345 537a 0b32 3032 3130 3531 3720 7b7d  CESz.20210517 {}
+00002770: 4e29 0172 6800 0000 2902 7244 0000 0072  N).rh...).rD...r
+00002780: 5500 0000 7a02 2573 da06 6275 7474 6f6e  U...z.%s..button
+00002790: 7a23 6675 6e63 7469 6f6e 2829 207b 204c  z#function() { L
+000027a0: 696e 6f2e 6c6f 6164 5f75 726c 2827 2573  ino.load_url('%s
+000027b0: 2729 3b20 7d29 03da 0578 7479 7065 7244  '); })...xtyperD
+000027c0: 0000 00da 0768 616e 646c 6572 2902 7244  .....handler).rD
+000027d0: 0000 00da 0468 7265 6672 6e00 0000 4672  .....hrefrn...Fr
+000027e0: 3600 0000 2922 7204 0000 0072 6f00 0000  6...)"r....ro...
+000027f0: 72f2 0000 0072 2700 0000 72a0 0000 0072  r....r'...r....r
+00002800: 1c00 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
+00002810: d200 0000 720d 0000 00da 0643 686f 6963  ....r......Choic
+00002820: 6572 4300 0000 7205 0000 00da 054d 6f64  erC...r......Mod
+00002830: 656c 72d8 0000 0072 4500 0000 720a 0000  elr....rE...r...
+00002840: 00da 0670 6172 656e 7472 6800 0000 7271  ...parentrh...rq
+00002850: 0000 0072 9500 0000 720b 0000 00da 0869  ...r....r......i
+00002860: 6e73 7461 6e63 65da 1069 6e73 7461 6e63  nstance..instanc
+00002870: 655f 6861 6e64 6c65 72da 0c68 616e 646c  e_handler..handl
+00002880: 6572 5f69 7465 6d72 a300 0000 72f0 0000  er_itemr....r...
+00002890: 0072 dc00 0000 da0f 7265 7175 6573 745f  .r......request_
+000028a0: 6861 6e64 6c65 72da 0b61 6374 696f 6e5f  handler..action_
+000028b0: 6361 6c6c 72b2 0000 00da 0a6a 6176 6173  callr......javas
+000028c0: 6372 6970 7472 f600 0000 da07 6765 7461  criptr......geta
+000028d0: 7474 72da 0173 2906 723f 0000 0072 a500  ttr..s).r?...r..
+000028e0: 0000 da01 68da 026a 7372 c900 0000 da03  ....h..jsr......
+000028f0: 7572 6c72 3600 0000 7236 0000 0072 3700  urlr6...r6...r7.
+00002900: 0000 723e 0000 0052 0100 0073 5400 0000  ..r>...R...sT...
+00002910: 0c04 0801 0a01 0e01 0c01 0201 0603 0c01  ................
+00002920: 0601 0a01 0801 0a01 0a01 0601 1603 0a02  ................
+00002930: 0a01 1001 0c01 0801 0e01 0a01 0601 1401  ................
+00002940: 0c01 1002 1001 0a02 0a01 1001 0a01 0801  ................
+00002950: 0607 0c02 0202 0601 0a02 06fd 0e04 1602  ................
+00002960: 0a02 0402 7a18 5265 6e64 6572 6572 2e70  ....z.Renderer.p
+00002970: 7932 6a73 5f63 6f6e 7665 7274 6572 6304  y2js_converterc.
+00002980: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00002990: 0000 0043 0000 0073 5000 0000 7400 7c01  ...C...sP...t.|.
+000029a0: 6a01 7c02 6401 8d02 7d04 7c01 6a02 721a  j.|.d...}.|.j.r.
+000029b0: 7c01 6a02 6a03 6a04 721a 7c04 6a05 6402  |.j.j.j.r.|.j.d.
+000029c0: 7c01 6a02 6a03 6a04 1700 6403 8d01 0100  |.j.j.j...d.....
+000029d0: 7406 6a07 6a08 7226 7c03 7226 7c04 6a05  t.j.j.r&|.r&|.j.
+000029e0: 7c03 6404 8d01 0100 7c04 5300 2905 da00  |.d.....|.S.)...
+000029f0: 2902 7244 0000 0072 f500 0000 7a07 782d  ).rD...r....z.x-
+00002a00: 7462 6172 2d29 01da 0769 636f 6e43 6c73  tbar-)...iconCls
+00002a10: 2901 da07 746f 6f6c 5469 7029 0972 7100  )...toolTip).rq.
+00002a20: 0000 7295 0000 0072 a300 0000 726c 0000  ..r....r....rl..
+00002a30: 0072 e400 0000 7277 0000 0072 0400 0000  .r....rw...r....
+00002a40: 726f 0000 00da 0d75 7365 5f71 7569 636b  ro.....use_quick
+00002a50: 7469 7073 2905 723f 0000 00da 026d 6972  tips).r?.....mir
+00002a60: f500 0000 72b2 0000 00da 0164 7236 0000  ....r......dr6..
+00002a70: 0072 3600 0000 7237 0000 0072 fd00 0000  .r6...r7...r....
+00002a80: a001 0000 730c 0000 000e 0410 0116 010c  ....s...........
+00002a90: 010c 0304 017a 1552 656e 6465 7265 722e  .....z.Renderer.
+00002aa0: 6861 6e64 6c65 725f 6974 656d 6302 0000  handler_itemc...
+00002ab0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+00002ac0: 004f 0000 0073 2000 0000 7c01 6a00 6402  .O...s ...|.j.d.
+00002ad0: 6900 7c03 a401 8e01 7d04 7c00 a001 7c01  i.|.....}.|...|.
+00002ae0: 7c01 6a02 7c04 a103 5300 2903 7a36 2047  |.j.|...S.).z6 G
+00002af0: 656e 6572 6174 6573 206a 7320 7374 7269  enerates js stri
+00002b00: 6e67 2066 6f72 2061 6374 696f 6e20 6275  ng for action bu
+00002b10: 7474 6f6e 2063 616c 6c73 2e0a 2020 2020  tton calls..    
+00002b20: 2020 2020 4e72 3600 0000 2903 72be 0000      Nr6...).r...
+00002b30: 0072 ff00 0000 72a3 0000 0029 0572 3f00  .r....r....).r?.
+00002b40: 0000 72c9 0000 0072 ca00 0000 72cb 0000  ..r....r....r...
+00002b50: 0072 cc00 0000 7236 0000 0072 3600 0000  .r....r6...r6...
+00002b60: 7237 0000 0072 fe00 0000 ae01 0000 7304  r7...r........s.
+00002b70: 0000 0010 0410 017a 1852 656e 6465 7265  .......z.Rendere
+00002b80: 722e 7265 7175 6573 745f 6861 6e64 6c65  r.request_handle
+00002b90: 7263 0400 0000 0000 0000 0000 0000 0800  rc..............
+00002ba0: 0000 0800 0000 4300 0000 739c 0000 007c  ......C...s....|
+00002bb0: 026a 007d 047c 02a0 01a1 00a0 0264 0164  .j.}.|.......d.d
+00002bc0: 02a1 025c 027d 057d 067c 0373 1169 007d  ...\.}.}.|.s.i.}
+00002bd0: 037c 0164 0075 0172 2274 037c 0164 0383  .|.d.u.r"t.|.d..
+00002be0: 0272 227c 016a 0464 0869 007c 03a4 018e  .r"|.j.d.i.|....
+00002bf0: 017d 037c 0172 2d7c 016a 0572 2d7c 016a  .}.|.r-|.j.r-|.j
+00002c00: 057c 0374 066a 073c 007c 0664 046b 0272  .|.t.j.<.|.d.k.r
+00002c10: 3974 037c 0364 0583 0272 397c 0364 053d  9t.|.d...r9|.d.=
+00002c20: 007c 0164 0075 0072 3f64 006e 027c 016a  .|.d.u.r?d.n.|.j
+00002c30: 087d 0764 0674 0974 0a7c 067c 057c 037c  .}.d.t.t.|.|.|.|
+00002c40: 0764 078d 0483 0116 0053 0029 094e da01  .d.......S.).N..
+00002c50: 2e72 2c00 0000 72be 0000 00da 0467 7269  .r,...r......gri
+00002c60: 6472 cf00 0000 72eb 0000 0029 0472 9400  dr....r....).r..
+00002c70: 0000 72e9 0000 0072 e000 0000 72e7 0000  ..r....r....r...
+00002c80: 0072 3600 0000 290b 726c 0000 00da 0966  .r6...).rl.....f
+00002c90: 756c 6c5f 6e61 6d65 da06 7273 706c 6974  ull_name..rsplit
+00002ca0: 7282 0000 0072 be00 0000 da0a 7375 6273  r....r......subs
+00002cb0: 745f 7573 6572 720c 0000 00da 1455 524c  t_userr......URL
+00002cc0: 5f50 4152 414d 5f53 5542 5354 5f55 5345  _PARAM_SUBST_USE
+00002cd0: 5272 ec00 0000 7226 0000 0072 7100 0000  Rr....r&...rq...
+00002ce0: 2908 723f 0000 0072 c900 0000 72a3 0000  ).r?...r....r...
+00002cf0: 0072 e000 0000 724f 0000 0072 e900 0000  .r....rO...r....
+00002d00: 7294 0000 0072 e700 0000 7236 0000 0072  r....r....r6...r
+00002d10: 3600 0000 7237 0000 0072 ff00 0000 b801  6...r7...r......
+00002d20: 0000 7322 0000 0006 0214 0204 0204 0112  ..s"............
+00002d30: 0210 010a 020c 0112 1106 0112 0206 0202  ................
+00002d40: 0102 0102 0102 010a fc7a 1452 656e 6465  .........z.Rende
+00002d50: 7265 722e 6163 7469 6f6e 5f63 616c 6c63  rer.action_callc
+00002d60: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002d70: 0400 0000 4300 0000 732e 0000 007c 0173  ....C...s....|.s
+00002d80: 0464 0053 0074 007c 0174 0183 0273 0d74  .d.S.t.|.t...s.t
+00002d90: 017c 0183 017d 0174 027c 0164 0164 028d  .|...}.t.|.d.d..
+00002da0: 027d 0164 037c 0117 0053 0029 044e 4629  .}.d.|...S.).NF)
+00002db0: 01da 0571 756f 7465 7a0b 6a61 7661 7363  ...quotez.javasc
+00002dc0: 7269 7074 3a29 0372 a000 0000 7245 0000  ript:).r....rE..
+00002dd0: 0072 0300 0000 2902 723f 0000 0072 0401  .r....).r?...r..
+00002de0: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00002df0: 00da 066a 7332 7572 6ce2 0100 0073 0c00  ...js2url....s..
+00002e00: 0000 0401 0401 0a02 0801 0c01 0801 7a0f  ..............z.
+00002e10: 5265 6e64 6572 6572 2e6a 7332 7572 6c63  Renderer.js2urlc
+00002e20: 0600 0000 0000 0000 0000 0000 0700 0000  ................
+00002e30: 0400 0000 4300 0000 7356 0000 0074 006a  ....C...sV...t.j
+00002e40: 016a 0272 2774 006a 016a 0372 0f64 017c  .j.r't.j.j.r.d.|
+00002e50: 047c 0566 0216 007d 066e 0264 027d 067c  .|.f...}.n.d.}.|
+00002e60: 0272 1974 0464 037c 067c 0283 037d 067c  .r.t.d.|.|...}.|
+00002e70: 0672 297c 016a 0564 047c 037c 0666 0216  .r)|.j.d.|.|.f..
+00002e80: 0064 058d 0101 0064 0053 0064 0053 0064  .d.....d.S.d.S.d
+00002e90: 0053 0029 064e 7a08 2825 732e 2573 2920  .S.).Nz.(%s.%s) 
+00002ea0: 7206 0100 007a 047b 7d7b 7d7a 0728 2573  r....z.{}{}z.(%s
+00002eb0: 2c25 7329 2901 da08 7175 6963 6b74 6970  ,%s))...quicktip
+00002ec0: 2906 7204 0000 0072 6f00 0000 7209 0100  ).r....ro...r...
+00002ed0: 00da 1973 686f 775f 696e 7465 726e 616c  ...show_internal
+00002ee0: 5f66 6965 6c64 5f6e 616d 6573 7206 0000  _field_namesr...
+00002ef0: 0072 7700 0000 2907 723f 0000 0072 cb00  .rw...).r?...r..
+00002f00: 0000 72b2 0000 0072 7400 0000 da0a 6461  ..r....rt.....da
+00002f10: 7461 736f 7572 6365 da09 6669 656c 646e  tasource..fieldn
+00002f20: 616d 65da 0374 7474 7236 0000 0072 3600  ame..tttr6...r6.
+00002f30: 0000 7237 0000 00da 0d61 6464 5f68 656c  ..r7.....add_hel
+00002f40: 705f 7465 7874 eb01 0000 7318 0000 0008  p_text....s.....
+00002f50: 0108 010e 0104 0204 010c 0104 0108 0402  ................
+00002f60: 010e ff04 f504 077a 1652 656e 6465 7265  .......z.Rendere
+00002f70: 722e 6164 645f 6865 6c70 5f74 6578 7463  r.add_help_textc
+00002f80: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00002f90: 0300 0000 4300 0000 7356 0000 0074 0083  ....C...sV...t..
+00002fa0: 007d 0264 017c 0117 0064 0217 007d 037c  .}.d.|...d...}.|
+00002fb0: 006a 01a0 0264 03a1 0164 0419 007d 047c  .j...d...d...}.|
+00002fc0: 0264 0575 0172 1c7c 037c 026a 0364 0217  .d.u.r.|.|.j.d..
+00002fd0: 0037 007d 037c 0374 04a0 05a1 0064 0317  .7.}.|.t.....d..
+00002fe0: 007c 0417 0037 007d 0364 067c 047c 0366  .|...7.}.d.|.|.f
+00002ff0: 0353 0029 077a 2c4c 696b 6520 6c69 6e6f  .S.).z,Like lino
+00003000: 5f6a 735f 7061 7274 732c 2062 7574 2066  _js_parts, but f
+00003010: 6f72 2061 6374 6f72 5f6c 6576 656c 2064  or actor_level d
+00003020: 6174 61da 054c 696e 6f5f da01 5f72 0c01  ata..Lino_.._r..
+00003030: 0000 722e 0000 004e da05 6361 6368 6529  ..r....N..cache)
+00003040: 0672 2900 0000 da11 6c69 6e6f 5f77 6562  .r).....lino_web
+00003050: 5f74 656d 706c 6174 6572 0f01 0000 7243  _templater....rC
+00003060: 0000 0072 0700 0000 da0c 6765 745f 6c61  ...r......get_la
+00003070: 6e67 7561 6765 2905 723f 0000 0072 e900  nguage).r?...r..
+00003080: 0000 da09 7573 6572 5f74 7970 65da 0866  ....user_type..f
+00003090: 696c 656e 616d 65da 0966 696c 655f 7479  ilename..file_ty
+000030a0: 7065 7236 0000 0072 3600 0000 7237 0000  per6...r6...r7..
+000030b0: 00da 156c 696e 6f5f 6a73 5f70 6172 7473  ...lino_js_parts
+000030c0: 5f63 6875 6e6b 6564 fa01 0000 730e 0000  _chunked....s...
+000030d0: 0006 020c 0110 0108 010e 0114 010a 017a  ...............z
+000030e0: 1e52 656e 6465 7265 722e 6c69 6e6f 5f6a  .Renderer.lino_j
+000030f0: 735f 7061 7274 735f 6368 756e 6b65 6463  s_parts_chunkedc
+00003100: 0200 0000 0000 0000 0000 0000 1100 0000  ................
+00003110: 0600 0000 4300 0000 73de 0100 0067 007d  ....C...s....g.}
+00003120: 0267 007d 037c 0144 005d e47d 047c 04a0  .g.}.|.D.].}.|..
+00003130: 00a1 007d 057c 0573 127c 046a 016a 0272  ...}.|.s.|.j.j.r
+00003140: cc74 036a 047c 046a 016a 0569 017d 067c  .t.j.|.j.j.i.}.|
+00003150: 0572 237c 066a 067c 056a 076a 0864 018d  .r#|.j.|.j.j.d..
+00003160: 0101 007c 046a 016a 0272 c767 007d 0774  ...|.j.j.r.g.}.t
+00003170: 0983 007d 087c 046a 0aa0 0b7c 046a 0174  ...}.|.j...|.j.t
+00003180: 0c83 00a1 0244 005d 727d 0974 097c 096a  .....D.]r}.t.|.j
+00003190: 016a 0564 028d 017d 0a7c 096a 016a 0d7d  .j.d...}.|.j.j.}
+000031a0: 0b7c 0b72 487c 0b7c 0a64 033c 007c 096a  .|.rH|.|.d.<.|.j
+000031b0: 016a 0e7d 0c7c 0c72 5e74 0f7c 0c83 0172  .j.}.|.r^t.|...r
+000031c0: 5a7c 0c7c 096a 0a83 017c 0a64 043c 006e  Z|.|.j...|.d.<.n
+000031d0: 047c 0c7c 0a64 043c 007c 096a 016a 1064  .|.|.d.<.|.j.j.d
+000031e0: 0575 0172 847c 096a 016a 107d 0d7c 0d7c  .u.r.|.j.j.}.|.|
+000031f0: 0876 0072 747c 087c 0d19 00a0 117c 0aa1  .v.rt|.|.....|..
+00003200: 0101 006e 1574 097c 0d64 068d 017d 0e7c  ...n.t.|.d...}.|
+00003210: 0a67 017c 087c 0d3c 007c 07a0 117c 0ea1  .g.|.|.<.|...|..
+00003220: 0101 006e 057c 07a0 117c 0aa1 0101 007c  ...n.|...|.....|
+00003230: 096a 016a 1272 a774 137c 096a 016a 1283  .j.j.r.t.|.j.j..
+00003240: 017d 0f74 147c 0f64 0783 0273 9e7c 096a  .}.t.|.d...s.|.j
+00003250: 016a 057c 0f64 073c 007c 0f7c 0376 0172  .j.|.d.<.|.|.v.r
+00003260: a77c 03a0 117c 0fa1 0101 0071 357c 0872  .|...|.....q5|.r
+00003270: c374 157c 0783 0144 005d 145c 027d 107d  .t.|...D.].\.}.}
+00003280: 0a7c 0aa0 1664 0864 09a1 0272 c27c 087c  .|...d.d...r.|.|
+00003290: 0a64 0819 0019 007c 077c 1019 0064 0a3c  .d.....|.|...d.<
+000032a0: 0071 ae7c 077c 0664 0b3c 007c 02a0 117c  .q.|.|.d.<.|...|
+000032b0: 06a1 0101 007c 046a 016a 1272 ea74 137c  .....|.j.j.r.t.|
+000032c0: 046a 016a 1283 017d 0f74 147c 0f64 0783  .j.j...}.t.|.d..
+000032d0: 0273 e17c 046a 016a 057c 0f64 073c 007c  .s.|.j.j.|.d.<.|
+000032e0: 0f7c 0376 0172 ea7c 03a0 117c 0fa1 0101  .|.v.r.|...|....
+000032f0: 0071 067c 027c 0366 0253 0029 0c7a 4543  .q.|.|.f.S.).zEC
+00003300: 6f6e 7665 7274 7320 6f66 2061 6c6c 2074  onverts of all t
+00003310: 6865 2062 6f75 6e64 6163 7469 6f6e 7320  he boundactions 
+00003320: 6f66 2061 6e20 6163 746f 7220 746f 206a  of an actor to j
+00003330: 736f 6e20 666f 726d 6174 2e0a 2020 2020  son format..    
+00003340: 2020 2020 a901 7265 0000 0029 0172 9400      ..re...).r..
+00003350: 0000 72b2 0000 00da 0a6a 735f 6861 6e64  ..r......js_hand
+00003360: 6c65 724e 2901 da05 636f 6d62 6f72 8f00  lerN)...combor..
+00003370: 0000 7225 0100 0046 7255 0000 00da 0e74  ..r%...FrU.....t
+00003380: 6f6f 6c62 6172 4163 7469 6f6e 7329 17da  oolbarActions)..
+00003390: 1167 6574 5f6c 6179 6f75 745f 6861 6e64  .get_layout_hand
+000033a0: 656c 726c 0000 00da 0b77 696e 646f 775f  elrl.....window_
+000033b0: 7479 7065 720c 0000 00da 1555 524c 5f50  typer......URL_P
+000033c0: 4152 414d 5f41 4354 494f 4e5f 4e41 4d45  ARAM_ACTION_NAME
+000033d0: 724d 0000 0072 7700 0000 72ab 0000 0072  rM...rw...r....r
+000033e0: 8700 0000 7271 0000 0072 9800 0000 da13  ....rq...r......
+000033f0: 6765 745f 746f 6f6c 6261 725f 6163 7469  get_toolbar_acti
+00003400: 6f6e 7372 2900 0000 72b2 0000 0072 2401  onsr)...r....r$.
+00003410: 0000 722f 0000 00da 0b63 6f6d 626f 5f67  ..r/.....combo_g
+00003420: 726f 7570 da06 6170 7065 6e64 da06 686f  roup..append..ho
+00003430: 746b 6579 da04 7661 7273 7282 0000 0072  tkey..varsr....r
+00003440: 3000 0000 72e5 0000 0029 1172 3f00 0000  0...r....).r?...
+00003450: da0c 6163 7469 6f6e 735f 6c69 7374 72a6  ..actions_listr.
+00003460: 0000 00da 0768 6f74 6b65 7973 728f 0000  .....hotkeysr...
+00003470: 00da 026c 68da 1161 6374 696f 6e5f 6465  ...lh..action_de
+00003480: 7363 7269 7074 6f72 da04 7462 6173 da09  scriptor..tbas..
+00003490: 636f 6d62 6f5f 6d61 7072 4f00 0000 da03  combo_maprO.....
+000034a0: 7462 6172 b200 0000 7224 0100 0072 2b01  tbar....r$...r+.
+000034b0: 0000 7225 0100 0072 2d01 0000 7234 0000  ..r%...r-...r4..
+000034c0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+000034d0: da0c 6163 7469 6f6e 7332 6a73 6f6e 0402  ..actions2json..
+000034e0: 0000 7368 0000 0004 0404 0108 0208 010c  ..sh............
+000034f0: 010e 0204 0110 0108 0104 0106 0106 0208  ................
+00003500: 0108 ff0e 0308 010c 0108 0104 0108 0110  ................
+00003510: 0108 020c 0208 0108 0210 010a 020a 010c  ................
+00003520: 010a 0208 020c 010a 010c 0108 010a 0102  ................
+00003530: 8004 0210 010c 0114 0102 8008 020a 0208  ................
+00003540: 020c 010a 010c 0108 010a 0102 8008 027a  ...............z
+00003550: 1552 656e 6465 7265 722e 6163 7469 6f6e  .Renderer.action
+00003560: 7332 6a73 6f6e 6302 0000 0000 0000 0000  s2jsonc.........
+00003570: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
+00003580: 5800 0000 6700 7d02 6400 7d03 7c01 4400  X...g.}.d.}.|.D.
+00003590: 5d14 7d04 7c04 6401 1900 6400 7500 7213  ].}.|.d...d.u.r.
+000035a0: 7c04 6402 1900 7d03 7106 7c02 a000 7401  |.d...}.q.|...t.
+000035b0: 7c04 8301 a101 0100 7106 7402 7c02 6403  |.......q.t.|.d.
+000035c0: 6404 8400 6405 8d02 7d02 7c02 a000 6400  d...d...}.|...d.
+000035d0: 7c03 6702 a101 0100 7c02 5300 2906 4e72  |.g.....|.S.).Nr
+000035e0: 0100 0000 722c 0000 0063 0100 0000 0000  ....r,...c......
+000035f0: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+00003600: 0000 7308 0000 007c 0064 0119 0053 0029  ..s....|.d...S.)
+00003610: 024e 7201 0000 0072 3600 0000 2901 7235  .Nr....r6...).r5
+00003620: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00003630: 0000 da08 3c6c 616d 6264 613e 5002 0000  ....<lambda>P...
+00003640: 7302 0000 0008 007a 2c52 656e 6465 7265  s......z,Rendere
+00003650: 722e 6469 7370 6c61 795f 6d6f 6465 326a  r.display_mode2j
+00003660: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6c61  son.<locals>.<la
+00003670: 6d62 6461 3ea9 0172 3300 0000 2903 722c  mbda>..r3...).r,
+00003680: 0100 0072 7800 0000 da06 736f 7274 6564  ...rx.....sorted
+00003690: 2905 723f 0000 00da 0c64 6973 706c 6179  ).r?.....display
+000036a0: 5f6d 6f64 65da 0364 6d73 da03 646d 6472  _mode..dms..dmdr
+000036b0: 9200 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+000036c0: 0000 00da 1164 6973 706c 6179 5f6d 6f64  .....display_mod
+000036d0: 6532 6a73 6f6e 4802 0000 7312 0000 0004  e2jsonH...s.....
+000036e0: 0104 0108 010c 010a 0110 0210 010e 0104  ................
+000036f0: 017a 1a52 656e 6465 7265 722e 6469 7370  .z.Renderer.disp
+00003700: 6c61 795f 6d6f 6465 326a 736f 6e63 0200  lay_mode2jsonc..
+00003710: 0000 0000 0000 0000 0000 1100 0000 0800  ................
+00003720: 0000 4300 0000 73fe 0200 0074 007c 0183  ..C...s....t.|..
+00003730: 0172 0974 017c 0174 0283 0273 0b4a 0082  .r.t.|.t...s.J..
+00003740: 017c 00a0 037c 016a 04a1 015c 027d 027d  .|...|.j...\.}.}
+00003750: 0374 057c 016a 067c 027c 01a0 07a1 0074  .t.|.j.|.|.....t
+00003760: 087c 016a 0983 017c 01a0 0a74 0b83 00a1  .|.j...|...t....
+00003770: 010c 0064 018d 057d 0474 0c7c 0383 0172  ...d...}.t.|...r
+00003780: 317c 046a 0d7c 0364 028d 0101 007c 01a0  1|.j.|.d.....|..
+00003790: 0ea1 007d 057c 056a 0f64 0075 0072 4374  ...}.|.j.d.u.rCt
+000037a0: 106a 116a 12a0 1364 037c 01a1 0201 006e  .j.j...d.|.....n
+000037b0: 5d74 147c 0564 0483 0272 9767 007d 0664  ]t.|.d...r.g.}.d
+000037c0: 057d 077c 05a0 15a1 007d 087c 0844 005d  .}.|.....}.|.D.]
+000037d0: 407d 097c 00a0 167c 09a1 017d 0a7c 0a6a  @}.|...|...}.|.j
+000037e0: 0d74 177c 056a 0f6a 187c 096a 196a 1a64  .t.|.j.j.|.j.j.d
+000037f0: 0664 0784 0064 088d 037c 0717 0064 098d  .d...d...|...d..
+00003800: 0101 0074 1b7c 0974 1c83 0272 8474 1b7c  ...t.|.t...r.t.|
+00003810: 0974 1d83 0273 847c 0a6a 0d7c 0a64 0a19  .t...s.|.j.|.d..
+00003820: 0064 0b17 0064 0c8d 0101 007c 0764 0b37  .d...d.....|.d.7
+00003830: 007d 0774 1b7c 0974 1e83 0272 8d7c 0764  .}.t.|.t...r.|.d
+00003840: 0d37 007d 077c 06a0 1f7c 0aa1 0101 0071  .7.}.|...|.....q
+00003850: 527c 067c 0464 0e3c 007c 04a0 0d74 207c  R|.|.d.<.|...t |
+00003860: 056a 0f64 0f83 02a1 0101 007c 04a0 0d74  .j.d.......|...t
+00003870: 207c 0164 1083 02a1 0101 0074 147c 016a   |.d.......t.|.j
+00003880: 2164 1183 0272 b47c 046a 0d64 1264 138d  !d...r.|.j.d.d..
+00003890: 0101 007c 016a 2264 0075 0172 c17c 00a0  ...|.j"d.u.r.|..
+000038a0: 237c 016a 22a1 017c 0464 143c 007c 016a  #|.j"..|.d.<.|.j
+000038b0: 2464 0075 0172 d67c 016a 24a0 25a1 007d  $d.u.r.|.j$.%..}
+000038c0: 0b7c 0b64 0075 0172 d67c 046a 0d7c 0b6a  .|.d.u.r.|.j.|.j
+000038d0: 2664 158d 0101 007c 016a 2772 e27c 046a  &d.....|.j'r.|.j
+000038e0: 0d74 287c 016a 2783 0164 168d 0101 0074  .t(|.j'..d.....t
+000038f0: 297c 0164 1764 0083 037d 0c7c 0c64 0075  )|.d.d...}.|.d.u
+00003900: 0172 f37c 046a 0d7c 0c6a 2664 188d 0101  .r.|.j.|.j&d....
+00003910: 0074 297c 0164 1964 0083 037d 0d7c 0d64  .t)|.d.d...}.|.d
+00003920: 0075 0190 0172 057c 046a 0d7c 0d6a 2664  .u...r.|.j.|.j&d
+00003930: 1a8d 0101 0074 297c 016a 2164 1b69 0083  .....t)|.j!d.i..
+00003940: 037d 0e7c 0e90 0172 1c7c 046a 0d64 1c64  .}.|...r.|.j.d.d
+00003950: 1d84 007c 0ea0 2aa1 0044 0083 0164 1e8d  ...|..*..D...d..
+00003960: 0101 0074 106a 11a0 2b64 1fa1 0190 0172  ...t.j..+d.....r
+00003970: 3f74 297c 0164 2064 0083 0364 0075 0190  ?t)|.d d...d.u..
+00003980: 0172 3f74 147c 016a 2164 2183 0290 0172  .r?t.|.j!d!....r
+00003990: 3f7c 046a 0d74 2c6a 2da0 2e7c 016a 21a1  ?|.j.t,j-..|.j!.
+000039a0: 016a 2f64 228d 0101 0064 2344 005d 177d  .j/d"....d#D.].}
+000039b0: 0f74 297c 017c 0f64 0083 037d 107c 1064  .t)|.|.d...}.|.d
+000039c0: 0075 0190 0172 577c 04a0 0d7c 0f7c 106a  .u...rW|...|.|.j
+000039d0: 306a 3169 01a1 0101 0090 0171 417c 016a  0j1i.......qA|.j
+000039e0: 3264 0075 0190 0172 7d7c 046a 0d7c 016a  2d.u...r}|.j.|.j
+000039f0: 326a 2664 2464 2584 007c 016a 326a 336a  2j&d$d%..|.j2j3j
+00003a00: 3444 0083 0164 268d 0201 0074 147c 0164  4D...d&....t.|.d
+00003a10: 2783 0290 0172 7d7c 046a 0d7c 016a 3564  '....r}|.j.|.j5d
+00003a20: 288d 0101 007c 0453 0029 294e 2905 da02  (....|.S.))N)...
+00003a30: 6964 722f 0100 0072 9500 0000 da05 736c  idr/...r......sl
+00003a40: 6176 65da 0865 6469 7461 626c 6529 0172  ave..editable).r
+00003a50: 3001 0000 7a0f 2573 2068 6173 206e 6f20  0...z.%s has no 
+00003a60: 7374 6f72 65da 0b67 6574 5f63 6f6c 756d  store..get_colum
+00003a70: 6e73 7201 0000 0063 0100 0000 0000 0000  nsr....c........
+00003a80: 0000 0000 0100 0000 0100 0000 5300 0000  ............S...
+00003a90: 7306 0000 007c 006a 0053 0072 3a00 0000  s....|.j.S.r:...
+00003aa0: a901 7252 0000 00a9 0172 8c00 0000 7236  ..rR.....r....r6
+00003ab0: 0000 0072 3600 0000 7237 0000 0072 3701  ...r6...r7...r7.
+00003ac0: 0000 6d02 0000 7302 0000 0006 007a 2552  ..m...s......z%R
+00003ad0: 656e 6465 7265 722e 6163 746f 7232 6a73  enderer.actor2js
+00003ae0: 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  on.<locals>.<lam
+00003af0: 6264 613e 7238 0100 0029 01da 0c66 6965  bda>r8...)...fie
+00003b00: 6c64 735f 696e 6465 7872 4401 0000 722c  lds_indexrD...r,
+00003b10: 0000 0029 01da 1366 6965 6c64 735f 696e  ...)...fields_in
+00003b20: 6465 785f 6869 6464 656e e902 0000 00da  dex_hidden......
+00003b30: 0363 6f6c da08 706b 5f69 6e64 6578 7ad0  .col..pk_indexz.
+00003b40: 7072 6576 6965 775f 6c69 6d69 7420 7573  preview_limit us
+00003b50: 655f 6465 7461 696c 5f70 6172 616d 5f70  e_detail_param_p
+00003b60: 616e 656c 2075 7365 5f64 6574 6169 6c5f  anel use_detail_
+00003b70: 7061 7261 6d73 5f76 616c 7565 2068 6964  params_value hid
+00003b80: 655f 6e61 7669 6761 746f 7220 7573 655f  e_navigator use_
+00003b90: 6465 7461 696c 5f70 6172 616d 735f 7661  detail_params_va
+00003ba0: 6c75 6520 7265 6163 745f 7265 7370 6f6e  lue react_respon
+00003bb0: 7369 7665 206d 6178 5f72 656e 6465 725f  sive max_render_
+00003bc0: 6465 7074 6820 7369 6d70 6c65 5f73 6c61  depth simple_sla
+00003bd0: 7665 6772 6964 5f68 6561 6465 7220 7061  vegrid_header pa
+00003be0: 6769 6e61 746f 725f 7465 6d70 6c61 7465  ginator_template
+00003bf0: 2068 6964 655f 746f 705f 746f 6f6c 6261   hide_top_toolba
+00003c00: 7220 6869 6465 5f69 665f 656d 7074 7920  r hide_if_empty 
+00003c10: da04 6669 6c65 5429 01da 0d63 6f6e 7461  ..fileT)...conta
+00003c20: 696e 5f6d 6564 6961 723a 0100 0072 2301  in_mediar:...r#.
+00003c30: 0000 2901 da0d 6163 7469 7665 5f66 6965  ..)...active_fie
+00003c40: 6c64 73da 0b63 6172 645f 6c61 796f 7574  lds..card_layout
+00003c50: 2901 724c 0100 00da 0b6c 6973 745f 6c61  ).rL.....list_la
+00003c60: 796f 7574 2901 724d 0100 00da 0e5f 6368  yout).rM....._ch
+00003c70: 6f6f 7365 7273 5f64 6963 7463 0100 0000  oosers_dictc....
+00003c80: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+00003c90: 5300 0000 7322 0000 0069 007c 005d 0d5c  S...s"...i.|.].\
+00003ca0: 027d 017d 027c 0164 0064 0184 007c 026a  .}.}.|.d.d...|.j
+00003cb0: 0044 0083 0193 0271 0253 0029 0263 0100  .D.....q.S.).c..
+00003cc0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00003cd0: 0000 5300 0000 f312 0000 0067 007c 005d  ..S........g.|.]
+00003ce0: 057d 017c 016a 0091 0271 0253 0072 3600  .}.|.j...q.S.r6.
+00003cf0: 0000 7242 0100 0029 0272 4600 0000 da02  ..rB...).rF.....
+00003d00: 6366 7236 0000 0072 3600 0000 7237 0000  cfr6...r6...r7..
+00003d10: 0072 4800 0000 a302 0000 f302 0000 0012  .rH.............
+00003d20: 007a 3252 656e 6465 7265 722e 6163 746f  .z2Renderer.acto
+00003d30: 7232 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e  r2json.<locals>.
+00003d40: 3c64 6963 7463 6f6d 703e 2e3c 6c69 7374  <dictcomp>.<list
+00003d50: 636f 6d70 3e29 01da 0e63 6f6e 7465 7874  comp>)...context
+00003d60: 5f66 6965 6c64 7329 0372 4600 0000 da02  _fields).rF.....
+00003d70: 666e 7247 0000 0072 3600 0000 7236 0000  fnrG...r6...r6..
+00003d80: 0072 3700 0000 724c 0000 00a3 0200 0073  .r7...rL.......s
+00003d90: 0600 0000 0600 0601 16ff 7a27 5265 6e64  ..........z'Rend
+00003da0: 6572 6572 2e61 6374 6f72 326a 736f 6e2e  erer.actor2json.
+00003db0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+00003dc0: 6d70 3e29 01da 0c63 686f 6f73 6572 5f64  mp>)...chooser_d
+00003dd0: 6963 74da 0c63 6f6e 7465 6e74 7479 7065  ict..contenttype
+00003de0: 73da 056d 6f64 656c da05 5f6d 6574 6129  s..model.._meta)
+00003df0: 01da 0c63 6f6e 7465 6e74 5f74 7970 6529  ...content_type)
+00003e00: 03da 0d64 6574 6169 6c5f 6163 7469 6f6e  ...detail_action
+00003e10: da0d 696e 7365 7274 5f61 6374 696f 6eda  ..insert_action.
+00003e20: 0e64 6566 6175 6c74 5f61 6374 696f 6e63  .default_actionc
+00003e30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003e40: 0300 0000 5300 0000 724f 0100 0072 3600  ....S...rO...r6.
+00003e50: 0000 7242 0100 0029 0272 4600 0000 728c  ..rB...).rF...r.
+00003e60: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00003e70: 0000 7248 0000 00b3 0200 0072 5101 0000  ..rH.......rQ...
+00003e80: 7a27 5265 6e64 6572 6572 2e61 6374 6f72  z'Renderer.actor
+00003e90: 326a 736f 6e2e 3c6c 6f63 616c 733e 2e3c  2json.<locals>.<
+00003ea0: 6c69 7374 636f 6d70 3e29 02da 0d70 6172  listcomp>)...par
+00003eb0: 616d 735f 6c61 796f 7574 da0d 7061 7261  ams_layout..para
+00003ec0: 6d73 5f66 6965 6c64 73da 1070 6172 616d  ms_fields..param
+00003ed0: 735f 7061 6e65 6c5f 706f 7329 0172 5e01  s_panel_pos).r^.
+00003ee0: 0000 2936 722b 0000 0072 b400 0000 721b  ..)6r+...r....r.
+00003ef0: 0000 0072 3601 0000 da0d 5f61 6374 696f  ...r6....._actio
+00003f00: 6e73 5f6c 6973 7472 7100 0000 72ef 0000  ns_listrq...r...
+00003f10: 00da 0f67 6574 5f61 6374 6f72 5f6c 6162  ...get_actor_lab
+00003f20: 656c da04 626f 6f6c da06 6d61 7374 6572  el..bool..master
+00003f30: da0c 6869 6465 5f65 6469 7469 6e67 7229  ..hide_editingr)
+00003f40: 0000 0072 d100 0000 7277 0000 00da 0a67  ...r....rw.....g
+00003f50: 6574 5f68 616e 646c 65da 0573 746f 7265  et_handle..store
+00003f60: 7204 0000 0072 6f00 0000 da06 6c6f 6767  r....ro.....logg
+00003f70: 6572 da07 7761 726e 696e 6772 8200 0000  er..warningr....
+00003f80: 7241 0100 0072 aa00 0000 7238 0000 00da  rA...r....r8....
+00003f90: 0b6c 6973 745f 6669 656c 6473 72b6 0000  .list_fieldsr...
+00003fa0: 0072 5200 0000 72a0 0000 0072 1f00 0000  .rR...r....r....
+00003fb0: 7220 0000 0072 2200 0000 722c 0100 0072  r ...r"...r,...r
+00003fc0: 2800 0000 7256 0100 0072 3a01 0000 723d  (...rV...r:...r=
+00003fd0: 0100 0072 5901 0000 da11 6765 745f 7769  ...rY.....get_wi
+00003fe0: 6e64 6f77 5f6c 6179 6f75 7472 8700 0000  ndow_layoutr....
+00003ff0: 724b 0100 0072 7800 0000 7201 0100 0072  rK...rx...r....r
+00004000: 6800 0000 7276 0000 0072 0e00 0000 da07  h...rv...r......
+00004010: 6f62 6a65 6374 73da 0d67 6574 5f66 6f72  objects..get_for
+00004020: 5f6d 6f64 656c 72d8 0000 0072 6c00 0000  _modelr....rl...
+00004030: 724d 0000 0072 5c01 0000 da0c 7061 7261  rM...r\.....para
+00004040: 6d73 5f73 746f 7265 da0c 7061 7261 6d5f  ms_store..param_
+00004050: 6669 656c 6473 725e 0100 0029 1172 3f00  fieldsr^...).r?.
+00004060: 0000 72a5 0000 00da 0261 6cda 0268 6b72  ..r......al..hkr
+00004070: a600 0000 da02 6168 da07 636f 6c75 6d6e  ......ah..column
+00004080: 73da 0969 6e64 6578 5f6d 6f64 da09 636f  s..index_mod..co
+00004090: 6c5f 656c 656d 7372 4701 0000 720b 0100  l_elemsrG...r...
+000040a0: 00da 0277 6c72 4c01 0000 724d 0100 0072  ...wlrL...rM...r
+000040b0: 5401 0000 72b7 0000 0072 8f00 0000 7236  T...r....r....r6
+000040c0: 0000 0072 3600 0000 7237 0000 00da 0a61  ...r6...r7.....a
+000040d0: 6374 6f72 326a 736f 6e54 0200 0073 8e00  ctor2jsonT...s..
+000040e0: 0000 1601 1001 0601 0201 0601 0801 0c01  ................
+000040f0: 06fc 0807 0c01 0802 0a01 1201 0a03 0401  ................
+00004100: 0401 0801 0801 0a01 1201 0601 04ff 0201  ................
+00004110: 08ff 1402 1403 0801 0a01 0801 0c01 0801  ................
+00004120: 1205 1001 0c0d 0c01 0a02 1001 0a02 0a01  ................
+00004130: 0801 0e01 0602 1201 0c02 0801 0e01 0c02  ................
+00004140: 0a01 0e02 0e03 0601 0a01 0601 0aff 2603  ..............&.
+00004150: 0201 06ff 1803 0801 0c01 0a01 1201 0480  ................
+00004160: 0c02 0402 0601 1201 06fe 0c04 0e01 0401  ................
+00004170: 7a13 5265 6e64 6572 6572 2e61 6374 6f72  z.Renderer.actor
+00004180: 326a 736f 6e63 0200 0000 0000 0000 0000  2jsonc..........
+00004190: 0000 0400 0000 0600 0000 0300 0000 7364  ..............sd
+000041a0: 0000 0064 0188 015f 0088 016a 0144 005d  ...d..._...j.D.]
+000041b0: 2289 0088 006a 0264 0075 0172 0e71 0674  "....j.d.u.r.q.t
+000041c0: 036a 046a 0588 01a0 0688 006a 07a1 018e  .j.j.......j....
+000041d0: 007d 0287 0087 0166 0264 0264 0384 087d  .}.....f.d.d...}
+000041e0: 0374 086a 096a 0aa0 0b7c 027c 037c 01a1  .t.j.j...|.|.|..
+000041f0: 0301 0071 0664 0488 015f 0074 0c83 00a0  ...q.d..._.t....
+00004200: 0d7c 01a1 0153 0029 054e 5463 0100 0000  .|...S.).NTc....
+00004210: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00004220: 1300 0000 7318 0000 007c 00a0 0074 0188  ....s....|...t..
+00004230: 01a0 0288 00a1 0183 01a1 0101 0064 0053  .............d.S
+00004240: 0072 3a00 0000 2903 728b 0000 0072 2600  .r:...).r....r&.
+00004250: 0000 7275 0100 0072 4301 0000 a902 7298  ..ru...rC.....r.
+00004260: 0000 0072 3f00 0000 7236 0000 0072 3700  ...r?...r6...r7.
+00004270: 0000 728b 0000 00c2 0200 0073 0200 0000  ..r........s....
+00004280: 1801 7a26 5265 6e64 6572 6572 2e62 7569  ..z&Renderer.bui
+00004290: 6c64 5f6a 735f 6361 6368 652e 3c6c 6f63  ld_js_cache.<loc
+000042a0: 616c 733e 2e77 7269 7465 4629 0e72 6e00  als>.writeF).rn.
+000042b0: 0000 726a 0000 00da 0f67 6574 5f68 616e  ..rj.....get_han
+000042c0: 646c 655f 6e61 6d65 727d 0000 00da 0470  dle_namer}.....p
+000042d0: 6174 68da 046a 6f69 6e72 2201 0000 72ef  ath..joinr"...r.
+000042e0: 0000 0072 0400 0000 726f 0000 0072 2300  ...r....ro...r#.
+000042f0: 0000 da0f 6d61 6b65 5f63 6163 6865 5f66  ....make_cache_f
+00004300: 696c 6572 3b00 0000 da0e 6275 696c 645f  iler;.....build_
+00004310: 6a73 5f63 6163 6865 2904 723f 0000 00da  js_cache).r?....
+00004320: 0566 6f72 6365 7253 0100 0072 8b00 0000  .forcerS...r....
+00004330: 7241 0000 0072 7601 0000 7237 0000 0072  rA...rv...r7...r
+00004340: 7b01 0000 b902 0000 7312 0000 0006 020a  {.......s.......
+00004350: 020a 0102 0114 010e 0214 0306 020c 017a  ...............z
+00004360: 1752 656e 6465 7265 722e 6275 696c 645f  .Renderer.build_
+00004370: 6a73 5f63 6163 6865 723a 0000 0029 2072  js_cacher:...) r
+00004380: b300 0000 da0a 5f5f 6d6f 6475 6c65 5f5f  ......__module__
+00004390: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+000043a0: 5f5f 646f 635f 5fda 0e69 735f 696e 7465  __doc__..is_inte
+000043b0: 7261 6374 6976 65da 0863 616e 5f61 7574  ractive..can_aut
+000043c0: 6872 1d01 0000 7221 0100 00da 1873 7570  hr....r!.....sup
+000043d0: 706f 7274 5f64 6173 6862 6f61 7264 5f6c  port_dashboard_l
+000043e0: 6179 6f75 7472 3c00 0000 7293 0000 0072  ayoutr<...r....r
+000043f0: 4e00 0000 7286 0000 0072 aa00 0000 72b8  N...r....r....r.
+00004400: 0000 0072 ce00 0000 72db 0000 0072 e200  ...r....r....r..
+00004410: 0000 72a4 0000 0072 de00 0000 723e 0000  ..r....r....r>..
+00004420: 0072 fd00 0000 72fe 0000 0072 ff00 0000  .r....r....r....
+00004430: 7213 0100 0072 1901 0000 7222 0100 0072  r....r....r"...r
+00004440: 3601 0000 723d 0100 0072 7501 0000 727b  6...r=...ru...r{
+00004450: 0100 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00004460: 5f5f 7236 0000 0072 3600 0000 7241 0000  __r6...r6...rA..
+00004470: 0072 3700 0000 7239 0000 003a 0000 0073  .r7...r9...:...s
+00004480: 3c00 0000 0800 0401 0403 0401 0402 0401  <...............
+00004490: 0401 0c02 0804 0855 081d 0808 081f 0803  .......U........
+000044a0: 0a18 0212 0aff 0815 080e 0821 084e 080e  ...........!.N..
+000044b0: 080a 082a 0809 080f 080a 0844 080c 1465  ...*.......D...e
+000044c0: 7239 0000 0072 3a00 0000 2946 727d 0000  r9...r:...)Fr}..
+000044d0: 00da 0770 6174 686c 6962 7202 0000 00da  ...pathlibr.....
+000044e0: 0468 746d 6c72 0300 0000 da0b 646a 616e  .htmlr......djan
+000044f0: 676f 2e63 6f6e 6672 0400 0000 da09 646a  go.confr......dj
+00004500: 616e 676f 2e64 6272 0500 0000 da11 646a  ango.dbr......dj
+00004510: 616e 676f 2e75 7469 6c73 2e74 6578 7472  ango.utils.textr
+00004520: 0600 0000 da0c 646a 616e 676f 2e75 7469  ......django.uti
+00004530: 6c73 7207 0000 00da 126c 696e 6f2e 636f  lsr......lino.co
+00004540: 7265 2e72 656e 6465 7265 7272 0800 0000  re.rendererr....
+00004550: 7209 0000 00da 0f6c 696e 6f2e 636f 7265  r......lino.core
+00004560: 2e6d 656e 7573 720a 0000 0072 0b00 0000  .menusr....r....
+00004570: da09 6c69 6e6f 2e63 6f72 6572 0c00 0000  ..lino.corer....
+00004580: 720d 0000 00da 0e6c 696e 6f2e 636f 7265  r......lino.core
+00004590: 2e67 666b 7372 0e00 0000 da1e 6c69 6e6f  .gfksr......lino
+000045a0: 2e6d 6f64 6c69 622e 6578 746a 732e 6578  .modlib.extjs.ex
+000045b0: 745f 7265 6e64 6572 6572 720f 0000 00da  t_rendererr.....
+000045c0: 116c 696e 6f2e 636f 7265 2e61 6374 696f  .lino.core.actio
+000045d0: 6e73 7210 0000 0072 1100 0000 7212 0000  nsr....r....r...
+000045e0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+000045f0: 7216 0000 0072 1700 0000 da15 6c69 6e6f  r....r......lino
+00004600: 2e63 6f72 652e 626f 756e 6461 6374 696f  .core.boundactio
+00004610: 6e72 1800 0000 da15 6c69 6e6f 2e63 6f72  nr......lino.cor
+00004620: 652e 6368 6f69 6365 6c69 7374 7372 1900  e.choicelistsr..
+00004630: 0000 da1e 6c69 6e6f 2e6d 6f64 6c69 622e  ....lino.modlib.
+00004640: 7379 7374 656d 2e63 686f 6963 656c 6973  system.choicelis
+00004650: 7473 721a 0000 00da 106c 696e 6f2e 636f  tsr......lino.co
+00004660: 7265 2e61 6374 6f72 7372 1b00 0000 da11  re.actorsr......
+00004670: 6c69 6e6f 2e63 6f72 652e 6c61 796f 7574  lino.core.layout
+00004680: 7372 1c00 0000 721d 0000 00da 0f6c 696e  sr....r......lin
+00004690: 6f2e 636f 7265 2e65 6c65 6d73 721e 0000  o.core.elemsr...
+000046a0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+000046b0: 7222 0000 0072 2300 0000 da0a 6574 6765  r"...r#.....etge
+000046c0: 6e2e 6874 6d6c 7224 0000 00da 0a6c 696e  n.htmlr$.....lin
+000046d0: 6f2e 7574 696c 7372 2500 0000 da10 6c69  o.utilsr%.....li
+000046e0: 6e6f 2e75 7469 6c73 2e6a 7367 656e 7226  no.utils.jsgenr&
+000046f0: 0000 0072 2700 0000 7228 0000 00da 176c  ...r'...r(.....l
+00004700: 696e 6f2e 6d6f 646c 6962 2e75 7365 7273  ino.modlib.users
+00004710: 2e75 7469 6c73 7229 0000 0072 2a00 0000  .utilsr)...r*...
+00004720: da07 696e 7370 6563 7472 2b00 0000 da05  ..inspectr+.....
+00004730: 6963 6f6e 7372 2d00 0000 7238 0000 0072  iconsr-...r8...r
+00004740: 3900 0000 7236 0000 0072 3600 0000 7236  9...r6...r6...r6
+00004750: 0000 0072 3700 0000 da08 3c6d 6f64 756c  ...r7.....<modul
+00004760: 653e 0100 0000 733a 0000 0008 040c 010c  e>....s:........
+00004770: 010c 010c 010c 010c 0110 0210 020c 010c  ................
+00004780: 010c 010c 0128 020c 030c 010c 010c 0110  .....(..........
+00004790: 011c 010c 020c 020c 0214 0110 020c 020c  ................
+000047a0: 020a 0314 0d                             .....
```

### Comparing `lino_react-23.6.1/lino_react/react/__pycache__/views.cpython-310.pyc` & `lino_react-23.6.2/lino_react/react/__pycache__/views.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar 24 10:38:37 2023 UTC, .py size: 28705 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ad7d 1d64 2170 0000  o........}.d!p..
+00000000: 6f0d 0d0a 0000 0000 6be5 8564 2170 0000  o.......k..d!p..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0e03 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6401 6403 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6401 6404 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
@@ -106,1183 +106,1184 @@
 00000690: 7461 6b65 7320 7468 6520 6974 7465 7227  takes the itter'
 000006a0: 7320 6974 656d 2061 6e64 2072 6574 7572  s item and retur
 000006b0: 6e73 2074 6861 7420 7761 6e74 6564 206d  ns that wanted m
 000006c0: 6174 6368 6564 2069 7465 6de9 ffff ffff  atched item.....
 000006d0: 2902 da08 6361 6c6c 6162 6c65 da09 656e  )...callable..en
 000006e0: 756d 6572 6174 6529 05da 0569 7474 6572  umerate)...itter
 000006f0: da06 7461 7267 6574 da03 6b65 79da 0169  ..target..key..i
-00000700: da01 78a9 0072 3600 0000 fa2e 2f68 6f6d  ..x..r6...../hom
-00000710: 652f 6c75 632f 776f 726b 2f72 6561 6374  e/luc/work/react
-00000720: 2f6c 696e 6f5f 7265 6163 742f 7265 6163  /lino_react/reac
-00000730: 742f 7669 6577 732e 7079 da04 6669 6e64  t/views.py..find
-00000740: 3800 0000 7310 0000 0018 0210 0204 0108  8...s...........
-00000750: 0108 0108 0102 ff04 0372 3800 0000 7a21  .........r8...z!
-00000760: 2573 2068 6173 206e 6f20 726f 7720 7769  %s has no row wi
-00000770: 7468 2070 7269 6d61 7279 206b 6579 2025  th primary key %
-00000780: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-00000790: 0000 0300 0000 4000 0000 732a 0000 0065  ......@...s*...e
-000007a0: 005a 0164 005a 0264 0864 0264 0384 015a  .Z.d.Z.d.d.d...Z
-000007b0: 0364 0864 0464 0584 015a 0464 0864 0664  .d.d.d...Z.d.d.d
-000007c0: 0784 015a 0564 0153 0029 0972 2b00 0000  ...Z.d.S.).r+...
-000007d0: 4e63 0500 0000 0000 0000 0000 0000 0800  Nc..............
-000007e0: 0000 0800 0000 4300 0000 7354 0000 007c  ......C...sT...|
-000007f0: 016a 007d 0574 017c 027c 037c 017c 0564  .j.}.t.|.|.|.|.d
-00000800: 0174 026a 036a 046a 056a 0664 028d 067d  .t.j.j.j.j.d...}
-00000810: 067c 0464 036b 0272 1e7c 06a0 07a1 007d  .|.d.k.r.|.....}
-00000820: 077c 0767 017c 065f 086e 057c 06a0 097c  .|.g.|._.n.|...|
-00000830: 04a1 0101 0074 026a 036a 0aa0 0b7c 06a1  .....t.j.j...|..
-00000840: 0153 0029 044e 54a9 01da 0872 656e 6465  .S.).NT....rende
-00000850: 7265 72fa 062d 3939 3939 3829 0cda 0450  rer..-99998)...P
-00000860: 4f53 5472 2000 0000 720b 0000 00da 0453  OSTr ...r......S
-00000870: 4954 45da 0770 6c75 6769 6e73 da05 7265  ITE..plugins..re
-00000880: 6163 7472 3a00 0000 da0f 6372 6561 7465  actr:.....create
-00000890: 5f69 6e73 7461 6e63 65da 0d73 656c 6563  _instance..selec
-000008a0: 7465 645f 726f 7773 da10 7365 745f 7365  ted_rows..set_se
-000008b0: 6c65 6374 6564 5f70 6b73 7226 0000 00da  lected_pksr&....
-000008c0: 0a72 756e 5f61 6374 696f 6e29 08da 0473  .run_action)...s
-000008d0: 656c 66da 0772 6571 7565 7374 da09 6170  elf..request..ap
-000008e0: 705f 6c61 6265 6cda 0561 6374 6f72 da02  p_label..actor..
-000008f0: 706b da04 6461 7461 da02 6172 da04 656c  pk..data..ar..el
-00000900: 656d 7236 0000 0072 3600 0000 7237 0000  emr6...r6...r7..
-00000910: 00da 0470 6f73 744f 0000 0073 1400 0000  ...postO...s....
-00000920: 0602 0201 0a01 0a01 06fe 0803 0801 0a01  ................
-00000930: 0a02 0e01 7a0f 4170 6945 6c65 6d65 6e74  ....z.ApiElement
-00000940: 2e70 6f73 7463 0500 0000 0000 0000 0000  .postc..........
-00000950: 0000 0700 0000 0800 0000 4300 0000 f340  ..........C....@
-00000960: 0000 0074 00a0 017c 016a 02a1 017d 0574  ...t...|.j...}.t
-00000970: 037c 027c 037c 017c 0564 0174 046a 056a  .|.|.|.|.d.t.j.j
-00000980: 066a 076a 0864 028d 067d 067c 06a0 097c  .j.j.d...}.|...|
-00000990: 04a1 0101 0074 046a 056a 0aa0 0b7c 06a1  .....t.j.j...|..
-000009a0: 0153 00a9 034e 4672 3900 0000 a90c 7209  .S...NFr9.....r.
-000009b0: 0000 00da 0951 7565 7279 4469 6374 da04  .....QueryDict..
-000009c0: 626f 6479 7220 0000 0072 0b00 0000 723d  bodyr ...r....r=
-000009d0: 0000 0072 3e00 0000 723f 0000 0072 3a00  ...r>...r?...r:.
-000009e0: 0000 7242 0000 0072 2600 0000 7243 0000  ..rB...r&...rC..
-000009f0: 00a9 0772 4400 0000 7245 0000 0072 4600  ...rD...rE...rF.
-00000a00: 0000 7247 0000 0072 4800 0000 7249 0000  ..rG...rH...rI..
-00000a10: 0072 4a00 0000 7236 0000 0072 3600 0000  .rJ...r6...r6...
-00000a20: 7237 0000 00da 0370 7574 5c00 0000 730e  r7.....put\...s.
-00000a30: 0000 000c 0102 030a 010a 0106 fe0a 030e  ................
-00000a40: 017a 0e41 7069 456c 656d 656e 742e 7075  .z.ApiElement.pu
-00000a50: 7463 0500 0000 0000 0000 0000 0000 0700  tc..............
-00000a60: 0000 0800 0000 4300 0000 724d 0000 0072  ......C...rM...r
-00000a70: 4e00 0000 724f 0000 0072 5200 0000 7236  N...rO...rR...r6
-00000a80: 0000 0072 3600 0000 7237 0000 00da 0664  ...r6...r7.....d
-00000a90: 656c 6574 6566 0000 0073 0e00 0000 0c01  eletef...s......
-00000aa0: 0201 0a01 0a01 06fe 0a03 0e01 7a11 4170  ............z.Ap
-00000ab0: 6945 6c65 6d65 6e74 2e64 656c 6574 65a9  iElement.delete.
-00000ac0: 034e 4e4e 2906 da08 5f5f 6e61 6d65 5f5f  .NNN)...__name__
-00000ad0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000ae0: 7175 616c 6e61 6d65 5f5f 724c 0000 0072  qualname__rL...r
-00000af0: 5300 0000 7254 0000 0072 3600 0000 7236  S...rT...r6...r6
-00000b00: 0000 0072 3600 0000 7237 0000 0072 2b00  ...r6...r7...r+.
-00000b10: 0000 4d00 0000 7308 0000 0008 000a 020a  ..M...s.........
-00000b20: 0d0e 0a72 2b00 0000 6300 0000 0000 0000  ...r+...c.......
-00000b30: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000b40: 0073 2000 0000 6500 5a01 6400 5a02 6406  .s ...e.Z.d.Z.d.
-00000b50: 6402 6403 8401 5a03 6406 6404 6405 8401  d.d...Z.d.d.d...
-00000b60: 5a04 6401 5300 2907 da07 4170 694c 6973  Z.d.S.)...ApiLis
-00000b70: 744e 6304 0000 0000 0000 0000 0000 0005  tNc.............
-00000b80: 0000 0006 0000 0043 0000 0073 3400 0000  .......C...s4...
-00000b90: 7400 7c02 7c03 7c01 7c01 6a01 6401 8305  t.|.|.|.|.j.d...
-00000ba0: 7d04 7c04 a002 a100 0100 7403 6a04 6a05  }.|.......t.j.j.
-00000bb0: 6a06 7c04 5f07 7403 6a04 6a05 a008 7c04  j.|._.t.j.j...|.
-00000bc0: a101 5300 2902 4e54 2909 7220 0000 0072  ..S.).NT).r ...r
-00000bd0: 3c00 0000 da0a 6765 745f 7374 6174 7573  <.....get_status
-00000be0: 720b 0000 0072 3d00 0000 7226 0000 00da  r....r=...r&....
-00000bf0: 1064 6566 6175 6c74 5f72 656e 6465 7265  .default_rendere
-00000c00: 7272 3a00 0000 7243 0000 0029 0572 4400  rr:...rC...).rD.
-00000c10: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-00000c20: 0072 4a00 0000 7236 0000 0072 3600 0000  .rJ...r6...r6...
-00000c30: 7237 0000 0072 4c00 0000 7000 0000 7308  r7...rL...p...s.
-00000c40: 0000 0012 0108 010c 010e 017a 0c41 7069  ...........z.Api
-00000c50: 4c69 7374 2e70 6f73 7463 0400 0000 0000  List.postc......
-00000c60: 0000 0000 0000 1300 0000 0800 0000 0300  ................
-00000c70: 0000 7376 0200 0074 007c 0183 017d 047c  ..sv...t.|...}.|
-00000c80: 0472 0a74 017c 0483 0153 0074 027c 027c  .r.t.|...S.t.|.|
-00000c90: 037c 017c 016a 0364 0183 0589 0088 00a0  .|.|.j.d........
-00000ca0: 04a1 0073 2064 02a0 0588 00a1 017d 0574  ...s d.......}.t
-00000cb0: 067c 0583 0182 0174 076a 086a 096a 0a88  .|.....t.j.j.j..
-00000cc0: 005f 0b88 006a 0c89 027c 016a 03a0 0d74  ._...j...|.j...t
-00000cd0: 0e6a 0f88 006a 106a 116a 12a1 027d 067c  .j...j.j.j...}.|
-00000ce0: 016a 03a0 0d74 0e6a 13a1 017d 077c 0772  .j...t.j...}.|.r
-00000cf0: 4474 076a 086a 09a0 1488 00a1 0153 007c  Dt.j.j.......S.|
-00000d00: 0674 0e6a 156b 0290 0172 3474 1688 006a  .t.j.k...r4t...j
-00000d10: 106a 1174 1783 0272 6088 00a0 18a1 007d  .j.t...r`......}
-00000d20: 0874 1988 0088 006a 0c7c 0883 037d 0974  .t.....j.|...}.t
-00000d30: 017c 0983 0153 007c 016a 03a0 0d74 0e6a  .|...S.|.j...t.j
-00000d40: 1a74 0e6a 1ba1 0289 0188 0174 0e6a 1c6b  .t.j.......t.j.k
-00000d50: 0272 8864 037d 0a67 007d 0b88 006a 1d44  .r.d.}.g.}...j.D
-00000d60: 005d 117d 0c7c 0a7c 0ca0 1e88 00a1 0137  .].}.|.|.......7
-00000d70: 007d 0a7c 0ba0 1f64 047c 0c6a 2069 01a1  .}.|...d.|.j i..
-00000d80: 0101 0071 756e 4088 0174 0e6a 216b 0272  ...qun@..t.j!k.r
-00000d90: b464 037d 0a67 007d 0b88 006a 1d44 005d  .d.}.g.}...j.D.]
-00000da0: 1e7d 0c88 00a0 227c 0ca1 017d 0d88 00a0  .}...."|...}....
-00000db0: 237c 0c7c 0da1 027d 0d64 05a0 057c 0da1  #|.|...}.d...|..
-00000dc0: 017d 0d7c 0a7c 0d37 007d 0a7c 0ba0 1f64  .}.|.|.7.}.|...d
-00000dd0: 047c 0c6a 2069 01a1 0101 0071 946e 1464  .|.j i.....q.n.d
-00000de0: 007d 0a87 0187 0266 0264 0664 0784 0889  .}.....f.d.d....
-00000df0: 0387 0087 0366 0264 0864 0984 0888 006a  .....f.d.d.....j
-00000e00: 1d44 0083 017d 0b88 00a0 24a1 007d 0e88  .D...}....$..}..
-00000e10: 0174 0e6a 1b6b 0272 fb88 00a0 25a1 0044  .t.j.k.r....%..D
-00000e20: 005d 257d 0f88 006a 2664 0075 0073 ec74  .]%}...j&d.u.s.t
-00000e30: 277c 0b83 0164 0a17 0088 006a 266b 0073  '|...d.....j&k.s
-00000e40: ec88 006a 267c 0e64 0a17 006b 0272 f688  ...j&|.d...k.r..
-00000e50: 0388 007c 0f83 027d 107c 0ba0 1f7c 10a1  ...|...}.|...|..
-00000e60: 0101 007c 0e64 0a37 007d 0e71 d574 287c  ...|.d.7.}.q.t(|
-00000e70: 0e7c 0b7c 0a64 0188 006a 2988 00a0 2aa1  .|.|.d...j)...*.
-00000e80: 0064 0b8d 067d 1188 0174 0e6a 1b6b 0390  .d...}...t.j.k..
-00000e90: 0172 1d88 00a0 2ba1 007d 127c 1264 0075  .r....+..}.|.d.u
-00000ea0: 0190 0172 1d7c 0ba0 2c64 0c7c 12a1 0201  ...r.|..,d.|....
-00000eb0: 0088 006a 2d6a 2e90 0172 307c 116a 2f88  ...j-j...r0|.j/.
-00000ec0: 006a 2d6a 306a 31a0 3288 0088 006a 33a1  .j-j0j1.2....j3.
-00000ed0: 0264 0d8d 0101 0074 017c 1183 0153 0074  .d.....t.|...S.t
-00000ee0: 076a 086a 09a0 1488 00a1 0153 0029 0e4e  .j.j.......S.).N
-00000ef0: 547a 174e 6f20 7065 726d 6973 7369 6f6e  Tz.No permission
-00000f00: 2074 6f20 7275 6e20 7b7d da00 da02 6964   to run {}....id
-00000f10: 7a09 3c70 3e7b 7d3c 2f70 3e63 0200 0000  z.<p>{}</p>c....
-00000f20: 0000 0000 0000 0000 0300 0000 0700 0000  ................
-00000f30: 1300 0000 7362 0000 0088 0074 006a 016b  ....sb.....t.j.k
-00000f40: 0272 0c88 016a 02a0 037c 007c 01a1 0253  .r...j...|.|...S
-00000f50: 0088 0074 006a 046b 0272 167c 01a0 057c  ...t.j.k.r.|...|
-00000f60: 00a1 0153 0088 0074 006a 066b 0272 2088  ...S...t.j.k.r .
-00000f70: 016a 026a 077d 026e 0488 016a 026a 087d  .j.j.}.n...j.j.}
-00000f80: 0288 016a 026a 097c 007c 017c 027c 00a0  ...j.j.|.|.|.|..
-00000f90: 0a7c 01a1 0164 018d 0453 0029 027a 4f55  .|...d...S.).zOU
-00000fa0: 7365 2064 6973 706c 6179 5f6d 6f64 6520  se display_mode 
-00000fb0: 746f 2064 6574 6572 6d69 6e65 2077 6869  to determine whi
-00000fc0: 6368 2073 6572 696c 6973 6174 696f 6e20  ch serilisation 
-00000fd0: 7374 6f72 6520 6d65 7468 6f64 2061 6e64  store method and
-00000fe0: 2066 6965 6c64 7320 746f 2075 7365 2902   fields to use).
-00000ff0: 7216 0000 00da 0a63 6172 645f 7469 746c  r......card_titl
-00001000: 6529 0b72 1b00 0000 da12 4449 5350 4c41  e).r......DISPLA
-00001010: 595f 4d4f 4445 5f54 4142 4c45 da05 7374  Y_MODE_TABLE..st
-00001020: 6f72 65da 0872 6f77 326c 6973 74da 1444  ore..row2list..D
-00001030: 4953 504c 4159 5f4d 4f44 455f 4741 4c4c  ISPLAY_MODE_GALL
-00001040: 4552 59da 1067 6574 5f67 616c 6c65 7279  ERY..get_gallery
-00001050: 5f69 7465 6dda 1244 4953 504c 4159 5f4d  _item..DISPLAY_M
-00001060: 4f44 455f 4341 5244 53da 0b63 6172 645f  ODE_CARDS..card_
-00001070: 6669 656c 6473 da0d 6465 7461 696c 5f66  fields..detail_f
-00001080: 6965 6c64 73da 0872 6f77 3264 6963 74da  ields..row2dict.
-00001090: 0e67 6574 5f63 6172 645f 7469 746c 6529  .get_card_title)
-000010a0: 0372 4a00 0000 da03 726f 7772 1600 0000  .rJ.....rowr....
-000010b0: 2902 da0c 6469 7370 6c61 795f 6d6f 6465  )...display_mode
-000010c0: da02 7268 7236 0000 0072 3700 0000 da09  ..rhr6...r7.....
-000010d0: 7365 7269 616c 697a 65b3 0000 0073 1400  serialize....s..
-000010e0: 0000 0a02 0e01 0a01 0a02 0a02 0a01 0802  ................
-000010f0: 0801 0c01 06ff 7a1e 4170 694c 6973 742e  ......z.ApiList.
-00001100: 6765 742e 3c6c 6f63 616c 733e 2e73 6572  get.<locals>.ser
-00001110: 6961 6c69 7a65 6301 0000 0000 0000 0000  ializec.........
-00001120: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-00001130: 1600 0000 6700 7c00 5d07 7d01 8801 8800  ....g.|.].}.....
-00001140: 7c01 8302 9102 7102 5300 7236 0000 0072  |.....q.S.r6...r
-00001150: 3600 0000 a902 da02 2e30 7269 0000 0029  6........0ri...)
-00001160: 0272 4a00 0000 726c 0000 0072 3600 0000  .rJ...rl...r6...
-00001170: 7237 0000 00da 0a3c 6c69 7374 636f 6d70  r7.....<listcomp
-00001180: 3ec2 0000 0073 0600 0000 0600 0201 0eff  >....s..........
-00001190: 7a1f 4170 694c 6973 742e 6765 742e 3c6c  z.ApiList.get.<l
-000011a0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000011b0: 3ee9 0100 0000 2906 da05 636f 756e 74da  >.....)...count.
-000011c0: 0472 6f77 73da 0968 746d 6c5f 7465 7874  .rows..html_text
-000011d0: da07 7375 6363 6573 73da 0c6e 6f5f 6461  ..success..no_da
-000011e0: 7461 5f74 6578 74da 0574 6974 6c65 7201  ta_text..titler.
-000011f0: 0000 0029 01da 0c70 6172 616d 5f76 616c  ...)...param_val
-00001200: 7565 7329 3472 2c00 0000 7221 0000 0072  ues)4r,...r!...r
-00001210: 2000 0000 da03 4745 54da 0e67 6574 5f70   .....GET..get_p
-00001220: 6572 6d69 7373 696f 6eda 0666 6f72 6d61  ermission..forma
-00001230: 7472 1200 0000 720b 0000 0072 3d00 0000  tr....r....r=...
-00001240: 7226 0000 0072 5b00 0000 723a 0000 00da  r&...r[...r:....
-00001250: 0261 68da 0367 6574 721b 0000 00da 1055  .ah..getr......U
-00001260: 524c 5f50 4152 414d 5f46 4f52 4d41 54da  RL_PARAM_FORMAT.
-00001270: 0c62 6f75 6e64 5f61 6374 696f 6eda 0661  .bound_action..a
-00001280: 6374 696f 6eda 0e64 6566 6175 6c74 5f66  ction..default_f
-00001290: 6f72 6d61 74da 1555 524c 5f50 4152 414d  ormat..URL_PARAM
-000012a0: 5f41 4354 494f 4e5f 4e41 4d45 7243 0000  _ACTION_NAMErC..
-000012b0: 00da 0f55 524c 5f46 4f52 4d41 545f 4a53  ...URL_FORMAT_JS
-000012c0: 4f4e da0a 6973 696e 7374 616e 6365 7225  ON..isinstancer%
-000012d0: 0000 0072 4000 0000 722d 0000 00da 1655  ...r@...r-.....U
-000012e0: 524c 5f50 4152 414d 5f44 4953 504c 4159  RL_PARAM_DISPLAY
-000012f0: 5f4d 4f44 4572 5f00 0000 da12 4449 5350  _MODEr_.....DISP
-00001300: 4c41 595f 4d4f 4445 5f53 544f 5259 da14  LAY_MODE_STORY..
-00001310: 736c 6963 6564 5f64 6174 615f 6974 6572  sliced_data_iter
-00001320: 6174 6f72 da0d 6173 5f73 746f 7279 5f69  ator..as_story_i
-00001330: 7465 6dda 0661 7070 656e 6472 4800 0000  tem..appendrH...
-00001340: da11 4449 5350 4c41 595f 4d4f 4445 5f4c  ..DISPLAY_MODE_L
-00001350: 4953 54da 1072 6f77 5f61 735f 7061 7261  IST..row_as_para
-00001360: 6772 6170 68da 0f61 6464 5f64 6574 6169  graph..add_detai
-00001370: 6c5f 6c69 6e6b da0f 6765 745f 746f 7461  l_link..get_tota
-00001380: 6c5f 636f 756e 74da 1363 7265 6174 655f  l_count..create_
-00001390: 7068 616e 746f 6d5f 726f 7773 da05 6c69  phantom_rows..li
-000013a0: 6d69 74da 036c 656e da04 6469 6374 7275  mit..len..dictru
-000013b0: 0000 00da 0967 6574 5f74 6974 6c65 da0d  .....get_title..
-000013c0: 6765 745f 6d61 696e 5f63 6172 64da 0669  get_main_card..i
-000013d0: 6e73 6572 7472 4700 0000 da0a 7061 7261  nsertrG.....para
-000013e0: 6d65 7465 7273 da06 7570 6461 7465 da0d  meters..update..
-000013f0: 7061 7261 6d73 5f6c 6179 6f75 74da 0c70  params_layout..p
-00001400: 6172 616d 735f 7374 6f72 65da 0770 7632  arams_store..pv2
-00001410: 6469 6374 7277 0000 0029 1372 4400 0000  dictrw...).rD...
-00001420: 7245 0000 0072 4600 0000 7247 0000 00da  rE...rF...rG....
-00001430: 0276 6dda 036d 7367 da03 666d 74da 0b61  .vm..msg..fmt..a
-00001440: 6374 696f 6e5f 6e61 6d65 724b 0000 00da  ction_namerK....
-00001450: 0764 6174 6172 6563 7273 0000 0072 7200  .datarecrs...rr.
-00001460: 0000 da03 6f62 6ada 0370 6172 da0b 746f  ....obj..par..to
-00001470: 7461 6c5f 636f 756e 7472 6900 0000 da01  tal_countri.....
-00001480: 64da 026b 77da 026d 6372 3600 0000 2904  d..kw..mcr6...).
-00001490: 724a 0000 0072 6a00 0000 726b 0000 0072  rJ...rj...rk...r
-000014a0: 6c00 0000 7237 0000 0072 7c00 0000 7600  l...r7...r|...v.
-000014b0: 0000 7390 0000 0008 0104 0108 0112 0108  ..s.............
-000014c0: 080a 0108 020c 0206 0106 0204 0108 0104  ................
-000014d0: fe0e 0404 020e 010c 020e 0108 010e 0108  ................
-000014e0: 0106 0208 0104 ff0a 0304 0104 010a 010e  ................
-000014f0: 0112 0102 fe0a 0304 0104 010a 010a 010c  ................
-00001500: 010a 0208 0612 0102 f504 0d0e 010c 0f04  ................
-00001510: 0106 ff08 030a 010c 012a 010a 010a 010a  .........*......
-00001520: 0104 0202 0102 0102 0104 0106 0106 fb0c  ................
-00001530: 0608 010a 010c 010a 0104 010a 0106 0102  ................
-00001540: ff06 ff08 030e 027a 0b41 7069 4c69 7374  .......z.ApiList
-00001550: 2e67 6574 2902 4e4e 2905 7256 0000 0072  .get).NN).rV...r
-00001560: 5700 0000 7258 0000 0072 4c00 0000 727c  W...rX...rL...r|
-00001570: 0000 0072 3600 0000 7236 0000 0072 3600  ...r6...r6...r6.
-00001580: 0000 7237 0000 0072 5900 0000 6f00 0000  ..r7...rY...o...
-00001590: 7306 0000 0008 000a 010e 0672 5900 0000  s..........rY...
-000015a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000015b0: 0002 0000 0040 0000 00f3 1800 0000 6500  .....@........e.
-000015c0: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
-000015d0: 5a04 6404 5300 2905 da0f 4368 6f69 6365  Z.d.S.)...Choice
-000015e0: 4c69 7374 4d6f 6465 6c7a a20a 2020 2020  ListModelz..    
-000015f0: 4372 6561 7465 7320 6120 6c61 7267 6520  Creates a large 
-00001600: 4a53 4f4e 206d 6f64 656c 2074 6861 7420  JSON model that 
-00001610: 636f 6e74 6169 6e73 2061 6c6c 2074 6865  contains all the
-00001620: 2063 686f 6963 656c 6973 7473 202b 2063   choicelists + c
-00001630: 686f 6963 6573 0a0a 2020 2020 4e6f 7465  hoices..    Note
-00001640: 3a20 5468 6973 2063 6f75 6c64 2062 6520  : This could be 
-00001650: 696d 7072 6f76 6564 2c20 6f72 206d 6967  improved, or mig
-00001660: 6874 2063 6175 7365 2069 7373 7565 7320  ht cause issues 
-00001670: 6475 6520 746f 2063 6861 6e67 696e 6720  due to changing 
-00001680: 6c61 6e67 7561 6765 0a20 2020 2063 0200  language.    c..
-00001690: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-000016a0: 0000 4300 0000 731c 0000 0064 0164 0284  ..C...s....d.d..
-000016b0: 0074 006a 01a0 02a1 0044 0083 017d 0274  .t.j.....D...}.t
-000016c0: 037c 0283 0153 0029 034e 6301 0000 0000  .|...S.).Nc.....
-000016d0: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
-000016e0: 0000 0073 2400 0000 6900 7c00 5d0e 7d01  ...s$...i.|.].}.
-000016f0: 7400 7c01 8301 6400 6401 8400 7c01 a001  t.|...d.d...|...
-00001700: a100 4400 8301 9302 7102 5300 2902 6301  ..D.....q.S.).c.
-00001710: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00001720: 0000 0053 0000 0073 3200 0000 6700 7c00  ...S...s2...g.|.
-00001730: 5d15 7d01 7400 7c01 6400 1900 8301 a001  ].}.t.|.d.......
-00001740: 6401 a101 7400 7c01 6402 1900 8301 a001  d...t.|.d.......
-00001750: 6401 a101 6403 9c02 9102 7102 5300 2904  d...d.....q.S.).
-00001760: 7201 0000 00fa 0122 7270 0000 0029 0272  r......"rp...).r
-00001770: 3300 0000 da04 7465 7874 2902 7215 0000  3.....text).r...
-00001780: 00da 0573 7472 6970 2902 726e 0000 00da  ...strip).rn....
-00001790: 0163 7236 0000 0072 3600 0000 7237 0000  .cr6...r6...r7..
-000017a0: 0072 6f00 0000 e800 0000 7302 0000 0032  .ro.......s....2
-000017b0: 007a 3243 686f 6963 654c 6973 744d 6f64  .z2ChoiceListMod
-000017c0: 656c 2e67 6574 2e3c 6c6f 6361 6c73 3e2e  el.get.<locals>.
-000017d0: 3c64 6963 7463 6f6d 703e 2e3c 6c69 7374  <dictcomp>.<list
-000017e0: 636f 6d70 3e29 02da 0373 7472 da0b 6765  comp>)...str..ge
-000017f0: 745f 6368 6f69 6365 7329 0272 6e00 0000  t_choices).rn...
-00001800: da02 636c 7236 0000 0072 3600 0000 7237  ..clr6...r6...r7
-00001810: 0000 00da 0a3c 6469 6374 636f 6d70 3ee8  .....<dictcomp>.
-00001820: 0000 0073 0600 0000 0600 0201 1cff 7a27  ...s..........z'
-00001830: 4368 6f69 6365 4c69 7374 4d6f 6465 6c2e  ChoiceListModel.
-00001840: 6765 742e 3c6c 6f63 616c 733e 2e3c 6469  get.<locals>.<di
-00001850: 6374 636f 6d70 3e29 0472 2600 0000 da0b  ctcomp>).r&.....
-00001860: 4348 4f49 4345 4c49 5354 53da 0676 616c  CHOICELISTS..val
-00001870: 7565 7372 2100 0000 2903 7244 0000 0072  uesr!...).rD...r
-00001880: 4500 0000 7249 0000 0072 3600 0000 7236  E...rI...r6...r6
-00001890: 0000 0072 3700 0000 727c 0000 00e7 0000  ...r7...r|......
-000018a0: 0073 0800 0000 0601 0802 06fe 0803 7a13  .s............z.
-000018b0: 4368 6f69 6365 4c69 7374 4d6f 6465 6c2e  ChoiceListModel.
-000018c0: 6765 744e a905 7256 0000 0072 5700 0000  getN..rV...rW...
-000018d0: 7258 0000 00da 075f 5f64 6f63 5f5f 727c  rX.....__doc__r|
-000018e0: 0000 0072 3600 0000 7236 0000 0072 3600  ...r6...r6...r6.
-000018f0: 0000 7237 0000 0072 a500 0000 e000 0000  ..r7...r........
-00001900: f306 0000 0008 0004 010c 0672 a500 0000  ...........r....
-00001910: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001920: 0003 0000 0040 0000 00f3 1600 0000 6500  .....@........e.
-00001930: 5a01 6400 5a02 6404 6402 6403 8401 5a03  Z.d.Z.d.d.d...Z.
-00001940: 6401 5300 2905 da07 4368 6f69 6365 734e  d.S.)...ChoicesN
-00001950: 6305 0000 0000 0000 0000 0000 000b 0000  c...............
-00001960: 0008 0000 004b 0000 0073 7c00 0000 7400  .....K...s|...t.
-00001970: 7c02 7c03 8302 7d06 6401 7d07 7c04 6401  |.|...}.d.}.|.d.
-00001980: 7500 7219 7c06 6a01 7c01 6402 8d01 7d08  u.r.|.j.|.d...}.
-00001990: 7c08 6a02 7d09 6403 6404 8400 7d0a 6e1b  |.j.}.d.d...}.n.
-000019a0: 7c06 a003 7c04 a101 7022 7c06 a004 7c04  |...|...p"|...|.
-000019b0: a101 7d04 7c04 6a05 7228 6405 7d07 7406  ..}.|.j.r(d.}.t.
-000019c0: 7c06 6a01 7c01 6402 8d01 7c06 7c04 8303  |.j.|.d...|.|...
-000019d0: 5c02 7d09 7d0a 7407 7c06 7c01 7c09 7c0a  \.}.}.t.|.|.|.|.
-000019e0: 7c07 7c04 6406 8d06 5300 2907 6141 0100  |.|.d...S.).aA..
-000019f0: 0049 6620 6066 6c64 6e61 6d65 6020 6973  .If `fldname` is
-00001a00: 2073 7065 6369 6669 6564 2c20 7265 7475   specified, retu
-00001a10: 726e 2061 204a 534f 4e20 6f62 6a65 6374  rn a JSON object
-00001a20: 2077 6974 6820 7477 6f0a 2020 2020 2020   with two.      
-00001a30: 2020 6174 7472 6962 7574 6573 2060 636f    attributes `co
-00001a40: 756e 7460 2061 6e64 2060 726f 7773 602c  unt` and `rows`,
-00001a50: 2077 6865 7265 2060 726f 7773 6020 6973   where `rows` is
-00001a60: 2061 206c 6973 7420 6f66 0a20 2020 2020   a list of.     
-00001a70: 2020 2060 2864 6973 706c 6179 5f74 6578     `(display_tex
-00001a80: 742c 2076 616c 7565 2960 2074 7570 6c65  t, value)` tuple
-00001a90: 732e 2020 5573 6564 2062 7920 436f 6d62  s.  Used by Comb
-00001aa0: 6f42 6f78 6573 206f 7220 7369 6d69 6c61  oBoxes or simila
-00001ab0: 720a 2020 2020 2020 2020 7769 6467 6574  r.        widget
-00001ac0: 732e 0a0a 2020 2020 2020 2020 4966 2060  s...        If `
-00001ad0: 666c 646e 616d 6560 2069 7320 6e6f 7420  fldname` is not 
-00001ae0: 7370 6563 6966 6965 642c 2072 6574 7572  specified, retur
-00001af0: 6e73 2074 6865 2063 686f 6963 6573 2066  ns the choices f
-00001b00: 6f72 2074 6865 0a20 2020 2020 2020 2060  or the.        `
-00001b10: 7265 636f 7264 5f73 656c 6563 746f 7260  record_selector`
-00001b20: 2077 6964 6765 742e 0a0a 2020 2020 2020   widget...      
-00001b30: 2020 4ea9 0172 4500 0000 6302 0000 0000    N..rE...c.....
-00001b40: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00001b50: 0000 0073 1e00 0000 7400 7c00 8301 7c01  ...s....t.|...|.
-00001b60: 7401 6a02 3c00 7c00 6a03 7c01 7401 6a04  t.j.<.|.j.|.t.j.
-00001b70: 3c00 7c01 5300 a901 4e29 0572 aa00 0000  <.|.S...N).r....
-00001b80: 721b 0000 00da 1243 484f 4943 4553 5f54  r......CHOICES_T
-00001b90: 4558 545f 4649 454c 4472 4800 0000 da13  EXT_FIELDrH.....
-00001ba0: 4348 4f49 4345 535f 5641 4c55 455f 4649  CHOICES_VALUE_FI
-00001bb0: 454c 4429 0272 9e00 0000 72a1 0000 0072  ELD).r....r....r
-00001bc0: 3600 0000 7236 0000 0072 3700 0000 7267  6...r6...r7...rg
-00001bd0: 0000 0007 0100 0073 0600 0000 0e01 0c02  .......s........
-00001be0: 0401 7a1d 4368 6f69 6365 732e 6765 742e  ..z.Choices.get.
-00001bf0: 3c6c 6f63 616c 733e 2e72 6f77 3264 6963  <locals>.row2dic
-00001c00: 7472 5c00 0000 a901 da05 6669 656c 6429  tr\.......field)
-00001c10: 0872 1f00 0000 7245 0000 00da 0d64 6174  .r....rE.....dat
-00001c20: 615f 6974 6572 6174 6f72 da0e 6765 745f  a_iterator..get_
-00001c30: 7061 7261 6d5f 656c 656d da0d 6765 745f  param_elem..get_
-00001c40: 6461 7461 5f65 6c65 6dda 0562 6c61 6e6b  data_elem..blank
-00001c50: 7218 0000 0072 2300 0000 290b 7244 0000  r....r#...).rD..
-00001c60: 0072 4500 0000 7246 0000 0072 4700 0000  .rE...rF...rG...
-00001c70: 72ba 0000 0072 a200 0000 da03 7270 74da  r....r......rpt.
-00001c80: 0a65 6d70 7479 5661 6c75 6572 4a00 0000  .emptyValuerJ...
-00001c90: da02 7173 7267 0000 0072 3600 0000 7236  ..qsrg...r6...r6
-00001ca0: 0000 0072 3700 0000 727c 0000 00f0 0000  ...r7...r|......
-00001cb0: 0073 1600 0000 0a0a 0401 0801 0c01 0606  .s..............
-00001cc0: 0a04 1409 0601 0402 1801 1402 7a0b 4368  ............z.Ch
-00001cd0: 6f69 6365 732e 6765 7472 5500 0000 a904  oices.getrU.....
-00001ce0: 7256 0000 0072 5700 0000 7258 0000 0072  rV...rW...rX...r
-00001cf0: 7c00 0000 7236 0000 0072 3600 0000 7236  |...r6...r6...r6
-00001d00: 0000 0072 3700 0000 72b4 0000 00ef 0000  ...r7...r.......
-00001d10: 00f3 0400 0000 0800 0e01 72b4 0000 0063  ..........r....c
-00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d30: 0300 0000 4000 0000 72b3 0000 0029 05da  ....@...r....)..
-00001d40: 0c44 656c 6179 6564 5661 6c75 654e 6306  .DelayedValueNc.
-00001d50: 0000 0000 0000 0000 0000 000d 0000 0005  ................
-00001d60: 0000 004b 0000 0073 9e00 0000 7400 7c02  ...K...s....t.|.
-00001d70: 7c03 8302 7d07 7c07 a001 7c05 a101 7d08  |...}.|...|...}.
-00001d80: 7c08 6400 7500 7215 6401 a002 7c07 7c05  |.d.u.r.d...|.|.
-00001d90: a102 7d09 6e34 7c07 6a03 7c01 7404 6a05  ..}.n4|.j.|.t.j.
-00001da0: 6a06 6a07 6a08 6402 8d02 7d0a 7c04 6403  j.j.j.d...}.|.d.
-00001db0: 6b02 7227 6400 7d0b 6e0a 7c0a a009 7c04  k.r'd.}.n.|...|.
-00001dc0: a101 0100 7c0a 6a0a 6404 1900 7d0b 740b  ....|.j.d...}.t.
-00001dd0: 7c07 7c08 7c05 8303 7d0c 7c0c 6400 7500  |.|.|...}.|.d.u.
-00001de0: 7243 6405 a002 7c07 7c08 7c05 a103 7d09  rCd...|.|.|...}.
-00001df0: 6e06 7c0c a00c 7c0b 7c0a a102 7d09 740d  n.|...|.|...}.t.
-00001e00: 6406 7c09 6901 8301 5300 2907 4e7a 197b  d.|.i...S.).Nz.{
-00001e10: 7d20 6861 7320 6e6f 2064 6174 6120 656c  } has no data el
-00001e20: 656d 656e 7420 7b7d a902 7245 0000 0072  ement {}..rE...r
-00001e30: 3a00 0000 723b 0000 0072 0100 0000 7a2c  :...r;...r....z,
-00001e40: 4f6f 7073 2c20 6765 745f 6174 6f6d 697a  Oops, get_atomiz
-00001e50: 6572 287b 7d2c 207b 7d2c 207b 7d29 2072  er({}, {}, {}) r
-00001e60: 6574 7572 6e65 6420 4e6f 6e65 7249 0000  eturned NonerI..
-00001e70: 0029 0e72 1f00 0000 72bd 0000 0072 7a00  .).r....r....rz.
-00001e80: 0000 7245 0000 0072 0b00 0000 723d 0000  ..rE...r....r=..
-00001e90: 0072 3e00 0000 723f 0000 0072 3a00 0000  .r>...r?...r:...
-00001ea0: 7242 0000 0072 4100 0000 7227 0000 00da  rB...rA...r'....
-00001eb0: 1666 756c 6c5f 7661 6c75 655f 6672 6f6d  .full_value_from
-00001ec0: 5f6f 626a 6563 7472 2100 0000 290d 7244  _objectr!...).rD
-00001ed0: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
-00001ee0: 0000 7248 0000 0072 ba00 0000 72a2 0000  ..rH...r....r...
-00001ef0: 0072 bf00 0000 da02 6465 da01 7672 4a00  .r......de..vrJ.
-00001f00: 0000 7269 0000 00da 0273 6672 3600 0000  ..ri.....sfr6...
-00001f10: 7236 0000 0072 3700 0000 727c 0000 001a  r6...r7...r|....
-00001f20: 0100 0073 1c00 0000 0a01 0a07 0801 0e01  ...s............
-00001f30: 1602 0801 0601 0a02 0a01 0c02 0801 1001  ................
-00001f40: 0c02 0c03 7a10 4465 6c61 7965 6456 616c  ....z.DelayedVal
-00001f50: 7565 2e67 6574 a904 4e4e 4e4e 72c2 0000  ue.get..NNNNr...
-00001f60: 0072 3600 0000 7236 0000 0072 3600 0000  .r6...r6...r6...
-00001f70: 7237 0000 0072 c400 0000 1901 0000 72c3  r7...r........r.
-00001f80: 0000 0072 c400 0000 6300 0000 0000 0000  ...r....c.......
-00001f90: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00001fa0: 0072 b300 0000 2905 da12 4163 7469 6f6e  .r....)...Action
-00001fb0: 5061 7261 6d43 686f 6963 6573 4e63 0600  ParamChoicesNc..
-00001fc0: 0000 0000 0000 0000 0000 0b00 0000 0800  ................
-00001fd0: 0000 4b00 0000 7376 0000 0074 007c 027c  ..K...sv...t.|.|
-00001fe0: 0383 027d 037c 03a0 017c 04a1 017d 077c  ...}.|...|...}.|
-00001ff0: 0764 0075 0072 1674 0264 017c 047c 0366  .d.u.r.t.d.|.|.f
-00002000: 0216 0083 0182 017c 076a 03a0 047c 05a1  .......|.j...|..
-00002010: 017d 0574 057c 076a 067c 0164 028d 017c  .}.t.|.j.|.d...|
-00002020: 076a 037c 0583 035c 027d 087d 097c 056a  .j.|...\.}.}.|.j
-00002030: 0772 2f64 037d 0a6e 0264 007d 0a74 087c  .r/d.}.n.d.}.t.|
-00002040: 037c 017c 087c 097c 0a7c 0564 048d 0653  .|.|.|.|.|.d...S
-00002050: 0029 054e 7a18 556e 6b6e 6f77 6e20 6163  .).Nz.Unknown ac
-00002060: 7469 6f6e 2025 7220 666f 7220 2573 72b5  tion %r for %sr.
-00002070: 0000 007a 053c 6272 2f3e 72b9 0000 0029  ...z.<br/>r....)
-00002080: 0972 1f00 0000 da0e 6765 745f 7572 6c5f  .r......get_url_
-00002090: 6163 7469 6f6e da09 4578 6365 7074 696f  action..Exceptio
-000020a0: 6e72 7f00 0000 72bc 0000 0072 1800 0000  nr....r....r....
-000020b0: 7245 0000 0072 be00 0000 7223 0000 0029  rE...r....r#...)
-000020c0: 0b72 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
-000020d0: 7247 0000 00da 0261 6e72 ba00 0000 72a2  rG.....anr....r.
-000020e0: 0000 00da 0262 6172 c100 0000 7267 0000  .....bar....rg..
-000020f0: 0072 c000 0000 7236 0000 0072 3600 0000  .r....r6...r6...
-00002100: 7237 0000 0072 7c00 0000 3a01 0000 7314  r7...r|...:...s.
-00002110: 0000 000a 010a 0108 0110 010c 011a 0106  ................
-00002120: 0106 0104 0214 017a 1641 6374 696f 6e50  .......z.ActionP
-00002130: 6172 616d 4368 6f69 6365 732e 6765 7472  aramChoices.getr
-00002140: ca00 0000 72c2 0000 0072 3600 0000 7236  ....r....r6...r6
-00002150: 0000 0072 3600 0000 7237 0000 0072 cb00  ...r6...r7...r..
-00002160: 0000 3801 0000 7304 0000 0008 000e 0272  ..8...s........r
-00002170: cb00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00002180: 0000 0000 0003 0000 0040 0000 0073 2e00  .........@...s..
-00002190: 0000 6500 5a01 6400 5a02 6401 5a03 6409  ..e.Z.d.Z.d.Z.d.
-000021a0: 6403 6404 8401 5a04 6409 6405 6406 8401  d.d...Z.d.d.d...
-000021b0: 5a05 6409 6407 6408 8401 5a06 6402 5300  Z.d.d.d...Z.d.S.
-000021c0: 290a da07 5265 7374 6675 6c7a 3c0a 2020  )...Restfulz<.  
-000021d0: 2020 5573 6564 2074 6f20 636f 6c6c 6162    Used to collab
-000021e0: 6f72 6174 6520 7769 7468 2061 2072 6573  orate with a res
-000021f0: 7466 756c 2045 7874 2e64 6174 612e 5374  tful Ext.data.St
-00002200: 6f72 652e 0a20 2020 204e 6305 0000 0000  ore..    Nc.....
-00002210: 0000 0000 0000 0009 0000 0006 0000 0043  ...............C
-00002220: 0000 0073 8800 0000 7400 7c02 7c03 8302  ...s....t.|.|...
-00002230: 7d05 7c05 6a01 7c01 6401 8d01 7d06 7c06  }.|.j.|.d...}.|.
-00002240: a002 a100 7d07 7c06 6a03 6a04 6400 7501  ....}.|.j.j.d.u.
-00002250: 721c 7c06 6a03 a004 7c07 7c01 a102 0100  r.|.j...|.|.....
-00002260: 7c01 6a05 a006 6402 a101 7d08 7407 a008  |.j...d...}.t...
-00002270: 7c08 a101 7d08 7c06 a009 7c08 7c07 6403  |...}.|...|.|.d.
-00002280: a103 0100 7c06 6a0a 7c06 6a0b 6a0c a00d  ....|.j.|.j.j...
-00002290: 7c06 7c07 7c06 6a0b 6a0c 6a0e a103 6701  |.|.|.j.j.j...g.
-000022a0: 6404 8d01 0100 740f 7c06 6a10 8301 5300  d.....t.|.j...S.
-000022b0: 2905 4e72 b500 0000 7272 0000 0054 a901  ).Nr....rr...T..
-000022c0: 7272 0000 0029 1172 1f00 0000 7245 0000  rr...).r....rE..
-000022d0: 0072 4000 0000 7247 0000 00da 1568 616e  .r@...rG.....han
-000022e0: 646c 655f 7570 6c6f 6164 6564 5f66 696c  dle_uploaded_fil
-000022f0: 6573 723c 0000 0072 7c00 0000 da04 6a73  esr<...r|.....js
-00002300: 6f6e da05 6c6f 6164 73da 1166 6f72 6d32  on..loads..form2
-00002310: 6f62 6a5f 616e 645f 7361 7665 da0c 7365  obj_and_save..se
-00002320: 745f 7265 7370 6f6e 7365 727b 0000 0072  t_responser{...r
-00002330: 6000 0000 7267 0000 00da 0b6c 6973 745f  `...rg.....list_
-00002340: 6669 656c 6473 7221 0000 00da 0872 6573  fieldsr!.....res
-00002350: 706f 6e73 6529 0972 4400 0000 7245 0000  ponse).rD...rE..
-00002360: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
-00002370: 72bf 0000 0072 4a00 0000 da08 696e 7374  r....rJ.....inst
-00002380: 616e 6365 7249 0000 0072 3600 0000 7236  ancerI...r6...r6
-00002390: 0000 0072 3700 0000 724c 0000 004d 0100  ...r7...rL...M..
-000023a0: 0073 1c00 0000 0a01 0c01 0802 0c03 0e01  .s..............
-000023b0: 0c02 0a01 0e01 0403 0801 0c01 04ff 06ff  ................
-000023c0: 0a03 7a0c 5265 7374 6675 6c2e 706f 7374  ..z.Restful.post
-000023d0: 6305 0000 0000 0000 0000 0000 000f 0000  c...............
-000023e0: 0005 0000 0003 0000 0073 6201 0000 7400  .........sb...t.
-000023f0: 7c02 7c03 8302 7d05 7c01 6a01 a002 7403  |.|...}.|.j...t.
-00002400: 6a04 6401 a102 7d06 7c01 6a01 a002 7403  j.d...}.|.j...t.
-00002410: 6a05 7403 6a06 a102 7d07 7c01 6a01 a007  j.t.j...}.|.j...
-00002420: 7403 6a08 a101 7d08 7c08 7322 7c04 6701  t.j...}.|.s"|.g.
-00002430: 7d08 7c05 6a09 7c01 7c08 6402 8d02 8900  }.|.j.|.|.d.....
-00002440: 7c04 6401 7500 7251 8800 6a0a 8901 8700  |.d.u.rQ..j.....
-00002450: 8701 6602 6403 6404 8408 8800 6a0b 4400  ..f.d.d.....j.D.
-00002460: 8301 7d09 740c 8800 a00d a100 7c09 6405  ..}.t.......|.d.
-00002470: 8d02 7d0a 7c0a 6a0e 740f 8800 a010 a100  ..}.|.j.t.......
-00002480: 8301 6406 8d01 0100 7411 7c0a 8301 5300  ..d.....t.|...S.
-00002490: 7c06 7259 7c05 a012 7c06 a101 7d0b 6e03  |.rY|...|...}.n.
-000024a0: 7c05 6a13 7d0b 8800 6a0a 7d0c 7c0b 6a09  |.j.}...j.}.|.j.
-000024b0: 7c01 7c08 6402 8d02 8900 8800 6a14 6407  |.|.d.......j.d.
-000024c0: 1900 7d0d 7c07 7403 6a06 6b02 72af 7c04  ..}.|.t.j.k.r.|.
-000024d0: 6408 6b02 7282 8800 a015 a100 7d0d 8800  d.k.r.......}...
-000024e0: a016 7c0c 7c0d a102 7d0e 7411 7c0e 8301  ..|.|...}.t.|...
-000024f0: 5300 7c04 6409 6b02 7294 8800 a015 a100  S.|.d.k.r.......
-00002500: 7d0d 7417 8800 7c0c 7c0d 8303 7d0e 7411  }.t...|.|...}.t.
-00002510: 7c0e 8301 5300 7c0d 6401 7500 72a6 740c  |...S.|.d.u.r.t.
-00002520: 640a 7418 7c05 7c04 6602 1600 640b 8d02  d.t.|.|.f...d...
-00002530: 7d0e 7411 7c0e 8301 5300 8800 a019 7c0d  }.t.|...S.....|.
-00002540: a101 7d0e 7411 7c0e 8301 5300 6401 5300  ..}.t.|...S.d.S.
-00002550: 290c 7a3b 0a20 2020 2020 2020 2057 6f72  ).z;.        Wor
-00002560: 6b73 2c20 6275 7420 6973 2075 676c 7920  ks, but is ugly 
-00002570: 746f 2067 6574 206c 6973 7420 616e 6420  to get list and 
-00002580: 6465 7461 696c 0a20 2020 2020 2020 204e  detail.        N
-00002590: 2902 7245 0000 00da 0c73 656c 6563 7465  ).rE.....selecte
-000025a0: 645f 706b 7363 0100 0000 0000 0000 0000  d_pksc..........
-000025b0: 0000 0200 0000 0700 0000 1300 0000 7320  ..............s 
-000025c0: 0000 0067 007c 005d 0c7d 0188 016a 00a0  ...g.|.].}...j..
-000025d0: 0188 007c 0188 016a 006a 02a1 0391 0271  ...|...j.j.....q
-000025e0: 0253 0072 3600 0000 2903 7260 0000 0072  .S.r6...).r`...r
-000025f0: 6700 0000 da0a 616c 6c5f 6669 656c 6473  g.....all_fields
-00002600: 726d 0000 00a9 0272 4a00 0000 726b 0000  rm.....rJ...rk..
-00002610: 0072 3600 0000 7237 0000 0072 6f00 0000  .r6...r7...ro...
-00002620: 7601 0000 7308 0000 0006 0002 0212 ff06  v...s...........
-00002630: ff7a 1f52 6573 7466 756c 2e67 6574 2e3c  .z.Restful.get.<
-00002640: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002650: 703e 2902 7271 0000 0072 7200 0000 2901  p>).rq...rr...).
-00002660: 7276 0000 0072 0100 0000 7a06 2d39 3939  rv...r....z.-999
-00002670: 3939 723b 0000 0046 2902 7274 0000 00da  99r;...F).rt....
-00002680: 076d 6573 7361 6765 291a 721f 0000 0072  .message).r....r
-00002690: 7800 0000 727c 0000 0072 1b00 0000 7281  x...r|...r....r.
-000026a0: 0000 0072 7d00 0000 7282 0000 00da 0767  ...r}...r......g
-000026b0: 6574 6c69 7374 da12 5552 4c5f 5041 5241  etlist..URL_PARA
-000026c0: 4d5f 5345 4c45 4354 4544 7245 0000 0072  M_SELECTEDrE...r
-000026d0: 7b00 0000 7286 0000 0072 9000 0000 728c  {...r....r....r.
-000026e0: 0000 0072 9500 0000 72aa 0000 0072 9100  ...r....r....r..
-000026f0: 0000 7221 0000 0072 cc00 0000 da0d 6465  ..r!...r......de
-00002700: 7461 696c 5f61 6374 696f 6e72 4100 0000  tail_actionrA...
-00002710: 7240 0000 00da 0f65 6c65 6d32 7265 635f  r@.....elem2rec_
-00002720: 696e 7365 7274 722d 0000 00da 094e 4f54  insertr-.....NOT
-00002730: 5f46 4f55 4e44 da11 656c 656d 3272 6563  _FOUND..elem2rec
-00002740: 5f64 6574 6169 6c65 6429 0f72 4400 0000  _detailed).rD...
-00002750: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
-00002760: 4800 0000 72bf 0000 0072 9c00 0000 729b  H...r....r....r.
-00002770: 0000 00da 0273 7272 7200 0000 72a2 0000  .....srrr...r...
-00002780: 0072 cf00 0000 727b 0000 0072 4b00 0000  .r....r{...rK...
-00002790: 729d 0000 0072 3600 0000 72dc 0000 0072  r....r6...r....r
-000027a0: 3700 0000 727c 0000 0067 0100 0073 5000  7...r|...g...sP.
-000027b0: 0000 0a04 1002 0601 0801 04ff 0e02 0401  ................
-000027c0: 0601 0e01 0801 0601 0c01 0402 06fe 1003  ................
-000027d0: 1401 0801 0403 0c01 0602 0601 0e01 0a01  ................
-000027e0: 0a01 0801 0801 0c01 0809 08f8 0801 0c01  ................
-000027f0: 0806 08fb 0201 0c01 06ff 0804 0aff 0801  ................
-00002800: 04f4 7a0b 5265 7374 6675 6c2e 6765 7463  ..z.Restful.getc
-00002810: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
-00002820: 0600 0000 4300 0000 73a8 0000 0074 007c  ....C...s....t.|
-00002830: 027c 0383 027d 057c 056a 017c 0164 018d  .|...}.|.j.|.d..
-00002840: 017d 067c 06a0 027c 04a1 0101 007c 066a  .}.|...|.....|.j
-00002850: 0364 0219 007d 077c 066a 047d 0874 05a0  .d...}.|.j.}.t..
-00002860: 067c 016a 07a1 01a0 0864 03a1 017d 0974  .|.j.....d...}.t
-00002870: 09a0 0a7c 09a1 017d 097c 05a0 0b7c 056a  ...|...}.|...|.j
-00002880: 0ca1 017d 0a7c 056a 017c 017c 0a64 048d  ...}.|.j.|.|.d..
-00002890: 027d 0674 0d6a 0e6a 0f6a 107c 065f 117c  .}.t.j.j.j.|._.|
-000028a0: 06a0 127c 097c 0764 05a1 0301 007c 066a  ...|.|.d.....|.j
-000028b0: 137c 086a 14a0 157c 067c 077c 086a 146a  .|.j...|.|.|.j.j
-000028c0: 16a1 0367 0164 068d 0101 0074 177c 066a  ...g.d.....t.|.j
-000028d0: 1883 0153 0029 074e 72b5 0000 0072 0100  ...S.).Nr....r..
-000028e0: 0000 7272 0000 0029 0272 4500 0000 727f  ..rr...).rE...r.
-000028f0: 0000 0046 72d1 0000 0029 1972 1f00 0000  ...Fr....).r....
-00002900: 7245 0000 0072 4200 0000 7241 0000 0072  rE...rB...rA...r
-00002910: 7b00 0000 7209 0000 0072 5000 0000 7251  {...r....rP...rQ
-00002920: 0000 0072 7c00 0000 72d3 0000 0072 d400  ...r|...r....r..
-00002930: 0000 72cc 0000 00da 1864 6566 6175 6c74  ..r......default
-00002940: 5f6c 6973 745f 6163 7469 6f6e 5f6e 616d  _list_action_nam
-00002950: 6572 0b00 0000 723d 0000 0072 2600 0000  er....r=...r&...
-00002960: da0e 6578 746a 735f 7265 6e64 6572 6572  ..extjs_renderer
-00002970: 723a 0000 0072 d500 0000 72d6 0000 0072  r:...r....r....r
-00002980: 6000 0000 7267 0000 0072 d700 0000 7221  `...rg...r....r!
-00002990: 0000 0072 d800 0000 290b 7244 0000 0072  ...r....).rD...r
-000029a0: 4500 0000 7246 0000 0072 4700 0000 7248  E...rF...rG...rH
-000029b0: 0000 0072 bf00 0000 724a 0000 0072 4b00  ...r....rJ...rK.
-000029c0: 0000 726b 0000 0072 4900 0000 da01 6172  ..rk...rI.....ar
-000029d0: 3600 0000 7236 0000 0072 3700 0000 7253  6...r6...r7...rS
-000029e0: 0000 0093 0100 0073 1e00 0000 0a01 0c01  .......s........
-000029f0: 0a01 0a01 0601 1202 0a01 0c01 0e01 0c01  ................
-00002a00: 0e01 0402 1401 06ff 0a02 7a0b 5265 7374  ..........z.Rest
-00002a10: 6675 6c2e 7075 7472 5500 0000 2907 7256  ful.putrU...).rV
-00002a20: 0000 0072 5700 0000 7258 0000 0072 b100  ...rW...rX...r..
-00002a30: 0000 724c 0000 0072 7c00 0000 7253 0000  ..rL...r|...rS..
-00002a40: 0072 3600 0000 7236 0000 0072 3600 0000  .r6...r6...r6...
-00002a50: 7237 0000 0072 d000 0000 4801 0000 730a  r7...r....H...s.
-00002a60: 0000 0008 0004 010a 040a 1a0e 2c72 d000  ............,r..
-00002a70: 0000 6303 0000 0000 0000 0000 0000 0009  ..c.............
-00002a80: 0000 0005 0000 0043 0000 0073 7000 0000  .......C...sp...
-00002a90: 7c00 a000 a100 7d03 7401 8300 7d04 7c03  |.....}.t...}.|.
-00002aa0: 6a02 7c04 6602 7d05 7c00 6a03 6406 6900  j.|.f.}.|.j.d.i.
-00002ab0: 7c02 a401 8e01 7d02 7c00 7c02 6401 3c00  |.....}.|.|.d.<.
-00002ac0: 7c00 6a04 7c02 6402 3c00 7405 6a06 6a07  |.j.|.d.<.t.j.j.
-00002ad0: 6a08 6a09 6a0a 7d06 7c06 a00b 7c01 a101  j.j.j.}.|...|...
-00002ae0: 7d07 740c 6a0d 7c07 6a0e 6406 6900 7c02  }.t.j.|.j.d.i.|.
-00002af0: a401 8e01 6403 6404 8d02 7d08 7c08 5300  ....d.d...}.|.S.
-00002b00: 2907 7a14 4465 7365 7276 6573 2061 2064  ).z.Deserves a d
-00002b10: 6f63 7374 7269 6e67 724a 0000 00da 046d  ocstringrJ.....m
-00002b20: 656d 6ffa 1974 6578 742f 6874 6d6c 3b63  emo..text/html;c
-00002b30: 6861 7273 6574 3d22 7574 662d 3822 a901  harset="utf-8"..
-00002b40: da0c 636f 6e74 656e 745f 7479 7065 4e72  ..content_typeNr
-00002b50: 3600 0000 290f da08 6765 745f 7573 6572  6...)...get_user
-00002b60: 7211 0000 00da 0975 7365 725f 7479 7065  r......user_type
-00002b70: da15 6765 745f 7072 696e 7461 626c 655f  ..get_printable_
-00002b80: 636f 6e74 6578 74da 0a70 6172 7365 5f6d  context..parse_m
-00002b90: 656d 6f72 0b00 0000 723d 0000 0072 3e00  emor....r=...r>.
-00002ba0: 0000 da05 6a69 6e6a 6172 3a00 0000 da09  ....jinjar:.....
-00002bb0: 6a69 6e6a 615f 656e 76da 0c67 6574 5f74  jinja_env..get_t
-00002bc0: 656d 706c 6174 6572 0900 0000 da0c 4874  emplater......Ht
-00002bd0: 7470 5265 7370 6f6e 7365 da06 7265 6e64  tpResponse..rend
-00002be0: 6572 2909 724a 0000 00da 0774 706c 6e61  er).rJ.....tplna
-00002bf0: 6d65 da07 636f 6e74 6578 74da 0175 da04  me..context..u..
-00002c00: 6c61 6e67 da01 6bda 0365 6e76 da08 7465  lang..k..env..te
-00002c10: 6d70 6c61 7465 72d8 0000 0072 3600 0000  mplater....r6...
-00002c20: 7236 0000 0072 3700 0000 da0d 6874 7470  r6...r7.....http
-00002c30: 5f72 6573 706f 6e73 65a6 0100 0073 1a00  _response....s..
-00002c40: 0000 0802 0601 0a01 1001 0801 0a01 0e01  ................
-00002c50: 0a01 0402 0e01 0201 06fe 0404 72fc 0000  ............r...
-00002c60: 0063 0300 0000 0000 0000 0000 0000 0c00  .c..............
-00002c70: 0000 0a00 0000 4300 0000 73ea 0000 007c  ......C...s....|
-00002c80: 006a 0064 1469 007c 02a4 018e 017d 027c  .j.d.i.|.....}.|
-00002c90: 026a 0174 0264 018d 0101 0074 036a 046a  .j.t.d.....t.j.j
-00002ca0: 056a 066a 076a 087d 037a 077c 03a0 097c  .j.j.j.}.z.|...|
-00002cb0: 01a1 017d 0457 006e 1604 0074 0a79 3201  ...}.W.n...t.y2.
-00002cc0: 007d 0501 007a 0a74 0ba0 0ca1 0057 0006  .}...z.t.....W..
-00002cd0: 0059 0064 027d 057e 0553 0064 027d 057e  .Y.d.}.~.S.d.}.~
-00002ce0: 0577 0177 0064 0364 0484 007d 067c 026a  .w.w.d.d...}.|.j
-00002cf0: 017c 0664 058d 0101 0064 0664 0784 007d  .|.d.....d.d...}
-00002d00: 0764 0864 0984 007d 0864 0a64 0b84 007d  .d.d...}.d.d...}
-00002d10: 097c 036a 0da0 0174 0e7c 077c 087c 0964  .|.j...t.|.|.|.d
-00002d20: 0c8d 03a1 0101 007c 01a0 0f64 0da1 0172  .......|...d...r
-00002d30: 5b64 0e6e 087c 01a0 0f64 0fa1 0172 6264  [d.n.|...d...rbd
-00002d40: 106e 0164 117d 0a74 0b6a 107c 046a 1164  .n.d.}.t.j.|.j.d
-00002d50: 1469 007c 02a4 018e 017c 0a64 1217 0064  .i.|.....|.d...d
-00002d60: 138d 027d 0b7c 0b53 0029 157a 6a0a 2020  ...}.|.S.).zj.  
-00002d70: 2020 5265 7370 6f6e 6520 7573 6564 2066    Respone used f
-00002d80: 6f72 2072 656e 6465 7269 6e67 2058 4d4c  or rendering XML
-00002d90: 2076 6965 7773 2069 6e20 7265 6163 742e   views in react.
-00002da0: 0a20 2020 2049 6e63 6c75 6465 7320 736f  .    Includes so
-00002db0: 6d65 2068 656c 7065 7220 6675 6e63 7469  me helper functi
-00002dc0: 6f6e 7320 666f 7220 7265 6e64 6572 696e  ons for renderin
-00002dd0: 672e 0a20 2020 2072 1a00 0000 4e63 0000  g..    r....Nc..
-00002de0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00002df0: 0000 5700 0000 7320 0000 0064 0164 0284  ..W...s ...d.d..
-00002e00: 007c 0044 0083 017d 0064 0364 04a0 007c  .|.D...}.d.d...|
-00002e10: 00a1 0117 0064 0517 0053 0029 067a 2748  .....d...S.).z'H
-00002e20: 656c 7065 7220 6675 6e63 7469 6f6e 2074  elper function t
-00002e30: 6f20 7772 6170 2061 2073 7472 696e 6720  o wrap a string 
-00002e40: 696e 207b 7d73 6301 0000 0000 0000 0000  in {}sc.........
-00002e50: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00002e60: 1400 0000 6700 7c00 5d06 7d01 7400 7c01  ....g.|.].}.t.|.
-00002e70: 8301 9102 7102 5300 7236 0000 0029 0172  ....q.S.r6...).r
-00002e80: aa00 0000 2902 726e 0000 0072 e700 0000  ....).rn...r....
-00002e90: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00002ea0: 6f00 0000 cd01 0000 7302 0000 0014 007a  o.......s......z
-00002eb0: 2e58 4d4c 5f72 6573 706f 6e73 652e 3c6c  .XML_response.<l
-00002ec0: 6f63 616c 733e 2e62 696e 642e 3c6c 6f63  ocals>.bind.<loc
-00002ed0: 616c 733e 2e3c 6c69 7374 636f 6d70 3eda  als>.<listcomp>.
-00002ee0: 017b 725c 0000 00da 017d 2901 da04 6a6f  .{r\.....})...jo
-00002ef0: 696e a901 da04 6172 6773 7236 0000 0072  in....argsr6...r
-00002f00: 3600 0000 7237 0000 00da 0462 696e 64cb  6...r7.....bind.
-00002f10: 0100 0073 0400 0000 0e02 1201 7a1a 584d  ...s........z.XM
-00002f20: 4c5f 7265 7370 6f6e 7365 2e3c 6c6f 6361  L_response.<loca
-00002f30: 6c73 3e2e 6269 6e64 2901 7202 0100 0063  ls>.bind).r....c
-00002f40: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00002f50: 0200 0000 5700 0000 730c 0000 0074 007c  ....W...s....t.|
-00002f60: 0083 0101 0064 0153 0029 027a 8844 6562  .....d.S.).z.Deb
-00002f70: 7567 6765 7220 6865 6c70 6572 3b20 7072  ugger helper; pr
-00002f80: 696e 7473 206f 7574 2061 6c6c 2061 7267  ints out all arg
-00002f90: 7320 7075 7420 696e 746f 2074 6865 2066  s put into the f
-00002fa0: 696c 7465 7220 6275 7420 646f 6573 6e27  ilter but doesn'
-00002fb0: 7420 696e 636c 7564 6520 7468 656d 2069  t include them i
-00002fc0: 6e20 7468 6520 7465 6d70 6c61 7465 2e0a  n the template..
-00002fd0: 2020 2020 2020 2020 7573 6167 653a 207b          usage: {
-00002fe0: 7b64 6562 7567 207c 2070 7d7d 0a20 2020  {debug | p}}.   
-00002ff0: 2020 2020 2072 5c00 0000 2901 da05 7072       r\...)...pr
-00003000: 696e 7472 0001 0000 7236 0000 0072 3600  intr....r6...r6.
-00003010: 0000 7237 0000 00da 0170 d201 0000 7304  ..r7.....p....s.
-00003020: 0000 0008 0404 017a 1758 4d4c 5f72 6573  .......z.XML_res
-00003030: 706f 6e73 652e 3c6c 6f63 616c 733e 2e70  ponse.<locals>.p
-00003040: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00003050: 0004 0000 0053 0000 0073 2000 0000 6401  .....S...s ...d.
-00003060: 6402 6c00 7d01 7c01 a001 7402 7c00 8301  d.l.}.|...t.|...
-00003070: a101 7d02 7c02 a003 6403 a101 5300 2904  ..}.|...d...S.).
-00003080: 7ab0 0a20 2020 2020 2020 2043 6f6d 7072  z..        Compr
-00003090: 6573 7320 6120 636f 6d70 6c65 7820 7661  ess a complex va
-000030a0: 6c75 6520 696e 206f 7264 6572 2074 6f20  lue in order to 
-000030b0: 6765 7420 6465 636f 6d70 7265 7373 2062  get decompress b
-000030c0: 7920 7468 6520 636f 6e74 726f 6c6c 6572  y the controller
-000030d0: 2061 6674 6572 7761 7264 730a 2020 2020   afterwards.    
-000030e0: 2020 2020 3a70 6172 616d 2073 3a20 7661      :param s: va
-000030f0: 6c75 6520 746f 2067 6574 2063 6f6d 7072  lue to get compr
-00003100: 6573 7365 642e 0a20 2020 2020 2020 203a  essed..        :
-00003110: 7265 7475 726e 3a20 436f 6d70 7265 7373  return: Compress
-00003120: 6564 2076 616c 7565 2e0a 2020 2020 2020  ed value..      
-00003130: 2020 7201 0000 004e da06 6261 7365 3634    r....N..base64
-00003140: 2904 da04 7a6c 6962 da08 636f 6d70 7265  )...zlib..compre
-00003150: 7373 72aa 0000 00da 0665 6e63 6f64 6529  ssr......encode)
-00003160: 03da 0173 7206 0100 00da 0a63 6f6d 7072  ...sr......compr
-00003170: 6573 7365 6472 3600 0000 7236 0000 0072  essedr6...r6...r
-00003180: 3700 0000 da0d 7a6c 6962 5f63 6f6d 7072  7.....zlib_compr
-00003190: 6573 73d9 0100 0073 0600 0000 0806 0e01  ess....s........
-000031a0: 0a01 7a23 584d 4c5f 7265 7370 6f6e 7365  ..z#XML_response
-000031b0: 2e3c 6c6f 6361 6c73 3e2e 7a6c 6962 5f63  .<locals>.zlib_c
-000031c0: 6f6d 7072 6573 7363 0200 0000 0000 0000  ompressc........
-000031d0: 0000 0000 0300 0000 0300 0000 5300 0000  ............S...
-000031e0: 7320 0000 007c 0072 0e7c 0144 005d 097d  s ...|.r.|.D.].}
-000031f0: 027c 007c 026b 0272 0d01 0064 0153 0071  .|.|.k.r...d.S.q
-00003200: 0464 0253 0029 037a f60a 2020 2020 2020  .d.S.).z..      
-00003210: 2020 6368 6563 6b20 6966 2074 6865 2066    check if the f
-00003220: 6965 6c64 7320 6973 2061 7661 696c 6162  ields is availab
-00003230: 6c65 2069 6e20 7468 6520 7365 7420 6f66  le in the set of
-00003240: 2063 6f6c 6c65 6374 696f 6e73 0a20 2020   collections.   
-00003250: 2020 2020 203a 7061 7261 6d20 7365 6172       :param sear
-00003260: 6368 6564 5f66 6965 6c64 3a20 7365 6172  ched_field: sear
-00003270: 6368 6564 2066 6965 6c64 0a20 2020 2020  ched field.     
-00003280: 2020 203a 7061 7261 6d20 636f 6c6c 6563     :param collec
-00003290: 7469 6f6e 733a 2073 6574 206f 6620 6669  tions: set of fi
-000032a0: 656c 6473 0a20 2020 2020 2020 203a 7265  elds.        :re
-000032b0: 7475 726e 3a20 5472 7565 2069 6620 7468  turn: True if th
-000032c0: 6520 6669 656c 6420 6973 2070 7265 7365  e field is prese
-000032d0: 6e74 2069 6e20 7468 6520 636f 6c6c 6563  nt in the collec
-000032e0: 7469 6f6e 732c 4661 6c73 6520 6f74 6865  tions,False othe
-000032f0: 7277 6973 652e 0a20 2020 2020 2020 2054  rwise..        T
-00003300: 4672 3600 0000 2903 da0e 7365 6172 6368  Fr6...)...search
-00003310: 6564 5f66 6965 6c64 da0b 636f 6c6c 6563  ed_field..collec
-00003320: 7469 6f6e 7372 ba00 0000 7236 0000 0072  tionsr....r6...r
-00003330: 3600 0000 7237 0000 00da 0d66 6965 6c64  6...r7.....field
-00003340: 735f 7365 6172 6368 e401 0000 730c 0000  s_search....s...
-00003350: 0004 0708 0108 0106 0102 ff04 027a 2358  .............z#X
-00003360: 4d4c 5f72 6573 706f 6e73 652e 3c6c 6f63  ML_response.<loc
-00003370: 616c 733e 2e66 6965 6c64 735f 7365 6172  als>.fields_sear
-00003380: 6368 2903 7204 0100 0072 0b01 0000 720e  ch).r....r....r.
-00003390: 0100 007a 042e 786d 6c7a 0874 6578 742f  ...z..xmlz.text/
-000033a0: 786d 6c7a 032e 6a73 fa16 6170 706c 6963  xmlz..js..applic
-000033b0: 6174 696f 6e2f 6a61 7661 7363 7269 7074  ation/javascript
-000033c0: 7a10 6170 706c 6963 6174 696f 6e2f 6a73  z.application/js
-000033d0: 6f6e 7a10 3b63 6861 7273 6574 3d22 7574  onz.;charset="ut
-000033e0: 662d 3822 72ea 0000 0072 3600 0000 2912  f-8"r....r6...).
-000033f0: 72ee 0000 0072 9500 0000 721b 0000 0072  r....r....r....r
-00003400: 0b00 0000 723d 0000 0072 3e00 0000 72f0  ....r=...r>...r.
-00003410: 0000 0072 3a00 0000 72f1 0000 0072 f200  ...r:...r....r..
-00003420: 0000 7204 0000 0072 0900 0000 da14 4874  ..r....r......Ht
-00003430: 7470 5265 7370 6f6e 7365 4e6f 7446 6f75  tpResponseNotFou
-00003440: 6e64 da07 6669 6c74 6572 7372 9000 0000  nd..filtersr....
-00003450: da08 656e 6473 7769 7468 72f3 0000 0072  ..endswithr....r
-00003460: f400 0000 290c 724a 0000 0072 f500 0000  ....).rJ...r....
-00003470: 72f6 0000 0072 fa00 0000 72fb 0000 00da  r....r....r.....
-00003480: 0165 7202 0100 0072 0401 0000 720b 0100  .er....r....r...
-00003490: 0072 0e01 0000 72eb 0000 0072 d800 0000  .r....r....r....
-000034a0: 7236 0000 0072 3600 0000 7237 0000 00da  r6...r6...r7....
-000034b0: 0c58 4d4c 5f72 6573 706f 6e73 65b9 0100  .XML_response...
-000034c0: 0073 3000 0000 1008 0c01 0e03 0201 0e01  .s0.............
-000034d0: 0e01 1401 0880 02ff 0803 0c05 0802 0807  ................
-000034e0: 080b 160d 0e01 0e01 0201 02fe 0403 0e01  ................
-000034f0: 0601 06fe 0404 7214 0100 0063 0000 0000  ......r....c....
-00003500: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00003510: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00003520: 0264 015a 0364 025a 0464 0353 0029 04da  .d.Z.d.Z.d.S.)..
-00003530: 0653 5756 6965 777a 1772 6561 6374 2f73  .SWViewz.react/s
-00003540: 6572 7669 6365 2d77 6f72 6b65 722e 6a73  ervice-worker.js
-00003550: 720f 0100 004e 2905 7256 0000 0072 5700  r....N).rV...rW.
-00003560: 0000 7258 0000 00da 0d74 656d 706c 6174  ..rX.....templat
-00003570: 655f 6e61 6d65 72eb 0000 0072 3600 0000  e_namer....r6...
-00003580: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00003590: 1501 0000 fc01 0000 7306 0000 0008 0004  ........s.......
-000035a0: 0108 0172 1501 0000 6300 0000 0000 0000  ...r....c.......
-000035b0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-000035c0: 0073 2000 0000 6500 5a01 6400 5a02 6401  .s ...e.Z.d.Z.d.
-000035d0: 5a03 8700 6601 6402 6403 8408 5a04 8700  Z...f.d.d...Z...
-000035e0: 0400 5a05 5300 2904 da06 5742 5669 6577  ..Z.S.)...WBView
-000035f0: 720f 0100 0063 0200 0000 0000 0000 0000  r....c..........
-00003600: 0000 0400 0000 0400 0000 0f00 0000 732c  ..............s,
-00003610: 0000 0074 0083 006a 017c 0167 017c 02a2  ...t...j.|.g.|..
-00003620: 0152 0069 007c 03a4 018e 0101 0064 017c  .R.i.|.......d.|
-00003630: 0364 0219 0017 007c 005f 0264 0053 0029  .d.....|._.d.S.)
-00003640: 034e 7a06 7265 6163 742f da07 776f 726b  .Nz.react/..work
-00003650: 626f 7829 03da 0573 7570 6572 da05 7365  box)...super..se
-00003660: 7475 7072 1601 0000 2904 7244 0000 0072  tupr....).rD...r
-00003670: 4500 0000 7201 0100 00da 066b 7761 7267  E...r......kwarg
-00003680: 73a9 01da 095f 5f63 6c61 7373 5f5f 7236  s....__class__r6
-00003690: 0000 0072 3700 0000 721a 0100 0003 0200  ...r7...r.......
-000036a0: 0073 0400 0000 1a01 1201 7a0c 5742 5669  .s........z.WBVi
-000036b0: 6577 2e73 6574 7570 2906 7256 0000 0072  ew.setup).rV...r
-000036c0: 5700 0000 7258 0000 0072 eb00 0000 721a  W...rX...r....r.
-000036d0: 0100 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-000036e0: 5f5f 7236 0000 0072 3600 0000 721c 0100  __r6...r6...r...
-000036f0: 0072 3700 0000 7217 0100 0000 0200 0073  .r7...r........s
-00003700: 0600 0000 0800 0401 1402 7217 0100 0063  ..........r....c
-00003710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003720: 0200 0000 4000 0000 f314 0000 0065 005a  ....@........e.Z
-00003730: 0164 005a 0264 0164 0284 005a 0364 0353  .d.Z.d.d...Z.d.S
-00003740: 0029 04da 084d 6169 6e48 746d 6c63 0200  .)...MainHtmlc..
-00003750: 0000 0000 0000 0000 0000 0700 0000 0400  ................
-00003760: 0000 4f00 0000 7358 0000 0074 006a 01a0  ..O...sX...t.j..
-00003770: 02a1 0001 0074 006a 016a 036a 046a 057d  .....t.j.j.j.j.}
-00003780: 0474 067c 017c 0464 018d 027d 0564 027c  .t.|.|.d...}.d.|
-00003790: 015f 0774 006a 01a0 087c 05a1 017d 067c  ._.t.j...|...}.|
-000037a0: 04a0 097c 06a1 017d 067c 056a 0a7c 0664  ...|...}.|.j.|.d
-000037b0: 038d 0101 0074 0b7c 056a 0c7c 056a 0d83  .....t.|.j.|.j..
-000037c0: 0253 0029 047a 3252 6574 7572 6e73 2061  .S.).z2Returns a
-000037d0: 206a 736f 6e20 7374 7275 6374 2066 6f72   json struct for
-000037e0: 2074 6865 206d 6169 6e20 7573 6572 2064   the main user d
-000037f0: 6173 6862 6f61 7264 2e72 3900 0000 7a0e  ashboard.r9...z.
-00003800: 6461 7368 626f 6172 642d 6d61 696e 7207  dashboard-mainr.
-00003810: 0000 0029 0e72 0b00 0000 723d 0000 00da  ...).r....r=....
-00003820: 0773 7461 7274 7570 723e 0000 0072 3f00  .startupr>...r?.
-00003830: 0000 723a 0000 0072 1c00 0000 da10 7265  ..r:...r......re
-00003840: 7175 6573 7469 6e67 5f70 616e 656c da0d  questing_panel..
-00003850: 6765 745f 6d61 696e 5f68 746d 6c72 7300  get_main_htmlrs.
-00003860: 0000 7274 0000 0072 2100 0000 72d8 0000  ..rt...r!...r...
-00003870: 0072 eb00 0000 2907 7244 0000 0072 4500  .r....).rD...rE.
-00003880: 0000 7201 0100 0072 a200 0000 da03 726e  ..r....r......rn
-00003890: 6472 4a00 0000 7208 0000 0072 3600 0000  drJ...r....r6...
-000038a0: 7236 0000 0072 3700 0000 727c 0000 0009  r6...r7...r|....
-000038b0: 0200 0073 1000 0000 0a03 0c02 0c01 0602  ...s............
-000038c0: 0c01 0a01 0c01 0e01 7a0c 4d61 696e 4874  ........z.MainHt
-000038d0: 6d6c 2e67 6574 4e72 c200 0000 7236 0000  ml.getNr....r6..
-000038e0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-000038f0: 7220 0100 0008 0200 00f3 0400 0000 0800  r ..............
-00003900: 0c01 7220 0100 0063 0000 0000 0000 0000  ..r ...c........
-00003910: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00003920: 721f 0100 0029 04da 0d44 6173 6862 6f61  r....)...Dashboa
-00003930: 7264 4974 656d 6303 0000 0000 0000 0000  rdItemc.........
-00003940: 0000 000a 0000 0005 0000 004f 0000 0073  ...........O...s
-00003950: 9800 0000 7400 7c01 8301 7d05 7401 6a02  ....t.|...}.t.j.
-00003960: 6a03 6a04 6a05 7c05 5f05 6401 7c02 9b00  j.j.j.|._.d.|...
-00003970: 9d02 7c05 5f06 7c05 a007 a100 a008 a100  ..|._.|.........
-00003980: 6a09 7d06 740a 7c06 8301 7c02 6b04 722b  j.}.t.|...|.k.r+
-00003990: 7c06 7c02 1900 7d07 6402 a00b 7c07 a00c  |.|...}.d...|...
-000039a0: 7c05 a101 a101 7d08 6e02 6402 7d08 740d  |.....}.n.d.}.t.
-000039b0: 7c08 6403 8d01 7d04 740e 7c01 8301 7d09  |.d...}.t.|...}.
-000039c0: 7c09 723d 7c04 a00f 7c09 a101 0100 7c05  |.r=|...|.....|.
-000039d0: 6a10 6405 6900 7c04 a401 8e01 0100 7411  j.d.i.|.......t.
-000039e0: 7c05 6a12 7c05 6a13 8302 5300 2906 7a3d  |.j.|.j...S.).z=
-000039f0: 5265 7475 726e 7320 6120 7265 6e64 6572  Returns a render
-00003a00: 6564 2048 544d 4c20 7665 7273 696f 6e20  ed HTML version 
-00003a10: 7468 6520 7265 7175 6573 7465 6420 7573  the requested us
-00003a20: 6572 2064 6173 6862 6f61 7264 2e7a 0a64  er dashboard.z.d
-00003a30: 6173 6862 6f61 7264 2d72 5c00 0000 7207  ashboard-r\...r.
-00003a40: 0000 004e 7236 0000 0029 1472 1c00 0000  ...Nr6...).r....
-00003a50: 720b 0000 0072 3d00 0000 723e 0000 0072  r....r=...r>...r
-00003a60: 3f00 0000 723a 0000 0072 2201 0000 72ec  ?...r:...r"...r.
-00003a70: 0000 00da 0f67 6574 5f70 7265 6665 7265  .....get_prefere
-00003a80: 6e63 6573 da0f 6461 7368 626f 6172 645f  nces..dashboard_
-00003a90: 6974 656d 7372 8f00 0000 72ff 0000 0072  itemsr....r....r
-00003aa0: f400 0000 7290 0000 0072 2c00 0000 7295  ....r....r,...r.
-00003ab0: 0000 0072 7400 0000 7221 0000 0072 d800  ...rt...r!...r..
-00003ac0: 0000 72eb 0000 0029 0a72 4400 0000 7245  ..r....).rD...rE
-00003ad0: 0000 00da 0569 6e64 6578 7201 0100 0072  .....indexr....r
-00003ae0: a200 0000 724a 0000 00da 0464 6173 68da  ....rJ.....dash.
-00003af0: 0469 7465 6d72 0800 0000 7299 0000 0072  .itemr....r....r
-00003b00: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
-00003b10: 0000 0019 0200 0073 1c00 0000 0802 0e01  .......s........
-00003b20: 0c01 0e01 0c01 0801 1203 0402 0a01 0801  ................
-00003b30: 0401 0a01 1001 0e01 7a11 4461 7368 626f  ........z.Dashbo
-00003b40: 6172 6449 7465 6d2e 6765 744e 72c2 0000  ardItem.getNr...
-00003b50: 0072 3600 0000 7236 0000 0072 3600 0000  .r6...r6...r6...
-00003b60: 7237 0000 0072 2601 0000 1802 0000 7225  r7...r&.......r%
-00003b70: 0100 0072 2601 0000 6300 0000 0000 0000  ...r&...c.......
-00003b80: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00003b90: 0073 2000 0000 6500 5a01 6400 5a02 6401  .s ...e.Z.d.Z.d.
-00003ba0: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
-00003bb0: 5a05 6406 5300 2907 da04 4e75 6c6c 7a6c  Z.d.S.)...Nullzl
-00003bc0: 4a75 7374 2072 6574 7572 6e73 2032 3030  Just returns 200
-00003bd0: 2c20 7573 6564 2069 6e20 616e 2069 6672  , used in an ifr
-00003be0: 616d 6520 746f 2063 6175 7365 2074 6865  ame to cause the
-00003bf0: 2062 726f 7773 6572 2074 6f20 7472 6967   browser to trig
-00003c00: 6765 7220 2244 6f20 796f 7520 7761 6e74  ger "Do you want
-00003c10: 2074 6f20 7265 6d65 6d62 6572 2074 6869   to remember thi
-00003c20: 7320 7077 2220 6469 616c 6f67 6302 0000  s pw" dialogc...
-00003c30: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00003c40: 0043 0000 00f3 0800 0000 7400 a001 a100  .C........t.....
-00003c50: 5300 72b6 0000 00a9 0272 0900 0000 72f3  S.r......r....r.
-00003c60: 0000 00a9 0272 4400 0000 7245 0000 0072  .....rD...rE...r
-00003c70: 3600 0000 7236 0000 0072 3700 0000 724c  6...r6...r7...rL
-00003c80: 0000 0031 0200 00f3 0200 0000 0801 7a09  ...1..........z.
-00003c90: 4e75 6c6c 2e70 6f73 7463 0200 0000 0000  Null.postc......
-00003ca0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00003cb0: 0000 722d 0100 0072 b600 0000 722e 0100  ..r-...r....r...
-00003cc0: 0072 2f01 0000 7236 0000 0072 3600 0000  .r/...r6...r6...
-00003cd0: 7237 0000 0072 7c00 0000 3402 0000 7230  r7...r|...4...r0
-00003ce0: 0100 007a 084e 756c 6c2e 6765 744e 2906  ...z.Null.getN).
-00003cf0: 7256 0000 0072 5700 0000 7258 0000 0072  rV...rW...rX...r
-00003d00: b100 0000 724c 0000 0072 7c00 0000 7236  ....rL...r|...r6
-00003d10: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00003d20: 0000 722c 0100 002e 0200 0073 0800 0000  ..r,.......s....
-00003d30: 0800 0401 0802 0c03 722c 0100 0063 0000  ........r,...c..
-00003d40: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00003d50: 0000 4000 0000 731c 0000 0065 005a 0164  ..@...s....e.Z.d
-00003d60: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00003d70: 005a 0464 0553 0029 06da 0c41 7574 6865  .Z.d.S.)...Authe
-00003d80: 6e74 6963 6174 6563 0200 0000 0000 0000  nticatec........
-00003d90: 0000 0000 0700 0000 0400 0000 4f00 0000  ............O...
-00003da0: 7336 0000 007c 016a 00a0 0174 026a 03a1  s6...|.j...t.j..
-00003db0: 017d 0409 007c 016a 04a0 0564 0364 00a1  .}...|.j...d.d..
-00003dc0: 027d 0574 06a0 077c 01a1 0101 0064 047d  .}.t...|.....d.}
-00003dd0: 0674 08a0 097c 06a1 0153 0029 054e 54da  .t...|...S.).NT.
-00003de0: 066c 6f67 6f75 74da 0875 7365 726e 616d  .logout..usernam
-00003df0: 65fa 012f 290b 7278 0000 0072 7c00 0000  e../).rx...r|...
-00003e00: 721b 0000 0072 8100 0000 da07 7365 7373  r....r......sess
-00003e10: 696f 6eda 0370 6f70 7213 0000 0072 3201  ion..popr....r2.
-00003e20: 0000 7209 0000 00da 1448 7474 7052 6573  ..r......HttpRes
-00003e30: 706f 6e73 6552 6564 6972 6563 74da 0748  ponseRedirect..H
-00003e40: 7474 7034 3034 2907 7244 0000 0072 4500  ttp404).rD...rE.
-00003e50: 0000 7201 0100 0072 a200 0000 729c 0000  ..r....r....r...
-00003e60: 0072 3301 0000 7232 0000 0072 3600 0000  .r3...r2...r6...
-00003e70: 7236 0000 0072 3700 0000 727c 0000 0039  r6...r7...r|...9
-00003e80: 0200 0073 0c00 0000 0e01 0201 0e01 0a01  ...s............
-00003e90: 0405 0a01 7a10 4175 7468 656e 7469 6361  ....z.Authentica
-00003ea0: 7465 2e67 6574 6302 0000 0000 0000 0000  te.getc.........
-00003eb0: 0000 0008 0000 0005 0000 004f 0000 0073  ...........O...s
-00003ec0: 4c00 0000 7c01 6a00 a001 6401 a101 7d04  L...|.j...d...}.
-00003ed0: 7c01 6a00 a001 6402 a101 7d05 7402 6a03  |.j...d...}.t.j.
-00003ee0: 7c01 7c04 7c05 6403 8d03 7d06 7402 6a04  |.|.|.d...}.t.j.
-00003ef0: 7c01 7c06 6404 6405 8d03 0100 6406 6407  |.|.d.d.....d.d.
-00003f00: 8400 7d07 7405 7c06 6a06 7c07 8302 5300  ..}.t.|.j.|...S.
-00003f10: 2908 7a46 6c6f 6773 2074 6865 2075 7365  ).zFlogs the use
-00003f20: 7220 696e 2061 6e64 2062 7569 6c64 7320  r in and builds 
-00003f30: 7468 6520 6c69 6e6f 7765 622e 6a73 2066  the linoweb.js f
-00003f40: 696c 6520 666f 7220 7468 6520 6c6f 6767  ile for the logg
-00003f50: 6564 2069 6e20 7573 6572 7233 0100 00da  ed in userr3....
-00003f60: 0870 6173 7377 6f72 6429 0272 3301 0000  .password).r3...
-00003f70: 7239 0100 007a 246c 696e 6f2e 636f 7265  r9...z$lino.core
-00003f80: 2e61 7574 682e 6261 636b 656e 6473 2e4d  .auth.backends.M
-00003f90: 6f64 656c 4261 636b 656e 6429 01da 0762  odelBackend)...b
-00003fa0: 6163 6b65 6e64 6300 0000 0000 0000 0000  ackendc.........
-00003fb0: 0000 0000 0000 0003 0000 0053 0000 0073  ...........S...s
-00003fc0: 2600 0000 7400 6a01 6a02 720d 7400 6a01  &...t.j.j.r.t.j.
-00003fd0: 6a03 6a04 6a05 a006 6401 a101 0100 7407  j.j.j...d.....t.
-00003fe0: 6402 6403 6901 8301 5300 2904 4e46 7274  d.d.i...S.).NFrt
-00003ff0: 0000 0054 2908 720b 0000 0072 3d00 0000  ...T).r....r=...
-00004000: da14 6465 7665 6c6f 7065 725f 7369 7465  ..developer_site
-00004010: 5f63 6163 6865 723e 0000 0072 3f00 0000  _cacher>...r?...
-00004020: 723a 0000 00da 0e62 7569 6c64 5f6a 735f  r:.....build_js_
-00004030: 6361 6368 6572 2100 0000 7236 0000 0072  cacher!...r6...r
-00004040: 3600 0000 7236 0000 0072 3700 0000 da06  6...r6...r7.....
-00004050: 7265 7375 6c74 5402 0000 7306 0000 0008  resultT...s.....
-00004060: 0112 010c 027a 2141 7574 6865 6e74 6963  .....z!Authentic
-00004070: 6174 652e 706f 7374 2e3c 6c6f 6361 6c73  ate.post.<locals
-00004080: 3e2e 7265 7375 6c74 2907 723c 0000 0072  >.result).r<...r
-00004090: 7c00 0000 7213 0000 00da 0c61 7574 6865  |...r......authe
-000040a0: 6e74 6963 6174 65da 056c 6f67 696e 7229  nticate..loginr)
-000040b0: 0000 0072 ed00 0000 2908 7244 0000 0072  ...r....).rD...r
-000040c0: 4500 0000 7201 0100 0072 a200 0000 7233  E...r....r....r3
-000040d0: 0100 0072 3901 0000 da04 7573 6572 723d  ...r9.....userr=
-000040e0: 0100 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-000040f0: 0000 724c 0000 004a 0200 0073 1000 0000  ..rL...J...s....
-00004100: 0c02 0c01 0402 0601 06ff 1002 0803 0c06  ................
-00004110: 7a11 4175 7468 656e 7469 6361 7465 2e70  z.Authenticate.p
-00004120: 6f73 744e 2905 7256 0000 0072 5700 0000  ostN).rV...rW...
-00004130: 7258 0000 0072 7c00 0000 724c 0000 0072  rX...r|...rL...r
-00004140: 3600 0000 7236 0000 0072 3600 0000 7237  6...r6...r6...r7
-00004150: 0000 0072 3101 0000 3802 0000 7306 0000  ...r1...8...s...
-00004160: 0008 0008 010c 1172 3101 0000 6300 0000  .......r1...c...
-00004170: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00004180: 0040 0000 0072 a400 0000 2905 da05 496e  .@...r....)...In
-00004190: 6465 787a 930a 2020 2020 4d61 696e 2061  dexz..    Main a
-000041a0: 7070 2065 6e74 7279 2070 6f69 6e74 2c0a  pp entry point,.
-000041b0: 2020 2020 416c 736f 2062 7569 6c64 7320      Also builds 
-000041c0: 6c69 6e6f 7765 6220 6669 6c65 2066 6f72  linoweb file for
-000041d0: 2063 7572 7265 6e74 2075 7365 7220 7479   current user ty
-000041e0: 7065 2e0a 2020 2020 436f 6e74 656e 7420  pe..    Content 
-000041f0: 6973 206d 6f73 746c 7920 696e 2074 6865  is mostly in the
-00004200: 203a 7866 696c 653a 6072 6561 6374 2f6d   :xfile:`react/m
-00004210: 6169 6e2e 6874 6d6c 6020 7465 6d70 6c61  ain.html` templa
-00004220: 7465 2e0a 2020 2020 6302 0000 0000 0000  te..    c.......
-00004230: 0000 0000 0003 0000 0003 0000 0003 0000  ................
-00004240: 0073 2e00 0000 8800 6a00 8901 0900 8800  .s......j.......
-00004250: 6a01 720a 8800 6a01 8901 8700 8701 6602  j.r...j.......f.
-00004260: 6402 6403 8408 7d02 7402 8801 6a03 7c02  d.d...}.t...j.|.
-00004270: 8302 5300 2904 4e54 6300 0000 0000 0000  ..S.).NTc.......
-00004280: 0000 0000 0007 0000 0006 0000 0013 0000  ................
-00004290: 0073 b600 0000 7400 6a01 6a02 6a03 7d00  .s....t.j.j.j.}.
-000042a0: 7404 8800 7c00 6a05 6401 8d02 7d01 7406  t...|.j.d...}.t.
-000042b0: 7c00 8800 8801 6402 8d03 7d02 7c02 6a07  |.....d...}.|.j.
-000042c0: 7c01 6403 8d01 0100 6404 7d03 6405 8800  |.d.....d.}.d...
-000042d0: 6a08 7600 7229 6406 a009 740a a00b 6407  j.v.r)d...t...d.
-000042e0: 6408 a102 a101 7d03 7c02 6a07 7c03 6409  d.....}.|.j.|.d.
-000042f0: 8d01 0100 7c01 6a0c 640f 6900 7c02 a401  ....|.j.d.i.|...
-00004300: 8e01 7d02 7400 6a01 6a02 6a0d 6a05 6a0e  ..}.t.j.j.j.j.j.
-00004310: 7d04 7c04 a00f 640a a101 7d05 7410 6a11  }.|...d...}.t.j.
-00004320: 7c05 6a12 640f 6900 7c02 a401 8e01 640b  |.j.d.i.|.....d.
-00004330: 640c 8d02 7d06 6405 8800 6a08 7600 7259  d...}.d...j.v.rY
-00004340: 640d 7c06 640e 3c00 7c06 5300 2910 4e72  d.|.d.<.|.S.).Nr
-00004350: c500 0000 2903 da09 6672 6f6e 745f 656e  ....)...front_en
-00004360: 6472 4500 0000 7240 0100 0029 0172 4a00  drE...r@...).rJ.
-00004370: 0000 725c 0000 00da 0c75 7064 6174 655f  ..r\.....update_
-00004380: 666f 756e 647a 093f 6d74 696d 653d 7b7d  foundz.?mtime={}
-00004390: 6907 b201 0069 3f42 0f00 2901 da08 6e6f  i....i?B..)...no
-000043a0: 5f63 6163 6865 7a0f 7265 6163 742f 6d61  _cachez.react/ma
-000043b0: 696e 2e68 746d 6c72 e900 0000 72ea 0000  in.htmlr....r...
-000043c0: 007a 1222 6361 6368 6522 2c20 2273 746f  .z."cache", "sto
-000043d0: 7261 6765 227a 0f43 6c65 6172 2d53 6974  rage"z.Clear-Sit
-000043e0: 652d 4461 7461 7236 0000 0029 1372 0b00  e-Datar6...).r..
-000043f0: 0000 723d 0000 0072 3e00 0000 723f 0000  ..r=...r>...r?..
-00004400: 0072 1c00 0000 723a 0000 0072 9000 0000  .r....r:...r....
-00004410: 7295 0000 0072 7800 0000 727a 0000 00da  r....rx...rz....
-00004420: 0672 616e 646f 6dda 0772 616e 6469 6e74  .random..randint
-00004430: 72ee 0000 0072 f000 0000 72f1 0000 0072  r....r....r....r
-00004440: f200 0000 7209 0000 0072 f300 0000 72f4  ....r....r....r.
-00004450: 0000 0029 07da 0275 6972 4a00 0000 72f6  ...)...uirJ...r.
-00004460: 0000 0072 4401 0000 72fa 0000 0072 fb00  ...rD...r....r..
-00004470: 0000 da04 7265 7370 a902 7245 0000 0072  ....resp..rE...r
-00004480: 4001 0000 7236 0000 0072 3700 0000 da05  @...r6...r7.....
-00004490: 6765 7469 7478 0200 0073 3200 0000 0a01  getitx...s2.....
-000044a0: 0203 0202 0401 06fd 0204 0204 0201 0201  ................
-000044b0: 06fa 0c08 0402 0a01 1201 0c01 1001 0e01  ................
-000044c0: 0a01 0401 0e01 0201 06fe 0a04 0801 0402  ................
-000044d0: 7a18 496e 6465 782e 6765 742e 3c6c 6f63  z.Index.get.<loc
-000044e0: 616c 733e 2e67 6574 6974 2904 7240 0100  als>.getit).r@..
-000044f0: 00da 0a73 7562 7374 5f75 7365 7272 2900  ...subst_userr).
-00004500: 0000 72ed 0000 00a9 0372 4400 0000 7245  ..r......rD...rE
-00004510: 0000 0072 4a01 0000 7236 0000 0072 4901  ...rJ...r6...rI.
-00004520: 0000 7237 0000 0072 7c00 0000 7102 0000  ..r7...r|...q...
-00004530: 730c 0000 0006 0202 0106 0106 010e 020c  s...............
-00004540: 227a 0949 6e64 6578 2e67 6574 4e72 b000  "z.Index.getNr..
-00004550: 0000 7236 0000 0072 3600 0000 7236 0000  ..r6...r6...r6..
-00004560: 0072 3700 0000 7241 0100 006a 0200 0072  .r7...rA...j...r
-00004570: b200 0000 7241 0100 0063 0000 0000 0000  ....rA...c......
-00004580: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00004590: 0000 72a4 0000 0029 05da 0c55 7365 7253  ..r....)...UserS
-000045a0: 6574 7469 6e67 737a 420a 2020 2020 416a  ettingszB.    Aj
-000045b0: 6178 2069 6e74 6572 6661 6365 2066 6f72  ax interface for
-000045c0: 2067 6574 7469 6e67 2074 6865 2063 7572   getting the cur
-000045d0: 7265 6e74 2073 6573 7369 6f6e 2f75 7365  rent session/use
-000045e0: 7220 7365 7474 696e 6773 2e63 0200 0000  r settings.c....
-000045f0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00004600: 0300 0000 734e 0000 0074 007c 0183 017d  ....sN...t.|...}
-00004610: 017c 016a 0189 037c 016a 0289 0188 0172  .|.j...|.j.....r
-00004620: 117c 016a 02a0 03a1 006e 0164 0189 0288  .|.j.....n.d....
-00004630: 036a 0489 0087 0087 0187 0287 0366 0464  .j...........f.d
-00004640: 0264 0384 087d 0274 0588 0170 2388 036a  .d...}.t...p#..j
-00004650: 067c 0283 0253 0029 044e 725c 0000 0063  .|...S.).Nr\...c
-00004660: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00004670: 1100 0000 1300 0000 737c 0100 0074 006a  ........s|...t.j
-00004680: 016a 0272 1174 006a 016a 0373 1174 006a  .j.r.t.j.j.s.t.j
-00004690: 016a 046a 056a 06a0 0764 01a1 0101 0074  .j.j.j...d.....t
-000046a0: 0888 036a 0974 0a88 03a0 0ba1 006a 0c83  ...j.t.......j..
-000046b0: 0188 036a 0d74 0e83 0074 006a 016a 0f74  ...j.t...t.j.j.t
-000046c0: 006a 016a 046a 056a 06a0 10a1 008e 0074  .j.j.j.j.......t
-000046d0: 006a 016a 116a 1288 0088 0072 3488 03a0  .j.j.j.....r4...
-000046e0: 13a1 006e 0374 1464 0283 0188 0274 1464  ...n.t.d.....t.d
-000046f0: 0383 0174 1464 0483 0174 1464 0483 0174  ...t.d...t.d...t
-00004700: 1464 0583 0174 006a 01a0 1564 06a1 0172  .d...t.j...d...r
-00004710: 5074 006a 016a 046a 166a 1770 5374 1464  Pt.j.j.j.j.pSt.d
-00004720: 0783 0188 036a 1864 088d 0f7d 0088 0272  .....j.d...}...r
-00004730: 6888 016a 1904 007c 0064 093c 007c 0064  h..j...|.d.<.|.d
-00004740: 0a3c 0088 016a 097c 0064 0b3c 0088 0072  .<...j.|.d.<...r
-00004750: ba88 03a0 1aa1 007c 0064 0c3c 0088 036a  .......|.d.<...j
-00004760: 1b7c 0064 0d3c 0074 006a 016a 046a 166a  .|.d.<.t.j.j.j.j
-00004770: 1c72 ba88 03a0 1da1 000c 007d 017c 0172  .r.........}.|.r
-00004780: ba88 036a 1e64 0075 0172 ba64 0e7c 0064  ...j.d.u.r.d.|.d
-00004790: 0f3c 0088 036a 1e74 1f6a 2074 006a 016a  .<...j.t.j t.j.j
-000047a0: 046a 166a 2164 108d 0117 007d 0274 22a0  .j.j!d.....}.t".
-000047b0: 2364 11a1 018f 1101 0074 1f6a 1fa0 2474  #d.......t.j..$t
-000047c0: 22a0 257c 02a1 01a1 017d 0357 0064 0004  ".%|.....}.W.d..
-000047d0: 0004 0083 0301 006e 0831 0073 b177 0101  .......n.1.s.w..
-000047e0: 0001 0001 0059 0001 007c 037c 0064 123c  .....Y...|.|.d.<
-000047f0: 0074 267c 0083 0153 0029 134e 46da 0941  .t&|...S.).NF..A
-00004800: 6e6f 6e79 6d6f 7573 7a31 596f 7520 6172  nonymousz1You ar
-00004810: 6520 6175 7468 6f72 6973 6564 2074 6f20  e authorised to 
-00004820: 6163 7420 6173 2074 6865 2066 6f6c 6c6f  act as the follo
-00004830: 7769 6e67 2075 7365 7273 2e7a 1341 6374  wing users.z.Act
-00004840: 2061 7320 616e 6f74 6865 7220 7573 6572   as another user
-00004850: 7a1b 5374 6f70 2061 6374 696e 6720 6173  z.Stop acting as
-00004860: 2061 6e6f 7468 6572 2075 7365 72da 0575   another user..u
-00004870: 7365 7273 7a0b 4d79 2073 6574 7469 6e67  sersz.My setting
-00004880: 7329 0f72 ed00 0000 7228 0100 00da 0565  s).r....r(.....e
-00004890: 6d61 696c 72f8 0000 00da 0973 6974 655f  mailr......site_
-000048a0: 6461 7461 da09 7369 7465 5f6e 616d 65da  data..site_name.
-000048b0: 096c 6f67 6765 645f 696e 7233 0100 00da  .logged_inr3....
-000048c0: 0773 755f 6e61 6d65 da0e 6163 745f 6173  .su_name..act_as
-000048d0: 5f73 7562 7465 7874 da11 6163 745f 6173  _subtext..act_as
-000048e0: 5f74 6974 6c65 5f74 6578 74da 1261 6374  _title_text..act
-000048f0: 5f61 735f 6275 7474 6f6e 5f74 6578 74da  _as_button_text.
-00004900: 1061 6374 5f61 735f 7365 6c66 5f74 6578  .act_as_self_tex
-00004910: 74da 0f6d 795f 7365 7474 696e 675f 7465  t..my_setting_te
-00004920: 7874 da07 7573 6572 5f69 6472 5a01 0000  xt..user_idrZ...
-00004930: da05 7375 5f69 64da 0c73 755f 7573 6572  ..su_id..su_user
-00004940: 5f74 7970 65da 0b61 7574 686f 7269 7469  _type..authoriti
-00004950: 6573 da10 6461 7368 626f 6172 645f 6c61  es..dashboard_la
-00004960: 796f 7574 54da 1472 6571 7569 7265 5f76  youtT..require_v
-00004970: 6572 6966 6963 6174 696f 6e29 01da 076d  erification)...m
-00004980: 696e 7574 6573 da03 5554 43da 0b63 6f64  inutes..UTC..cod
-00004990: 655f 6578 7069 7279 2927 720b 0000 0072  e_expiry)'r....r
-000049a0: 3d00 0000 723b 0100 00da 166e 6576 6572  =...r;.....never
-000049b0: 5f62 7569 6c64 5f73 6974 655f 6361 6368  _build_site_cach
-000049c0: 6572 3e00 0000 723f 0000 0072 3a00 0000  er>...r?...r:...
-000049d0: 723c 0100 0072 9000 0000 72ed 0000 0072  r<...r....r....r
-000049e0: 8f00 0000 7227 0100 0072 2801 0000 7250  ....r'...r(...rP
-000049f0: 0100 0072 1100 0000 da14 6275 696c 645f  ...r......build_
-00004a00: 7369 7465 5f63 6163 6865 5f75 726c da0d  site_cache_url..
-00004a10: 6c69 6e6f 5f6a 735f 7061 7274 73da 0b70  lino_js_parts..p
-00004a20: 726f 6a65 6374 5f64 6972 da04 6e61 6d65  roject_dir..name
-00004a30: da0d 6765 745f 6675 6c6c 5f6e 616d 65da  ..get_full_name.
-00004a40: 015f da0c 6973 5f69 6e73 7461 6c6c 6564  ._..is_installed
-00004a50: 724f 0100 0072 5901 0000 7248 0000 0072  rO...rY...rH...r
-00004a60: 5d00 0000 da0f 6765 745f 6175 7468 6f72  ].....get_author
-00004a70: 6974 6965 7372 5e01 0000 da19 616c 6c6f  itiesr^.....allo
-00004a80: 775f 6f6e 6c69 6e65 5f72 6567 6973 7472  w_online_registr
-00004a90: 6174 696f 6eda 0b69 735f 7665 7269 6669  ation..is_verifi
-00004aa0: 6564 da19 7665 7269 6669 6361 7469 6f6e  ed..verification
-00004ab0: 5f63 6f64 655f 7365 6e74 5f6f 6eda 0864  _code_sent_on..d
-00004ac0: 6174 6574 696d 65da 0974 696d 6564 656c  atetime..timedel
-00004ad0: 7461 da19 7665 7269 6669 6361 7469 6f6e  ta..verification
-00004ae0: 5f63 6f64 655f 6578 7069 7265 7372 0f00  _code_expiresr..
-00004af0: 0000 da08 6f76 6572 7269 6465 da09 7469  ....override..ti
-00004b00: 6d65 7374 616d 70da 0a6d 616b 655f 6e61  mestamp..make_na
-00004b10: 6976 6572 2100 0000 2904 da0d 7573 6572  iver!...)...user
-00004b20: 5f73 6574 7469 6e67 7372 5f01 0000 da0b  _settingsr_.....
-00004b30: 6578 7069 7279 5f74 696d 65da 0c65 7870  expiry_time..exp
-00004b40: 6972 795f 7374 616d 70a9 04da 086e 6f74  iry_stamp....not
-00004b50: 5f61 6e6f 6eda 0273 7572 5401 0000 72f7  _anon..surT...r.
-00004b60: 0000 0072 3600 0000 7237 0000 0072 4a01  ...r6...r7...rJ.
-00004b70: 0000 aa02 0000 7352 0000 0008 0206 0102  ......sR........
-00004b80: ff12 0202 0204 010c 0104 0104 0216 0108  ................
-00004b90: 0102 0112 0102 0106 0106 0106 0106 011e  ................
-00004ba0: 0204 0106 ef04 1412 010a 0104 020c 010a  ................
-00004bb0: 010c 020a 010e 0108 0108 010a 0108 ff0c  ................
-00004bc0: 0306 0108 0106 ff1c ff08 0308 027a 1f55  .............z.U
-00004bd0: 7365 7253 6574 7469 6e67 732e 6765 742e  serSettings.get.
-00004be0: 3c6c 6f63 616c 733e 2e67 6574 6974 2907  <locals>.getit).
-00004bf0: 721c 0000 0072 4001 0000 724b 0100 0072  r....r@...rK...r
-00004c00: 6801 0000 da10 6973 5f61 7574 6865 6e74  h.....is_authent
-00004c10: 6963 6174 6564 7229 0000 0072 ed00 0000  icatedr)...r....
-00004c20: 724c 0100 0072 3600 0000 7278 0100 0072  rL...r6...rx...r
-00004c30: 3700 0000 727c 0000 00a1 0200 0073 0e00  7...r|.......s..
-00004c40: 0000 0801 0601 0601 1201 0603 1202 1032  ...............2
-00004c50: 7a10 5573 6572 5365 7474 696e 6773 2e67  z.UserSettings.g
-00004c60: 6574 4e72 b000 0000 7236 0000 0072 3600  etNr....r6...r6.
-00004c70: 0000 7236 0000 0072 3700 0000 724d 0100  ..r6...r7...rM..
-00004c80: 009d 0200 0073 0600 0000 0800 0401 0c03  .....s..........
-00004c90: 724d 0100 0072 b600 0000 2962 72b1 0000  rM...r....)br...
-00004ca0: 00da 026f 7372 0200 0000 726f 0100 00da  ...osr....ro....
-00004cb0: 0272 65da 0363 6769 da03 6173 7472 d300  .re..cgi..astr..
-00004cc0: 0000 7245 0100 0072 0800 0000 da05 7479  ..rE...r......ty
-00004cd0: 7065 7372 0300 0000 da11 6a69 6e6a 6132  pesr......jinja2
-00004ce0: 2e65 7863 6570 7469 6f6e 7372 0400 0000  .exceptionsr....
-00004cf0: da0a 6574 6765 6e2e 6874 6d6c 7205 0000  ..etgen.htmlr...
-00004d00: 0072 0600 0000 da05 6574 6765 6eda 0678  .r......etgen..x
-00004d10: 6768 746d 6cda 0664 6a61 6e67 6f72 0900  ghtml..djangor..
-00004d20: 0000 da09 646a 616e 676f 2e64 6272 0a00  ....django.dbr..
-00004d30: 0000 da0b 646a 616e 676f 2e63 6f6e 6672  ....django.confr
-00004d40: 0b00 0000 da14 646a 616e 676f 2e76 6965  ......django.vie
-00004d50: 7773 2e67 656e 6572 6963 720c 0000 00da  ws.genericr.....
-00004d60: 1964 6a61 6e67 6f2e 7669 6577 732e 6765  .django.views.ge
-00004d70: 6e65 7269 632e 6261 7365 720d 0000 00da  neric.baser.....
-00004d80: 0b64 6a61 6e67 6f2e 636f 7265 720e 0000  .django.corer...
-00004d90: 00da 0c64 6a61 6e67 6f2e 7574 696c 7372  ...django.utilsr
-00004da0: 0f00 0000 da18 646a 616e 676f 2e75 7469  ......django.uti
-00004db0: 6c73 2e74 7261 6e73 6c61 7469 6f6e 7210  ls.translationr.
-00004dc0: 0000 0072 6901 0000 7211 0000 00da 1664  ...ri...r......d
-00004dd0: 6a61 6e67 6f2e 636f 7265 2e65 7863 6570  jango.core.excep
-00004de0: 7469 6f6e 7372 1200 0000 da09 6c69 6e6f  tionsr......lino
-00004df0: 2e63 6f72 6572 1300 0000 da0a 6c69 6e6f  .corer......lino
-00004e00: 2e75 7469 6c73 7214 0000 00da 106c 696e  .utilsr......lin
-00004e10: 6f2e 7574 696c 732e 6a73 6765 6e72 1500  o.utils.jsgenr..
-00004e20: 0000 7216 0000 00da 0f6c 696e 6f2e 636f  ..r......lino.co
-00004e30: 7265 2e65 6c65 6d73 7217 0000 00da 106c  re.elemsr......l
-00004e40: 696e 6f2e 636f 7265 2e66 6965 6c64 7372  ino.core.fieldsr
-00004e50: 1800 0000 da0e 6c69 6e6f 2e63 6f72 652e  ......lino.core.
-00004e60: 6766 6b73 7219 0000 0072 1b00 0000 da12  gfksr....r......
-00004e70: 6c69 6e6f 2e63 6f72 652e 7265 7175 6573  lino.core.reques
-00004e80: 7473 721c 0000 0072 1d00 0000 da16 6c69  tsr....r......li
-00004e90: 6e6f 2e63 6f72 652e 7461 626c 6572 6571  no.core.tablereq
-00004ea0: 7565 7374 721e 0000 00da 0f6c 696e 6f2e  uestr......lino.
-00004eb0: 636f 7265 2e76 6965 7773 721f 0000 0072  core.viewsr....r
-00004ec0: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-00004ed0: 0000 00da 0f6c 696e 6f2e 636f 7265 2e75  .....lino.core.u
-00004ee0: 7469 6c73 7224 0000 00da 116c 696e 6f2e  tilsr$.....lino.
-00004ef0: 636f 7265 2e61 6374 696f 6e73 7225 0000  core.actionsr%..
-00004f00: 0072 2600 0000 da0f 6c69 6e6f 2e63 6f72  .r&.....lino.cor
-00004f10: 652e 7374 6f72 6572 2700 0000 da17 6c69  e.storer'.....li
-00004f20: 6e6f 2e6d 6f64 6c69 622e 7573 6572 732e  no.modlib.users.
-00004f30: 7574 696c 7372 2800 0000 7229 0000 00da  utilsr(...r)....
-00004f40: 086c 696e 6f2e 6170 6972 2a00 0000 da17  .lino.apir*.....
-00004f50: 6c69 6e6f 2e6d 6f64 6c69 622e 6578 746a  lino.modlib.extj
-00004f60: 732e 7669 6577 7372 2b00 0000 722c 0000  s.viewsr+...r,..
-00004f70: 0072 2d00 0000 7238 0000 0072 e200 0000  .r-...r8...r....
-00004f80: 7259 0000 0072 a500 0000 72b4 0000 0072  rY...r....r....r
-00004f90: c400 0000 72cb 0000 0072 d000 0000 72fc  ....r....r....r.
-00004fa0: 0000 0072 1401 0000 7215 0100 0072 1701  ...r....r....r..
-00004fb0: 0000 7220 0100 0072 2601 0000 722c 0100  ..r ...r&...r,..
-00004fc0: 0072 3101 0000 7241 0100 0072 4d01 0000  .r1...rA...rM...
-00004fd0: 7236 0000 0072 3600 0000 7236 0000 0072  r6...r6...r6...r
-00004fe0: 3700 0000 da08 3c6d 6f64 756c 653e 0100  7.....<module>..
-00004ff0: 0000 737c 0000 0004 040c 0308 0108 0108  ..s|............
-00005000: 0108 0108 0108 0108 010c 010c 0110 010c  ................
-00005010: 010c 020c 010c 010c 010c 010c 010c 010c  ................
-00005020: 010c 010c 010c 030c 010c 010c 010c 010c  ................
-00005030: 010c 010c 0110 010c 0110 0110 010c 010c  ................
-00005040: 010c 010c 010c 0110 020c 0114 010a 0304  ................
-00005050: 0e10 0710 2210 7110 0f10 2a10 1f10 1008  ....".q...*.....
-00005060: 5e08 1310 4310 0410 0810 1010 1610 0a10  ^...C...........
-00005070: 3214 33                                  2.3
+00000700: da01 78a9 0072 3600 0000 fa42 2f68 6f6d  ..x..r6....B/hom
+00000710: 652f 626c 7572 7279 2f6c 696e 6f2f 656e  e/blurry/lino/en
+00000720: 762f 7265 706f 7369 746f 7269 6573 2f72  v/repositories/r
+00000730: 6561 6374 2f6c 696e 6f5f 7265 6163 742f  eact/lino_react/
+00000740: 7265 6163 742f 7669 6577 732e 7079 da04  react/views.py..
+00000750: 6669 6e64 3800 0000 7310 0000 0018 0210  find8...s.......
+00000760: 0204 0108 0108 0108 0102 ff04 0372 3800  .............r8.
+00000770: 0000 7a21 2573 2068 6173 206e 6f20 726f  ..z!%s has no ro
+00000780: 7720 7769 7468 2070 7269 6d61 7279 206b  w with primary k
+00000790: 6579 2025 7263 0000 0000 0000 0000 0000  ey %rc..........
+000007a0: 0000 0000 0000 0300 0000 4000 0000 732a  ..........@...s*
+000007b0: 0000 0065 005a 0164 005a 0264 0864 0264  ...e.Z.d.Z.d.d.d
+000007c0: 0384 015a 0364 0864 0464 0584 015a 0464  ...Z.d.d.d...Z.d
+000007d0: 0864 0664 0784 015a 0564 0153 0029 0972  .d.d...Z.d.S.).r
+000007e0: 2b00 0000 4e63 0500 0000 0000 0000 0000  +...Nc..........
+000007f0: 0000 0800 0000 0800 0000 4300 0000 7354  ..........C...sT
+00000800: 0000 007c 016a 007d 0574 017c 027c 037c  ...|.j.}.t.|.|.|
+00000810: 017c 0564 0174 026a 036a 046a 056a 0664  .|.d.t.j.j.j.j.d
+00000820: 028d 067d 067c 0464 036b 0272 1e7c 06a0  ...}.|.d.k.r.|..
+00000830: 07a1 007d 077c 0767 017c 065f 086e 057c  ...}.|.g.|._.n.|
+00000840: 06a0 097c 04a1 0101 0074 026a 036a 0aa0  ...|.....t.j.j..
+00000850: 0b7c 06a1 0153 0029 044e 54a9 01da 0872  .|...S.).NT....r
+00000860: 656e 6465 7265 72fa 062d 3939 3939 3829  enderer..-99998)
+00000870: 0cda 0450 4f53 5472 2000 0000 720b 0000  ...POSTr ...r...
+00000880: 00da 0453 4954 45da 0770 6c75 6769 6e73  ...SITE..plugins
+00000890: da05 7265 6163 7472 3a00 0000 da0f 6372  ..reactr:.....cr
+000008a0: 6561 7465 5f69 6e73 7461 6e63 65da 0d73  eate_instance..s
+000008b0: 656c 6563 7465 645f 726f 7773 da10 7365  elected_rows..se
+000008c0: 745f 7365 6c65 6374 6564 5f70 6b73 7226  t_selected_pksr&
+000008d0: 0000 00da 0a72 756e 5f61 6374 696f 6e29  .....run_action)
+000008e0: 08da 0473 656c 66da 0772 6571 7565 7374  ...self..request
+000008f0: da09 6170 705f 6c61 6265 6cda 0561 6374  ..app_label..act
+00000900: 6f72 da02 706b da04 6461 7461 da02 6172  or..pk..data..ar
+00000910: da04 656c 656d 7236 0000 0072 3600 0000  ..elemr6...r6...
+00000920: 7237 0000 00da 0470 6f73 744f 0000 0073  r7.....postO...s
+00000930: 1400 0000 0602 0201 0a01 0a01 06fe 0803  ................
+00000940: 0801 0a01 0a02 0e01 7a0f 4170 6945 6c65  ........z.ApiEle
+00000950: 6d65 6e74 2e70 6f73 7463 0500 0000 0000  ment.postc......
+00000960: 0000 0000 0000 0700 0000 0800 0000 4300  ..............C.
+00000970: 0000 f340 0000 0074 00a0 017c 016a 02a1  ...@...t...|.j..
+00000980: 017d 0574 037c 027c 037c 017c 0564 0174  .}.t.|.|.|.|.d.t
+00000990: 046a 056a 066a 076a 0864 028d 067d 067c  .j.j.j.j.d...}.|
+000009a0: 06a0 097c 04a1 0101 0074 046a 056a 0aa0  ...|.....t.j.j..
+000009b0: 0b7c 06a1 0153 00a9 034e 4672 3900 0000  .|...S...NFr9...
+000009c0: a90c 7209 0000 00da 0951 7565 7279 4469  ..r......QueryDi
+000009d0: 6374 da04 626f 6479 7220 0000 0072 0b00  ct..bodyr ...r..
+000009e0: 0000 723d 0000 0072 3e00 0000 723f 0000  ..r=...r>...r?..
+000009f0: 0072 3a00 0000 7242 0000 0072 2600 0000  .r:...rB...r&...
+00000a00: 7243 0000 00a9 0772 4400 0000 7245 0000  rC.....rD...rE..
+00000a10: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
+00000a20: 7249 0000 0072 4a00 0000 7236 0000 0072  rI...rJ...r6...r
+00000a30: 3600 0000 7237 0000 00da 0370 7574 5c00  6...r7.....put\.
+00000a40: 0000 730e 0000 000c 0102 030a 010a 0106  ..s.............
+00000a50: fe0a 030e 017a 0e41 7069 456c 656d 656e  .....z.ApiElemen
+00000a60: 742e 7075 7463 0500 0000 0000 0000 0000  t.putc..........
+00000a70: 0000 0700 0000 0800 0000 4300 0000 724d  ..........C...rM
+00000a80: 0000 0072 4e00 0000 724f 0000 0072 5200  ...rN...rO...rR.
+00000a90: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00000aa0: 00da 0664 656c 6574 6566 0000 0073 0e00  ...deletef...s..
+00000ab0: 0000 0c01 0201 0a01 0a01 06fe 0a03 0e01  ................
+00000ac0: 7a11 4170 6945 6c65 6d65 6e74 2e64 656c  z.ApiElement.del
+00000ad0: 6574 65a9 034e 4e4e 2906 da08 5f5f 6e61  ete..NNN)...__na
+00000ae0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000af0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 724c  ..__qualname__rL
+00000b00: 0000 0072 5300 0000 7254 0000 0072 3600  ...rS...rT...r6.
+00000b10: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00000b20: 0072 2b00 0000 4d00 0000 7308 0000 0008  .r+...M...s.....
+00000b30: 000a 020a 0d0e 0a72 2b00 0000 6300 0000  .......r+...c...
+00000b40: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000b50: 0040 0000 0073 2000 0000 6500 5a01 6400  .@...s ...e.Z.d.
+00000b60: 5a02 6406 6402 6403 8401 5a03 6406 6404  Z.d.d.d...Z.d.d.
+00000b70: 6405 8401 5a04 6401 5300 2907 da07 4170  d...Z.d.S.)...Ap
+00000b80: 694c 6973 744e 6304 0000 0000 0000 0000  iListNc.........
+00000b90: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00000ba0: 3400 0000 7400 7c02 7c03 7c01 7c01 6a01  4...t.|.|.|.|.j.
+00000bb0: 6401 8305 7d04 7c04 a002 a100 0100 7403  d...}.|.......t.
+00000bc0: 6a04 6a05 6a06 7c04 5f07 7403 6a04 6a05  j.j.j.|._.t.j.j.
+00000bd0: a008 7c04 a101 5300 2902 4e54 2909 7220  ..|...S.).NT).r 
+00000be0: 0000 0072 3c00 0000 da0a 6765 745f 7374  ...r<.....get_st
+00000bf0: 6174 7573 720b 0000 0072 3d00 0000 7226  atusr....r=...r&
+00000c00: 0000 00da 1064 6566 6175 6c74 5f72 656e  .....default_ren
+00000c10: 6465 7265 7272 3a00 0000 7243 0000 0029  dererr:...rC...)
+00000c20: 0572 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
+00000c30: 7247 0000 0072 4a00 0000 7236 0000 0072  rG...rJ...r6...r
+00000c40: 3600 0000 7237 0000 0072 4c00 0000 7000  6...r7...rL...p.
+00000c50: 0000 7308 0000 0012 0108 010c 010e 017a  ..s............z
+00000c60: 0c41 7069 4c69 7374 2e70 6f73 7463 0400  .ApiList.postc..
+00000c70: 0000 0000 0000 0000 0000 1300 0000 0800  ................
+00000c80: 0000 0300 0000 7376 0200 0074 007c 0183  ......sv...t.|..
+00000c90: 017d 047c 0472 0a74 017c 0483 0153 0074  .}.|.r.t.|...S.t
+00000ca0: 027c 027c 037c 017c 016a 0364 0183 0589  .|.|.|.|.j.d....
+00000cb0: 0088 00a0 04a1 0073 2064 02a0 0588 00a1  .......s d......
+00000cc0: 017d 0574 067c 0583 0182 0174 076a 086a  .}.t.|.....t.j.j
+00000cd0: 096a 0a88 005f 0b88 006a 0c89 027c 016a  .j..._...j...|.j
+00000ce0: 03a0 0d74 0e6a 0f88 006a 106a 116a 12a1  ...t.j...j.j.j..
+00000cf0: 027d 067c 016a 03a0 0d74 0e6a 13a1 017d  .}.|.j...t.j...}
+00000d00: 077c 0772 4474 076a 086a 09a0 1488 00a1  .|.rDt.j.j......
+00000d10: 0153 007c 0674 0e6a 156b 0290 0172 3474  .S.|.t.j.k...r4t
+00000d20: 1688 006a 106a 1174 1783 0272 6088 00a0  ...j.j.t...r`...
+00000d30: 18a1 007d 0874 1988 0088 006a 0c7c 0883  ...}.t.....j.|..
+00000d40: 037d 0974 017c 0983 0153 007c 016a 03a0  .}.t.|...S.|.j..
+00000d50: 0d74 0e6a 1a74 0e6a 1ba1 0289 0188 0174  .t.j.t.j.......t
+00000d60: 0e6a 1c6b 0272 8864 037d 0a67 007d 0b88  .j.k.r.d.}.g.}..
+00000d70: 006a 1d44 005d 117d 0c7c 0a7c 0ca0 1e88  .j.D.].}.|.|....
+00000d80: 00a1 0137 007d 0a7c 0ba0 1f64 047c 0c6a  ...7.}.|...d.|.j
+00000d90: 2069 01a1 0101 0071 756e 4088 0174 0e6a   i.....qun@..t.j
+00000da0: 216b 0272 b464 037d 0a67 007d 0b88 006a  !k.r.d.}.g.}...j
+00000db0: 1d44 005d 1e7d 0c88 00a0 227c 0ca1 017d  .D.].}...."|...}
+00000dc0: 0d88 00a0 237c 0c7c 0da1 027d 0d64 05a0  ....#|.|...}.d..
+00000dd0: 057c 0da1 017d 0d7c 0a7c 0d37 007d 0a7c  .|...}.|.|.7.}.|
+00000de0: 0ba0 1f64 047c 0c6a 2069 01a1 0101 0071  ...d.|.j i.....q
+00000df0: 946e 1464 007d 0a87 0187 0266 0264 0664  .n.d.}.....f.d.d
+00000e00: 0784 0889 0387 0087 0366 0264 0864 0984  .........f.d.d..
+00000e10: 0888 006a 1d44 0083 017d 0b88 00a0 24a1  ...j.D...}....$.
+00000e20: 007d 0e88 0174 0e6a 1b6b 0272 fb88 00a0  .}...t.j.k.r....
+00000e30: 25a1 0044 005d 257d 0f88 006a 2664 0075  %..D.]%}...j&d.u
+00000e40: 0073 ec74 277c 0b83 0164 0a17 0088 006a  .s.t'|...d.....j
+00000e50: 266b 0073 ec88 006a 267c 0e64 0a17 006b  &k.s...j&|.d...k
+00000e60: 0272 f688 0388 007c 0f83 027d 107c 0ba0  .r.....|...}.|..
+00000e70: 1f7c 10a1 0101 007c 0e64 0a37 007d 0e71  .|.....|.d.7.}.q
+00000e80: d574 287c 0e7c 0b7c 0a64 0188 006a 2988  .t(|.|.|.d...j).
+00000e90: 00a0 2aa1 0064 0b8d 067d 1188 0174 0e6a  ..*..d...}...t.j
+00000ea0: 1b6b 0390 0172 1d88 00a0 2ba1 007d 127c  .k...r....+..}.|
+00000eb0: 1264 0075 0190 0172 1d7c 0ba0 2c64 0c7c  .d.u...r.|..,d.|
+00000ec0: 12a1 0201 0088 006a 2d6a 2e90 0172 307c  .......j-j...r0|
+00000ed0: 116a 2f88 006a 2d6a 306a 31a0 3288 0088  .j/..j-j0j1.2...
+00000ee0: 006a 33a1 0264 0d8d 0101 0074 017c 1183  .j3..d.....t.|..
+00000ef0: 0153 0074 076a 086a 09a0 1488 00a1 0153  .S.t.j.j.......S
+00000f00: 0029 0e4e 547a 174e 6f20 7065 726d 6973  .).NTz.No permis
+00000f10: 7369 6f6e 2074 6f20 7275 6e20 7b7d da00  sion to run {}..
+00000f20: da02 6964 7a09 3c70 3e7b 7d3c 2f70 3e63  ..idz.<p>{}</p>c
+00000f30: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000f40: 0700 0000 1300 0000 7362 0000 0088 0074  ........sb.....t
+00000f50: 006a 016b 0272 0c88 016a 02a0 037c 007c  .j.k.r...j...|.|
+00000f60: 01a1 0253 0088 0074 006a 046b 0272 167c  ...S...t.j.k.r.|
+00000f70: 01a0 057c 00a1 0153 0088 0074 006a 066b  ...|...S...t.j.k
+00000f80: 0272 2088 016a 026a 077d 026e 0488 016a  .r ..j.j.}.n...j
+00000f90: 026a 087d 0288 016a 026a 097c 007c 017c  .j.}...j.j.|.|.|
+00000fa0: 027c 00a0 0a7c 01a1 0164 018d 0453 0029  .|...|...d...S.)
+00000fb0: 027a 4f55 7365 2064 6973 706c 6179 5f6d  .zOUse display_m
+00000fc0: 6f64 6520 746f 2064 6574 6572 6d69 6e65  ode to determine
+00000fd0: 2077 6869 6368 2073 6572 696c 6973 6174   which serilisat
+00000fe0: 696f 6e20 7374 6f72 6520 6d65 7468 6f64  ion store method
+00000ff0: 2061 6e64 2066 6965 6c64 7320 746f 2075   and fields to u
+00001000: 7365 2902 7216 0000 00da 0a63 6172 645f  se).r......card_
+00001010: 7469 746c 6529 0b72 1b00 0000 da12 4449  title).r......DI
+00001020: 5350 4c41 595f 4d4f 4445 5f54 4142 4c45  SPLAY_MODE_TABLE
+00001030: da05 7374 6f72 65da 0872 6f77 326c 6973  ..store..row2lis
+00001040: 74da 1444 4953 504c 4159 5f4d 4f44 455f  t..DISPLAY_MODE_
+00001050: 4741 4c4c 4552 59da 1067 6574 5f67 616c  GALLERY..get_gal
+00001060: 6c65 7279 5f69 7465 6dda 1244 4953 504c  lery_item..DISPL
+00001070: 4159 5f4d 4f44 455f 4341 5244 53da 0b63  AY_MODE_CARDS..c
+00001080: 6172 645f 6669 656c 6473 da0d 6465 7461  ard_fields..deta
+00001090: 696c 5f66 6965 6c64 73da 0872 6f77 3264  il_fields..row2d
+000010a0: 6963 74da 0e67 6574 5f63 6172 645f 7469  ict..get_card_ti
+000010b0: 746c 6529 0372 4a00 0000 da03 726f 7772  tle).rJ.....rowr
+000010c0: 1600 0000 2902 da0c 6469 7370 6c61 795f  ....)...display_
+000010d0: 6d6f 6465 da02 7268 7236 0000 0072 3700  mode..rhr6...r7.
+000010e0: 0000 da09 7365 7269 616c 697a 65b3 0000  ....serialize...
+000010f0: 0073 1400 0000 0a02 0e01 0a01 0a02 0a02  .s..............
+00001100: 0a01 0802 0801 0c01 06ff 7a1e 4170 694c  ..........z.ApiL
+00001110: 6973 742e 6765 742e 3c6c 6f63 616c 733e  ist.get.<locals>
+00001120: 2e73 6572 6961 6c69 7a65 6301 0000 0000  .serializec.....
+00001130: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00001140: 0000 0073 1600 0000 6700 7c00 5d07 7d01  ...s....g.|.].}.
+00001150: 8801 8800 7c01 8302 9102 7102 5300 7236  ....|.....q.S.r6
+00001160: 0000 0072 3600 0000 a902 da02 2e30 7269  ...r6........0ri
+00001170: 0000 0029 0272 4a00 0000 726c 0000 0072  ...).rJ...rl...r
+00001180: 3600 0000 7237 0000 00da 0a3c 6c69 7374  6...r7.....<list
+00001190: 636f 6d70 3ec2 0000 0073 0600 0000 0600  comp>....s......
+000011a0: 0201 0eff 7a1f 4170 694c 6973 742e 6765  ....z.ApiList.ge
+000011b0: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
+000011c0: 636f 6d70 3ee9 0100 0000 2906 da05 636f  comp>.....)...co
+000011d0: 756e 74da 0472 6f77 73da 0968 746d 6c5f  unt..rows..html_
+000011e0: 7465 7874 da07 7375 6363 6573 73da 0c6e  text..success..n
+000011f0: 6f5f 6461 7461 5f74 6578 74da 0574 6974  o_data_text..tit
+00001200: 6c65 7201 0000 0029 01da 0c70 6172 616d  ler....)...param
+00001210: 5f76 616c 7565 7329 3472 2c00 0000 7221  _values)4r,...r!
+00001220: 0000 0072 2000 0000 da03 4745 54da 0e67  ...r .....GET..g
+00001230: 6574 5f70 6572 6d69 7373 696f 6eda 0666  et_permission..f
+00001240: 6f72 6d61 7472 1200 0000 720b 0000 0072  ormatr....r....r
+00001250: 3d00 0000 7226 0000 0072 5b00 0000 723a  =...r&...r[...r:
+00001260: 0000 00da 0261 68da 0367 6574 721b 0000  .....ah..getr...
+00001270: 00da 1055 524c 5f50 4152 414d 5f46 4f52  ...URL_PARAM_FOR
+00001280: 4d41 54da 0c62 6f75 6e64 5f61 6374 696f  MAT..bound_actio
+00001290: 6eda 0661 6374 696f 6eda 0e64 6566 6175  n..action..defau
+000012a0: 6c74 5f66 6f72 6d61 74da 1555 524c 5f50  lt_format..URL_P
+000012b0: 4152 414d 5f41 4354 494f 4e5f 4e41 4d45  ARAM_ACTION_NAME
+000012c0: 7243 0000 00da 0f55 524c 5f46 4f52 4d41  rC.....URL_FORMA
+000012d0: 545f 4a53 4f4e da0a 6973 696e 7374 616e  T_JSON..isinstan
+000012e0: 6365 7225 0000 0072 4000 0000 722d 0000  cer%...r@...r-..
+000012f0: 00da 1655 524c 5f50 4152 414d 5f44 4953  ...URL_PARAM_DIS
+00001300: 504c 4159 5f4d 4f44 4572 5f00 0000 da12  PLAY_MODEr_.....
+00001310: 4449 5350 4c41 595f 4d4f 4445 5f53 544f  DISPLAY_MODE_STO
+00001320: 5259 da14 736c 6963 6564 5f64 6174 615f  RY..sliced_data_
+00001330: 6974 6572 6174 6f72 da0d 6173 5f73 746f  iterator..as_sto
+00001340: 7279 5f69 7465 6dda 0661 7070 656e 6472  ry_item..appendr
+00001350: 4800 0000 da11 4449 5350 4c41 595f 4d4f  H.....DISPLAY_MO
+00001360: 4445 5f4c 4953 54da 1072 6f77 5f61 735f  DE_LIST..row_as_
+00001370: 7061 7261 6772 6170 68da 0f61 6464 5f64  paragraph..add_d
+00001380: 6574 6169 6c5f 6c69 6e6b da0f 6765 745f  etail_link..get_
+00001390: 746f 7461 6c5f 636f 756e 74da 1363 7265  total_count..cre
+000013a0: 6174 655f 7068 616e 746f 6d5f 726f 7773  ate_phantom_rows
+000013b0: da05 6c69 6d69 74da 036c 656e da04 6469  ..limit..len..di
+000013c0: 6374 7275 0000 00da 0967 6574 5f74 6974  ctru.....get_tit
+000013d0: 6c65 da0d 6765 745f 6d61 696e 5f63 6172  le..get_main_car
+000013e0: 64da 0669 6e73 6572 7472 4700 0000 da0a  d..insertrG.....
+000013f0: 7061 7261 6d65 7465 7273 da06 7570 6461  parameters..upda
+00001400: 7465 da0d 7061 7261 6d73 5f6c 6179 6f75  te..params_layou
+00001410: 74da 0c70 6172 616d 735f 7374 6f72 65da  t..params_store.
+00001420: 0770 7632 6469 6374 7277 0000 0029 1372  .pv2dictrw...).r
+00001430: 4400 0000 7245 0000 0072 4600 0000 7247  D...rE...rF...rG
+00001440: 0000 00da 0276 6dda 036d 7367 da03 666d  .....vm..msg..fm
+00001450: 74da 0b61 6374 696f 6e5f 6e61 6d65 724b  t..action_namerK
+00001460: 0000 00da 0764 6174 6172 6563 7273 0000  .....datarecrs..
+00001470: 0072 7200 0000 da03 6f62 6ada 0370 6172  .rr.....obj..par
+00001480: da0b 746f 7461 6c5f 636f 756e 7472 6900  ..total_countri.
+00001490: 0000 da01 64da 026b 77da 026d 6372 3600  ....d..kw..mcr6.
+000014a0: 0000 2904 724a 0000 0072 6a00 0000 726b  ..).rJ...rj...rk
+000014b0: 0000 0072 6c00 0000 7237 0000 0072 7c00  ...rl...r7...r|.
+000014c0: 0000 7600 0000 7390 0000 0008 0104 0108  ..v...s.........
+000014d0: 0112 0108 080a 0108 020c 0206 0106 0204  ................
+000014e0: 0108 0104 fe0e 0404 020e 010c 020e 0108  ................
+000014f0: 010e 0108 0106 0208 0104 ff0a 0304 0104  ................
+00001500: 010a 010e 0112 0102 fe0a 0304 0104 010a  ................
+00001510: 010a 010c 010a 0208 0612 0102 f504 0d0e  ................
+00001520: 010c 0f04 0106 ff08 030a 010c 012a 010a  .............*..
+00001530: 010a 010a 0104 0202 0102 0102 0104 0106  ................
+00001540: 0106 fb0c 0608 010a 010c 010a 0104 010a  ................
+00001550: 0106 0102 ff06 ff08 030e 027a 0b41 7069  ...........z.Api
+00001560: 4c69 7374 2e67 6574 2902 4e4e 2905 7256  List.get).NN).rV
+00001570: 0000 0072 5700 0000 7258 0000 0072 4c00  ...rW...rX...rL.
+00001580: 0000 727c 0000 0072 3600 0000 7236 0000  ..r|...r6...r6..
+00001590: 0072 3600 0000 7237 0000 0072 5900 0000  .r6...r7...rY...
+000015a0: 6f00 0000 7306 0000 0008 000a 010e 0672  o...s..........r
+000015b0: 5900 0000 6300 0000 0000 0000 0000 0000  Y...c...........
+000015c0: 0000 0000 0002 0000 0040 0000 00f3 1800  .........@......
+000015d0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+000015e0: 6403 8400 5a04 6404 5300 2905 da0f 4368  d...Z.d.S.)...Ch
+000015f0: 6f69 6365 4c69 7374 4d6f 6465 6c7a a20a  oiceListModelz..
+00001600: 2020 2020 4372 6561 7465 7320 6120 6c61      Creates a la
+00001610: 7267 6520 4a53 4f4e 206d 6f64 656c 2074  rge JSON model t
+00001620: 6861 7420 636f 6e74 6169 6e73 2061 6c6c  hat contains all
+00001630: 2074 6865 2063 686f 6963 656c 6973 7473   the choicelists
+00001640: 202b 2063 686f 6963 6573 0a0a 2020 2020   + choices..    
+00001650: 4e6f 7465 3a20 5468 6973 2063 6f75 6c64  Note: This could
+00001660: 2062 6520 696d 7072 6f76 6564 2c20 6f72   be improved, or
+00001670: 206d 6967 6874 2063 6175 7365 2069 7373   might cause iss
+00001680: 7565 7320 6475 6520 746f 2063 6861 6e67  ues due to chang
+00001690: 696e 6720 6c61 6e67 7561 6765 0a20 2020  ing language.   
+000016a0: 2063 0200 0000 0000 0000 0000 0000 0300   c..............
+000016b0: 0000 0300 0000 4300 0000 731c 0000 0064  ......C...s....d
+000016c0: 0164 0284 0074 006a 01a0 02a1 0044 0083  .d...t.j.....D..
+000016d0: 017d 0274 037c 0283 0153 0029 034e 6301  .}.t.|...S.).Nc.
+000016e0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+000016f0: 0000 0053 0000 0073 2400 0000 6900 7c00  ...S...s$...i.|.
+00001700: 5d0e 7d01 7400 7c01 8301 6400 6401 8400  ].}.t.|...d.d...
+00001710: 7c01 a001 a100 4400 8301 9302 7102 5300  |.....D.....q.S.
+00001720: 2902 6301 0000 0000 0000 0000 0000 0002  ).c.............
+00001730: 0000 0006 0000 0053 0000 0073 3200 0000  .......S...s2...
+00001740: 6700 7c00 5d15 7d01 7400 7c01 6400 1900  g.|.].}.t.|.d...
+00001750: 8301 a001 6401 a101 7400 7c01 6402 1900  ....d...t.|.d...
+00001760: 8301 a001 6401 a101 6403 9c02 9102 7102  ....d...d.....q.
+00001770: 5300 2904 7201 0000 00fa 0122 7270 0000  S.).r......"rp..
+00001780: 0029 0272 3300 0000 da04 7465 7874 2902  .).r3.....text).
+00001790: 7215 0000 00da 0573 7472 6970 2902 726e  r......strip).rn
+000017a0: 0000 00da 0163 7236 0000 0072 3600 0000  .....cr6...r6...
+000017b0: 7237 0000 0072 6f00 0000 e800 0000 7302  r7...ro.......s.
+000017c0: 0000 0032 007a 3243 686f 6963 654c 6973  ...2.z2ChoiceLis
+000017d0: 744d 6f64 656c 2e67 6574 2e3c 6c6f 6361  tModel.get.<loca
+000017e0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2e3c  ls>.<dictcomp>.<
+000017f0: 6c69 7374 636f 6d70 3e29 02da 0373 7472  listcomp>)...str
+00001800: da0b 6765 745f 6368 6f69 6365 7329 0272  ..get_choices).r
+00001810: 6e00 0000 da02 636c 7236 0000 0072 3600  n.....clr6...r6.
+00001820: 0000 7237 0000 00da 0a3c 6469 6374 636f  ..r7.....<dictco
+00001830: 6d70 3ee8 0000 0073 0600 0000 0600 0201  mp>....s........
+00001840: 1cff 7a27 4368 6f69 6365 4c69 7374 4d6f  ..z'ChoiceListMo
+00001850: 6465 6c2e 6765 742e 3c6c 6f63 616c 733e  del.get.<locals>
+00001860: 2e3c 6469 6374 636f 6d70 3e29 0472 2600  .<dictcomp>).r&.
+00001870: 0000 da0b 4348 4f49 4345 4c49 5354 53da  ....CHOICELISTS.
+00001880: 0676 616c 7565 7372 2100 0000 2903 7244  .valuesr!...).rD
+00001890: 0000 0072 4500 0000 7249 0000 0072 3600  ...rE...rI...r6.
+000018a0: 0000 7236 0000 0072 3700 0000 727c 0000  ..r6...r7...r|..
+000018b0: 00e7 0000 0073 0800 0000 0601 0802 06fe  .....s..........
+000018c0: 0803 7a13 4368 6f69 6365 4c69 7374 4d6f  ..z.ChoiceListMo
+000018d0: 6465 6c2e 6765 744e a905 7256 0000 0072  del.getN..rV...r
+000018e0: 5700 0000 7258 0000 00da 075f 5f64 6f63  W...rX.....__doc
+000018f0: 5f5f 727c 0000 0072 3600 0000 7236 0000  __r|...r6...r6..
+00001900: 0072 3600 0000 7237 0000 0072 a500 0000  .r6...r7...r....
+00001910: e000 0000 f306 0000 0008 0004 010c 0672  ...............r
+00001920: a500 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00001930: 0000 0000 0003 0000 0040 0000 00f3 1600  .........@......
+00001940: 0000 6500 5a01 6400 5a02 6404 6402 6403  ..e.Z.d.Z.d.d.d.
+00001950: 8401 5a03 6401 5300 2905 da07 4368 6f69  ..Z.d.S.)...Choi
+00001960: 6365 734e 6305 0000 0000 0000 0000 0000  cesNc...........
+00001970: 000b 0000 0008 0000 004b 0000 0073 7c00  .........K...s|.
+00001980: 0000 7400 7c02 7c03 8302 7d06 6401 7d07  ..t.|.|...}.d.}.
+00001990: 7c04 6401 7500 7219 7c06 6a01 7c01 6402  |.d.u.r.|.j.|.d.
+000019a0: 8d01 7d08 7c08 6a02 7d09 6403 6404 8400  ..}.|.j.}.d.d...
+000019b0: 7d0a 6e1b 7c06 a003 7c04 a101 7022 7c06  }.n.|...|...p"|.
+000019c0: a004 7c04 a101 7d04 7c04 6a05 7228 6405  ..|...}.|.j.r(d.
+000019d0: 7d07 7406 7c06 6a01 7c01 6402 8d01 7c06  }.t.|.j.|.d...|.
+000019e0: 7c04 8303 5c02 7d09 7d0a 7407 7c06 7c01  |...\.}.}.t.|.|.
+000019f0: 7c09 7c0a 7c07 7c04 6406 8d06 5300 2907  |.|.|.|.d...S.).
+00001a00: 6141 0100 0049 6620 6066 6c64 6e61 6d65  aA...If `fldname
+00001a10: 6020 6973 2073 7065 6369 6669 6564 2c20  ` is specified, 
+00001a20: 7265 7475 726e 2061 204a 534f 4e20 6f62  return a JSON ob
+00001a30: 6a65 6374 2077 6974 6820 7477 6f0a 2020  ject with two.  
+00001a40: 2020 2020 2020 6174 7472 6962 7574 6573        attributes
+00001a50: 2060 636f 756e 7460 2061 6e64 2060 726f   `count` and `ro
+00001a60: 7773 602c 2077 6865 7265 2060 726f 7773  ws`, where `rows
+00001a70: 6020 6973 2061 206c 6973 7420 6f66 0a20  ` is a list of. 
+00001a80: 2020 2020 2020 2060 2864 6973 706c 6179         `(display
+00001a90: 5f74 6578 742c 2076 616c 7565 2960 2074  _text, value)` t
+00001aa0: 7570 6c65 732e 2020 5573 6564 2062 7920  uples.  Used by 
+00001ab0: 436f 6d62 6f42 6f78 6573 206f 7220 7369  ComboBoxes or si
+00001ac0: 6d69 6c61 720a 2020 2020 2020 2020 7769  milar.        wi
+00001ad0: 6467 6574 732e 0a0a 2020 2020 2020 2020  dgets...        
+00001ae0: 4966 2060 666c 646e 616d 6560 2069 7320  If `fldname` is 
+00001af0: 6e6f 7420 7370 6563 6966 6965 642c 2072  not specified, r
+00001b00: 6574 7572 6e73 2074 6865 2063 686f 6963  eturns the choic
+00001b10: 6573 2066 6f72 2074 6865 0a20 2020 2020  es for the.     
+00001b20: 2020 2060 7265 636f 7264 5f73 656c 6563     `record_selec
+00001b30: 746f 7260 2077 6964 6765 742e 0a0a 2020  tor` widget...  
+00001b40: 2020 2020 2020 4ea9 0172 4500 0000 6302        N..rE...c.
+00001b50: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001b60: 0000 0053 0000 0073 1e00 0000 7400 7c00  ...S...s....t.|.
+00001b70: 8301 7c01 7401 6a02 3c00 7c00 6a03 7c01  ..|.t.j.<.|.j.|.
+00001b80: 7401 6a04 3c00 7c01 5300 a901 4e29 0572  t.j.<.|.S...N).r
+00001b90: aa00 0000 721b 0000 00da 1243 484f 4943  ....r......CHOIC
+00001ba0: 4553 5f54 4558 545f 4649 454c 4472 4800  ES_TEXT_FIELDrH.
+00001bb0: 0000 da13 4348 4f49 4345 535f 5641 4c55  ....CHOICES_VALU
+00001bc0: 455f 4649 454c 4429 0272 9e00 0000 72a1  E_FIELD).r....r.
+00001bd0: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00001be0: 0000 7267 0000 0007 0100 0073 0600 0000  ..rg.......s....
+00001bf0: 0e01 0c02 0401 7a1d 4368 6f69 6365 732e  ......z.Choices.
+00001c00: 6765 742e 3c6c 6f63 616c 733e 2e72 6f77  get.<locals>.row
+00001c10: 3264 6963 7472 5c00 0000 a901 da05 6669  2dictr\.......fi
+00001c20: 656c 6429 0872 1f00 0000 7245 0000 00da  eld).r....rE....
+00001c30: 0d64 6174 615f 6974 6572 6174 6f72 da0e  .data_iterator..
+00001c40: 6765 745f 7061 7261 6d5f 656c 656d da0d  get_param_elem..
+00001c50: 6765 745f 6461 7461 5f65 6c65 6dda 0562  get_data_elem..b
+00001c60: 6c61 6e6b 7218 0000 0072 2300 0000 290b  lankr....r#...).
+00001c70: 7244 0000 0072 4500 0000 7246 0000 0072  rD...rE...rF...r
+00001c80: 4700 0000 72ba 0000 0072 a200 0000 da03  G...r....r......
+00001c90: 7270 74da 0a65 6d70 7479 5661 6c75 6572  rpt..emptyValuer
+00001ca0: 4a00 0000 da02 7173 7267 0000 0072 3600  J.....qsrg...r6.
+00001cb0: 0000 7236 0000 0072 3700 0000 727c 0000  ..r6...r7...r|..
+00001cc0: 00f0 0000 0073 1600 0000 0a0a 0401 0801  .....s..........
+00001cd0: 0c01 0606 0a04 1409 0601 0402 1801 1402  ................
+00001ce0: 7a0b 4368 6f69 6365 732e 6765 7472 5500  z.Choices.getrU.
+00001cf0: 0000 a904 7256 0000 0072 5700 0000 7258  ....rV...rW...rX
+00001d00: 0000 0072 7c00 0000 7236 0000 0072 3600  ...r|...r6...r6.
+00001d10: 0000 7236 0000 0072 3700 0000 72b4 0000  ..r6...r7...r...
+00001d20: 00ef 0000 00f3 0400 0000 0800 0e01 72b4  ..............r.
+00001d30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001d40: 0000 0000 0300 0000 4000 0000 72b3 0000  ........@...r...
+00001d50: 0029 05da 0c44 656c 6179 6564 5661 6c75  .)...DelayedValu
+00001d60: 654e 6306 0000 0000 0000 0000 0000 000d  eNc.............
+00001d70: 0000 0005 0000 004b 0000 0073 9e00 0000  .......K...s....
+00001d80: 7400 7c02 7c03 8302 7d07 7c07 a001 7c05  t.|.|...}.|...|.
+00001d90: a101 7d08 7c08 6400 7500 7215 6401 a002  ..}.|.d.u.r.d...
+00001da0: 7c07 7c05 a102 7d09 6e34 7c07 6a03 7c01  |.|...}.n4|.j.|.
+00001db0: 7404 6a05 6a06 6a07 6a08 6402 8d02 7d0a  t.j.j.j.j.d...}.
+00001dc0: 7c04 6403 6b02 7227 6400 7d0b 6e0a 7c0a  |.d.k.r'd.}.n.|.
+00001dd0: a009 7c04 a101 0100 7c0a 6a0a 6404 1900  ..|.....|.j.d...
+00001de0: 7d0b 740b 7c07 7c08 7c05 8303 7d0c 7c0c  }.t.|.|.|...}.|.
+00001df0: 6400 7500 7243 6405 a002 7c07 7c08 7c05  d.u.rCd...|.|.|.
+00001e00: a103 7d09 6e06 7c0c a00c 7c0b 7c0a a102  ..}.n.|...|.|...
+00001e10: 7d09 740d 6406 7c09 6901 8301 5300 2907  }.t.d.|.i...S.).
+00001e20: 4e7a 197b 7d20 6861 7320 6e6f 2064 6174  Nz.{} has no dat
+00001e30: 6120 656c 656d 656e 7420 7b7d a902 7245  a element {}..rE
+00001e40: 0000 0072 3a00 0000 723b 0000 0072 0100  ...r:...r;...r..
+00001e50: 0000 7a2c 4f6f 7073 2c20 6765 745f 6174  ..z,Oops, get_at
+00001e60: 6f6d 697a 6572 287b 7d2c 207b 7d2c 207b  omizer({}, {}, {
+00001e70: 7d29 2072 6574 7572 6e65 6420 4e6f 6e65  }) returned None
+00001e80: 7249 0000 0029 0e72 1f00 0000 72bd 0000  rI...).r....r...
+00001e90: 0072 7a00 0000 7245 0000 0072 0b00 0000  .rz...rE...r....
+00001ea0: 723d 0000 0072 3e00 0000 723f 0000 0072  r=...r>...r?...r
+00001eb0: 3a00 0000 7242 0000 0072 4100 0000 7227  :...rB...rA...r'
+00001ec0: 0000 00da 1666 756c 6c5f 7661 6c75 655f  .....full_value_
+00001ed0: 6672 6f6d 5f6f 626a 6563 7472 2100 0000  from_objectr!...
+00001ee0: 290d 7244 0000 0072 4500 0000 7246 0000  ).rD...rE...rF..
+00001ef0: 0072 4700 0000 7248 0000 0072 ba00 0000  .rG...rH...r....
+00001f00: 72a2 0000 0072 bf00 0000 da02 6465 da01  r....r......de..
+00001f10: 7672 4a00 0000 7269 0000 00da 0273 6672  vrJ...ri.....sfr
+00001f20: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
+00001f30: 0000 001a 0100 0073 1c00 0000 0a01 0a07  .......s........
+00001f40: 0801 0e01 1602 0801 0601 0a02 0a01 0c02  ................
+00001f50: 0801 1001 0c02 0c03 7a10 4465 6c61 7965  ........z.Delaye
+00001f60: 6456 616c 7565 2e67 6574 a904 4e4e 4e4e  dValue.get..NNNN
+00001f70: 72c2 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
+00001f80: 3600 0000 7237 0000 0072 c400 0000 1901  6...r7...r......
+00001f90: 0000 72c3 0000 0072 c400 0000 6300 0000  ..r....r....c...
+00001fa0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00001fb0: 0040 0000 0072 b300 0000 2905 da12 4163  .@...r....)...Ac
+00001fc0: 7469 6f6e 5061 7261 6d43 686f 6963 6573  tionParamChoices
+00001fd0: 4e63 0600 0000 0000 0000 0000 0000 0b00  Nc..............
+00001fe0: 0000 0800 0000 4b00 0000 7376 0000 0074  ......K...sv...t
+00001ff0: 007c 027c 0383 027d 037c 03a0 017c 04a1  .|.|...}.|...|..
+00002000: 017d 077c 0764 0075 0072 1674 0264 017c  .}.|.d.u.r.t.d.|
+00002010: 047c 0366 0216 0083 0182 017c 076a 03a0  .|.f.......|.j..
+00002020: 047c 05a1 017d 0574 057c 076a 067c 0164  .|...}.t.|.j.|.d
+00002030: 028d 017c 076a 037c 0583 035c 027d 087d  ...|.j.|...\.}.}
+00002040: 097c 056a 0772 2f64 037d 0a6e 0264 007d  .|.j.r/d.}.n.d.}
+00002050: 0a74 087c 037c 017c 087c 097c 0a7c 0564  .t.|.|.|.|.|.|.d
+00002060: 048d 0653 0029 054e 7a18 556e 6b6e 6f77  ...S.).Nz.Unknow
+00002070: 6e20 6163 7469 6f6e 2025 7220 666f 7220  n action %r for 
+00002080: 2573 72b5 0000 007a 053c 6272 2f3e 72b9  %sr....z.<br/>r.
+00002090: 0000 0029 0972 1f00 0000 da0e 6765 745f  ...).r......get_
+000020a0: 7572 6c5f 6163 7469 6f6e da09 4578 6365  url_action..Exce
+000020b0: 7074 696f 6e72 7f00 0000 72bc 0000 0072  ptionr....r....r
+000020c0: 1800 0000 7245 0000 0072 be00 0000 7223  ....rE...r....r#
+000020d0: 0000 0029 0b72 4400 0000 7245 0000 0072  ...).rD...rE...r
+000020e0: 4600 0000 7247 0000 00da 0261 6e72 ba00  F...rG.....anr..
+000020f0: 0000 72a2 0000 00da 0262 6172 c100 0000  ..r......bar....
+00002100: 7267 0000 0072 c000 0000 7236 0000 0072  rg...r....r6...r
+00002110: 3600 0000 7237 0000 0072 7c00 0000 3a01  6...r7...r|...:.
+00002120: 0000 7314 0000 000a 010a 0108 0110 010c  ..s.............
+00002130: 011a 0106 0106 0104 0214 017a 1641 6374  ...........z.Act
+00002140: 696f 6e50 6172 616d 4368 6f69 6365 732e  ionParamChoices.
+00002150: 6765 7472 ca00 0000 72c2 0000 0072 3600  getr....r....r6.
+00002160: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00002170: 0072 cb00 0000 3801 0000 7304 0000 0008  .r....8...s.....
+00002180: 000e 0272 cb00 0000 6300 0000 0000 0000  ...r....c.......
+00002190: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000021a0: 0073 2e00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000021b0: 5a03 6409 6403 6404 8401 5a04 6409 6405  Z.d.d.d...Z.d.d.
+000021c0: 6406 8401 5a05 6409 6407 6408 8401 5a06  d...Z.d.d.d...Z.
+000021d0: 6402 5300 290a da07 5265 7374 6675 6c7a  d.S.)...Restfulz
+000021e0: 3c0a 2020 2020 5573 6564 2074 6f20 636f  <.    Used to co
+000021f0: 6c6c 6162 6f72 6174 6520 7769 7468 2061  llaborate with a
+00002200: 2072 6573 7466 756c 2045 7874 2e64 6174   restful Ext.dat
+00002210: 612e 5374 6f72 652e 0a20 2020 204e 6305  a.Store..    Nc.
+00002220: 0000 0000 0000 0000 0000 0009 0000 0006  ................
+00002230: 0000 0043 0000 0073 8800 0000 7400 7c02  ...C...s....t.|.
+00002240: 7c03 8302 7d05 7c05 6a01 7c01 6401 8d01  |...}.|.j.|.d...
+00002250: 7d06 7c06 a002 a100 7d07 7c06 6a03 6a04  }.|.....}.|.j.j.
+00002260: 6400 7501 721c 7c06 6a03 a004 7c07 7c01  d.u.r.|.j...|.|.
+00002270: a102 0100 7c01 6a05 a006 6402 a101 7d08  ....|.j...d...}.
+00002280: 7407 a008 7c08 a101 7d08 7c06 a009 7c08  t...|...}.|...|.
+00002290: 7c07 6403 a103 0100 7c06 6a0a 7c06 6a0b  |.d.....|.j.|.j.
+000022a0: 6a0c a00d 7c06 7c07 7c06 6a0b 6a0c 6a0e  j...|.|.|.j.j.j.
+000022b0: a103 6701 6404 8d01 0100 740f 7c06 6a10  ..g.d.....t.|.j.
+000022c0: 8301 5300 2905 4e72 b500 0000 7272 0000  ..S.).Nr....rr..
+000022d0: 0054 a901 7272 0000 0029 1172 1f00 0000  .T..rr...).r....
+000022e0: 7245 0000 0072 4000 0000 7247 0000 00da  rE...r@...rG....
+000022f0: 1568 616e 646c 655f 7570 6c6f 6164 6564  .handle_uploaded
+00002300: 5f66 696c 6573 723c 0000 0072 7c00 0000  _filesr<...r|...
+00002310: da04 6a73 6f6e da05 6c6f 6164 73da 1166  ..json..loads..f
+00002320: 6f72 6d32 6f62 6a5f 616e 645f 7361 7665  orm2obj_and_save
+00002330: da0c 7365 745f 7265 7370 6f6e 7365 727b  ..set_responser{
+00002340: 0000 0072 6000 0000 7267 0000 00da 0b6c  ...r`...rg.....l
+00002350: 6973 745f 6669 656c 6473 7221 0000 00da  ist_fieldsr!....
+00002360: 0872 6573 706f 6e73 6529 0972 4400 0000  .response).rD...
+00002370: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
+00002380: 4800 0000 72bf 0000 0072 4a00 0000 da08  H...r....rJ.....
+00002390: 696e 7374 616e 6365 7249 0000 0072 3600  instancerI...r6.
+000023a0: 0000 7236 0000 0072 3700 0000 724c 0000  ..r6...r7...rL..
+000023b0: 004d 0100 0073 1c00 0000 0a01 0c01 0802  .M...s..........
+000023c0: 0c03 0e01 0c02 0a01 0e01 0403 0801 0c01  ................
+000023d0: 04ff 06ff 0a03 7a0c 5265 7374 6675 6c2e  ......z.Restful.
+000023e0: 706f 7374 6305 0000 0000 0000 0000 0000  postc...........
+000023f0: 000f 0000 0005 0000 0003 0000 0073 6201  .............sb.
+00002400: 0000 7400 7c02 7c03 8302 7d05 7c01 6a01  ..t.|.|...}.|.j.
+00002410: a002 7403 6a04 6401 a102 7d06 7c01 6a01  ..t.j.d...}.|.j.
+00002420: a002 7403 6a05 7403 6a06 a102 7d07 7c01  ..t.j.t.j...}.|.
+00002430: 6a01 a007 7403 6a08 a101 7d08 7c08 7322  j...t.j...}.|.s"
+00002440: 7c04 6701 7d08 7c05 6a09 7c01 7c08 6402  |.g.}.|.j.|.|.d.
+00002450: 8d02 8900 7c04 6401 7500 7251 8800 6a0a  ....|.d.u.rQ..j.
+00002460: 8901 8700 8701 6602 6403 6404 8408 8800  ......f.d.d.....
+00002470: 6a0b 4400 8301 7d09 740c 8800 a00d a100  j.D...}.t.......
+00002480: 7c09 6405 8d02 7d0a 7c0a 6a0e 740f 8800  |.d...}.|.j.t...
+00002490: a010 a100 8301 6406 8d01 0100 7411 7c0a  ......d.....t.|.
+000024a0: 8301 5300 7c06 7259 7c05 a012 7c06 a101  ..S.|.rY|...|...
+000024b0: 7d0b 6e03 7c05 6a13 7d0b 8800 6a0a 7d0c  }.n.|.j.}...j.}.
+000024c0: 7c0b 6a09 7c01 7c08 6402 8d02 8900 8800  |.j.|.|.d.......
+000024d0: 6a14 6407 1900 7d0d 7c07 7403 6a06 6b02  j.d...}.|.t.j.k.
+000024e0: 72af 7c04 6408 6b02 7282 8800 a015 a100  r.|.d.k.r.......
+000024f0: 7d0d 8800 a016 7c0c 7c0d a102 7d0e 7411  }.....|.|...}.t.
+00002500: 7c0e 8301 5300 7c04 6409 6b02 7294 8800  |...S.|.d.k.r...
+00002510: a015 a100 7d0d 7417 8800 7c0c 7c0d 8303  ....}.t...|.|...
+00002520: 7d0e 7411 7c0e 8301 5300 7c0d 6401 7500  }.t.|...S.|.d.u.
+00002530: 72a6 740c 640a 7418 7c05 7c04 6602 1600  r.t.d.t.|.|.f...
+00002540: 640b 8d02 7d0e 7411 7c0e 8301 5300 8800  d...}.t.|...S...
+00002550: a019 7c0d a101 7d0e 7411 7c0e 8301 5300  ..|...}.t.|...S.
+00002560: 6401 5300 290c 7a3b 0a20 2020 2020 2020  d.S.).z;.       
+00002570: 2057 6f72 6b73 2c20 6275 7420 6973 2075   Works, but is u
+00002580: 676c 7920 746f 2067 6574 206c 6973 7420  gly to get list 
+00002590: 616e 6420 6465 7461 696c 0a20 2020 2020  and detail.     
+000025a0: 2020 204e 2902 7245 0000 00da 0c73 656c     N).rE.....sel
+000025b0: 6563 7465 645f 706b 7363 0100 0000 0000  ected_pksc......
+000025c0: 0000 0000 0000 0200 0000 0700 0000 1300  ................
+000025d0: 0000 7320 0000 0067 007c 005d 0c7d 0188  ..s ...g.|.].}..
+000025e0: 016a 00a0 0188 007c 0188 016a 006a 02a1  .j.....|...j.j..
+000025f0: 0391 0271 0253 0072 3600 0000 2903 7260  ...q.S.r6...).r`
+00002600: 0000 0072 6700 0000 da0a 616c 6c5f 6669  ...rg.....all_fi
+00002610: 656c 6473 726d 0000 00a9 0272 4a00 0000  eldsrm.....rJ...
+00002620: 726b 0000 0072 3600 0000 7237 0000 0072  rk...r6...r7...r
+00002630: 6f00 0000 7601 0000 7308 0000 0006 0002  o...v...s.......
+00002640: 0212 ff06 ff7a 1f52 6573 7466 756c 2e67  .....z.Restful.g
+00002650: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  et.<locals>.<lis
+00002660: 7463 6f6d 703e 2902 7271 0000 0072 7200  tcomp>).rq...rr.
+00002670: 0000 2901 7276 0000 0072 0100 0000 7a06  ..).rv...r....z.
+00002680: 2d39 3939 3939 723b 0000 0046 2902 7274  -99999r;...F).rt
+00002690: 0000 00da 076d 6573 7361 6765 291a 721f  .....message).r.
+000026a0: 0000 0072 7800 0000 727c 0000 0072 1b00  ...rx...r|...r..
+000026b0: 0000 7281 0000 0072 7d00 0000 7282 0000  ..r....r}...r...
+000026c0: 00da 0767 6574 6c69 7374 da12 5552 4c5f  ...getlist..URL_
+000026d0: 5041 5241 4d5f 5345 4c45 4354 4544 7245  PARAM_SELECTEDrE
+000026e0: 0000 0072 7b00 0000 7286 0000 0072 9000  ...r{...r....r..
+000026f0: 0000 728c 0000 0072 9500 0000 72aa 0000  ..r....r....r...
+00002700: 0072 9100 0000 7221 0000 0072 cc00 0000  .r....r!...r....
+00002710: da0d 6465 7461 696c 5f61 6374 696f 6e72  ..detail_actionr
+00002720: 4100 0000 7240 0000 00da 0f65 6c65 6d32  A...r@.....elem2
+00002730: 7265 635f 696e 7365 7274 722d 0000 00da  rec_insertr-....
+00002740: 094e 4f54 5f46 4f55 4e44 da11 656c 656d  .NOT_FOUND..elem
+00002750: 3272 6563 5f64 6574 6169 6c65 6429 0f72  2rec_detailed).r
+00002760: 4400 0000 7245 0000 0072 4600 0000 7247  D...rE...rF...rG
+00002770: 0000 0072 4800 0000 72bf 0000 0072 9c00  ...rH...r....r..
+00002780: 0000 729b 0000 00da 0273 7272 7200 0000  ..r......srrr...
+00002790: 72a2 0000 0072 cf00 0000 727b 0000 0072  r....r....r{...r
+000027a0: 4b00 0000 729d 0000 0072 3600 0000 72dc  K...r....r6...r.
+000027b0: 0000 0072 3700 0000 727c 0000 0067 0100  ...r7...r|...g..
+000027c0: 0073 5000 0000 0a04 1002 0601 0801 04ff  .sP.............
+000027d0: 0e02 0401 0601 0e01 0801 0601 0c01 0402  ................
+000027e0: 06fe 1003 1401 0801 0403 0c01 0602 0601  ................
+000027f0: 0e01 0a01 0a01 0801 0801 0c01 0809 08f8  ................
+00002800: 0801 0c01 0806 08fb 0201 0c01 06ff 0804  ................
+00002810: 0aff 0801 04f4 7a0b 5265 7374 6675 6c2e  ......z.Restful.
+00002820: 6765 7463 0500 0000 0000 0000 0000 0000  getc............
+00002830: 0b00 0000 0600 0000 4300 0000 73a8 0000  ........C...s...
+00002840: 0074 007c 027c 0383 027d 057c 056a 017c  .t.|.|...}.|.j.|
+00002850: 0164 018d 017d 067c 06a0 027c 04a1 0101  .d...}.|...|....
+00002860: 007c 066a 0364 0219 007d 077c 066a 047d  .|.j.d...}.|.j.}
+00002870: 0874 05a0 067c 016a 07a1 01a0 0864 03a1  .t...|.j.....d..
+00002880: 017d 0974 09a0 0a7c 09a1 017d 097c 05a0  .}.t...|...}.|..
+00002890: 0b7c 056a 0ca1 017d 0a7c 056a 017c 017c  .|.j...}.|.j.|.|
+000028a0: 0a64 048d 027d 0674 0d6a 0e6a 0f6a 107c  .d...}.t.j.j.j.|
+000028b0: 065f 117c 06a0 127c 097c 0764 05a1 0301  ._.|...|.|.d....
+000028c0: 007c 066a 137c 086a 14a0 157c 067c 077c  .|.j.|.j...|.|.|
+000028d0: 086a 146a 16a1 0367 0164 068d 0101 0074  .j.j...g.d.....t
+000028e0: 177c 066a 1883 0153 0029 074e 72b5 0000  .|.j...S.).Nr...
+000028f0: 0072 0100 0000 7272 0000 0029 0272 4500  .r....rr...).rE.
+00002900: 0000 727f 0000 0046 72d1 0000 0029 1972  ..r....Fr....).r
+00002910: 1f00 0000 7245 0000 0072 4200 0000 7241  ....rE...rB...rA
+00002920: 0000 0072 7b00 0000 7209 0000 0072 5000  ...r{...r....rP.
+00002930: 0000 7251 0000 0072 7c00 0000 72d3 0000  ..rQ...r|...r...
+00002940: 0072 d400 0000 72cc 0000 00da 1864 6566  .r....r......def
+00002950: 6175 6c74 5f6c 6973 745f 6163 7469 6f6e  ault_list_action
+00002960: 5f6e 616d 6572 0b00 0000 723d 0000 0072  _namer....r=...r
+00002970: 2600 0000 da0e 6578 746a 735f 7265 6e64  &.....extjs_rend
+00002980: 6572 6572 723a 0000 0072 d500 0000 72d6  ererr:...r....r.
+00002990: 0000 0072 6000 0000 7267 0000 0072 d700  ...r`...rg...r..
+000029a0: 0000 7221 0000 0072 d800 0000 290b 7244  ..r!...r....).rD
+000029b0: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
+000029c0: 0000 7248 0000 0072 bf00 0000 724a 0000  ..rH...r....rJ..
+000029d0: 0072 4b00 0000 726b 0000 0072 4900 0000  .rK...rk...rI...
+000029e0: da01 6172 3600 0000 7236 0000 0072 3700  ..ar6...r6...r7.
+000029f0: 0000 7253 0000 0093 0100 0073 1e00 0000  ..rS.......s....
+00002a00: 0a01 0c01 0a01 0a01 0601 1202 0a01 0c01  ................
+00002a10: 0e01 0c01 0e01 0402 1401 06ff 0a02 7a0b  ..............z.
+00002a20: 5265 7374 6675 6c2e 7075 7472 5500 0000  Restful.putrU...
+00002a30: 2907 7256 0000 0072 5700 0000 7258 0000  ).rV...rW...rX..
+00002a40: 0072 b100 0000 724c 0000 0072 7c00 0000  .r....rL...r|...
+00002a50: 7253 0000 0072 3600 0000 7236 0000 0072  rS...r6...r6...r
+00002a60: 3600 0000 7237 0000 0072 d000 0000 4801  6...r7...r....H.
+00002a70: 0000 730a 0000 0008 0004 010a 040a 1a0e  ..s.............
+00002a80: 2c72 d000 0000 6303 0000 0000 0000 0000  ,r....c.........
+00002a90: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
+00002aa0: 7000 0000 7c00 a000 a100 7d03 7401 8300  p...|.....}.t...
+00002ab0: 7d04 7c03 6a02 7c04 6602 7d05 7c00 6a03  }.|.j.|.f.}.|.j.
+00002ac0: 6406 6900 7c02 a401 8e01 7d02 7c00 7c02  d.i.|.....}.|.|.
+00002ad0: 6401 3c00 7c00 6a04 7c02 6402 3c00 7405  d.<.|.j.|.d.<.t.
+00002ae0: 6a06 6a07 6a08 6a09 6a0a 7d06 7c06 a00b  j.j.j.j.j.}.|...
+00002af0: 7c01 a101 7d07 740c 6a0d 7c07 6a0e 6406  |...}.t.j.|.j.d.
+00002b00: 6900 7c02 a401 8e01 6403 6404 8d02 7d08  i.|.....d.d...}.
+00002b10: 7c08 5300 2907 7a14 4465 7365 7276 6573  |.S.).z.Deserves
+00002b20: 2061 2064 6f63 7374 7269 6e67 724a 0000   a docstringrJ..
+00002b30: 00da 046d 656d 6ffa 1974 6578 742f 6874  ...memo..text/ht
+00002b40: 6d6c 3b63 6861 7273 6574 3d22 7574 662d  ml;charset="utf-
+00002b50: 3822 a901 da0c 636f 6e74 656e 745f 7479  8"....content_ty
+00002b60: 7065 4e72 3600 0000 290f da08 6765 745f  peNr6...)...get_
+00002b70: 7573 6572 7211 0000 00da 0975 7365 725f  userr......user_
+00002b80: 7479 7065 da15 6765 745f 7072 696e 7461  type..get_printa
+00002b90: 626c 655f 636f 6e74 6578 74da 0a70 6172  ble_context..par
+00002ba0: 7365 5f6d 656d 6f72 0b00 0000 723d 0000  se_memor....r=..
+00002bb0: 0072 3e00 0000 da05 6a69 6e6a 6172 3a00  .r>.....jinjar:.
+00002bc0: 0000 da09 6a69 6e6a 615f 656e 76da 0c67  ....jinja_env..g
+00002bd0: 6574 5f74 656d 706c 6174 6572 0900 0000  et_templater....
+00002be0: da0c 4874 7470 5265 7370 6f6e 7365 da06  ..HttpResponse..
+00002bf0: 7265 6e64 6572 2909 724a 0000 00da 0774  render).rJ.....t
+00002c00: 706c 6e61 6d65 da07 636f 6e74 6578 74da  plname..context.
+00002c10: 0175 da04 6c61 6e67 da01 6bda 0365 6e76  .u..lang..k..env
+00002c20: da08 7465 6d70 6c61 7465 72d8 0000 0072  ..templater....r
+00002c30: 3600 0000 7236 0000 0072 3700 0000 da0d  6...r6...r7.....
+00002c40: 6874 7470 5f72 6573 706f 6e73 65a6 0100  http_response...
+00002c50: 0073 1a00 0000 0802 0601 0a01 1001 0801  .s..............
+00002c60: 0a01 0e01 0a01 0402 0e01 0201 06fe 0404  ................
+00002c70: 72fc 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00002c80: 0000 0c00 0000 0a00 0000 4300 0000 73ea  ..........C...s.
+00002c90: 0000 007c 006a 0064 1469 007c 02a4 018e  ...|.j.d.i.|....
+00002ca0: 017d 027c 026a 0174 0264 018d 0101 0074  .}.|.j.t.d.....t
+00002cb0: 036a 046a 056a 066a 076a 087d 037a 077c  .j.j.j.j.j.}.z.|
+00002cc0: 03a0 097c 01a1 017d 0457 006e 1604 0074  ...|...}.W.n...t
+00002cd0: 0a79 3201 007d 0501 007a 0a74 0ba0 0ca1  .y2..}...z.t....
+00002ce0: 0057 0006 0059 0064 027d 057e 0553 0064  .W...Y.d.}.~.S.d
+00002cf0: 027d 057e 0577 0177 0064 0364 0484 007d  .}.~.w.w.d.d...}
+00002d00: 067c 026a 017c 0664 058d 0101 0064 0664  .|.j.|.d.....d.d
+00002d10: 0784 007d 0764 0864 0984 007d 0864 0a64  ...}.d.d...}.d.d
+00002d20: 0b84 007d 097c 036a 0da0 0174 0e7c 077c  ...}.|.j...t.|.|
+00002d30: 087c 0964 0c8d 03a1 0101 007c 01a0 0f64  .|.d.......|...d
+00002d40: 0da1 0172 5b64 0e6e 087c 01a0 0f64 0fa1  ...r[d.n.|...d..
+00002d50: 0172 6264 106e 0164 117d 0a74 0b6a 107c  .rbd.n.d.}.t.j.|
+00002d60: 046a 1164 1469 007c 02a4 018e 017c 0a64  .j.d.i.|.....|.d
+00002d70: 1217 0064 138d 027d 0b7c 0b53 0029 157a  ...d...}.|.S.).z
+00002d80: 6a0a 2020 2020 5265 7370 6f6e 6520 7573  j.    Respone us
+00002d90: 6564 2066 6f72 2072 656e 6465 7269 6e67  ed for rendering
+00002da0: 2058 4d4c 2076 6965 7773 2069 6e20 7265   XML views in re
+00002db0: 6163 742e 0a20 2020 2049 6e63 6c75 6465  act..    Include
+00002dc0: 7320 736f 6d65 2068 656c 7065 7220 6675  s some helper fu
+00002dd0: 6e63 7469 6f6e 7320 666f 7220 7265 6e64  nctions for rend
+00002de0: 6572 696e 672e 0a20 2020 2072 1a00 0000  ering..    r....
+00002df0: 4e63 0000 0000 0000 0000 0000 0000 0100  Nc..............
+00002e00: 0000 0400 0000 5700 0000 7320 0000 0064  ......W...s ...d
+00002e10: 0164 0284 007c 0044 0083 017d 0064 0364  .d...|.D...}.d.d
+00002e20: 04a0 007c 00a1 0117 0064 0517 0053 0029  ...|.....d...S.)
+00002e30: 067a 2748 656c 7065 7220 6675 6e63 7469  .z'Helper functi
+00002e40: 6f6e 2074 6f20 7772 6170 2061 2073 7472  on to wrap a str
+00002e50: 696e 6720 696e 207b 7d73 6301 0000 0000  ing in {}sc.....
+00002e60: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00002e70: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
+00002e80: 7400 7c01 8301 9102 7102 5300 7236 0000  t.|.....q.S.r6..
+00002e90: 0029 0172 aa00 0000 2902 726e 0000 0072  .).r....).rn...r
+00002ea0: e700 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+00002eb0: 0000 0072 6f00 0000 cd01 0000 7302 0000  ...ro.......s...
+00002ec0: 0014 007a 2e58 4d4c 5f72 6573 706f 6e73  ...z.XML_respons
+00002ed0: 652e 3c6c 6f63 616c 733e 2e62 696e 642e  e.<locals>.bind.
+00002ee0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00002ef0: 6d70 3eda 017b 725c 0000 00da 017d 2901  mp>..{r\.....}).
+00002f00: da04 6a6f 696e a901 da04 6172 6773 7236  ..join....argsr6
+00002f10: 0000 0072 3600 0000 7237 0000 00da 0462  ...r6...r7.....b
+00002f20: 696e 64cb 0100 0073 0400 0000 0e02 1201  ind....s........
+00002f30: 7a1a 584d 4c5f 7265 7370 6f6e 7365 2e3c  z.XML_response.<
+00002f40: 6c6f 6361 6c73 3e2e 6269 6e64 2901 7202  locals>.bind).r.
+00002f50: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002f60: 0100 0000 0200 0000 5700 0000 730c 0000  ........W...s...
+00002f70: 0074 007c 0083 0101 0064 0153 0029 027a  .t.|.....d.S.).z
+00002f80: 8844 6562 7567 6765 7220 6865 6c70 6572  .Debugger helper
+00002f90: 3b20 7072 696e 7473 206f 7574 2061 6c6c  ; prints out all
+00002fa0: 2061 7267 7320 7075 7420 696e 746f 2074   args put into t
+00002fb0: 6865 2066 696c 7465 7220 6275 7420 646f  he filter but do
+00002fc0: 6573 6e27 7420 696e 636c 7564 6520 7468  esn't include th
+00002fd0: 656d 2069 6e20 7468 6520 7465 6d70 6c61  em in the templa
+00002fe0: 7465 2e0a 2020 2020 2020 2020 7573 6167  te..        usag
+00002ff0: 653a 207b 7b64 6562 7567 207c 2070 7d7d  e: {{debug | p}}
+00003000: 0a20 2020 2020 2020 2072 5c00 0000 2901  .        r\...).
+00003010: da05 7072 696e 7472 0001 0000 7236 0000  ..printr....r6..
+00003020: 0072 3600 0000 7237 0000 00da 0170 d201  .r6...r7.....p..
+00003030: 0000 7304 0000 0008 0404 017a 1758 4d4c  ..s........z.XML
+00003040: 5f72 6573 706f 6e73 652e 3c6c 6f63 616c  _response.<local
+00003050: 733e 2e70 6301 0000 0000 0000 0000 0000  s>.pc...........
+00003060: 0003 0000 0004 0000 0053 0000 0073 2000  .........S...s .
+00003070: 0000 6401 6402 6c00 7d01 7c01 a001 7402  ..d.d.l.}.|...t.
+00003080: 7c00 8301 a101 7d02 7c02 a003 6403 a101  |.....}.|...d...
+00003090: 5300 2904 7ab0 0a20 2020 2020 2020 2043  S.).z..        C
+000030a0: 6f6d 7072 6573 7320 6120 636f 6d70 6c65  ompress a comple
+000030b0: 7820 7661 6c75 6520 696e 206f 7264 6572  x value in order
+000030c0: 2074 6f20 6765 7420 6465 636f 6d70 7265   to get decompre
+000030d0: 7373 2062 7920 7468 6520 636f 6e74 726f  ss by the contro
+000030e0: 6c6c 6572 2061 6674 6572 7761 7264 730a  ller afterwards.
+000030f0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+00003100: 3a20 7661 6c75 6520 746f 2067 6574 2063  : value to get c
+00003110: 6f6d 7072 6573 7365 642e 0a20 2020 2020  ompressed..     
+00003120: 2020 203a 7265 7475 726e 3a20 436f 6d70     :return: Comp
+00003130: 7265 7373 6564 2076 616c 7565 2e0a 2020  ressed value..  
+00003140: 2020 2020 2020 7201 0000 004e da06 6261        r....N..ba
+00003150: 7365 3634 2904 da04 7a6c 6962 da08 636f  se64)...zlib..co
+00003160: 6d70 7265 7373 72aa 0000 00da 0665 6e63  mpressr......enc
+00003170: 6f64 6529 03da 0173 7206 0100 00da 0a63  ode)...sr......c
+00003180: 6f6d 7072 6573 7365 6472 3600 0000 7236  ompressedr6...r6
+00003190: 0000 0072 3700 0000 da0d 7a6c 6962 5f63  ...r7.....zlib_c
+000031a0: 6f6d 7072 6573 73d9 0100 0073 0600 0000  ompress....s....
+000031b0: 0806 0e01 0a01 7a23 584d 4c5f 7265 7370  ......z#XML_resp
+000031c0: 6f6e 7365 2e3c 6c6f 6361 6c73 3e2e 7a6c  onse.<locals>.zl
+000031d0: 6962 5f63 6f6d 7072 6573 7363 0200 0000  ib_compressc....
+000031e0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000031f0: 5300 0000 7320 0000 007c 0072 0e7c 0144  S...s ...|.r.|.D
+00003200: 005d 097d 027c 007c 026b 0272 0d01 0064  .].}.|.|.k.r...d
+00003210: 0153 0071 0464 0253 0029 037a f60a 2020  .S.q.d.S.).z..  
+00003220: 2020 2020 2020 6368 6563 6b20 6966 2074        check if t
+00003230: 6865 2066 6965 6c64 7320 6973 2061 7661  he fields is ava
+00003240: 696c 6162 6c65 2069 6e20 7468 6520 7365  ilable in the se
+00003250: 7420 6f66 2063 6f6c 6c65 6374 696f 6e73  t of collections
+00003260: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003270: 7365 6172 6368 6564 5f66 6965 6c64 3a20  searched_field: 
+00003280: 7365 6172 6368 6564 2066 6965 6c64 0a20  searched field. 
+00003290: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+000032a0: 6c6c 6563 7469 6f6e 733a 2073 6574 206f  llections: set o
+000032b0: 6620 6669 656c 6473 0a20 2020 2020 2020  f fields.       
+000032c0: 203a 7265 7475 726e 3a20 5472 7565 2069   :return: True i
+000032d0: 6620 7468 6520 6669 656c 6420 6973 2070  f the field is p
+000032e0: 7265 7365 6e74 2069 6e20 7468 6520 636f  resent in the co
+000032f0: 6c6c 6563 7469 6f6e 732c 4661 6c73 6520  llections,False 
+00003300: 6f74 6865 7277 6973 652e 0a20 2020 2020  otherwise..     
+00003310: 2020 2054 4672 3600 0000 2903 da0e 7365     TFr6...)...se
+00003320: 6172 6368 6564 5f66 6965 6c64 da0b 636f  arched_field..co
+00003330: 6c6c 6563 7469 6f6e 7372 ba00 0000 7236  llectionsr....r6
+00003340: 0000 0072 3600 0000 7237 0000 00da 0d66  ...r6...r7.....f
+00003350: 6965 6c64 735f 7365 6172 6368 e401 0000  ields_search....
+00003360: 730c 0000 0004 0708 0108 0106 0102 ff04  s...............
+00003370: 027a 2358 4d4c 5f72 6573 706f 6e73 652e  .z#XML_response.
+00003380: 3c6c 6f63 616c 733e 2e66 6965 6c64 735f  <locals>.fields_
+00003390: 7365 6172 6368 2903 7204 0100 0072 0b01  search).r....r..
+000033a0: 0000 720e 0100 007a 042e 786d 6c7a 0874  ..r....z..xmlz.t
+000033b0: 6578 742f 786d 6c7a 032e 6a73 fa16 6170  ext/xmlz..js..ap
+000033c0: 706c 6963 6174 696f 6e2f 6a61 7661 7363  plication/javasc
+000033d0: 7269 7074 7a10 6170 706c 6963 6174 696f  riptz.applicatio
+000033e0: 6e2f 6a73 6f6e 7a10 3b63 6861 7273 6574  n/jsonz.;charset
+000033f0: 3d22 7574 662d 3822 72ea 0000 0072 3600  ="utf-8"r....r6.
+00003400: 0000 2912 72ee 0000 0072 9500 0000 721b  ..).r....r....r.
+00003410: 0000 0072 0b00 0000 723d 0000 0072 3e00  ...r....r=...r>.
+00003420: 0000 72f0 0000 0072 3a00 0000 72f1 0000  ..r....r:...r...
+00003430: 0072 f200 0000 7204 0000 0072 0900 0000  .r....r....r....
+00003440: da14 4874 7470 5265 7370 6f6e 7365 4e6f  ..HttpResponseNo
+00003450: 7446 6f75 6e64 da07 6669 6c74 6572 7372  tFound..filtersr
+00003460: 9000 0000 da08 656e 6473 7769 7468 72f3  ......endswithr.
+00003470: 0000 0072 f400 0000 290c 724a 0000 0072  ...r....).rJ...r
+00003480: f500 0000 72f6 0000 0072 fa00 0000 72fb  ....r....r....r.
+00003490: 0000 00da 0165 7202 0100 0072 0401 0000  .....er....r....
+000034a0: 720b 0100 0072 0e01 0000 72eb 0000 0072  r....r....r....r
+000034b0: d800 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+000034c0: 0000 00da 0c58 4d4c 5f72 6573 706f 6e73  .....XML_respons
+000034d0: 65b9 0100 0073 3000 0000 1008 0c01 0e03  e....s0.........
+000034e0: 0201 0e01 0e01 1401 0880 02ff 0803 0c05  ................
+000034f0: 0802 0807 080b 160d 0e01 0e01 0201 02fe  ................
+00003500: 0403 0e01 0601 06fe 0404 7214 0100 0063  ..........r....c
+00003510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003520: 0100 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
+00003530: 0164 005a 0264 015a 0364 025a 0464 0353  .d.Z.d.Z.d.Z.d.S
+00003540: 0029 04da 0653 5756 6965 777a 1772 6561  .)...SWViewz.rea
+00003550: 6374 2f73 6572 7669 6365 2d77 6f72 6b65  ct/service-worke
+00003560: 722e 6a73 720f 0100 004e 2905 7256 0000  r.jsr....N).rV..
+00003570: 0072 5700 0000 7258 0000 00da 0d74 656d  .rW...rX.....tem
+00003580: 706c 6174 655f 6e61 6d65 72eb 0000 0072  plate_namer....r
+00003590: 3600 0000 7236 0000 0072 3600 0000 7237  6...r6...r6...r7
+000035a0: 0000 0072 1501 0000 fc01 0000 7306 0000  ...r........s...
+000035b0: 0008 0004 0108 0172 1501 0000 6300 0000  .......r....c...
+000035c0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+000035d0: 0000 0000 0073 2000 0000 6500 5a01 6400  .....s ...e.Z.d.
+000035e0: 5a02 6401 5a03 8700 6601 6402 6403 8408  Z.d.Z...f.d.d...
+000035f0: 5a04 8700 0400 5a05 5300 2904 da06 5742  Z.....Z.S.)...WB
+00003600: 5669 6577 720f 0100 0063 0200 0000 0000  Viewr....c......
+00003610: 0000 0000 0000 0400 0000 0400 0000 0f00  ................
+00003620: 0000 732c 0000 0074 0083 006a 017c 0167  ..s,...t...j.|.g
+00003630: 017c 02a2 0152 0069 007c 03a4 018e 0101  .|...R.i.|......
+00003640: 0064 017c 0364 0219 0017 007c 005f 0264  .d.|.d.....|._.d
+00003650: 0053 0029 034e 7a06 7265 6163 742f da07  .S.).Nz.react/..
+00003660: 776f 726b 626f 7829 03da 0573 7570 6572  workbox)...super
+00003670: da05 7365 7475 7072 1601 0000 2904 7244  ..setupr....).rD
+00003680: 0000 0072 4500 0000 7201 0100 00da 066b  ...rE...r......k
+00003690: 7761 7267 73a9 01da 095f 5f63 6c61 7373  wargs....__class
+000036a0: 5f5f 7236 0000 0072 3700 0000 721a 0100  __r6...r7...r...
+000036b0: 0003 0200 0073 0400 0000 1a01 1201 7a0c  .....s........z.
+000036c0: 5742 5669 6577 2e73 6574 7570 2906 7256  WBView.setup).rV
+000036d0: 0000 0072 5700 0000 7258 0000 0072 eb00  ...rW...rX...r..
+000036e0: 0000 721a 0100 00da 0d5f 5f63 6c61 7373  ..r......__class
+000036f0: 6365 6c6c 5f5f 7236 0000 0072 3600 0000  cell__r6...r6...
+00003700: 721c 0100 0072 3700 0000 7217 0100 0000  r....r7...r.....
+00003710: 0200 0073 0600 0000 0800 0401 1402 7217  ...s..........r.
+00003720: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00003730: 0000 0000 0200 0000 4000 0000 f314 0000  ........@.......
+00003740: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00003750: 0364 0353 0029 04da 084d 6169 6e48 746d  .d.S.)...MainHtm
+00003760: 6c63 0200 0000 0000 0000 0000 0000 0700  lc..............
+00003770: 0000 0400 0000 4f00 0000 7358 0000 0074  ......O...sX...t
+00003780: 006a 01a0 02a1 0001 0074 006a 016a 036a  .j.......t.j.j.j
+00003790: 046a 057d 0474 067c 017c 0464 018d 027d  .j.}.t.|.|.d...}
+000037a0: 0564 027c 015f 0774 006a 01a0 087c 05a1  .d.|._.t.j...|..
+000037b0: 017d 067c 04a0 097c 06a1 017d 067c 056a  .}.|...|...}.|.j
+000037c0: 0a7c 0664 038d 0101 0074 0b7c 056a 0c7c  .|.d.....t.|.j.|
+000037d0: 056a 0d83 0253 0029 047a 3252 6574 7572  .j...S.).z2Retur
+000037e0: 6e73 2061 206a 736f 6e20 7374 7275 6374  ns a json struct
+000037f0: 2066 6f72 2074 6865 206d 6169 6e20 7573   for the main us
+00003800: 6572 2064 6173 6862 6f61 7264 2e72 3900  er dashboard.r9.
+00003810: 0000 7a0e 6461 7368 626f 6172 642d 6d61  ..z.dashboard-ma
+00003820: 696e 7207 0000 0029 0e72 0b00 0000 723d  inr....).r....r=
+00003830: 0000 00da 0773 7461 7274 7570 723e 0000  .....startupr>..
+00003840: 0072 3f00 0000 723a 0000 0072 1c00 0000  .r?...r:...r....
+00003850: da10 7265 7175 6573 7469 6e67 5f70 616e  ..requesting_pan
+00003860: 656c da0d 6765 745f 6d61 696e 5f68 746d  el..get_main_htm
+00003870: 6c72 7300 0000 7274 0000 0072 2100 0000  lrs...rt...r!...
+00003880: 72d8 0000 0072 eb00 0000 2907 7244 0000  r....r....).rD..
+00003890: 0072 4500 0000 7201 0100 0072 a200 0000  .rE...r....r....
+000038a0: da03 726e 6472 4a00 0000 7208 0000 0072  ..rndrJ...r....r
+000038b0: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
+000038c0: 0000 0009 0200 0073 1000 0000 0a03 0c02  .......s........
+000038d0: 0c01 0602 0c01 0a01 0c01 0e01 7a0c 4d61  ............z.Ma
+000038e0: 696e 4874 6d6c 2e67 6574 4e72 c200 0000  inHtml.getNr....
+000038f0: 7236 0000 0072 3600 0000 7236 0000 0072  r6...r6...r6...r
+00003900: 3700 0000 7220 0100 0008 0200 00f3 0400  7...r ..........
+00003910: 0000 0800 0c01 7220 0100 0063 0000 0000  ......r ...c....
+00003920: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00003930: 4000 0000 721f 0100 0029 04da 0d44 6173  @...r....)...Das
+00003940: 6862 6f61 7264 4974 656d 6303 0000 0000  hboardItemc.....
+00003950: 0000 0000 0000 000a 0000 0005 0000 004f  ...............O
+00003960: 0000 0073 9800 0000 7400 7c01 8301 7d05  ...s....t.|...}.
+00003970: 7401 6a02 6a03 6a04 6a05 7c05 5f05 6401  t.j.j.j.j.|._.d.
+00003980: 7c02 9b00 9d02 7c05 5f06 7c05 a007 a100  |.....|._.|.....
+00003990: a008 a100 6a09 7d06 740a 7c06 8301 7c02  ....j.}.t.|...|.
+000039a0: 6b04 722b 7c06 7c02 1900 7d07 6402 a00b  k.r+|.|...}.d...
+000039b0: 7c07 a00c 7c05 a101 a101 7d08 6e02 6402  |...|.....}.n.d.
+000039c0: 7d08 740d 7c08 6403 8d01 7d04 740e 7c01  }.t.|.d...}.t.|.
+000039d0: 8301 7d09 7c09 723d 7c04 a00f 7c09 a101  ..}.|.r=|...|...
+000039e0: 0100 7c05 6a10 6405 6900 7c04 a401 8e01  ..|.j.d.i.|.....
+000039f0: 0100 7411 7c05 6a12 7c05 6a13 8302 5300  ..t.|.j.|.j...S.
+00003a00: 2906 7a3d 5265 7475 726e 7320 6120 7265  ).z=Returns a re
+00003a10: 6e64 6572 6564 2048 544d 4c20 7665 7273  ndered HTML vers
+00003a20: 696f 6e20 7468 6520 7265 7175 6573 7465  ion the requeste
+00003a30: 6420 7573 6572 2064 6173 6862 6f61 7264  d user dashboard
+00003a40: 2e7a 0a64 6173 6862 6f61 7264 2d72 5c00  .z.dashboard-r\.
+00003a50: 0000 7207 0000 004e 7236 0000 0029 1472  ..r....Nr6...).r
+00003a60: 1c00 0000 720b 0000 0072 3d00 0000 723e  ....r....r=...r>
+00003a70: 0000 0072 3f00 0000 723a 0000 0072 2201  ...r?...r:...r".
+00003a80: 0000 72ec 0000 00da 0f67 6574 5f70 7265  ..r......get_pre
+00003a90: 6665 7265 6e63 6573 da0f 6461 7368 626f  ferences..dashbo
+00003aa0: 6172 645f 6974 656d 7372 8f00 0000 72ff  ard_itemsr....r.
+00003ab0: 0000 0072 f400 0000 7290 0000 0072 2c00  ...r....r....r,.
+00003ac0: 0000 7295 0000 0072 7400 0000 7221 0000  ..r....rt...r!..
+00003ad0: 0072 d800 0000 72eb 0000 0029 0a72 4400  .r....r....).rD.
+00003ae0: 0000 7245 0000 00da 0569 6e64 6578 7201  ..rE.....indexr.
+00003af0: 0100 0072 a200 0000 724a 0000 00da 0464  ...r....rJ.....d
+00003b00: 6173 68da 0469 7465 6d72 0800 0000 7299  ash..itemr....r.
+00003b10: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00003b20: 0000 727c 0000 0019 0200 0073 1c00 0000  ..r|.......s....
+00003b30: 0802 0e01 0c01 0e01 0c01 0801 1203 0402  ................
+00003b40: 0a01 0801 0401 0a01 1001 0e01 7a11 4461  ............z.Da
+00003b50: 7368 626f 6172 6449 7465 6d2e 6765 744e  shboardItem.getN
+00003b60: 72c2 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
+00003b70: 3600 0000 7237 0000 0072 2601 0000 1802  6...r7...r&.....
+00003b80: 0000 7225 0100 0072 2601 0000 6300 0000  ..r%...r&...c...
+00003b90: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00003ba0: 0040 0000 0073 2000 0000 6500 5a01 6400  .@...s ...e.Z.d.
+00003bb0: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
+00003bc0: 6405 8400 5a05 6406 5300 2907 da04 4e75  d...Z.d.S.)...Nu
+00003bd0: 6c6c 7a6c 4a75 7374 2072 6574 7572 6e73  llzlJust returns
+00003be0: 2032 3030 2c20 7573 6564 2069 6e20 616e   200, used in an
+00003bf0: 2069 6672 616d 6520 746f 2063 6175 7365   iframe to cause
+00003c00: 2074 6865 2062 726f 7773 6572 2074 6f20   the browser to 
+00003c10: 7472 6967 6765 7220 2244 6f20 796f 7520  trigger "Do you 
+00003c20: 7761 6e74 2074 6f20 7265 6d65 6d62 6572  want to remember
+00003c30: 2074 6869 7320 7077 2220 6469 616c 6f67   this pw" dialog
+00003c40: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00003c50: 0002 0000 0043 0000 00f3 0800 0000 7400  .....C........t.
+00003c60: a001 a100 5300 72b6 0000 00a9 0272 0900  ....S.r......r..
+00003c70: 0000 72f3 0000 00a9 0272 4400 0000 7245  ..r......rD...rE
+00003c80: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00003c90: 0000 724c 0000 0031 0200 00f3 0200 0000  ..rL...1........
+00003ca0: 0801 7a09 4e75 6c6c 2e70 6f73 7463 0200  ..z.Null.postc..
+00003cb0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00003cc0: 0000 4300 0000 722d 0100 0072 b600 0000  ..C...r-...r....
+00003cd0: 722e 0100 0072 2f01 0000 7236 0000 0072  r....r/...r6...r
+00003ce0: 3600 0000 7237 0000 0072 7c00 0000 3402  6...r7...r|...4.
+00003cf0: 0000 7230 0100 007a 084e 756c 6c2e 6765  ..r0...z.Null.ge
+00003d00: 744e 2906 7256 0000 0072 5700 0000 7258  tN).rV...rW...rX
+00003d10: 0000 0072 b100 0000 724c 0000 0072 7c00  ...r....rL...r|.
+00003d20: 0000 7236 0000 0072 3600 0000 7236 0000  ..r6...r6...r6..
+00003d30: 0072 3700 0000 722c 0100 002e 0200 0073  .r7...r,.......s
+00003d40: 0800 0000 0800 0401 0802 0c03 722c 0100  ............r,..
+00003d50: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003d60: 0000 0200 0000 4000 0000 731c 0000 0065  ......@...s....e
+00003d70: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00003d80: 0364 0484 005a 0464 0553 0029 06da 0c41  .d...Z.d.S.)...A
+00003d90: 7574 6865 6e74 6963 6174 6563 0200 0000  uthenticatec....
+00003da0: 0000 0000 0000 0000 0700 0000 0400 0000  ................
+00003db0: 4f00 0000 7336 0000 007c 016a 00a0 0174  O...s6...|.j...t
+00003dc0: 026a 03a1 017d 0409 007c 016a 04a0 0564  .j...}...|.j...d
+00003dd0: 0364 00a1 027d 0574 06a0 077c 01a1 0101  .d...}.t...|....
+00003de0: 0064 047d 0674 08a0 097c 06a1 0153 0029  .d.}.t...|...S.)
+00003df0: 054e 54da 066c 6f67 6f75 74da 0875 7365  .NT..logout..use
+00003e00: 726e 616d 65fa 012f 290b 7278 0000 0072  rname../).rx...r
+00003e10: 7c00 0000 721b 0000 0072 8100 0000 da07  |...r....r......
+00003e20: 7365 7373 696f 6eda 0370 6f70 7213 0000  session..popr...
+00003e30: 0072 3201 0000 7209 0000 00da 1448 7474  .r2...r......Htt
+00003e40: 7052 6573 706f 6e73 6552 6564 6972 6563  pResponseRedirec
+00003e50: 74da 0748 7474 7034 3034 2907 7244 0000  t..Http404).rD..
+00003e60: 0072 4500 0000 7201 0100 0072 a200 0000  .rE...r....r....
+00003e70: 729c 0000 0072 3301 0000 7232 0000 0072  r....r3...r2...r
+00003e80: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
+00003e90: 0000 0039 0200 0073 0c00 0000 0e01 0201  ...9...s........
+00003ea0: 0e01 0a01 0405 0a01 7a10 4175 7468 656e  ........z.Authen
+00003eb0: 7469 6361 7465 2e67 6574 6302 0000 0000  ticate.getc.....
+00003ec0: 0000 0000 0000 0008 0000 0005 0000 004f  ...............O
+00003ed0: 0000 0073 4c00 0000 7c01 6a00 a001 6401  ...sL...|.j...d.
+00003ee0: a101 7d04 7c01 6a00 a001 6402 a101 7d05  ..}.|.j...d...}.
+00003ef0: 7402 6a03 7c01 7c04 7c05 6403 8d03 7d06  t.j.|.|.|.d...}.
+00003f00: 7402 6a04 7c01 7c06 6404 6405 8d03 0100  t.j.|.|.d.d.....
+00003f10: 6406 6407 8400 7d07 7405 7c06 6a06 7c07  d.d...}.t.|.j.|.
+00003f20: 8302 5300 2908 7a46 6c6f 6773 2074 6865  ..S.).zFlogs the
+00003f30: 2075 7365 7220 696e 2061 6e64 2062 7569   user in and bui
+00003f40: 6c64 7320 7468 6520 6c69 6e6f 7765 622e  lds the linoweb.
+00003f50: 6a73 2066 696c 6520 666f 7220 7468 6520  js file for the 
+00003f60: 6c6f 6767 6564 2069 6e20 7573 6572 7233  logged in userr3
+00003f70: 0100 00da 0870 6173 7377 6f72 6429 0272  .....password).r
+00003f80: 3301 0000 7239 0100 007a 246c 696e 6f2e  3...r9...z$lino.
+00003f90: 636f 7265 2e61 7574 682e 6261 636b 656e  core.auth.backen
+00003fa0: 6473 2e4d 6f64 656c 4261 636b 656e 6429  ds.ModelBackend)
+00003fb0: 01da 0762 6163 6b65 6e64 6300 0000 0000  ...backendc.....
+00003fc0: 0000 0000 0000 0000 0000 0003 0000 0053  ...............S
+00003fd0: 0000 0073 2600 0000 7400 6a01 6a02 720d  ...s&...t.j.j.r.
+00003fe0: 7400 6a01 6a03 6a04 6a05 a006 6401 a101  t.j.j.j.j...d...
+00003ff0: 0100 7407 6402 6403 6901 8301 5300 2904  ..t.d.d.i...S.).
+00004000: 4e46 7274 0000 0054 2908 720b 0000 0072  NFrt...T).r....r
+00004010: 3d00 0000 da14 6465 7665 6c6f 7065 725f  =.....developer_
+00004020: 7369 7465 5f63 6163 6865 723e 0000 0072  site_cacher>...r
+00004030: 3f00 0000 723a 0000 00da 0e62 7569 6c64  ?...r:.....build
+00004040: 5f6a 735f 6361 6368 6572 2100 0000 7236  _js_cacher!...r6
+00004050: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00004060: 0000 da06 7265 7375 6c74 5402 0000 7306  ....resultT...s.
+00004070: 0000 0008 0112 010c 027a 2141 7574 6865  .........z!Authe
+00004080: 6e74 6963 6174 652e 706f 7374 2e3c 6c6f  nticate.post.<lo
+00004090: 6361 6c73 3e2e 7265 7375 6c74 2907 723c  cals>.result).r<
+000040a0: 0000 0072 7c00 0000 7213 0000 00da 0c61  ...r|...r......a
+000040b0: 7574 6865 6e74 6963 6174 65da 056c 6f67  uthenticate..log
+000040c0: 696e 7229 0000 0072 ed00 0000 2908 7244  inr)...r....).rD
+000040d0: 0000 0072 4500 0000 7201 0100 0072 a200  ...rE...r....r..
+000040e0: 0000 7233 0100 0072 3901 0000 da04 7573  ..r3...r9.....us
+000040f0: 6572 723d 0100 0072 3600 0000 7236 0000  err=...r6...r6..
+00004100: 0072 3700 0000 724c 0000 004a 0200 0073  .r7...rL...J...s
+00004110: 1000 0000 0c02 0c01 0402 0601 06ff 1002  ................
+00004120: 0803 0c06 7a11 4175 7468 656e 7469 6361  ....z.Authentica
+00004130: 7465 2e70 6f73 744e 2905 7256 0000 0072  te.postN).rV...r
+00004140: 5700 0000 7258 0000 0072 7c00 0000 724c  W...rX...r|...rL
+00004150: 0000 0072 3600 0000 7236 0000 0072 3600  ...r6...r6...r6.
+00004160: 0000 7237 0000 0072 3101 0000 3802 0000  ..r7...r1...8...
+00004170: 7306 0000 0008 0008 010c 1172 3101 0000  s..........r1...
+00004180: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004190: 0002 0000 0040 0000 0072 a400 0000 2905  .....@...r....).
+000041a0: da05 496e 6465 787a 930a 2020 2020 4d61  ..Indexz..    Ma
+000041b0: 696e 2061 7070 2065 6e74 7279 2070 6f69  in app entry poi
+000041c0: 6e74 2c0a 2020 2020 416c 736f 2062 7569  nt,.    Also bui
+000041d0: 6c64 7320 6c69 6e6f 7765 6220 6669 6c65  lds linoweb file
+000041e0: 2066 6f72 2063 7572 7265 6e74 2075 7365   for current use
+000041f0: 7220 7479 7065 2e0a 2020 2020 436f 6e74  r type..    Cont
+00004200: 656e 7420 6973 206d 6f73 746c 7920 696e  ent is mostly in
+00004210: 2074 6865 203a 7866 696c 653a 6072 6561   the :xfile:`rea
+00004220: 6374 2f6d 6169 6e2e 6874 6d6c 6020 7465  ct/main.html` te
+00004230: 6d70 6c61 7465 2e0a 2020 2020 6302 0000  mplate..    c...
+00004240: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00004250: 0003 0000 0073 2e00 0000 8800 6a00 8901  .....s......j...
+00004260: 0900 8800 6a01 720a 8800 6a01 8901 8700  ....j.r...j.....
+00004270: 8701 6602 6402 6403 8408 7d02 7402 8801  ..f.d.d...}.t...
+00004280: 6a03 7c02 8302 5300 2904 4e54 6300 0000  j.|...S.).NTc...
+00004290: 0000 0000 0000 0000 0007 0000 0006 0000  ................
+000042a0: 0013 0000 0073 b600 0000 7400 6a01 6a02  .....s....t.j.j.
+000042b0: 6a03 7d00 7404 8800 7c00 6a05 6401 8d02  j.}.t...|.j.d...
+000042c0: 7d01 7406 7c00 8800 8801 6402 8d03 7d02  }.t.|.....d...}.
+000042d0: 7c02 6a07 7c01 6403 8d01 0100 6404 7d03  |.j.|.d.....d.}.
+000042e0: 6405 8800 6a08 7600 7229 6406 a009 740a  d...j.v.r)d...t.
+000042f0: a00b 6407 6408 a102 a101 7d03 7c02 6a07  ..d.d.....}.|.j.
+00004300: 7c03 6409 8d01 0100 7c01 6a0c 640f 6900  |.d.....|.j.d.i.
+00004310: 7c02 a401 8e01 7d02 7400 6a01 6a02 6a0d  |.....}.t.j.j.j.
+00004320: 6a05 6a0e 7d04 7c04 a00f 640a a101 7d05  j.j.}.|...d...}.
+00004330: 7410 6a11 7c05 6a12 640f 6900 7c02 a401  t.j.|.j.d.i.|...
+00004340: 8e01 640b 640c 8d02 7d06 6405 8800 6a08  ..d.d...}.d...j.
+00004350: 7600 7259 640d 7c06 640e 3c00 7c06 5300  v.rYd.|.d.<.|.S.
+00004360: 2910 4e72 c500 0000 2903 da09 6672 6f6e  ).Nr....)...fron
+00004370: 745f 656e 6472 4500 0000 7240 0100 0029  t_endrE...r@...)
+00004380: 0172 4a00 0000 725c 0000 00da 0c75 7064  .rJ...r\.....upd
+00004390: 6174 655f 666f 756e 647a 093f 6d74 696d  ate_foundz.?mtim
+000043a0: 653d 7b7d 6907 b201 0069 3f42 0f00 2901  e={}i....i?B..).
+000043b0: da08 6e6f 5f63 6163 6865 7a0f 7265 6163  ..no_cachez.reac
+000043c0: 742f 6d61 696e 2e68 746d 6c72 e900 0000  t/main.htmlr....
+000043d0: 72ea 0000 007a 1222 6361 6368 6522 2c20  r....z."cache", 
+000043e0: 2273 746f 7261 6765 227a 0f43 6c65 6172  "storage"z.Clear
+000043f0: 2d53 6974 652d 4461 7461 7236 0000 0029  -Site-Datar6...)
+00004400: 1372 0b00 0000 723d 0000 0072 3e00 0000  .r....r=...r>...
+00004410: 723f 0000 0072 1c00 0000 723a 0000 0072  r?...r....r:...r
+00004420: 9000 0000 7295 0000 0072 7800 0000 727a  ....r....rx...rz
+00004430: 0000 00da 0672 616e 646f 6dda 0772 616e  .....random..ran
+00004440: 6469 6e74 72ee 0000 0072 f000 0000 72f1  dintr....r....r.
+00004450: 0000 0072 f200 0000 7209 0000 0072 f300  ...r....r....r..
+00004460: 0000 72f4 0000 0029 07da 0275 6972 4a00  ..r....)...uirJ.
+00004470: 0000 72f6 0000 0072 4401 0000 72fa 0000  ..r....rD...r...
+00004480: 0072 fb00 0000 da04 7265 7370 a902 7245  .r......resp..rE
+00004490: 0000 0072 4001 0000 7236 0000 0072 3700  ...r@...r6...r7.
+000044a0: 0000 da05 6765 7469 7478 0200 0073 3200  ....getitx...s2.
+000044b0: 0000 0a01 0203 0202 0401 06fd 0204 0204  ................
+000044c0: 0201 0201 06fa 0c08 0402 0a01 1201 0c01  ................
+000044d0: 1001 0e01 0a01 0401 0e01 0201 06fe 0a04  ................
+000044e0: 0801 0402 7a18 496e 6465 782e 6765 742e  ....z.Index.get.
+000044f0: 3c6c 6f63 616c 733e 2e67 6574 6974 2904  <locals>.getit).
+00004500: 7240 0100 00da 0a73 7562 7374 5f75 7365  r@.....subst_use
+00004510: 7272 2900 0000 72ed 0000 00a9 0372 4400  rr)...r......rD.
+00004520: 0000 7245 0000 0072 4a01 0000 7236 0000  ..rE...rJ...r6..
+00004530: 0072 4901 0000 7237 0000 0072 7c00 0000  .rI...r7...r|...
+00004540: 7102 0000 730c 0000 0006 0202 0106 0106  q...s...........
+00004550: 010e 020c 227a 0949 6e64 6578 2e67 6574  ...."z.Index.get
+00004560: 4e72 b000 0000 7236 0000 0072 3600 0000  Nr....r6...r6...
+00004570: 7236 0000 0072 3700 0000 7241 0100 006a  r6...r7...rA...j
+00004580: 0200 0072 b200 0000 7241 0100 0063 0000  ...r....rA...c..
+00004590: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+000045a0: 0000 4000 0000 72a4 0000 0029 05da 0c55  ..@...r....)...U
+000045b0: 7365 7253 6574 7469 6e67 737a 420a 2020  serSettingszB.  
+000045c0: 2020 416a 6178 2069 6e74 6572 6661 6365    Ajax interface
+000045d0: 2066 6f72 2067 6574 7469 6e67 2074 6865   for getting the
+000045e0: 2063 7572 7265 6e74 2073 6573 7369 6f6e   current session
+000045f0: 2f75 7365 7220 7365 7474 696e 6773 2e63  /user settings.c
+00004600: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00004610: 0400 0000 0300 0000 734e 0000 0074 007c  ........sN...t.|
+00004620: 0183 017d 017c 016a 0189 037c 016a 0289  ...}.|.j...|.j..
+00004630: 0188 0172 117c 016a 02a0 03a1 006e 0164  ...r.|.j.....n.d
+00004640: 0189 0288 036a 0489 0087 0087 0187 0287  .....j..........
+00004650: 0366 0464 0264 0384 087d 0274 0588 0170  .f.d.d...}.t...p
+00004660: 2388 036a 067c 0283 0253 0029 044e 725c  #..j.|...S.).Nr\
+00004670: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00004680: 0400 0000 1100 0000 1300 0000 737c 0100  ............s|..
+00004690: 0074 006a 016a 0272 1174 006a 016a 0373  .t.j.j.r.t.j.j.s
+000046a0: 1174 006a 016a 046a 056a 06a0 0764 01a1  .t.j.j.j.j...d..
+000046b0: 0101 0074 0888 036a 0974 0a88 03a0 0ba1  ...t...j.t......
+000046c0: 006a 0c83 0188 036a 0d74 0e83 0074 006a  .j.....j.t...t.j
+000046d0: 016a 0f74 006a 016a 046a 056a 06a0 10a1  .j.t.j.j.j.j....
+000046e0: 008e 0074 006a 016a 116a 1288 0088 0072  ...t.j.j.j.....r
+000046f0: 3488 03a0 13a1 006e 0374 1464 0283 0188  4......n.t.d....
+00004700: 0274 1464 0383 0174 1464 0483 0174 1464  .t.d...t.d...t.d
+00004710: 0483 0174 1464 0583 0174 006a 01a0 1564  ...t.d...t.j...d
+00004720: 06a1 0172 5074 006a 016a 046a 166a 1770  ...rPt.j.j.j.j.p
+00004730: 5374 1464 0783 0188 036a 1864 088d 0f7d  St.d.....j.d...}
+00004740: 0088 0272 6888 016a 1904 007c 0064 093c  ...rh..j...|.d.<
+00004750: 007c 0064 0a3c 0088 016a 097c 0064 0b3c  .|.d.<...j.|.d.<
+00004760: 0088 0072 ba88 03a0 1aa1 007c 0064 0c3c  ...r.......|.d.<
+00004770: 0088 036a 1b7c 0064 0d3c 0074 006a 016a  ...j.|.d.<.t.j.j
+00004780: 046a 166a 1c72 ba88 03a0 1da1 000c 007d  .j.j.r.........}
+00004790: 017c 0172 ba88 036a 1e64 0075 0172 ba64  .|.r...j.d.u.r.d
+000047a0: 0e7c 0064 0f3c 0088 036a 1e74 1f6a 2074  .|.d.<...j.t.j t
+000047b0: 006a 016a 046a 166a 2164 108d 0117 007d  .j.j.j.j!d.....}
+000047c0: 0274 22a0 2364 11a1 018f 1101 0074 1f6a  .t".#d.......t.j
+000047d0: 1fa0 2474 22a0 257c 02a1 01a1 017d 0357  ..$t".%|.....}.W
+000047e0: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+000047f0: b177 0101 0001 0001 0059 0001 007c 037c  .w.......Y...|.|
+00004800: 0064 123c 0074 267c 0083 0153 0029 134e  .d.<.t&|...S.).N
+00004810: 46da 0941 6e6f 6e79 6d6f 7573 7a31 596f  F..Anonymousz1Yo
+00004820: 7520 6172 6520 6175 7468 6f72 6973 6564  u are authorised
+00004830: 2074 6f20 6163 7420 6173 2074 6865 2066   to act as the f
+00004840: 6f6c 6c6f 7769 6e67 2075 7365 7273 2e7a  ollowing users.z
+00004850: 1341 6374 2061 7320 616e 6f74 6865 7220  .Act as another 
+00004860: 7573 6572 7a1b 5374 6f70 2061 6374 696e  userz.Stop actin
+00004870: 6720 6173 2061 6e6f 7468 6572 2075 7365  g as another use
+00004880: 72da 0575 7365 7273 7a0b 4d79 2073 6574  r..usersz.My set
+00004890: 7469 6e67 7329 0f72 ed00 0000 7228 0100  tings).r....r(..
+000048a0: 00da 0565 6d61 696c 72f8 0000 00da 0973  ...emailr......s
+000048b0: 6974 655f 6461 7461 da09 7369 7465 5f6e  ite_data..site_n
+000048c0: 616d 65da 096c 6f67 6765 645f 696e 7233  ame..logged_inr3
+000048d0: 0100 00da 0773 755f 6e61 6d65 da0e 6163  .....su_name..ac
+000048e0: 745f 6173 5f73 7562 7465 7874 da11 6163  t_as_subtext..ac
+000048f0: 745f 6173 5f74 6974 6c65 5f74 6578 74da  t_as_title_text.
+00004900: 1261 6374 5f61 735f 6275 7474 6f6e 5f74  .act_as_button_t
+00004910: 6578 74da 1061 6374 5f61 735f 7365 6c66  ext..act_as_self
+00004920: 5f74 6578 74da 0f6d 795f 7365 7474 696e  _text..my_settin
+00004930: 675f 7465 7874 da07 7573 6572 5f69 6472  g_text..user_idr
+00004940: 5a01 0000 da05 7375 5f69 64da 0c73 755f  Z.....su_id..su_
+00004950: 7573 6572 5f74 7970 65da 0b61 7574 686f  user_type..autho
+00004960: 7269 7469 6573 da10 6461 7368 626f 6172  rities..dashboar
+00004970: 645f 6c61 796f 7574 54da 1472 6571 7569  d_layoutT..requi
+00004980: 7265 5f76 6572 6966 6963 6174 696f 6e29  re_verification)
+00004990: 01da 076d 696e 7574 6573 da03 5554 43da  ...minutes..UTC.
+000049a0: 0b63 6f64 655f 6578 7069 7279 2927 720b  .code_expiry)'r.
+000049b0: 0000 0072 3d00 0000 723b 0100 00da 166e  ...r=...r;.....n
+000049c0: 6576 6572 5f62 7569 6c64 5f73 6974 655f  ever_build_site_
+000049d0: 6361 6368 6572 3e00 0000 723f 0000 0072  cacher>...r?...r
+000049e0: 3a00 0000 723c 0100 0072 9000 0000 72ed  :...r<...r....r.
+000049f0: 0000 0072 8f00 0000 7227 0100 0072 2801  ...r....r'...r(.
+00004a00: 0000 7250 0100 0072 1100 0000 da14 6275  ..rP...r......bu
+00004a10: 696c 645f 7369 7465 5f63 6163 6865 5f75  ild_site_cache_u
+00004a20: 726c da0d 6c69 6e6f 5f6a 735f 7061 7274  rl..lino_js_part
+00004a30: 73da 0b70 726f 6a65 6374 5f64 6972 da04  s..project_dir..
+00004a40: 6e61 6d65 da0d 6765 745f 6675 6c6c 5f6e  name..get_full_n
+00004a50: 616d 65da 015f da0c 6973 5f69 6e73 7461  ame.._..is_insta
+00004a60: 6c6c 6564 724f 0100 0072 5901 0000 7248  lledrO...rY...rH
+00004a70: 0000 0072 5d00 0000 da0f 6765 745f 6175  ...r].....get_au
+00004a80: 7468 6f72 6974 6965 7372 5e01 0000 da19  thoritiesr^.....
+00004a90: 616c 6c6f 775f 6f6e 6c69 6e65 5f72 6567  allow_online_reg
+00004aa0: 6973 7472 6174 696f 6eda 0b69 735f 7665  istration..is_ve
+00004ab0: 7269 6669 6564 da19 7665 7269 6669 6361  rified..verifica
+00004ac0: 7469 6f6e 5f63 6f64 655f 7365 6e74 5f6f  tion_code_sent_o
+00004ad0: 6eda 0864 6174 6574 696d 65da 0974 696d  n..datetime..tim
+00004ae0: 6564 656c 7461 da19 7665 7269 6669 6361  edelta..verifica
+00004af0: 7469 6f6e 5f63 6f64 655f 6578 7069 7265  tion_code_expire
+00004b00: 7372 0f00 0000 da08 6f76 6572 7269 6465  sr......override
+00004b10: da09 7469 6d65 7374 616d 70da 0a6d 616b  ..timestamp..mak
+00004b20: 655f 6e61 6976 6572 2100 0000 2904 da0d  e_naiver!...)...
+00004b30: 7573 6572 5f73 6574 7469 6e67 7372 5f01  user_settingsr_.
+00004b40: 0000 da0b 6578 7069 7279 5f74 696d 65da  ....expiry_time.
+00004b50: 0c65 7870 6972 795f 7374 616d 70a9 04da  .expiry_stamp...
+00004b60: 086e 6f74 5f61 6e6f 6eda 0273 7572 5401  .not_anon..surT.
+00004b70: 0000 72f7 0000 0072 3600 0000 7237 0000  ..r....r6...r7..
+00004b80: 0072 4a01 0000 aa02 0000 7352 0000 0008  .rJ.......sR....
+00004b90: 0206 0102 ff12 0202 0204 010c 0104 0104  ................
+00004ba0: 0216 0108 0102 0112 0102 0106 0106 0106  ................
+00004bb0: 0106 011e 0204 0106 ef04 1412 010a 0104  ................
+00004bc0: 020c 010a 010c 020a 010e 0108 0108 010a  ................
+00004bd0: 0108 ff0c 0306 0108 0106 ff1c ff08 0308  ................
+00004be0: 027a 1f55 7365 7253 6574 7469 6e67 732e  .z.UserSettings.
+00004bf0: 6765 742e 3c6c 6f63 616c 733e 2e67 6574  get.<locals>.get
+00004c00: 6974 2907 721c 0000 0072 4001 0000 724b  it).r....r@...rK
+00004c10: 0100 0072 6801 0000 da10 6973 5f61 7574  ...rh.....is_aut
+00004c20: 6865 6e74 6963 6174 6564 7229 0000 0072  henticatedr)...r
+00004c30: ed00 0000 724c 0100 0072 3600 0000 7278  ....rL...r6...rx
+00004c40: 0100 0072 3700 0000 727c 0000 00a1 0200  ...r7...r|......
+00004c50: 0073 0e00 0000 0801 0601 0601 1201 0603  .s..............
+00004c60: 1202 1032 7a10 5573 6572 5365 7474 696e  ...2z.UserSettin
+00004c70: 6773 2e67 6574 4e72 b000 0000 7236 0000  gs.getNr....r6..
+00004c80: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+00004c90: 724d 0100 009d 0200 0073 0600 0000 0800  rM.......s......
+00004ca0: 0401 0c03 724d 0100 0072 b600 0000 2962  ....rM...r....)b
+00004cb0: 72b1 0000 00da 026f 7372 0200 0000 726f  r......osr....ro
+00004cc0: 0100 00da 0272 65da 0363 6769 da03 6173  .....re..cgi..as
+00004cd0: 7472 d300 0000 7245 0100 0072 0800 0000  tr....rE...r....
+00004ce0: da05 7479 7065 7372 0300 0000 da11 6a69  ..typesr......ji
+00004cf0: 6e6a 6132 2e65 7863 6570 7469 6f6e 7372  nja2.exceptionsr
+00004d00: 0400 0000 da0a 6574 6765 6e2e 6874 6d6c  ......etgen.html
+00004d10: 7205 0000 0072 0600 0000 da05 6574 6765  r....r......etge
+00004d20: 6eda 0678 6768 746d 6cda 0664 6a61 6e67  n..xghtml..djang
+00004d30: 6f72 0900 0000 da09 646a 616e 676f 2e64  or......django.d
+00004d40: 6272 0a00 0000 da0b 646a 616e 676f 2e63  br......django.c
+00004d50: 6f6e 6672 0b00 0000 da14 646a 616e 676f  onfr......django
+00004d60: 2e76 6965 7773 2e67 656e 6572 6963 720c  .views.genericr.
+00004d70: 0000 00da 1964 6a61 6e67 6f2e 7669 6577  .....django.view
+00004d80: 732e 6765 6e65 7269 632e 6261 7365 720d  s.generic.baser.
+00004d90: 0000 00da 0b64 6a61 6e67 6f2e 636f 7265  .....django.core
+00004da0: 720e 0000 00da 0c64 6a61 6e67 6f2e 7574  r......django.ut
+00004db0: 696c 7372 0f00 0000 da18 646a 616e 676f  ilsr......django
+00004dc0: 2e75 7469 6c73 2e74 7261 6e73 6c61 7469  .utils.translati
+00004dd0: 6f6e 7210 0000 0072 6901 0000 7211 0000  onr....ri...r...
+00004de0: 00da 1664 6a61 6e67 6f2e 636f 7265 2e65  ...django.core.e
+00004df0: 7863 6570 7469 6f6e 7372 1200 0000 da09  xceptionsr......
+00004e00: 6c69 6e6f 2e63 6f72 6572 1300 0000 da0a  lino.corer......
+00004e10: 6c69 6e6f 2e75 7469 6c73 7214 0000 00da  lino.utilsr.....
+00004e20: 106c 696e 6f2e 7574 696c 732e 6a73 6765  .lino.utils.jsge
+00004e30: 6e72 1500 0000 7216 0000 00da 0f6c 696e  nr....r......lin
+00004e40: 6f2e 636f 7265 2e65 6c65 6d73 7217 0000  o.core.elemsr...
+00004e50: 00da 106c 696e 6f2e 636f 7265 2e66 6965  ...lino.core.fie
+00004e60: 6c64 7372 1800 0000 da0e 6c69 6e6f 2e63  ldsr......lino.c
+00004e70: 6f72 652e 6766 6b73 7219 0000 0072 1b00  ore.gfksr....r..
+00004e80: 0000 da12 6c69 6e6f 2e63 6f72 652e 7265  ....lino.core.re
+00004e90: 7175 6573 7473 721c 0000 0072 1d00 0000  questsr....r....
+00004ea0: da16 6c69 6e6f 2e63 6f72 652e 7461 626c  ..lino.core.tabl
+00004eb0: 6572 6571 7565 7374 721e 0000 00da 0f6c  erequestr......l
+00004ec0: 696e 6f2e 636f 7265 2e76 6965 7773 721f  ino.core.viewsr.
+00004ed0: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
+00004ee0: 0000 7223 0000 00da 0f6c 696e 6f2e 636f  ..r#.....lino.co
+00004ef0: 7265 2e75 7469 6c73 7224 0000 00da 116c  re.utilsr$.....l
+00004f00: 696e 6f2e 636f 7265 2e61 6374 696f 6e73  ino.core.actions
+00004f10: 7225 0000 0072 2600 0000 da0f 6c69 6e6f  r%...r&.....lino
+00004f20: 2e63 6f72 652e 7374 6f72 6572 2700 0000  .core.storer'...
+00004f30: da17 6c69 6e6f 2e6d 6f64 6c69 622e 7573  ..lino.modlib.us
+00004f40: 6572 732e 7574 696c 7372 2800 0000 7229  ers.utilsr(...r)
+00004f50: 0000 00da 086c 696e 6f2e 6170 6972 2a00  .....lino.apir*.
+00004f60: 0000 da17 6c69 6e6f 2e6d 6f64 6c69 622e  ....lino.modlib.
+00004f70: 6578 746a 732e 7669 6577 7372 2b00 0000  extjs.viewsr+...
+00004f80: 722c 0000 0072 2d00 0000 7238 0000 0072  r,...r-...r8...r
+00004f90: e200 0000 7259 0000 0072 a500 0000 72b4  ....rY...r....r.
+00004fa0: 0000 0072 c400 0000 72cb 0000 0072 d000  ...r....r....r..
+00004fb0: 0000 72fc 0000 0072 1401 0000 7215 0100  ..r....r....r...
+00004fc0: 0072 1701 0000 7220 0100 0072 2601 0000  .r....r ...r&...
+00004fd0: 722c 0100 0072 3101 0000 7241 0100 0072  r,...r1...rA...r
+00004fe0: 4d01 0000 7236 0000 0072 3600 0000 7236  M...r6...r6...r6
+00004ff0: 0000 0072 3700 0000 da08 3c6d 6f64 756c  ...r7.....<modul
+00005000: 653e 0100 0000 737c 0000 0004 040c 0308  e>....s|........
+00005010: 0108 0108 0108 0108 0108 0108 010c 010c  ................
+00005020: 0110 010c 010c 020c 010c 010c 010c 010c  ................
+00005030: 010c 010c 010c 010c 010c 030c 010c 010c  ................
+00005040: 010c 010c 010c 010c 0110 010c 0110 0110  ................
+00005050: 010c 010c 010c 010c 010c 0110 020c 0114  ................
+00005060: 010a 0304 0e10 0710 2210 7110 0f10 2a10  ........".q...*.
+00005070: 1f10 1008 5e08 1310 4310 0410 0810 1010  ....^...C.......
+00005080: 1610 0a10 3214 33                        ....2.3
```

### Comparing `lino_react-23.6.1/lino_react/react/config/react/main.html` & `lino_react-23.6.2/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/config/react/service-worker.js` & `lino_react-23.6.2/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/icons.py` & `lino_react-23.6.2/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/renderer.py` & `lino_react-23.6.2/lino_react/react/renderer.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.6.2/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.6.2/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.6.2/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.6.2/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/static/react/main.js` & `lino_react-23.6.2/lino_react/react/static/react/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5318,20 +5318,20 @@
                             document.querySelector(".layout-main .l-header").contains(document.activeElement) || this.state.window_width == t || this.setState({
                                 show_top_toolbar: !(0, _.tq)() && void 0 !== this.props.actorData.col,
                                 window_width: window.innerWidth
                             })
                         }
                     }, {
                         key: "update_params_values",
-                        value: function(e) {
+                        value: function(e, t, n) {
                             (0, _.ku)(this.data.params_values, this.props.actorData.params_fields);
-                            var t = Object.assign({}, this.data.params_values, Ke({}, e)),
-                                n = (0, _.ku)(t, this.props.actorData.params_fields);
-                            this.data.pv = n, Object.assign(this.data, {
-                                params_values: t
+                            var o = Object.assign({}, this.data.params_values, Ke({}, e)),
+                                r = (0, _.ku)(o, this.props.actorData.params_fields);
+                            this.data.pv = r, Object.assign(this.data, {
+                                params_values: o
                             }), this.reload()
                         }
                     }, {
                         key: "get_current_grid_config",
                         value: function(e) {
                             var t = this.props.actorData.col,
                                 n = [],
@@ -12554,116 +12554,14 @@
                                 onExit: this.onOverlayExit,
                                 onExited: this.onOverlayExited,
                                 transitionOptions: this.props.transitionOptions
                             }, a, l, s, p))
                         }
                     }]), i
                 }(o.Component);
-
-                function Qt(e) {
-                    return Qt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                        return typeof e
-                    } : function(e) {
-                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, Qt(e)
-                }
-
-                function $t() {
-                    return $t = Object.assign || function(e) {
-                        for (var t = 1; t < arguments.length; t++) {
-                            var n = arguments[t];
-                            for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
-                        }
-                        return e
-                    }, $t.apply(this, arguments)
-                }
-
-                function en(e, t, n) {
-                    return t in e ? Object.defineProperty(e, t, {
-                        value: n,
-                        enumerable: !0,
-                        configurable: !0,
-                        writable: !0
-                    }) : e[t] = n, e
-                }
-
-                function tn(e, t) {
-                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                }
-
-                function nn(e, t) {
-                    for (var n = 0; n < t.length; n++) {
-                        var o = t[n];
-                        o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
-                    }
-                }
-
-                function on(e, t, n) {
-                    return t && nn(e.prototype, t), n && nn(e, n), Object.defineProperty(e, "prototype", {
-                        writable: !1
-                    }), e
-                }
-
-                function rn(e, t) {
-                    if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                    Object.defineProperty(e, "prototype", {
-                        value: Object.create(t && t.prototype, {
-                            constructor: {
-                                value: e,
-                                writable: !0,
-                                configurable: !0
-                            }
-                        }),
-                        writable: !1
-                    }), t && an(e, t)
-                }
-
-                function an(e, t) {
-                    return an = Object.setPrototypeOf || function(e, t) {
-                        return e.__proto__ = t, e
-                    }, an(e, t)
-                }
-
-                function ln(e) {
-                    var t = function() {
-                        if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                        if (Reflect.construct.sham) return !1;
-                        if ("function" == typeof Proxy) return !0;
-                        try {
-                            return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                        } catch (e) {
-                            return !1
-                        }
-                    }();
-                    return function() {
-                        var n, o = un(e);
-                        if (t) {
-                            var r = un(this).constructor;
-                            n = Reflect.construct(o, arguments, r)
-                        } else n = o.apply(this, arguments);
-                        return sn(this, n)
-                    }
-                }
-
-                function sn(e, t) {
-                    if (t && ("object" === Qt(t) || "function" == typeof t)) return t;
-                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return pn(e)
-                }
-
-                function pn(e) {
-                    if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                    return e
-                }
-
-                function un(e) {
-                    return un = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                        return e.__proto__ || Object.getPrototypeOf(e)
-                    }, un(e)
-                }
                 Ht(Jt, "defaultProps", {
                     id: null,
                     inputRef: null,
                     name: null,
                     value: null,
                     visible: !1,
                     viewDate: null,
@@ -12737,40 +12635,151 @@
                     onChange: null,
                     onViewDateChange: null,
                     onTodayButtonClick: null,
                     onClearButtonClick: null,
                     onShow: null,
                     onHide: null
                 });
-                var cn = function(e) {
-                        rn(n, e);
-                        var t = ln(n);
+                var Qt = n(1008);
+
+                function $t(e) {
+                    return $t = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                        return typeof e
+                    } : function(e) {
+                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+                    }, $t(e)
+                }
+
+                function en() {
+                    return en = Object.assign || function(e) {
+                        for (var t = 1; t < arguments.length; t++) {
+                            var n = arguments[t];
+                            for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
+                        }
+                        return e
+                    }, en.apply(this, arguments)
+                }
+
+                function tn(e, t, n) {
+                    return t in e ? Object.defineProperty(e, t, {
+                        value: n,
+                        enumerable: !0,
+                        configurable: !0,
+                        writable: !0
+                    }) : e[t] = n, e
+                }
+
+                function nn(e, t) {
+                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+                }
+
+                function on(e, t) {
+                    for (var n = 0; n < t.length; n++) {
+                        var o = t[n];
+                        o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
+                    }
+                }
+
+                function rn(e, t, n) {
+                    return t && on(e.prototype, t), n && on(e, n), Object.defineProperty(e, "prototype", {
+                        writable: !1
+                    }), e
+                }
+
+                function an(e, t) {
+                    if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
+                    Object.defineProperty(e, "prototype", {
+                        value: Object.create(t && t.prototype, {
+                            constructor: {
+                                value: e,
+                                writable: !0,
+                                configurable: !0
+                            }
+                        }),
+                        writable: !1
+                    }), t && ln(e, t)
+                }
+
+                function ln(e, t) {
+                    return ln = Object.setPrototypeOf || function(e, t) {
+                        return e.__proto__ = t, e
+                    }, ln(e, t)
+                }
+
+                function sn(e) {
+                    var t = function() {
+                        if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
+                        if (Reflect.construct.sham) return !1;
+                        if ("function" == typeof Proxy) return !0;
+                        try {
+                            return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
+                        } catch (e) {
+                            return !1
+                        }
+                    }();
+                    return function() {
+                        var n, o = cn(e);
+                        if (t) {
+                            var r = cn(this).constructor;
+                            n = Reflect.construct(o, arguments, r)
+                        } else n = o.apply(this, arguments);
+                        return pn(this, n)
+                    }
+                }
+
+                function pn(e, t) {
+                    if (t && ("object" === $t(t) || "function" == typeof t)) return t;
+                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
+                    return un(e)
+                }
+
+                function un(e) {
+                    if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                    return e
+                }
+
+                function cn(e) {
+                    return cn = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                        return e.__proto__ || Object.getPrototypeOf(e)
+                    }, cn(e)
+                }
+                var dn = function(e) {
+                        an(n, e);
+                        var t = sn(n);
 
                         function n(e) {
                             var o;
-                            return tn(this, n), (o = t.call(this, e)).state = {
+                            return nn(this, n), (o = t.call(this, e)).state = {
                                 unsaved: !1,
                                 value: o.convertValueToDate(qn(e))
-                            }, o.componentDidMount = Fn.bind(pn(o)), o.getSnapshotBeforeUpdate = zn.bind(pn(o)), o.defaultCDU = Un.bind(pn(o)), o.componentWillUnmount = Kn.bind(pn(o)), o.update_props = o.update_props.bind(pn(o)), o
+                            }, o.componentDidMount = Fn.bind(un(o)), o.getSnapshotBeforeUpdate = zn.bind(un(o)), o.defaultCDU = Un.bind(un(o)), o.componentWillUnmount = Kn.bind(un(o)), o.update_props = o.update_props.bind(un(o)), o
                         }
-                        return on(n, [{
+                        return rn(n, [{
                             key: "componentDidUpdate",
                             value: function(e, t, n) {
                                 if (null !== n && (this.defaultCDU(e, t, n), n.hasOwnProperty("newValue"))) {
                                     var o = qn(this.props);
                                     this.setState({
                                         value: this.convertValueToDate(o)
                                     })
                                 }
                             }
                         }, {
                             key: "update_props",
                             value: function(e) {
-                                var t = e.value;
-                                [null, void 0].includes(t) && (t = ""), this.props.update_value(en({}, Tn(this.props), this.formattedDate(t)), this.props.elem, this.props.column)
+                                var t = this,
+                                    n = function(e, n, o) {
+                                        t.props.update_value(e, n, o)
+                                    },
+                                    o = e.value;
+                                if ([null, void 0].includes(o)) {
+                                    if (this.props.window_type === Qt.Mj) return void("" === e.originalEvent.target.value && n(tn({}, Tn(this.props), null), this.props.elem, this.props.column));
+                                    o = ""
+                                }
+                                n(tn({}, Tn(this.props), this.formattedDate(o)), this.props.elem, this.props.column)
                             }
                         }, {
                             key: "convertValueToDate",
                             value: function(e) {
                                 if (e instanceof Date) return e;
                                 var t = e ? e.split(".") : [];
                                 return 3 === t.length ? new Date(t[2], t[1] - 1, t[0]) : e
@@ -12800,51 +12809,50 @@
                                                 value: t.value
                                             }), e.update_props(t), "click" === t.originalEvent.type && e.inputEl.reFocusInputField()
                                         },
                                         onSelect: function(t) {
                                             return e.update_props(t)
                                         },
                                         onClearButtonClick: function(t) {
-                                            t.value = "", e.update_props(t)
+                                            t.value = null, e.update_props(t)
                                         },
                                         yearNavigator: !0,
                                         yearRange: "1900:2900",
                                         showButtonBar: !0,
                                         showOnFocus: !1,
                                         ref: function(t) {
                                             return e.inputEl = t
                                         },
-                                        readOnlyInput: "p" === this.props.window_type,
                                         className: "l-DateFieldElement"
                                     });
-                                return o.createElement(Dn, $t({}, this.props, {
+                                return o.createElement(Dn, en({}, this.props, {
                                     elem: this.props.elem,
                                     labeled: this.props.labeled,
                                     isFilled: this.state.value
                                 }), this.props.editing_mode && !An(this.props) ? this.props.in_grid ? o.createElement("div", {
                                     onClick: function(e) {
                                         return e.stopPropagation()
                                     }
                                 }, t) : t : Rn(this.formattedDate(this.state.value), this.props))
                             }
                         }]), n
                     }(o.Component),
-                    dn = function(e) {
-                        rn(n, e);
-                        var t = ln(n);
+                    fn = function(e) {
+                        an(n, e);
+                        var t = sn(n);
 
                         function n(e) {
                             var o;
-                            return tn(this, n), (o = t.call(this, e)).state = {
+                            return nn(this, n), (o = t.call(this, e)).state = {
                                 unsaved: !1,
                                 value: o.str2date(qn(e)),
                                 overlayPanelHookElementId: "time-input-" + Math.floor(1e3 * Math.random()).toString()
-                            }, o.componentDidMount = Fn.bind(pn(o)), o.getSnapshotBeforeUpdate = zn.bind(pn(o)), o.defaultCDU = Un.bind(pn(o)), o.componentWillUnmount = Kn.bind(pn(o)), o.str2date = o.str2date.bind(pn(o)), o.getElementForOverlayPanel = o.getElementForOverlayPanel.bind(pn(o)), o
+                            }, o.componentDidMount = Fn.bind(un(o)), o.getSnapshotBeforeUpdate = zn.bind(un(o)), o.defaultCDU = Un.bind(un(o)), o.componentWillUnmount = Kn.bind(un(o)), o.str2date = o.str2date.bind(un(o)), o.getElementForOverlayPanel = o.getElementForOverlayPanel.bind(un(o)), o
                         }
-                        return on(n, [{
+                        return rn(n, [{
                             key: "componentDidUpdate",
                             value: function(e, t, n) {
                                 if (null !== n && (this.defaultCDU(e, t, n), n.hasOwnProperty("newValue"))) {
                                     var o = qn(this.props);
                                     this.setState({
                                         value: this.str2date(o)
                                     })
@@ -12873,15 +12881,15 @@
                             value: function() {
                                 return document.getElementById(this.state.overlayPanelHookElementId)
                             }
                         }, {
                             key: "render",
                             value: function() {
                                 var e = this;
-                                return o.createElement(Dn, $t({}, this.props, {
+                                return o.createElement(Dn, en({}, this.props, {
                                     elem: this.props.elem,
                                     labeled: this.props.labeled,
                                     isFilled: this.state.value
                                 }), this.props.editing_mode && !An(this.props) ? o.createElement(o.Fragment, null, o.createElement(Jt, {
                                     style: {
                                         width: "100%"
                                     },
@@ -12893,32 +12901,34 @@
                                     inputStyle: {
                                         width: "100%"
                                     },
                                     value: this.state.value,
                                     keepInvalid: !0,
                                     hourFormat: "24",
                                     onChange: function(t) {
-                                        var n;
-                                        e.state.unsaved || e.setState({
-                                            unsaved: !0
-                                        }), t.value instanceof Date ? (e.setState({
+                                        var n, o = function(t, n, o) {
+                                            e.props.update_value(t, n, o)
+                                        };
+                                        if (e.state.unsaved || e.setState({
+                                                unsaved: !0
+                                            }), t.value instanceof Date) e.setState({
                                             value: t.value
-                                        }), n = e.date2str(t.value)) : n = t.value, e.props.update_value(en({}, Tn(e.props), n), e.props.elem, e.props.column)
+                                        }), n = e.date2str(t.value);
+                                        else if (n = t.value, e.props.window_type === Qt.Mj) return void("" === n && o(tn({}, Tn(e.props), null), e.props.elem, e.props.column));
+                                        o(tn({}, Tn(e.props), n), e.props.elem, e.props.column)
                                     },
-                                    readOnlyInput: "p" === this.props.window_type,
                                     ref: function(t) {
                                         return e.inputEl = t
                                     }
                                 }), o.createElement("div", {
                                     id: this.state.overlayPanelHookElementId
                                 })) : Rn(qn(this.props), this.props))
                             }
                         }]), n
-                    }(o.Component),
-                    fn = n(1008);
+                    }(o.Component);
 
                 function hn(e) {
                     return hn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, hn(e)
@@ -13970,16 +13980,16 @@
                                     checked: t || !1
                                 })))
                             }
                         }]), n
                     }(o.Component),
                     PreviewTextFieldElement: Rt,
                     TextFieldElement: qt,
-                    DateFieldElement: cn,
-                    TimeFieldElement: dn,
+                    DateFieldElement: dn,
+                    TimeFieldElement: fn,
                     ForeignKeyElement: nt,
                     FileFieldElement: function(e) {
                         _n(n, e);
                         var t = On(n);
 
                         function n() {
                             var e;
@@ -14037,15 +14047,15 @@
                             }, o.messageInterceptor = o.messageInterceptor.bind(Sn(o)), o
                         }
                         return xn(n, [{
                             key: "componentDidMount",
                             value: function() {
                                 this.widthInCh = parseInt(this.container.offsetWidth / this.chInPx.offsetWidth);
                                 var e = (0, Ge.ol)(this.props.elem.display_mode, this.widthInCh);
-                                if ([fn.BQ, fn.Jg, fn.do, fn.UZ].includes(e)) {
+                                if ([Qt.BQ, Qt.Jg, Qt.do, Qt.UZ].includes(e)) {
                                     var t = this.props.elem[e],
                                         n = Zn[t.react_name];
                                     this.elem = o.createElement(n, vn({}, this.props, {
                                         elem: t,
                                         parent: this.props.parent
                                     }))
                                 } else {
@@ -15199,15 +15209,15 @@
                         return y(this, n), (o = t.call(this, e)).state = {
                             query: e.parent.data.query || ""
                         }, o.parent = e.parent, o.controller = new(i()), o.renderActionBar = o.renderActionBar.bind(C(o)), o.renderDataViewSortButton = o.renderDataViewSortButton.bind(C(o)), o.renderDetailNavigator = o.renderDetailNavigator.bind(C(o)), o.renderEditorButton = o.renderEditorButton.bind(C(o)), o.renderParamValueControls = o.renderParamValueControls.bind(C(o)), o.renderQuickFilter = o.renderQuickFilter.bind(C(o)), o.renderToggle_colControls = o.renderToggle_colControls.bind(C(o)), o
                     }
                     return k(n, [{
                         key: "componentDidUpdate",
                         value: function(e, t, n) {
-                            window.App.isMobile || this.parent.data.editing_mode || window.App.data.dialogs.length || "calview" === this.parent.props.packId || this.inputEl && this.inputEl.focus()
+                            window.App.isMobile || this.parent.data.editing_mode || window.App.data.dialogs.length || "calview" === this.parent.props.packId || this.parent.state.showPVDialog || this.inputEl && this.inputEl.focus()
                         }
                     }, {
                         key: "renderActionBar",
                         value: function(e, t) {
                             return o.createElement(d.Z, {
                                 actorData: this.parent.props.actorData,
                                 disabledFields: this.parent.data.disabled_fields,
```

### Comparing `lino_react-23.6.1/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.6.2/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/react/views.py` & `lino_react-23.6.2/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.1/lino_react/setup_info.py` & `lino_react-23.6.2/lino_react/setup_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.6.1',
+    version='23.6.2',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.6.1/lino_react.egg-info/PKG-INFO` & `lino_react-23.6.2/lino_react.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-react
-Version: 23.6.1
+Version: 23.6.2
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
 Classifier:   Environment :: Web Environment
 Classifier:   Framework :: Django
 Classifier:   Intended Audience :: Developers
 Classifier:   Intended Audience :: System Administrators
@@ -25,9 +23,7 @@
 
 
 The React front end for Lino
 
 Project homepage is https://gitlab.com/lino-framework/react
 
 
-
-
```

