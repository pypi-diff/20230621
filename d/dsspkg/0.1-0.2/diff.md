# Comparing `tmp/dsspkg-0.1.tar.gz` & `tmp/dsspkg-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsspkg-0.1.tar", last modified: Sat Jun 17 13:08:26 2023, max compression
+gzip compressed data, was "dsspkg-0.2.tar", last modified: Wed Jun 21 03:25:41 2023, max compression
```

## Comparing `dsspkg-0.1.tar` & `dsspkg-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-17 13:08:26.222738 dsspkg-0.1/
--rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.1/LICENSE
--rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.1/MANIFEST.in
--rw-r--r--   0 danielwu   (501) staff       (20)      221 2023-06-17 13:08:26.222602 dsspkg-0.1/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:43:30.000000 dsspkg-0.1/README.md
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-17 13:08:26.221065 dsspkg-0.1/dsspkg/
--rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.1/dsspkg/__init__.py
--rw-r--r--   0 danielwu   (501) staff       (20)    21070 2023-06-17 09:15:49.000000 dsspkg-0.1/dsspkg/data_scaling_split.py
--rw-r--r--   0 danielwu   (501) staff       (20)      509 2023-06-17 12:40:56.000000 dsspkg-0.1/dsspkg/dss.py
--rw-r--r--   0 danielwu   (501) staff       (20)    16665 2023-06-17 12:36:15.000000 dsspkg-0.1/dsspkg/dss_p.py
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-17 13:08:26.222425 dsspkg-0.1/dsspkg/sth/
--rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.1/dsspkg/sth/minus.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.1/dsspkg/sth/minus_p.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.1/dsspkg/sth/radio.pkl
--rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.1/dsspkg/sth/radio_p.pkl
-drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-17 13:08:26.221906 dsspkg-0.1/dsspkg.egg-info/
--rw-r--r--   0 danielwu   (501) staff       (20)      221 2023-06-17 13:08:26.000000 dsspkg-0.1/dsspkg.egg-info/PKG-INFO
--rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-17 13:08:26.000000 dsspkg-0.1/dsspkg.egg-info/SOURCES.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-17 13:08:26.000000 dsspkg-0.1/dsspkg.egg-info/dependency_links.txt
--rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-17 13:08:26.000000 dsspkg-0.1/dsspkg.egg-info/top_level.txt
--rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-17 13:08:26.222772 dsspkg-0.1/setup.cfg
--rw-r--r--   0 danielwu   (501) staff       (20)      528 2023-06-17 13:07:18.000000 dsspkg-0.1/setup.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-21 03:25:41.763996 dsspkg-0.2/
+-rw-r--r--   0 danielwu   (501) staff       (20)     1073 2023-06-17 13:01:56.000000 dsspkg-0.2/LICENSE
+-rw-r--r--   0 danielwu   (501) staff       (20)       16 2023-06-17 13:08:05.000000 dsspkg-0.2/MANIFEST.in
+-rw-r--r--   0 danielwu   (501) staff       (20)      326 2023-06-21 03:25:41.763793 dsspkg-0.2/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      102 2023-06-21 03:24:46.000000 dsspkg-0.2/README.md
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-21 03:25:41.762051 dsspkg-0.2/dsspkg/
+-rw-r--r--   0 danielwu   (501) staff       (20)        0 2023-06-17 12:42:12.000000 dsspkg-0.2/dsspkg/__init__.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    21070 2023-06-17 09:15:49.000000 dsspkg-0.2/dsspkg/data_scaling_split.py
+-rw-r--r--   0 danielwu   (501) staff       (20)      555 2023-06-18 03:32:09.000000 dsspkg-0.2/dsspkg/dss.py
+-rw-r--r--   0 danielwu   (501) staff       (20)    16665 2023-06-17 12:36:15.000000 dsspkg-0.2/dsspkg/dss_p.py
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-21 03:25:41.763551 dsspkg-0.2/dsspkg/sth/
+-rw-r--r--   0 danielwu   (501) staff       (20)     6465 2023-04-15 09:36:22.000000 dsspkg-0.2/dsspkg/sth/minus.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2/dsspkg/sth/minus_p.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     6554 2023-04-15 09:36:22.000000 dsspkg-0.2/dsspkg/sth/radio.pkl
+-rw-r--r--   0 danielwu   (501) staff       (20)     1082 2023-06-17 06:49:36.000000 dsspkg-0.2/dsspkg/sth/radio_p.pkl
+drwxr-xr-x   0 danielwu   (501) staff       (20)        0 2023-06-21 03:25:41.762946 dsspkg-0.2/dsspkg.egg-info/
+-rw-r--r--   0 danielwu   (501) staff       (20)      326 2023-06-21 03:25:41.000000 dsspkg-0.2/dsspkg.egg-info/PKG-INFO
+-rw-r--r--   0 danielwu   (501) staff       (20)      324 2023-06-21 03:25:41.000000 dsspkg-0.2/dsspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        1 2023-06-21 03:25:41.000000 dsspkg-0.2/dsspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)        7 2023-06-21 03:25:41.000000 dsspkg-0.2/dsspkg.egg-info/top_level.txt
+-rw-r--r--   0 danielwu   (501) staff       (20)       38 2023-06-21 03:25:41.764037 dsspkg-0.2/setup.cfg
+-rw-r--r--   0 danielwu   (501) staff       (20)      528 2023-06-21 03:24:46.000000 dsspkg-0.2/setup.py
```

### Comparing `dsspkg-0.1/LICENSE` & `dsspkg-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsspkg-0.1/dsspkg/data_scaling_split.py` & `dsspkg-0.2/dsspkg/data_scaling_split.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.1/dsspkg/dss_p.py` & `dsspkg-0.2/dsspkg/dss_p.py`

 * *Files identical despite different names*

### Comparing `dsspkg-0.1/dsspkg/sth/minus.pkl` & `dsspkg-0.2/dsspkg/sth/minus.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.1/dsspkg/sth/minus_p.pkl` & `dsspkg-0.2/dsspkg/sth/minus_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.1/dsspkg/sth/radio.pkl` & `dsspkg-0.2/dsspkg/sth/radio.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.1/dsspkg/sth/radio_p.pkl` & `dsspkg-0.2/dsspkg/sth/radio_p.pkl`

 * *Files identical despite different names*

### Comparing `dsspkg-0.1/setup.py` & `dsspkg-0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dsspkg",   # 包名字
-    version="0.1",
+    version="0.2",
     description="A data splitting and scaling package",
     long_description=long_description,  # 将说明文件设置为README.md
     long_description_content_type="text/markdown",
     packages=find_packages(),   # 默认从当前目录下搜索包
     author="DW",
-    author_email="wwwsbx@live.com",
+    author_email="prwe98@gmail.com",
     python_requires='>=3.10',
-
 )
```

