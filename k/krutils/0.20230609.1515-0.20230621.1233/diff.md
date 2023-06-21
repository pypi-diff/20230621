# Comparing `tmp/krutils-0.20230609.1515.tar.gz` & `tmp/krutils-0.20230621.1233.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230609.1515.tar", last modified: Fri Jun  9 06:15:16 2023, max compression
+gzip compressed data, was "krutils-0.20230621.1233.tar", last modified: Wed Jun 21 03:33:04 2023, max compression
```

## Comparing `krutils-0.20230609.1515.tar` & `krutils-0.20230621.1233.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.410208 krutils-0.20230609.1515/
--rw-rw-rw-   0        0        0      526 2023-06-09 06:15:16.384976 krutils-0.20230609.1515/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230609.1515/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.030764 krutils-0.20230609.1515/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230609.1515/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230609.1515/krutils/CONST.py
--rw-rw-rw-   0        0        0      115 2023-06-07 14:26:39.000000 krutils-0.20230609.1515/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230609.1515/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2933 2023-06-09 06:14:27.000000 krutils-0.20230609.1515/krutils/futils.py
--rw-rw-rw-   0        0        0    12812 2023-06-09 06:11:45.000000 krutils-0.20230609.1515/krutils/logger.py
--rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230609.1515/krutils/logger2.py
--rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230609.1515/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.278864 krutils-0.20230609.1515/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 06:15:16.412361 krutils-0.20230609.1515/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-09 06:15:13.000000 krutils-0.20230609.1515/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.380453 krutils-0.20230609.1515/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230609.1515/test/test_futils.py
--rw-rw-rw-   0        0        0      231 2023-06-07 14:23:57.000000 krutils-0.20230609.1515/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.487017 krutils-0.20230621.1233/
+-rw-rw-rw-   0        0        0      526 2023-06-21 03:33:04.487017 krutils-0.20230621.1233/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230621.1233/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.452060 krutils-0.20230621.1233/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230621.1233/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230621.1233/krutils/CONST.py
+-rw-rw-rw-   0        0        0      115 2023-06-07 14:26:39.000000 krutils-0.20230621.1233/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230621.1233/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2956 2023-06-20 05:26:47.000000 krutils-0.20230621.1233/krutils/futils.py
+-rw-rw-rw-   0        0        0    12812 2023-06-09 06:11:45.000000 krutils-0.20230621.1233/krutils/logger.py
+-rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230621.1233/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230621.1233/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.468432 krutils-0.20230621.1233/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:33:04.487017 krutils-0.20230621.1233/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-21 03:33:03.000000 krutils-0.20230621.1233/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.482021 krutils-0.20230621.1233/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230621.1233/test/test_futils.py
+-rw-rw-rw-   0        0        0      231 2023-06-07 14:23:57.000000 krutils-0.20230621.1233/test/test_logger.py
```

### Comparing `krutils-0.20230609.1515/krutils/CONST.py` & `krutils-0.20230621.1233/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230609.1515/krutils/_dbmgr.py` & `krutils-0.20230621.1233/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230609.1515/krutils/futils.py` & `krutils-0.20230621.1233/krutils/futils.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
     if file_name == None or len(file_name.strip()) == 0:
         raise Exception('찾고자하는 파일명을 입력해 주세요')
 
     data_file_path = get_file_path_fr(file_name)
 
     if (data_file_path == None):
-        raise Exception('지정한 파일을 찾을 수 없습니다 [{0}]'.format(file_name))
+        # raise Exception('지정한 파일을 찾을 수 없습니다 [{0}]'.format(file_name))
+        return None
 
     import json
     with open(data_file_path, encoding='UTF8') as df:
         json_data = json.load(df)
 
     return json_data
```

### Comparing `krutils-0.20230609.1515/krutils/logger.py` & `krutils-0.20230621.1233/krutils/logger.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230609.1515/krutils/logger2.py` & `krutils-0.20230621.1233/krutils/logger2.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230609.1515/krutils/utils.py` & `krutils-0.20230621.1233/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230609.1515/setup.py` & `krutils-0.20230621.1233/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230609.1515",
+    version="0.20230621.1233",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

