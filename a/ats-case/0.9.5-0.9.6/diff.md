# Comparing `tmp/ats_case-0.9.5.tar.gz` & `tmp/ats_case-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.9.5.tar", last modified: Wed Jun 21 07:30:39 2023, max compression
+gzip compressed data, was "ats_case-0.9.6.tar", last modified: Wed Jun 21 09:08:19 2023, max compression
```

## Comparing `ats_case-0.9.5.tar` & `ats_case-0.9.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.301689 ats_case-0.9.5/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-21 07:30:39.297698 ats_case-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 07:30:38.927687 ats_case-0.9.5/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.5/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.129149 ats_case-0.9.5/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.5/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18838 2023-06-21 00:54:29.000000 ats_case-0.9.5/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12177 2023-06-21 07:23:49.000000 ats_case-0.9.5/ats_case/case/context.py
--rw-rw-rw-   0        0        0     8280 2023-06-21 01:24:47.000000 ats_case-0.9.5/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.5/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.186993 ats_case-0.9.5/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.5/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.5/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.5/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.243842 ats_case-0.9.5/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.5/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.5/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.5/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.285730 ats_case-0.9.5/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.5/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.5/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-21 07:30:39.015452 ats_case-0.9.5/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 07:30:38.000000 ats_case-0.9.5/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 07:30:39.301689 ats_case-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-21 07:24:38.000000 ats_case-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 09:08:19.867433 ats_case-0.9.6/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-21 09:08:19.864441 ats_case-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 09:08:19.415331 ats_case-0.9.6/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.6/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 09:08:19.620794 ats_case-0.9.6/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.6/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18838 2023-06-21 00:54:29.000000 ats_case-0.9.6/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12477 2023-06-21 09:07:37.000000 ats_case-0.9.6/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     8314 2023-06-21 09:01:59.000000 ats_case-0.9.6/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.6/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-21 09:08:19.684613 ats_case-0.9.6/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.6/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.6/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.6/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-21 09:08:19.773683 ats_case-0.9.6/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.6/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.6/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.6/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-21 09:08:19.825545 ats_case-0.9.6/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.6/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.6/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-21 09:08:19.510079 ats_case-0.9.6/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-21 09:08:18.000000 ats_case-0.9.6/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-21 09:08:19.000000 ats_case-0.9.6/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 09:08:18.000000 ats_case-0.9.6/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-21 09:08:18.000000 ats_case-0.9.6/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 09:08:18.000000 ats_case-0.9.6/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 09:08:19.867433 ats_case-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-21 09:07:45.000000 ats_case-0.9.6/setup.py
```

### Comparing `ats_case-0.9.5/PKG-INFO` & `ats_case-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.9.5
+Version: 0.9.6
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.5/README.md` & `ats_case-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/ats_case/case/command.py` & `ats_case-0.9.6/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/ats_case/case/context.py` & `ats_case-0.9.6/ats_case/case/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -332,25 +332,31 @@
             self._sas = {}
             # 多帧时使用
             self._final_result = None
 
         def test_report(self):
             sc = fc = 0
             fs = []
+            error = False
             for s, result in self.sas.items():
                 if str(result).find('不合格') >= 0:
                     fc += 1
                     fs.append(str(s))
+                elif str(result).find('程序异常') >= 0:
+                    error = True
                 else:
                     sc += 1
 
             pattern = "{0:<11}\t{1:<6}\r\n"
-            msg = pattern.format('用例步骤:', '{}步'.format(len(self._parent.case.steps)))
-            msg += pattern.format('执行合格:', '{}步'.format(sc))
-            msg += pattern.format('执行不合格:', '{}步 ~ {}'.format(fc, ','.join(fs)))
+            if error:
+                msg = pattern.format('系统错误:', '第{}步, 程序出错导致用例异常退出'.format(self._step))
+            else:
+                msg = pattern.format('用例步骤:', '{}步'.format(len(self._parent.case.steps)))
+                msg += pattern.format('执行合格:', '{}步'.format(sc))
+                msg += pattern.format('执行不合格:', '{}步 ~ {}'.format(fc, ','.join(fs)))
 
             return msg
 
         @property
         def step(self):
             return self._step
```

### Comparing `ats_case-0.9.5/ats_case/case/executor.py` & `ats_case-0.9.6/ats_case/case/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,18 @@
         if self.is_exec():
             try:
                 getattr(self._model, 'step_{}'.format(self._context.runtime.step))(self._context)
             except APIError as ae:
                 logger.info(str(ae))
                 raise AssertionError(str(ae))
             except Exception as e:
-                self._context.runtime.sas[self._context.runtime.step] = '结论: 不合格 - 程序异常'
+                self._context.runtime.sas[self._context.runtime.step] = '结论: 程序异常'
                 logger.error(str(e))
                 command.client().message(str(e)).error(self._context)
+                raise AssertionError(str(e))
 
     def loop_meet(self):
         loops = self._context.case.control.get('loops')
 
         if loops is None or type(loops) is not list or len(loops) <= 0:
             return False
```

### Comparing `ats_case-0.9.5/ats_case/case/translator.py` & `ats_case-0.9.6/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/ats_case/common/error.py` & `ats_case-0.9.6/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/ats_case/manage/core.py` & `ats_case-0.9.6/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/ats_case/manage/start.py` & `ats_case-0.9.6/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/ats_case/template/testcase_v1.tmp` & `ats_case-0.9.6/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/ats_case.egg-info/PKG-INFO` & `ats_case-0.9.6/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.9.5
+Version: 0.9.6
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.5/ats_case.egg-info/SOURCES.txt` & `ats_case-0.9.6/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.5/setup.py` & `ats_case-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.9.5",
+    version="0.9.6",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

