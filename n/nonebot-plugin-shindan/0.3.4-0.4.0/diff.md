# Comparing `tmp/nonebot_plugin_shindan-0.3.4.tar.gz` & `tmp/nonebot_plugin_shindan-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_shindan-0.3.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_shindan-0.4.0.tar", max compression
```

## Comparing `nonebot_plugin_shindan-0.3.4.tar` & `nonebot_plugin_shindan-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/LICENSE
--rw-r--r--   0        0        0     1746 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/README.md
--rw-r--r--   0        0        0     8442 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/__init__.py
--rw-r--r--   0        0        0      119 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/config.py
--rw-r--r--   0        0        0     2374 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/manager.py
--rw-r--r--   0        0        0     3393 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
--rw-r--r--   0        0        0      530 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/model.py
--rw-r--r--   0        0        0     4707 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/shindanmaker.py
--rw-r--r--   0        0        0   180778 2023-05-10 02:37:27.587660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.css
--rw-r--r--   0        0        0   247324 2023-05-10 02:37:27.587660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.js
--rw-r--r--   0        0        0   477118 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/chart.js
--rw-r--r--   0        0        0      339 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/shindan.html
--rw-r--r--   0        0        0     1965 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/shindan_list.html
--rw-r--r--   0        0        0      843 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1746 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/README.md
+-rw-r--r--   0        0        0     6835 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/__init__.py
+-rw-r--r--   0        0        0      119 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/config.py
+-rw-r--r--   0        0        0     2374 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/manager.py
+-rw-r--r--   0        0        0     3393 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
+-rw-r--r--   0        0        0      530 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/model.py
+-rw-r--r--   0        0        0     2919 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/onebot.py
+-rw-r--r--   0        0        0     4707 2023-06-21 10:52:43.930493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/shindanmaker.py
+-rw-r--r--   0        0        0   180778 2023-06-21 10:52:43.934493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/app.css
+-rw-r--r--   0        0        0   247324 2023-06-21 10:52:43.934493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/app.js
+-rw-r--r--   0        0        0   477118 2023-06-21 10:52:43.938493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/chart.js
+-rw-r--r--   0        0        0      339 2023-06-21 10:52:43.938493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/shindan.html
+-rw-r--r--   0        0        0     1965 2023-06-21 10:52:43.938493 nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/shindan_list.html
+-rw-r--r--   0        0        0      980 2023-06-21 10:52:43.938493 nonebot_plugin_shindan-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_shindan-0.3.4/LICENSE` & `nonebot_plugin_shindan-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/README.md` & `nonebot_plugin_shindan-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/__init__.py` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import re
 import traceback
-from typing import List, Union
+from typing import List, Optional, Union
 
 from nonebot import on_command, on_message, require
-from nonebot.adapters.onebot.v11 import Bot as V11Bot
-from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
-from nonebot.adapters.onebot.v11 import Message as V11Msg
-from nonebot.adapters.onebot.v11 import MessageEvent as V11MEvent
-from nonebot.adapters.onebot.v11 import MessageSegment as V11MsgSeg
-from nonebot.adapters.onebot.v12 import Bot as V12Bot
-from nonebot.adapters.onebot.v12 import Message as V12Msg
-from nonebot.adapters.onebot.v12 import MessageEvent as V12MEvent
-from nonebot.adapters.onebot.v12 import MessageSegment as V12MsgSeg
+from nonebot.adapters import Bot, Event, Message
 from nonebot.log import logger
+from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, EventMessage, EventPlainText
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
 from nonebot.rule import Rule, to_me
 from nonebot.typing import T_State
 
 require("nonebot_plugin_datastore")
 require("nonebot_plugin_htmlrender")
+require("nonebot_plugin_saa")
 
 from nonebot_plugin_datastore.db import post_db_init
+from nonebot_plugin_saa import Image, MessageFactory
+from nonebot_plugin_saa import __plugin_meta__ as saa_plugin_meta
 
 from .config import Config
 from .manager import shindan_manager
 from .shindanmaker import (
     download_image,
     get_shindan_title,
     make_shindan,
@@ -35,20 +31,23 @@
 
 post_db_init(shindan_manager.load_shindan_records)
 
 __plugin_meta__ = PluginMetadata(
     name="趣味占卜",
     description="使用ShindanMaker网站的趣味占卜",
     usage="发送“占卜列表”查看可用占卜\n发送“{占卜名} {名字}”使用占卜",
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-shindan",
     config=Config,
+    supported_adapters=saa_plugin_meta.supported_adapters,
     extra={
         "unique_name": "shindan",
         "example": "人设生成 小Q",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.3.4",
+        "version": "0.4.0",
     },
 )
 
 add_usage = """Usage:
 添加占卜 {id} {指令}
 如：添加占卜 917962 人设生成"""
 
@@ -72,127 +71,108 @@
 
 @cmd_sd.handle()
 async def _():
     await cmd_sd.finish(__plugin_meta__.usage)
 
 
 @cmd_ls.handle()
-async def _(bot: Union[V11Bot, V12Bot]):
+async def _(matcher: Matcher):
     if not shindan_manager.shindan_records:
-        await cmd_ls.finish("尚未添加任何占卜")
+        await matcher.finish("尚未添加任何占卜")
 
     img = await render_shindan_list(shindan_manager.shindan_records)
-
-    if isinstance(bot, V11Bot):
-        await cmd_ls.finish(V11MsgSeg.image(img))
-    elif isinstance(bot, V12Bot):
-        resp = await bot.upload_file(type="data", name="shindan", data=img)
-        file_id = resp["file_id"]
-        await cmd_ls.finish(V12MsgSeg.image(file_id))
+    await MessageFactory(Image(img)).send()
+    await matcher.finish()
 
 
 @cmd_add.handle()
-async def _(msg: Union[V11Msg, V12Msg] = CommandArg()):
+async def _(matcher: Matcher, msg: Message = CommandArg()):
     arg = msg.extract_plain_text().strip()
     if not arg:
-        await cmd_add.finish(add_usage)
+        await matcher.finish(add_usage)
 
     args = arg.split()
     if len(args) != 2 or not args[0].isdigit():
-        await cmd_add.finish(add_usage)
+        await matcher.finish(add_usage)
 
     id = args[0]
     command = args[1]
     title = await get_shindan_title(id)
     if not title:
-        await cmd_add.finish("找不到该占卜，请检查id")
+        await matcher.finish("找不到该占卜，请检查id")
 
     if resp := await shindan_manager.add_shindan(id, command, title):
-        await cmd_add.finish(resp)
+        await matcher.finish(resp)
     else:
-        await cmd_add.finish(f"成功添加占卜“{title}”，可通过“{command} 名字”使用")
+        await matcher.finish(f"成功添加占卜“{title}”，可通过“{command} 名字”使用")
 
 
 @cmd_del.handle()
-async def _(msg: Union[V11Msg, V12Msg] = CommandArg()):
+async def _(matcher: Matcher, msg: Message = CommandArg()):
     arg = msg.extract_plain_text().strip()
     if not arg:
-        await cmd_del.finish(del_usage)
+        await matcher.finish(del_usage)
 
     if not arg.isdigit():
-        await cmd_del.finish(del_usage)
+        await matcher.finish(del_usage)
 
     id = arg
 
     if resp := await shindan_manager.remove_shindan(id):
-        await cmd_add.finish(resp)
+        await matcher.finish(resp)
     else:
-        await cmd_del.finish("成功删除该占卜")
+        await matcher.finish("成功删除该占卜")
 
 
 @cmd_set.handle()
-async def _(msg: Union[V11Msg, V12Msg] = CommandArg()):
+async def _(matcher: Matcher, msg: Message = CommandArg()):
     arg = msg.extract_plain_text().strip()
     if not arg:
-        await cmd_set.finish(set_usage)
+        await matcher.finish(set_usage)
 
     args = arg.split()
     if len(args) != 2 or not args[0].isdigit() or args[1] not in ["text", "image"]:
-        await cmd_set.finish(set_usage)
+        await matcher.finish(set_usage)
 
     id = args[0]
     mode = args[1]
 
     if resp := await shindan_manager.set_shindan_mode(id, mode):
-        await cmd_add.finish(resp)
+        await matcher.finish(resp)
     else:
-        await cmd_set.finish("设置成功")
+        await matcher.finish("设置成功")
+
+
+try:
+    from .onebot import get_mention_username, get_sender_username
+except ImportError:
+    get_mention_username = None
+    get_sender_username = None
 
 
 def sd_handler() -> Rule:
     async def handle(
-        bot: Union[V11Bot, V12Bot],
-        event: Union[V11MEvent, V12MEvent],
+        bot: Bot,
+        event: Event,
         state: T_State,
-        msg: Union[V11Msg, V12Msg] = EventMessage(),
+        msg: Message = EventMessage(),
         msg_text: str = EventPlainText(),
     ) -> bool:
-        async def get_name(command: str) -> str:
-            name = ""
-            if isinstance(bot, V11Bot):
-                assert isinstance(event, V11MEvent)
-                for msg_seg in msg:
-                    if msg_seg.type == "at":
-                        assert isinstance(event, V11GMEvent)
-                        info = await bot.get_group_member_info(
-                            group_id=event.group_id, user_id=msg_seg.data["qq"]
-                        )
-                        name = info.get("card", "") or info.get("nickname", "")
-                        break
-                if not name:
-                    name = msg_text[len(command) :].strip()
-                if not name:
-                    name = event.sender.card or event.sender.nickname
-            elif isinstance(bot, V12Bot):
-                assert isinstance(event, V12MEvent)
-
-                async def get_user_name(user_id: str):
-                    resp = await bot.get_user_info(user_id=user_id)
-                    return resp["user_displayname"] or resp["user_name"]
-
-                for msg_seg in msg:
-                    if msg_seg.type == "mention":
-                        name = await get_user_name(msg_seg.data["user_id"])
-                        break
-                if not name:
-                    name = msg_text[len(command) :].strip()
-                if not name:
-                    name = await get_user_name(event.user_id)
+        async def get_name(command: str) -> Optional[str]:
+            name = None
+            if get_mention_username:
+                name = await get_mention_username(bot, event, msg)
+
+            if not name:
+                name = msg_text[len(command) :].strip()
+
+            if not name and get_sender_username:
+                name = await get_sender_username(bot, event)
 
-            return name or ""
+            return name
 
         for record in sorted(
             shindan_manager.shindan_records,
             reverse=True,
             key=lambda record: record.command,
         ):
             if msg_text.startswith(record.command):
@@ -206,23 +186,27 @@
     return Rule(handle)
 
 
 sd_matcher = on_message(sd_handler(), priority=13)
 
 
 @sd_matcher.handle()
-async def _(bot: Union[V11Bot, V12Bot], state: T_State):
+async def _(state: T_State, matcher: Matcher):
     id: str = state["id"]
-    name: str = state["name"]
+    name: Optional[str] = state["name"]
     mode: str = state["mode"]
+
+    if name is None:
+        await matcher.finish("无法获取名字，请加上名字再试")
+
     try:
         res = await make_shindan(id, name, mode)
     except:
         logger.warning(traceback.format_exc())
-        await sd_matcher.finish("出错了，请稍后再试")
+        await matcher.finish("出错了，请稍后再试")
 
     msgs: List[Union[str, bytes]] = []
     if isinstance(res, str):
         img_pattern = r"((?:http|https)://\S+\.(?:jpg|jpeg|png|gif|bmp|webp))"
         for msg in re.split(img_pattern, res):
             if re.match(img_pattern, msg):
                 try:
@@ -232,26 +216,17 @@
                     logger.warning(f"{msg} 下载出错！")
             else:
                 msgs.append(msg)
     elif isinstance(res, bytes):
         msgs.append(res)
 
     if not msgs:
-        await sd_matcher.finish()
+        await matcher.finish()
 
-    if isinstance(bot, V11Bot):
-        message = V11Msg()
-        for msg in msgs:
-            if isinstance(msg, bytes):
-                message.append(V11MsgSeg.image(msg))
-            else:
-                message.append(msg)
-    else:
-        message = V12Msg()
-        for msg in msgs:
-            if isinstance(msg, bytes):
-                resp = await bot.upload_file(type="data", name="shindan", data=msg)
-                file_id = resp["file_id"]
-                message.append(V12MsgSeg.image(file_id))
-            else:
-                message.append(msg)
-    await sd_matcher.finish(message)
+    msg_builder = MessageFactory([])
+    for msg in msgs:
+        if isinstance(msg, bytes):
+            msg_builder.append(Image(msg))
+        else:
+            msg_builder.append(msg)
+    await msg_builder.send()
+    await matcher.finish()
```

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/manager.py` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/model.py` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/shindanmaker.py` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/shindanmaker.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.css` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/app.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.js` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/app.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/chart.js` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/chart.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/shindan_list.html` & `nonebot_plugin_shindan-0.4.0/nonebot_plugin_shindan/templates/shindan_list.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.4/pyproject.toml` & `nonebot_plugin_shindan-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 [tool.poetry]
 name = "nonebot_plugin_shindan"
-version = "0.3.4"
+version = "0.4.0"
 description = "Nonebot2 plugin for using ShindanMaker"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-shindan"
 repository = "https://github.com/noneplugin/nonebot-plugin-shindan"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.0"
-nonebot-plugin-htmlrender = ">=0.0.4"
-nonebot-plugin-datastore = "^0.6.0a1"
-httpx = ">=0.19.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
+nonebot-plugin-htmlrender = "^0.2.0"
+nonebot-plugin-datastore = "^1.0.0"
+httpx = ">=0.19.0,<1.0.0"
 lxml = "^4.0.0"
 Jinja2 = "^3.0.0"
 beautifulsoup4 = "^4.0.0"
 
+[tool.poetry.group.adapters]
+optional = true
+
+[tool.poetry.group.adapters.dependencies]
+nonebot-adapter-onebot = "^2.2.0"
+
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^1.0.0"
 black = "^22.1.0"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_shindan"]
```

### Comparing `nonebot_plugin_shindan-0.3.4/PKG-INFO` & `nonebot_plugin_shindan-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-shindan
-Version: 0.3.4
+Version: 0.4.0
 Summary: Nonebot2 plugin for using ShindanMaker
 Home-page: https://github.com/noneplugin/nonebot-plugin-shindan
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
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.0.0,<5.0.0)
-Requires-Dist: httpx (>=0.19.0)
+Requires-Dist: httpx (>=0.19.0,<1.0.0)
 Requires-Dist: lxml (>=4.0.0,<5.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
-Requires-Dist: nonebot-plugin-datastore (>=0.6.0a1,<0.7.0)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.0.4)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot-plugin-datastore (>=1.0.0,<2.0.0)
+Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-shindan
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-shindan
 
 使用 [ShindanMaker](https://shindanmaker.com) 网站的~~无聊~~趣味占卜
```

