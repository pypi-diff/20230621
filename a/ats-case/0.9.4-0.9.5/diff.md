# Comparing `tmp/ats_case-0.9.4.tar.gz` & `tmp/ats_case-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.9.4.tar", last modified: Wed Jun 21 01:25:47 2023, max compression
+gzip compressed data, was "ats_case-0.9.5.tar", last modified: Wed Jun 21 07:30:39 2023, max compression
```

## Comparing `ats_case-0.9.4.tar` & `ats_case-0.9.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 01:25:47.742054 ats_case-0.9.4/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-21 01:25:47.740058 ats_case-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 01:25:47.273301 ats_case-0.9.4/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.4/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:25:47.465789 ats_case-0.9.4/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.4/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18838 2023-06-21 00:54:29.000000 ats_case-0.9.4/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12081 2023-06-21 00:54:29.000000 ats_case-0.9.4/ats_case/case/context.py
--rw-rw-rw-   0        0        0     8280 2023-06-21 01:24:47.000000 ats_case-0.9.4/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.4/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:25:47.532611 ats_case-0.9.4/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.4/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.4/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.4/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:25:47.691189 ats_case-0.9.4/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.4/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.4/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.4/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:25:47.726096 ats_case-0.9.4/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.4/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.4/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-21 01:25:47.356081 ats_case-0.9.4/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-21 01:25:46.000000 ats_case-0.9.4/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-21 01:25:46.000000 ats_case-0.9.4/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 01:25:46.000000 ats_case-0.9.4/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-21 01:25:46.000000 ats_case-0.9.4/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 01:25:46.000000 ats_case-0.9.4/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 01:25:47.743051 ats_case-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-21 01:25:18.000000 ats_case-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.301689 ats_case-0.9.5/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-21 07:30:39.297698 ats_case-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 07:30:38.927687 ats_case-0.9.5/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.5/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.129149 ats_case-0.9.5/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.5/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18838 2023-06-21 00:54:29.000000 ats_case-0.9.5/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12177 2023-06-21 07:23:49.000000 ats_case-0.9.5/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     8280 2023-06-21 01:24:47.000000 ats_case-0.9.5/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.5/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.186993 ats_case-0.9.5/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.5/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.5/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.5/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.243842 ats_case-0.9.5/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.5/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.5/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.5/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.285730 ats_case-0.9.5/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.5/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.5/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.015452 ats_case-0.9.5/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 07:30:39.301689 ats_case-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-21 07:24:38.000000 ats_case-0.9.5/setup.py
```

### Comparing `ats_case-0.9.4/PKG-INFO` & `ats_case-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.9.4
+Version: 0.9.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.4/README.md` & `ats_case-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case/case/command.py` & `ats_case-0.9.5/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case/case/context.py` & `ats_case-0.9.5/ats_case/case/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,14 +186,15 @@
         # @property
         # def code(self):
         #     return self._code
         #
         # @property
         # def version(self):
         #     return self._version
+
     #
     #     @property
     #     def scope(self):
     #         return self._scope
     #
     #     @property
     #     def purpose(self):
@@ -338,17 +339,18 @@
             for s, result in self.sas.items():
                 if str(result).find('不合格') >= 0:
                     fc += 1
                     fs.append(str(s))
                 else:
                     sc += 1
 
-            msg = '本用例共: {}步\r\n'.format(len(self._parent.case.steps))
-            msg += '执行合格: {}步\r\n'.format(sc)
-            msg += '执行不合格: {}步 ~ {}\r\n'.format(fc, ','.join(fs))
+            pattern = "{0:<11}\t{1:<6}\r\n"
+            msg = pattern.format('用例步骤:', '{}步'.format(len(self._parent.case.steps)))
+            msg += pattern.format('执行合格:', '{}步'.format(sc))
+            msg += pattern.format('执行不合格:', '{}步 ~ {}'.format(fc, ','.join(fs)))
 
             return msg
 
         @property
         def step(self):
             return self._step
 
@@ -417,7 +419,9 @@
             self._parent = parent
 
         def get(self, name: str, key: str):
             return mm.Dict.get('{}:{}'.format(self._parent.test_sn, name), key)
 
         def set(self, name: str, key: str, data):
             return mm.Dict.put('{}:{}'.format(self._parent.test_sn, name), key, data)
+
+
```

### Comparing `ats_case-0.9.4/ats_case/case/executor.py` & `ats_case-0.9.5/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case/case/translator.py` & `ats_case-0.9.5/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case/common/error.py` & `ats_case-0.9.5/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case/manage/core.py` & `ats_case-0.9.5/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case/manage/start.py` & `ats_case-0.9.5/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case/template/testcase_v1.tmp` & `ats_case-0.9.5/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/ats_case.egg-info/PKG-INFO` & `ats_case-0.9.5/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.9.4
+Version: 0.9.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.4/ats_case.egg-info/SOURCES.txt` & `ats_case-0.9.5/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.4/setup.py` & `ats_case-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.9.4",
+    version="0.9.5",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

