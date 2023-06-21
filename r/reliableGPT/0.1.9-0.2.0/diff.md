# Comparing `tmp/reliableGPT-0.1.9.tar.gz` & `tmp/reliableGPT-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.1.9.tar", last modified: Tue Jun 20 21:53:08 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.0.tar", last modified: Wed Jun 21 00:49:10 2023, max compression
```

## Comparing `reliableGPT-0.1.9.tar` & `reliableGPT-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-20 21:53:08.139170 reliableGPT-0.1.9/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.1.9/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-20 21:53:08.139076 reliableGPT-0.1.9/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.1.9/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-20 21:53:08.138551 reliableGPT-0.1.9/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       24 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-20 21:53:08.138949 reliableGPT-0.1.9/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.1.9/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4229 2023-06-20 21:44:53.000000 reliableGPT-0.1.9/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1830 2023-06-20 21:45:33.000000 reliableGPT-0.1.9/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-20 21:53:08.139200 reliableGPT-0.1.9/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      293 2023-06-20 21:52:40.000000 reliableGPT-0.1.9/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:49:10.001815 reliableGPT-0.2.0/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.0/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 00:49:10.001724 reliableGPT-0.2.0/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.2.0/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:49:10.001027 reliableGPT-0.2.0/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       32 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:49:10.001448 reliableGPT-0.2.0/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.0/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7201 2023-06-21 00:44:15.000000 reliableGPT-0.2.0/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3469 2023-06-21 00:43:23.000000 reliableGPT-0.2.0/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-21 00:49:10.001845 reliableGPT-0.2.0/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      312 2023-06-21 00:48:53.000000 reliableGPT-0.2.0/setup.py
```

### Comparing `reliableGPT-0.1.9/LICENSE` & `reliableGPT-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.1.9/README.md` & `reliableGPT-0.2.0/README.md`

 * *Files identical despite different names*

