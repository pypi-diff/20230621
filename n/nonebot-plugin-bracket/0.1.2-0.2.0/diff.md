# Comparing `tmp/nonebot_plugin_bracket-0.1.2.tar.gz` & `tmp/nonebot_plugin_bracket-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bracket-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_bracket-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_bracket-0.1.2.tar` & `nonebot_plugin_bracket-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2023-03-26 13:44:52.635315 nonebot_plugin_bracket-0.1.2/LICENSE
--rw-r--r--   0        0        0      357 2023-03-26 13:44:52.635315 nonebot_plugin_bracket-0.1.2/README.md
--rw-r--r--   0        0        0     1727 2023-03-26 13:44:52.635315 nonebot_plugin_bracket-0.1.2/nonebot_plugin_bracket/__init__.py
--rw-r--r--   0        0        0      450 2023-03-26 13:44:52.635315 nonebot_plugin_bracket-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 nonebot_plugin_bracket-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 14:51:42.121688 nonebot_plugin_bracket-0.2.0/LICENSE
+-rw-r--r--   0        0        0      357 2023-06-21 14:51:42.121688 nonebot_plugin_bracket-0.2.0/README.md
+-rw-r--r--   0        0        0     1849 2023-06-21 14:51:42.121688 nonebot_plugin_bracket-0.2.0/nonebot_plugin_bracket/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-21 14:51:42.121688 nonebot_plugin_bracket-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 nonebot_plugin_bracket-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_bracket-0.1.2/LICENSE` & `nonebot_plugin_bracket-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bracket-0.1.2/nonebot_plugin_bracket/__init__.py` & `nonebot_plugin_bracket-0.2.0/nonebot_plugin_bracket/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from nonebot.plugin import PluginMetadata
 from nonebot.typing import T_State
 
 __plugin_meta__ = PluginMetadata(
     name="括号补全",
     description="补全消息中的括号，治愈强迫症",
     usage="发送带括号的消息即可",
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-bracket",
+    supported_adapters=None,
     extra={
         "unique_name": "bracket",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.1.2",
+        "version": "0.2.0",
     },
 )
 
 bracket_pairs = {
     "(": ")",
     "（": "）",
     "[": "]",
```

### Comparing `nonebot_plugin_bracket-0.1.2/PKG-INFO` & `nonebot_plugin_bracket-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bracket
-Version: 0.1.2
+Version: 0.2.0
 Summary: Nonebot2 插件，用于补全左括号
+Home-page: https://github.com/noneplugin/nonebot-plugin-bracket
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-bracket
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-bracket
 
 [Nonebot2](https://github.com/nonebot/nonebot2) 插件，用于补全消息中的括号，治愈强迫症
```

