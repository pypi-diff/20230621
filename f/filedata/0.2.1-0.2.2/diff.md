# Comparing `tmp/filedata-0.2.1.tar.gz` & `tmp/filedata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedata-0.2.1.tar", last modified: Wed Mar 15 15:58:07 2023, max compression
+gzip compressed data, was "filedata-0.2.2.tar", last modified: Wed Jun 21 01:08:30 2023, max compression
```

## Comparing `filedata-0.2.1.tar` & `filedata-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-15 15:58:07.856860 filedata-0.2.1/
--rw-r--r--   0 jadbin     (501) staff       (20)      107 2023-02-15 14:58:14.000000 filedata-0.2.1/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)      546 2023-03-15 15:58:07.856577 filedata-0.2.1/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)       57 2023-02-15 14:58:03.000000 filedata-0.2.1/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-15 15:58:07.853314 filedata-0.2.1/filedata/
--rw-r--r--   0 jadbin     (501) staff       (20)       22 2023-03-15 15:57:04.000000 filedata-0.2.1/filedata/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      841 2023-02-15 15:39:30.000000 filedata-0.2.1/filedata/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3399 2023-03-15 15:56:53.000000 filedata-0.2.1/filedata/file.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2895 2023-02-16 09:21:38.000000 filedata-0.2.1/filedata/html.py
--rw-r--r--   0 jadbin     (501) staff       (20)     6466 2023-02-21 06:15:07.000000 filedata-0.2.1/filedata/image.py
--rw-r--r--   0 jadbin     (501) staff       (20)      801 2023-03-15 15:55:57.000000 filedata-0.2.1/filedata/pdf.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1198 2023-02-15 15:33:38.000000 filedata-0.2.1/filedata/retry.py
--rw-r--r--   0 jadbin     (501) staff       (20)      624 2023-02-15 15:52:33.000000 filedata-0.2.1/filedata/text.py
--rw-r--r--   0 jadbin     (501) staff       (20)       94 2021-09-18 08:02:02.000000 filedata-0.2.1/filedata/time.py
--rw-r--r--   0 jadbin     (501) staff       (20)      466 2023-02-16 07:02:15.000000 filedata-0.2.1/filedata/utils.py
--rw-r--r--   0 jadbin     (501) staff       (20)      252 2023-02-15 15:27:57.000000 filedata-0.2.1/filedata/video.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-15 15:58:07.855530 filedata-0.2.1/filedata.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)      546 2023-03-15 15:58:07.000000 filedata-0.2.1/filedata.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      457 2023-03-15 15:58:07.000000 filedata-0.2.1/filedata.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-03-15 15:58:07.000000 filedata-0.2.1/filedata.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-02-16 00:44:59.000000 filedata-0.2.1/filedata.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)      124 2023-03-15 15:58:07.000000 filedata-0.2.1/filedata.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        9 2023-03-15 15:58:07.000000 filedata-0.2.1/filedata.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-15 15:58:07.855814 filedata-0.2.1/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:04.000000 filedata-0.2.1/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2023-03-15 15:58:07.856970 filedata-0.2.1/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     1549 2023-02-19 15:03:08.000000 filedata-0.2.1/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-15 15:58:07.856274 filedata-0.2.1/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-04-15 01:21:31.000000 filedata-0.2.1/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.626152 filedata-0.2.2/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-06-21 00:08:49.000000 filedata-0.2.2/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 01:08:30.626152 filedata-0.2.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-06-21 00:08:49.000000 filedata-0.2.2/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.344731 filedata-0.2.2/filedata/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-21 01:07:14.000000 filedata-0.2.2/filedata/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     3399 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/file.py
+-rwxrwxrwx   0 root         (0) root         (0)     2895 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/html.py
+-rwxrwxrwx   0 root         (0) root         (0)     6466 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/image.py
+-rwxrwxrwx   0 root         (0) root         (0)      801 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/pdf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1198 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/retry.py
+-rwxrwxrwx   0 root         (0) root         (0)      624 2023-06-21 01:07:06.000000 filedata-0.2.2/filedata/text.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.516776 filedata-0.2.2/filedata/text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:11:15.000000 filedata-0.2.2/filedata/text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2939 2023-06-21 01:03:57.000000 filedata-0.2.2/filedata/text_algo/ac.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/time.py
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)      252 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/video.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.454276 filedata-0.2.2/filedata.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-21 01:08:30.000000 filedata-0.2.2/filedata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)      124 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.532401 filedata-0.2.2/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-21 00:08:49.000000 filedata-0.2.2/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-21 01:08:30.626152 filedata-0.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1549 2023-06-21 00:08:49.000000 filedata-0.2.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.563651 filedata-0.2.2/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:08:49.000000 filedata-0.2.2/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.594901 filedata-0.2.2/tests/test_text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:58:58.000000 filedata-0.2.2/tests/test_text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 01:06:46.000000 filedata-0.2.2/tests/test_text_algo/test_ac.py
```

### Comparing `filedata-0.2.1/filedata/config.py` & `filedata-0.2.2/filedata/config.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.1/filedata/file.py` & `filedata-0.2.2/filedata/file.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.1/filedata/html.py` & `filedata-0.2.2/filedata/html.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.1/filedata/image.py` & `filedata-0.2.2/filedata/image.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.1/filedata/pdf.py` & `filedata-0.2.2/filedata/pdf.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.1/filedata/retry.py` & `filedata-0.2.2/filedata/retry.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.1/filedata/text.py` & `filedata-0.2.2/filedata/text.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.1/setup.py` & `filedata-0.2.2/setup.py`

 * *Files identical despite different names*

