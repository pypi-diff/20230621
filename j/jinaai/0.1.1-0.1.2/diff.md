# Comparing `tmp/jinaai-0.1.1.tar.gz` & `tmp/jinaai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.1.1.tar", last modified: Mon Jun 12 03:55:38 2023, max compression
+gzip compressed data, was "jinaai-0.1.2.tar", last modified: Wed Jun 21 05:46:03 2023, max compression
```

## Comparing `jinaai-0.1.1.tar` & `jinaai-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 03:55:38.170729 jinaai-0.1.1/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.1.1/LICENSE
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      208 2023-06-12 03:55:38.170535 jinaai-0.1.1/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      627 2023-06-09 08:24:51.000000 jinaai-0.1.1/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 03:55:38.169874 jinaai-0.1.1/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      383 2023-06-09 08:13:55.000000 jinaai-0.1.1/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 03:55:38.170401 jinaai-0.1.1/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      208 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      165 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-12 03:55:38.170768 jinaai-0.1.1/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      307 2023-06-12 03:53:51.000000 jinaai-0.1.1/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.427412 jinaai-0.1.2/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.1.2/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-21 05:46:03.427099 jinaai-0.1.2/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12653 2023-06-21 05:42:42.000000 jinaai-0.1.2/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.424633 jinaai-0.1.2/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2617 2023-06-20 03:59:26.000000 jinaai-0.1.2/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.426862 jinaai-0.1.2/jinaai/clients/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1809 2023-06-20 05:46:39.000000 jinaai-0.1.2/jinaai/clients/ChatCatClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.1.2/jinaai/clients/HTTPClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2110 2023-06-19 04:25:56.000000 jinaai-0.1.2/jinaai/clients/PromptPerfectClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.1.2/jinaai/clients/RationaleClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.1.2/jinaai/clients/SceneXClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.1.2/jinaai/clients/__init__.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.1.2/jinaai/utils.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.425289 jinaai-0.1.2/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      372 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-21 05:46:03.427460 jinaai-0.1.2/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      483 2023-06-21 05:45:46.000000 jinaai-0.1.2/setup.py
```

### Comparing `jinaai-0.1.1/LICENSE` & `jinaai-0.1.2/LICENSE`

 * *Files identical despite different names*

