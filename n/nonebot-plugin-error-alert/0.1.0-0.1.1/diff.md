# Comparing `tmp/nonebot_plugin_error_alert-0.1.0.tar.gz` & `tmp/nonebot_plugin_error_alert-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_error_alert-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_error_alert-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_error_alert-0.1.0.tar` & `nonebot_plugin_error_alert-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1054 2023-06-21 16:15:46.364062 nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/__init__.py
--rw-r--r--   0        0        0     3394 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/alert.py
--rw-r--r--   0        0        0      273 2023-06-21 16:12:51.641013 nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/config.py
--rw-r--r--   0        0        0     2009 2023-06-21 16:24:46.458536 nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/matcher.py
--rw-r--r--   0        0        0     7985 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/subscribe.py
--rw-r--r--   0        0        0      526 2023-06-21 16:21:54.796696 nonebot_plugin_error_alert-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      652 2023-06-21 16:16:57.822181 nonebot_plugin_error_alert-0.1.0/README.md
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 nonebot_plugin_error_alert-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-21 16:29:40.314045 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/__init__.py
+-rw-r--r--   0        0        0     3394 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/alert.py
+-rw-r--r--   0        0        0      273 2023-06-21 16:12:51.641013 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/config.py
+-rw-r--r--   0        0        0     2009 2023-06-21 16:24:46.458536 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/matcher.py
+-rw-r--r--   0        0        0     7985 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/subscribe.py
+-rw-r--r--   0        0        0      526 2023-06-21 16:29:40.319046 nonebot_plugin_error_alert-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      652 2023-06-21 16:26:44.383665 nonebot_plugin_error_alert-0.1.1/README.md
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 nonebot_plugin_error_alert-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/__init__.py` & `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,12 @@
     name="错误告警",
     description="当Bot发生运行错误时发送消息提醒",
     usage="""
 /error_alert subscribe：订阅错误告警。发生错误时立即发送告警至本账号。
 /error_alert subscribe <cron>：订阅错误告警。但不会在发生错误时立即发送告警，而是在满足cron表达式的时间点统一发送该时间段发生的错误告警。
 /error_alert unsubscribe：取消订阅错误告警。
     """.strip(),
-    homepage="https://github.com/bot-kuraku/nonebot-plugin-error-alert",
+    homepage="https://github.com/bot-ssttkkl/nonebot-plugin-error-alert",
+    type="application",
     config=Config,
     supported_adapters=nonebot_plugin_saa.__plugin_meta__.supported_adapters
 )
```

### Comparing `nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/alert.py` & `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/alert.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/matcher.py` & `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_error_alert-0.1.0/nonebot_plugin_error_alert/subscribe.py` & `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/subscribe.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_error_alert-0.1.0/pyproject.toml` & `nonebot_plugin_error_alert-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-error-alert"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_error_alert"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_error_alert-0.1.0/README.md` & `nonebot_plugin_error_alert-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 nonebot-plugin-error-alert
 ========
 
 当Bot发生运行错误时发送消息提醒
 
 ## 卖家秀
 
-![1](img/1.jpg)
+![1](img/1.png)
 
 ## 指令
 
 ### `/error_alert subscribe`
 
 订阅错误告警。发生错误时立即发送告警至本账号。
```

### Comparing `nonebot_plugin_error_alert-0.1.0/PKG-INFO` & `nonebot_plugin_error_alert-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-error-alert
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 nonebot-plugin-error-alert
 ========
 
 当Bot发生运行错误时发送消息提醒
 
 ## 卖家秀
 
-![1](img/1.jpg)
+![1](img/1.png)
 
 ## 指令
 
 ### `/error_alert subscribe`
 
 订阅错误告警。发生错误时立即发送告警至本账号。
```

