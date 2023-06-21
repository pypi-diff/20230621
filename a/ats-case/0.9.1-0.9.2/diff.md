# Comparing `tmp/ats_case-0.9.1.tar.gz` & `tmp/ats_case-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.9.1.tar", last modified: Tue Jun 20 08:45:08 2023, max compression
+gzip compressed data, was "ats_case-0.9.2.tar", last modified: Wed Jun 21 00:57:14 2023, max compression
```

## Comparing `ats_case-0.9.1.tar` & `ats_case-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.246277 ats_case-0.9.1/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.1/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-20 08:45:08.244275 ats_case-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 08:45:07.880602 ats_case-0.9.1/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.1/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.073093 ats_case-0.9.1/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.1/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18857 2023-06-19 03:05:41.000000 ats_case-0.9.1/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12148 2023-06-20 07:39:55.000000 ats_case-0.9.1/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7868 2023-06-20 08:44:47.000000 ats_case-0.9.1/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.1/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.134895 ats_case-0.9.1/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.1/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.1/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.1/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.193738 ats_case-0.9.1/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.1/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.1/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.1/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.225685 ats_case-0.9.1/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.1/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.9.1/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-20 08:45:07.968376 ats_case-0.9.1/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 08:45:08.246277 ats_case-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-20 08:44:54.000000 ats_case-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:57:14.383060 ats_case-0.9.2/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-21 00:57:14.381066 ats_case-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 00:57:13.989560 ats_case-0.9.2/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.2/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:57:14.203214 ats_case-0.9.2/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.2/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18838 2023-06-21 00:54:29.000000 ats_case-0.9.2/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12081 2023-06-21 00:54:29.000000 ats_case-0.9.2/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7868 2023-06-20 08:44:47.000000 ats_case-0.9.2/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.2/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:57:14.274347 ats_case-0.9.2/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.2/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.2/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.2/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:57:14.335187 ats_case-0.9.2/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.2/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.2/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.2/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:57:14.372089 ats_case-0.9.2/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.2/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.2/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-21 00:57:14.082179 ats_case-0.9.2/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-21 00:57:13.000000 ats_case-0.9.2/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-21 00:57:13.000000 ats_case-0.9.2/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 00:57:13.000000 ats_case-0.9.2/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-21 00:57:13.000000 ats_case-0.9.2/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 00:57:13.000000 ats_case-0.9.2/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 00:57:14.384058 ats_case-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-21 00:54:43.000000 ats_case-0.9.2/setup.py
```

### Comparing `ats_case-0.9.1/PKG-INFO` & `ats_case-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.9.1
+Version: 0.9.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.1/README.md` & `ats_case-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.1/ats_case/case/command.py` & `ats_case-0.9.2/ats_case/case/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -261,40 +261,40 @@
 
         if index == 0:
             self._parse = context.runtime.final_result
             self._flush(context)
             return self._parse
 
     def _flush(self, context: Context):
-        context.runtime.steps.update({context.runtime.step: func.to_dict(obj='meter', op=self._operation
+        context.runtime.sos.update({context.runtime.step: func.to_dict(obj='meter', op=self._operation
                                                                          , element=self._element
                                                                          , parameter=self._parameter,
                                                                          result=self._parse)})
 
     def acv(self, context: Context):
         result = str(self._parse)
         if self._func is not None:
             if type(self._func_parameter) is dict:
                 self._func_parameter = _replace(context, self._func_parameter)
             try:
                 if self._expect_result is None:
-                    expect_result = context.runtime.steps[context.runtime.step - 1]
+                    expect_result = context.runtime.sos[context.runtime.step - 1]
                 else:
-                    expect_result = context.runtime.steps[int(self._expect_result)]
+                    expect_result = context.runtime.sos[int(self._expect_result)]
             except:
                 expect_result = None
             data = func.to_dict(result=self._parse, expect_result=expect_result, parameter=self._func_parameter)
 
             logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
                 self._func_module, self._func, self._func_parameter))
             result = udm.handle(module='meter.{}'.format(self._func_module), function=self._func
                                 , data=data, debug_url=context.acd_url)
             logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._func_module, self._func, result))
 
-            context.runtime.acvs[context.runtime.step] = result
+            context.runtime.sas[context.runtime.step] = result
 
         return result
 
     def exec(self, context: Context):
         self.encode(context)
         result = send(context,
                       todo={'meter:comm': {'channel': context.case.steps[str(context.runtime.step)].get('channel'),
@@ -329,40 +329,40 @@
         self._parameter = param
         return self
 
     def handle(self, context: Context):
         try:
             if self._parameter is None:
                 self._parameter = {}
-            self._parameter = context.runtime.steps[context.runtime.step - 1]['result']
+            self._parameter = context.runtime.sos[context.runtime.step - 1]['result']
             self._parameter['session_key'] = context.test_sn
         except:
             pass
 
         logger.info(
             '~ @EM-> protocol:{} operation:{} parameter:{}'.format(self._protocol, self._operation, self._parameter))
         self._result = em.handle(self._protocol.name, self._operation, self._parameter)
         logger.info('~ @EM<- protocol:{} operation:{} result:{}'.format(self._protocol, self._operation, self._result))
         self._flush(context)
 
     def _flush(self, context: Context):
-        context.runtime.steps.update({context.runtime.step: func.to_dict(obj='em', op=self._operation
+        context.runtime.sos.update({context.runtime.step: func.to_dict(obj='em', op=self._operation
                                                                          , parameter=self._parameter,
                                                                          result=self._result)})
 
     def acv(self, context: Context):
         data = func.to_dict(result=self._result)
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             self._protocol.name, self._operation, self._parameter))
         result = udm.handle(module='em.{}'.format(self._protocol.name), function=self._operation
                             , data=data, debug_url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._protocol.name, self._operation, result))
 
-        context.runtime.acvs[context.runtime.step] = result
+        context.runtime.sas[context.runtime.step] = result
 
         return result
 
     def exec(self, context: Context):
         self.handle(context)
         send(context, todo={'app:show': {'msg': self.acv(context)}})
 
@@ -445,30 +445,30 @@
         result = str(self._result)
         data = func.to_dict(result=self._result)
         if self._func is not None:
             if type(self._func_parameter) is dict:
                 data['parameter'] = _replace_bench0(context, self._func_parameter)
             try:
                 if self._expect_result is None:
-                    data['expect_result'] = context.runtime.steps[context.runtime.step - 1]
+                    data['expect_result'] = context.runtime.sos[context.runtime.step - 1]
                 else:
-                    data['expect_result'] = context.runtime.steps[int(self._expect_result)]
+                    data['expect_result'] = context.runtime.sos[int(self._expect_result)]
             except:
                 pass
 
             logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format('bench', self._func, data['parameter']))
             result = udm.handle(module='bench', function=self._func, data=data, debug_url=context.acd_url)
             logger.info('~ @ACD<- module:{} function:{} result:{}'.format('bench', self._func, result))
 
-            context.runtime.acvs[context.runtime.step] = result
+            context.runtime.sas[context.runtime.step] = result
 
         return result
 
     def _flush(self, context: Context):
-        context.runtime.steps.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
+        context.runtime.sos.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
                                                                          , parameter=self._parameter,
                                                                          result=self._result)})
 
     def rest(self, context: Context):
         if self._result == '1' and self._sleep > 0:
             send(context, todo={'app:show': {'msg': '系统休眠{}秒, 等待表台调整完毕...'.format(self._sleep)}})
             sleep(self._sleep)
```

### Comparing `ats_case-0.9.1/ats_case/case/context.py` & `ats_case-0.9.2/ats_case/case/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,25 +321,25 @@
             self._parent = parent
             self._step = -1
             self._loop_sn = 0
             self._loop_start_step = 0
             self._loop_end_step = 0
             self._loop_count = 0
             self._loop_index = 0
-            # 解帧结果
-            self._steps = {}
+            # 步骤操作返回结果集
+            self._sos = {}
+            # 步骤对比返回结果集 - 用例结束时统计执行结果
+            self._sas = {}
             # 多帧时使用
             self._final_result = None
-            # 对比结果 - 用例结束时统计执行结果
-            self._acvs = {}
 
-        def acv_result(self):
+        def test_report(self):
             sc = fc = 0
             fs = []
-            for s, result in self.acvs.items():
+            for s, result in self.sas.items():
                 if str(result).find('不合格') >= 0:
                     fc += 1
                     fs.append(str(s))
                 else:
                     sc += 1
 
             msg = '本用例共: {}步\r\n'.format(len(self._parent.case.steps))
@@ -393,33 +393,29 @@
             return self._loop_index
 
         @loop_index.setter
         def loop_index(self, value):
             self._loop_index = value
 
         @property
-        def steps(self):
-            return self._steps
+        def sos(self):
+            return self._sos
+
+        @property
+        def sas(self):
+            return self._sas
 
         @property
         def final_result(self):
             return self._final_result
 
         @final_result.setter
         def final_result(self, value):
             self._final_result = value
 
-        @property
-        def acvs(self):
-            return self._acvs
-
-        @acvs.setter
-        def acvs(self, value):
-            self._acvs = value
-
     class Session(object):
         def __init__(self, parent):
             self._parent = parent
 
         def get(self, name: str, key: str):
             return mm.Dict.get('{}:{}'.format(self._parent.test_sn, name), key)
```

### Comparing `ats_case-0.9.1/ats_case/case/executor.py` & `ats_case-0.9.2/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.1/ats_case/case/translator.py` & `ats_case-0.9.2/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.1/ats_case/common/error.py` & `ats_case-0.9.2/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.1/ats_case/manage/core.py` & `ats_case-0.9.2/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.1/ats_case/manage/start.py` & `ats_case-0.9.2/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.1/ats_case/template/testcase_v1.tmp` & `ats_case-0.9.2/ats_case/template/testcase_v1.tmp`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         :return:
         """
         try:
             msg = '[{}]测试结束 - 测试用例[{}], 电表[{}].\r\n'.format(func.sys_current_time(),
                                                               CaseContext.case.name,
                                                               CaseContext.meter.no)
             msg += '--------------------测试报告--------------------\r\n'
-            msg += CaseContext.runtime.acv_result()
+            msg += CaseContext.runtime.test_report()
             command.client().message(msg).show(CaseContext, types=1)
         except APIError as ae:
             logger.info(str(ae))
             raise AssertionError(str(ae))
 
         logger.info('~ @TCC-MSG-> TEST CASE[{}-{}] METER[{}] END.'.format(CaseContext.case.id,
                                                                           CaseContext.case.name,
```

### Comparing `ats_case-0.9.1/ats_case.egg-info/PKG-INFO` & `ats_case-0.9.2/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.9.1
+Version: 0.9.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.1/ats_case.egg-info/SOURCES.txt` & `ats_case-0.9.2/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.1/setup.py` & `ats_case-0.9.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.9.1",
+    version="0.9.2",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

