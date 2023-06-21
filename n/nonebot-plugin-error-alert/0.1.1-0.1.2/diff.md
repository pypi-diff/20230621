# Comparing `tmp/nonebot_plugin_error_alert-0.1.1.tar.gz` & `tmp/nonebot_plugin_error_alert-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_error_alert-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_error_alert-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_error_alert-0.1.1.tar` & `nonebot_plugin_error_alert-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2023-06-21 16:29:40.314045 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/__init__.py
--rw-r--r--   0        0        0     3394 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/alert.py
--rw-r--r--   0        0        0      273 2023-06-21 16:12:51.641013 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/config.py
--rw-r--r--   0        0        0     2009 2023-06-21 16:24:46.458536 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/matcher.py
--rw-r--r--   0        0        0     7985 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/subscribe.py
--rw-r--r--   0        0        0      526 2023-06-21 16:29:40.319046 nonebot_plugin_error_alert-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      652 2023-06-21 16:26:44.383665 nonebot_plugin_error_alert-0.1.1/README.md
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 nonebot_plugin_error_alert-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1160 2023-06-21 16:48:45.036908 nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/__init__.py
+-rw-r--r--   0        0        0     3394 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/alert.py
+-rw-r--r--   0        0        0      273 2023-06-21 16:12:51.641013 nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/config.py
+-rw-r--r--   0        0        0     2009 2023-06-21 16:24:46.458536 nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/matcher.py
+-rw-r--r--   0        0        0     7985 2023-06-19 15:56:09.064000 nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/subscribe.py
+-rw-r--r--   0        0        0      526 2023-06-21 16:48:10.461770 nonebot_plugin_error_alert-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      998 2023-06-21 16:48:10.457770 nonebot_plugin_error_alert-0.1.2/README.md
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 nonebot_plugin_error_alert-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/__init__.py` & `nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 from .config import Config
 
 __plugin_meta__ = PluginMetadata(
     name="错误告警",
     description="当Bot发生运行错误时发送消息提醒",
     usage="""
-/error_alert subscribe：订阅错误告警。发生错误时立即发送告警至本账号。
-/error_alert subscribe <cron>：订阅错误告警。但不会在发生错误时立即发送告警，而是在满足cron表达式的时间点统一发送该时间段发生的错误告警。
+/error_alert subscribe：订阅错误告警。发生错误时立即发送消息提醒至本账号。
+/error_alert subscribe --cron <cron>：订阅错误告警。但不会在发生错误时立即发送消息提醒，而是在满足cron表达式的时间点统一发送该时间段发生的错误告警。
 /error_alert unsubscribe：取消订阅错误告警。
+/error_alert show：查看本账号订阅的错误告警。
     """.strip(),
     homepage="https://github.com/bot-ssttkkl/nonebot-plugin-error-alert",
     type="application",
     config=Config,
     supported_adapters=nonebot_plugin_saa.__plugin_meta__.supported_adapters
 )
```

### Comparing `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/alert.py` & `nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/alert.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/matcher.py` & `nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_error_alert-0.1.1/nonebot_plugin_error_alert/subscribe.py` & `nonebot_plugin_error_alert-0.1.2/nonebot_plugin_error_alert/subscribe.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_error_alert-0.1.1/pyproject.toml` & `nonebot_plugin_error_alert-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-error-alert"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_error_alert"}]
 
 [tool.poetry.dependencies]
```

