# Comparing `tmp/nonebot_plugin_session-0.0.4.tar.gz` & `tmp/nonebot_plugin_session-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_session-0.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_session-0.0.5.tar", max compression
```

## Comparing `nonebot_plugin_session-0.0.4.tar` & `nonebot_plugin_session-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/LICENSE
--rw-r--r--   0        0        0     4340 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/README.md
--rw-r--r--   0        0        0      161 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/__init__.py
--rw-r--r--   0        0        0       75 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/__init__.py
--rw-r--r--   0        0        0      585 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/console.py
--rw-r--r--   0        0        0     1190 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/kaiheila.py
--rw-r--r--   0        0        0     2719 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3537 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v12.py
--rw-r--r--   0        0        0     1565 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/qqguild.py
--rw-r--r--   0        0        0     2616 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/telegram.py
--rw-r--r--   0        0        0      398 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/const.py
--rw-r--r--   0        0        0     2700 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/extractor.py
--rw-r--r--   0        0        0     1525 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
--rw-r--r--   0        0        0     2814 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/model.py
--rw-r--r--   0        0        0     2207 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/saa.py
--rw-r--r--   0        0        0     2053 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/session.py
--rw-r--r--   0        0        0     1879 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4340 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/README.md
+-rw-r--r--   0        0        0      601 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/__init__.py
+-rw-r--r--   0        0        0      585 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/console.py
+-rw-r--r--   0        0        0     1190 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/kaiheila.py
+-rw-r--r--   0        0        0     2719 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3537 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     1565 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/qqguild.py
+-rw-r--r--   0        0        0     2616 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/telegram.py
+-rw-r--r--   0        0        0      398 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/const.py
+-rw-r--r--   0        0        0     2700 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/extractor.py
+-rw-r--r--   0        0        0     1525 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
+-rw-r--r--   0        0        0     2814 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/model.py
+-rw-r--r--   0        0        0     2207 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/saa.py
+-rw-r--r--   0        0        0     2053 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/session.py
+-rw-r--r--   0        0        0     1874 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5391 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_session-0.0.4/LICENSE` & `nonebot_plugin_session-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/README.md` & `nonebot_plugin_session-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/console.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/kaiheila.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v11.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v12.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/qqguild.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/telegram.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/extractor.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/extractor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/migrations/36de70108aeb_init_db.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/migrations/36de70108aeb_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/model.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/saa.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/saa.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/nonebot_plugin_session/session.py` & `nonebot_plugin_session-0.0.5/nonebot_plugin_session/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.4/pyproject.toml` & `nonebot_plugin_session-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "nonebot_plugin_session"
-version = "0.0.4"
+version = "0.0.5"
 description = "Nonebot2 会话信息提取与会话id定义"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-session"
 repository = "https://github.com/noneplugin/nonebot-plugin-session"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
 strenum = "^0.4.8"
-nonebot-plugin-datastore = { version = "^0.6.3", optional = true }
-nonebot-plugin-send-anything-anywhere = { version = "^0.2.4", optional = true }
+nonebot-plugin-datastore = { version = "^1.0.0", optional = true }
+nonebot-plugin-send-anything-anywhere = { version = "^0.2.7", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.20.0"
@@ -27,15 +27,15 @@
 optional = true
 
 [tool.poetry.group.adapters.dependencies]
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-adapter-console = "^0.3.2"
 nonebot-adapter-qqguild = "^0.2.1"
 nonebot-adapter-kaiheila = { version = "^0.2.4", python = ">=3.9" }
-nonebot-adapter-telegram = "^0.1.0b10"
+nonebot-adapter-telegram = "^0.1.0b13"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_session"]
 adapters = [
   { name = "Console", module_name = "nonebot.adapters.console" },
   { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
   { name = "OneBot V12", module_name = "nonebot.adapters.onebot.v12" },
```

### Comparing `nonebot_plugin_session-0.0.4/PKG-INFO` & `nonebot_plugin_session-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-session
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nonebot2 会话信息提取与会话id定义
 Home-page: https://github.com/noneplugin/nonebot-plugin-session
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: datastore
 Provides-Extra: saa
-Requires-Dist: nonebot-plugin-datastore (>=0.6.3,<0.7.0) ; extra == "datastore" or extra == "all"
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4,<0.3.0) ; extra == "saa" or extra == "all"
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot-plugin-datastore (>=1.0.0,<2.0.0) ; extra == "datastore" or extra == "all"
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0) ; extra == "saa" or extra == "all"
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Requires-Dist: strenum (>=0.4.8,<0.5.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-session
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   <a href="https://v2.nonebot.dev/">
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.5 Summary:
 Nonebot2 ä¼è¯ä¿¡æ¯æåä¸ä¼è¯idå®ä¹ Home-page: https://github.com/
 noneplugin/nonebot-plugin-session License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
 Provides-Extra: datastore Provides-Extra: saa Requires-Dist: nonebot-plugin-
-datastore (>=0.6.3,<0.7.0) ; extra == "datastore" or extra == "all" Requires-
-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4,<0.3.0) ; extra == "saa"
-or extra == "all" Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
-Requires-Dist: strenum (>=0.4.8,<0.5.0) Project-URL: Repository, https://
-github.com/noneplugin/nonebot-plugin-session Description-Content-Type: text/
-markdown
+datastore (>=1.0.0,<2.0.0) ; extra == "datastore" or extra == "all" Requires-
+Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0) ; extra == "saa"
+or extra == "all" Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Requires-
+Dist: strenum (>=0.4.8,<0.5.0) Project-URL: Repository, https://github.com/
+noneplugin/nonebot-plugin-session Description-Content-Type: text/markdown
 [nonebot] # nonebot-plugin-session _â¨ [Nonebot2](https://github.com/nonebot/
           nonebot2) ä¼è¯ä¿¡æ¯æåä¸ä¼è¯ id å®ä¹æä»¶ â¨_
                       [license] [Python] [NoneBot] [pypi]
 - è¿ä¸ªæä»¶å¯ä»¥åä»ä¹ï¼ æ¬æä»¶æä¾äºä¸ä¸ªç»ä¸çä¼è¯æ¨¡å
 `Session`ï¼ å¯ä»¥ä»ä¸åééå¨ç `Bot` å `Event`
 ä¸­æåä¸ä¼è¯ç¸å³ç
 âå¹³å°âãâä¼è¯ç­çº§âï¼åç¨æ·ãåçº§ç¾¤ç»ãä¸¤çº§ç¾¤ç»ï¼ãâç®æ 
```

