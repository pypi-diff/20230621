# Comparing `tmp/nonebot_plugin_emojimix-0.2.0.tar.gz` & `tmp/nonebot_plugin_emojimix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_emojimix-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_emojimix-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_emojimix-0.2.0.tar` & `nonebot_plugin_emojimix-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-01-28 05:16:55.714118 nonebot_plugin_emojimix-0.2.0/LICENSE
--rw-r--r--   0        0        0      485 2023-01-28 05:16:55.714118 nonebot_plugin_emojimix-0.2.0/README.md
--rw-r--r--   0        0        0     1680 2023-01-28 05:16:55.714118 nonebot_plugin_emojimix-0.2.0/nonebot_plugin_emojimix/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 05:16:55.714118 nonebot_plugin_emojimix-0.2.0/nonebot_plugin_emojimix/config.py
--rw-r--r--   0        0        0     1728 2023-01-28 05:16:55.714118 nonebot_plugin_emojimix-0.2.0/nonebot_plugin_emojimix/data_source.py
--rw-r--r--   0        0        0    11938 2023-01-28 05:16:55.714118 nonebot_plugin_emojimix-0.2.0/nonebot_plugin_emojimix/emoji_data.py
--rw-r--r--   0        0        0      646 2023-01-28 05:16:55.714118 nonebot_plugin_emojimix-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 nonebot_plugin_emojimix-0.2.0/setup.py
--rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 nonebot_plugin_emojimix-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 15:09:56.287390 nonebot_plugin_emojimix-0.3.0/LICENSE
+-rw-r--r--   0        0        0      485 2023-06-21 15:09:56.287390 nonebot_plugin_emojimix-0.3.0/README.md
+-rw-r--r--   0        0        0     1967 2023-06-21 15:09:56.287390 nonebot_plugin_emojimix-0.3.0/nonebot_plugin_emojimix/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-21 15:09:56.287390 nonebot_plugin_emojimix-0.3.0/nonebot_plugin_emojimix/config.py
+-rw-r--r--   0        0        0     1726 2023-06-21 15:09:56.287390 nonebot_plugin_emojimix-0.3.0/nonebot_plugin_emojimix/data_source.py
+-rw-r--r--   0        0        0    11938 2023-06-21 15:09:56.287390 nonebot_plugin_emojimix-0.3.0/nonebot_plugin_emojimix/emoji_data.py
+-rw-r--r--   0        0        0      663 2023-06-21 15:09:56.291390 nonebot_plugin_emojimix-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1361 1970-01-01 00:00:00.000000 nonebot_plugin_emojimix-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_emojimix-0.2.0/LICENSE` & `nonebot_plugin_emojimix-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_emojimix-0.2.0/nonebot_plugin_emojimix/data_source.py` & `nonebot_plugin_emojimix-0.3.0/nonebot_plugin_emojimix/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import httpx
 import traceback
-from typing import List, Union, Optional
+from typing import List, Optional, Union
 
+import httpx
 from nonebot import get_driver
 from nonebot.log import logger
 
 from .config import Config
-from .emoji_data import emojis, dates
-
+from .emoji_data import dates, emojis
 
 emoji_config = Config.parse_obj(get_driver().config.dict())
 
 API = "https://www.gstatic.com/android/keyboard/emojikitchen/"
 
 
 def create_url(date: str, emoji1: List[int], emoji2: List[int]) -> str:
```

### Comparing `nonebot_plugin_emojimix-0.2.0/nonebot_plugin_emojimix/emoji_data.py` & `nonebot_plugin_emojimix-0.3.0/nonebot_plugin_emojimix/emoji_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_emojimix-0.2.0/pyproject.toml` & `nonebot_plugin_emojimix-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot_plugin_emojimix"
-version = "0.2.0"
+version = "0.3.0"
 description = "Nonebot2 plugin for emojimix"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-emojimix"
 repository = "https://github.com/noneplugin/nonebot-plugin-emojimix"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.0"
-httpx = ">=0.19.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
+httpx = ">=0.19.0,<1.0.0"
 emoji = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_emojimix-0.2.0/PKG-INFO` & `nonebot_plugin_emojimix-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-emojimix
-Version: 0.2.0
+Version: 0.3.0
 Summary: Nonebot2 plugin for emojimix
 Home-page: https://github.com/noneplugin/nonebot-plugin-emojimix
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
 Requires-Dist: emoji (>=2.0.0,<3.0.0)
-Requires-Dist: httpx (>=0.19.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: httpx (>=0.19.0,<1.0.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-emojimix
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-emojimix
 
 适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的 emoji 合成器
```

