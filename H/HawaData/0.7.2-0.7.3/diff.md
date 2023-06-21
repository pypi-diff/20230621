# Comparing `tmp/HawaData-0.7.2.tar.gz` & `tmp/HawaData-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.7.2.tar", last modified: Wed Jun 21 13:18:27 2023, max compression
+gzip compressed data, was "HawaData-0.7.3.tar", last modified: Wed Jun 21 13:28:38 2023, max compression
```

## Comparing `HawaData-0.7.2.tar` & `HawaData-0.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.889094 HawaData-0.7.2/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.875389 HawaData-0.7.2/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3033 2023-06-21 13:18:27.000000 HawaData-0.7.2/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-21 13:18:27.000000 HawaData-0.7.2/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-21 13:18:27.000000 HawaData-0.7.2/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-21 13:18:27.000000 HawaData-0.7.2/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3033 2023-06-21 13:18:27.888749 HawaData-0.7.2/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.2/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.875931 HawaData-0.7.2/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.2/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.878617 HawaData-0.7.2/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.2/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.2/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.2/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.2/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.2/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.880766 HawaData-0.7.2/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.2/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    12092 2023-06-21 13:18:12.000000 HawaData-0.7.2/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.2/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.2/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.7.2/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.884549 HawaData-0.7.2/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.2/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.2/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.2/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.2/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-21 13:09:45.000000 HawaData-0.7.2/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.2/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.886980 HawaData-0.7.2/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.2/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28321 2023-06-21 09:11:05.000000 HawaData-0.7.2/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.2/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-21 13:18:27.889235 HawaData-0.7.2/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.2/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:18:27.887826 HawaData-0.7.2/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.2/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.765908 HawaData-0.7.3/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.754854 HawaData-0.7.3/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3073 2023-06-21 13:28:38.000000 HawaData-0.7.3/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-21 13:28:38.000000 HawaData-0.7.3/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-21 13:28:38.000000 HawaData-0.7.3/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-21 13:28:38.000000 HawaData-0.7.3/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3073 2023-06-21 13:28:38.765630 HawaData-0.7.3/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.3/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.755427 HawaData-0.7.3/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.3/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.758252 HawaData-0.7.3/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.3/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.3/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.3/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.3/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.3/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.760166 HawaData-0.7.3/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.3/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    12444 2023-06-21 13:26:47.000000 HawaData-0.7.3/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.3/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.3/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.7.3/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.763301 HawaData-0.7.3/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.3/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.3/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.3/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.3/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-21 13:09:45.000000 HawaData-0.7.3/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.3/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.764434 HawaData-0.7.3/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.3/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28321 2023-06-21 09:11:05.000000 HawaData-0.7.3/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.3/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-21 13:28:38.765985 HawaData-0.7.3/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.3/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 13:28:38.765003 HawaData-0.7.3/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.3/test/test_query.py
```

### Comparing `HawaData-0.7.2/HawaData.egg-info/PKG-INFO` & `HawaData-0.7.3/HawaData.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.2
+Version: 0.7.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -104,7 +104,8 @@
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
+- 0.7.3 add is_leaf to cascade students
```

### Comparing `HawaData-0.7.2/HawaData.egg-info/SOURCES.txt` & `HawaData-0.7.3/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/PKG-INFO` & `HawaData-0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.2
+Version: 0.7.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -104,7 +104,8 @@
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
+- 0.7.3 add is_leaf to cascade students
```

### Comparing `HawaData-0.7.2/README.md` & `HawaData-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/base/db.py` & `HawaData-0.7.3/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/base/init.py` & `HawaData-0.7.3/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/common/data.py` & `HawaData-0.7.3/hawa/common/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """通用的 report data 构造器，支持 校、区、市、省、全国级别的通用报告数据构造"""
 import json
 from collections import Counter, defaultdict
 from dataclasses import dataclass, field
-from pprint import pprint
 from typing import Optional, ClassVar, Any, Set
 
 import pandas as pd
 import pendulum
 from munch import Munch
 
 from hawa.base.db import DbUtil, RedisUtil
@@ -284,18 +283,30 @@
 
     def get_cascade_students(self):
         """年级/班级/学生嵌套"""
         data = self.final_scores
         data['cls'] = data['student_id'].apply(lambda x: str(x)[:15])
         res = []
         for grade, grade_group in data.groupby('grade'):
-            grade_row = {'label': f'{grade}年级', 'value': grade, 'children': []}
+            grade_row = {
+                'label': f'{grade}年级', 'value': grade,
+                'children': [], "is_leaf": False
+            }
             for cls, cls_group in grade_group.groupby('cls'):
-                cls_row = {'label': f'{cls[13:]}班', 'value': int(cls), 'children': []}
+                cls_row = {
+                    'label': f'{cls[13:]}班', 'value': int(cls),
+                    'children': [], "is_leaf": False
+                }
                 for _, student_g_row in cls_group.iterrows():
                     student_row = {
                         'label': student_g_row['username'],
-                        'value': str(student_g_row['student_id'])}
+                        'value': str(student_g_row['student_id']),
+                        "is_leaf": True
+                    }
                     cls_row['children'].append(student_row)
+                if not cls_row['children']:
+                    cls_row['is_leaf'] = True
                 grade_row['children'].append(cls_row)
+            if not grade_row['children']:
+                grade_row['is_leaf'] = True
             res.append(grade_row)
         return res
```

### Comparing `HawaData-0.7.2/hawa/common/query.py` & `HawaData-0.7.3/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/common/utils.py` & `HawaData-0.7.3/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/config.py` & `HawaData-0.7.3/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/data/klass.py` & `HawaData-0.7.3/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/data/school.py` & `HawaData-0.7.3/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/data/student.py` & `HawaData-0.7.3/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/paper/health.py` & `HawaData-0.7.3/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/hawa/paper/mht.py` & `HawaData-0.7.3/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/setup.py` & `HawaData-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.2/test/test_query.py` & `HawaData-0.7.3/test/test_query.py`

 * *Files identical despite different names*

