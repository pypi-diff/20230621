# Comparing `tmp/nonebot_plugin_oddtext-0.1.2.tar.gz` & `tmp/nonebot_plugin_oddtext-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_oddtext-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_oddtext-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_oddtext-0.1.2.tar` & `nonebot_plugin_oddtext-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-02-01 02:44:52.560480 nonebot_plugin_oddtext-0.1.2/LICENSE
--rw-r--r--   0        0        0     1814 2023-02-01 02:44:52.560480 nonebot_plugin_oddtext-0.1.2/README.md
--rw-r--r--   0        0        0     1525 2023-02-01 02:44:52.564480 nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/__init__.py
--rw-r--r--   0        0        0     3112 2023-02-01 02:44:52.564480 nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/bug.py
--rw-r--r--   0        0        0   508009 2023-02-01 02:44:52.564480 nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/cxh.py
--rw-r--r--   0        0        0     4369 2023-02-01 02:44:52.564480 nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/data_source.py
--rw-r--r--   0        0        0      788 2023-02-01 02:44:52.564480 nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/flip.py
--rw-r--r--   0        0        0    34299 2023-02-01 02:44:52.564480 nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/hxw.py
--rw-r--r--   0        0        0      609 2023-02-01 02:44:52.564480 nonebot_plugin_oddtext-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 nonebot_plugin_oddtext-0.1.2/setup.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 nonebot_plugin_oddtext-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 14:35:05.600801 nonebot_plugin_oddtext-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1814 2023-06-21 14:35:05.600801 nonebot_plugin_oddtext-0.2.0/README.md
+-rw-r--r--   0        0        0     1650 2023-06-21 14:35:05.600801 nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/__init__.py
+-rw-r--r--   0        0        0     3112 2023-06-21 14:35:05.600801 nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/bug.py
+-rw-r--r--   0        0        0   508009 2023-06-21 14:35:05.604801 nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/cxh.py
+-rw-r--r--   0        0        0     4367 2023-06-21 14:35:05.604801 nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/data_source.py
+-rw-r--r--   0        0        0      788 2023-06-21 14:35:05.604801 nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/flip.py
+-rw-r--r--   0        0        0    34299 2023-06-21 14:35:05.604801 nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/hxw.py
+-rw-r--r--   0        0        0      604 2023-06-21 14:35:05.604801 nonebot_plugin_oddtext-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 nonebot_plugin_oddtext-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_oddtext-0.1.2/LICENSE` & `nonebot_plugin_oddtext-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_oddtext-0.1.2/README.md` & `nonebot_plugin_oddtext-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/__init__.py` & `nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import traceback
+
 from nonebot import on_command
+from nonebot.adapters import Message
 from nonebot.log import logger
 from nonebot.matcher import Matcher
-from nonebot.adapters import Message
-from nonebot.typing import T_Handler
 from nonebot.params import CommandArg
 from nonebot.plugin import PluginMetadata
+from nonebot.typing import T_Handler
 
-from .data_source import commands, Command
-
+from .data_source import Command, commands
 
 __plugin_meta__ = PluginMetadata(
     name="文本生成器",
     description="抽象话等多种文本生成",
     usage=f"{'/'.join(sum([list(command.keywords) for command in commands], []))} + 文本",
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-oddtext",
+    supported_adapters=None,
     extra={
         "unique_name": "oddtext",
         "example": "抽象话 那真的牛逼",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.1.1",
+        "version": "0.2.0",
     },
 )
 
 
 def create_matchers():
     def create_handler(command: Command) -> T_Handler:
         async def handler(matcher: Matcher, msg: Message = CommandArg()):
```

### Comparing `nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/bug.py` & `nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/bug.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/cxh.py` & `nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/cxh.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/data_source.py` & `nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import math
 import random
-
 from dataclasses import dataclass
-from typing import Tuple, Protocol
+from typing import Protocol, Tuple
 
-from .flip import flip_table
-from .cxh import emoji, pinyin
 from .bug import bug_code, bug_level
-from .hxw import enchars, encharhxw, ftw, hxw, jtw
+from .cxh import emoji, pinyin
+from .flip import flip_table
+from .hxw import encharhxw, enchars, ftw, hxw, jtw
 
 
 def cxh_text(text: str) -> str:
     def get_pinyin(s):
         if s in pinyin:
             return pinyin[s]
         return ""
```

### Comparing `nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/flip.py` & `nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/flip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_oddtext-0.1.2/nonebot_plugin_oddtext/hxw.py` & `nonebot_plugin_oddtext-0.2.0/nonebot_plugin_oddtext/hxw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_oddtext-0.1.2/pyproject.toml` & `nonebot_plugin_oddtext-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "nonebot_plugin_oddtext"
-version = "0.1.2"
+version = "0.2.0"
 description = "Nonebot2 插件，用于抽象话等文本生成"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-oddtext"
 repository = "https://github.com/noneplugin/nonebot-plugin-oddtext"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
 rcnb = "^1.0.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_oddtext-0.1.2/PKG-INFO` & `nonebot_plugin_oddtext-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-oddtext
-Version: 0.1.2
+Version: 0.2.0
 Summary: Nonebot2 插件，用于抽象话等文本生成
 Home-page: https://github.com/noneplugin/nonebot-plugin-oddtext
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
 Requires-Dist: rcnb (>=1.0.3,<2.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-oddtext
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-oddtext
 
 [Nonebot2](https://github.com/nonebot/nonebot2) 插件，用于抽象话等文本生成
```

