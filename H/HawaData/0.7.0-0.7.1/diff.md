# Comparing `tmp/HawaData-0.7.0.tar.gz` & `tmp/HawaData-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.7.0.tar", last modified: Mon Jun 19 09:02:19 2023, max compression
+gzip compressed data, was "HawaData-0.7.1.tar", last modified: Wed Jun 21 09:43:31 2023, max compression
```

## Comparing `HawaData-0.7.0.tar` & `HawaData-0.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.252437 HawaData-0.7.0/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.246690 HawaData-0.7.0/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2967 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2967 2023-06-19 09:02:19.252207 HawaData-0.7.0/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.0/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.247480 HawaData-0.7.0/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.0/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.248724 HawaData-0.7.0/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.0/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.0/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.0/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.0/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.0/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.249643 HawaData-0.7.0/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.0/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    11184 2023-06-14 03:54:52.000000 HawaData-0.7.0/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.0/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.0/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.7.0/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.250976 HawaData-0.7.0/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.0/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.0/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.0/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.0/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.7.0/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.0/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.251669 HawaData-0.7.0/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.0/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28118 2023-06-14 03:37:58.000000 HawaData-0.7.0/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.0/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-19 09:02:19.252500 HawaData-0.7.0/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.0/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.251917 HawaData-0.7.0/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.0/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.805557 HawaData-0.7.1/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.794882 HawaData-0.7.1/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3004 2023-06-21 09:43:31.000000 HawaData-0.7.1/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-21 09:43:31.000000 HawaData-0.7.1/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-21 09:43:31.000000 HawaData-0.7.1/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-21 09:43:31.000000 HawaData-0.7.1/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3004 2023-06-21 09:43:31.805273 HawaData-0.7.1/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.1/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.795470 HawaData-0.7.1/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.1/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.797990 HawaData-0.7.1/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.1/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.1/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.1/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.1/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.1/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.799844 HawaData-0.7.1/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.1/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    11184 2023-06-14 03:54:52.000000 HawaData-0.7.1/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.1/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.1/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.7.1/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.802760 HawaData-0.7.1/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.1/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.1/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.1/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.1/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.7.1/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.1/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.804183 HawaData-0.7.1/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.1/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28321 2023-06-21 09:11:05.000000 HawaData-0.7.1/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.1/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-21 09:43:31.805638 HawaData-0.7.1/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.1/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-21 09:43:31.804692 HawaData-0.7.1/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.1/test/test_query.py
```

### Comparing `HawaData-0.7.0/HawaData.egg-info/PKG-INFO` & `HawaData-0.7.1/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.0
+Version: 0.7.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -102,7 +102,8 @@
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
+- 0.7.1 count score rank with gender
```

### Comparing `HawaData-0.7.0/HawaData.egg-info/SOURCES.txt` & `HawaData-0.7.1/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/PKG-INFO` & `HawaData-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.0
+Version: 0.7.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -102,7 +102,8 @@
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
+- 0.7.1 count score rank with gender
```

### Comparing `HawaData-0.7.0/README.md` & `HawaData-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/base/db.py` & `HawaData-0.7.1/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/base/init.py` & `HawaData-0.7.1/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/common/data.py` & `HawaData-0.7.1/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/common/query.py` & `HawaData-0.7.1/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/common/utils.py` & `HawaData-0.7.1/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/config.py` & `HawaData-0.7.1/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/data/klass.py` & `HawaData-0.7.1/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/data/school.py` & `HawaData-0.7.1/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/data/student.py` & `HawaData-0.7.1/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/hawa/paper/health.py` & `HawaData-0.7.1/hawa/paper/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,24 @@
             self.cases = self.cases.loc[self.cases['id'] % 100 == self.grade, :]
             self.case_ids = self.cases['id'].tolist()
             self.case_project_ids = Counter(self.cases['project_id'].tolist())
             project.logger.debug(f'cases: {len(self.cases)}')
         if len(self.cases) == 0:
             raise NoCasesError(f'grade {self.grade} cases is empty')
 
-    def score_rank(self, grade: int):
-        """某年级 健康素养水平各等级占比"""
+    def score_rank(self, grade: int, gender: str = ''):
+        """
+        某年级 健康素养水平各等级占比
+        :param grade: 年级
+        :param gender: 性别 '' 全部 'M' 男 'F' 女
+        """
         base = {'优秀': 0, '良好': 0, '中等': 0, '待提高': 0}
-        final_scores = self.__get_grade_final_scores(grade=grade)
+        fs = final_scores = self.__get_grade_final_scores(grade=grade)
+        if gender:
+            final_scores = fs.loc[fs.gender == gender, :]
         raw = final_scores.level.value_counts().to_dict()
         data = base | raw
         sum_data = sum(data.values())
         if not sum_data:
             raise ValueError(f'grade {grade} score rank is empty')
         percent = {k: round(v * 100 / sum_data, 2) for k, v in data.items()}
         return percent
```

### Comparing `HawaData-0.7.0/hawa/paper/mht.py` & `HawaData-0.7.1/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/setup.py` & `HawaData-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.0/test/test_query.py` & `HawaData-0.7.1/test/test_query.py`

 * *Files identical despite different names*

