# Comparing `tmp/nonebot_plugin_minesweeper-0.2.0.tar.gz` & `tmp/nonebot_plugin_minesweeper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_minesweeper-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_minesweeper-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_minesweeper-0.2.0.tar` & `nonebot_plugin_minesweeper-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1063 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/LICENSE
--rw-r--r--   0        0        0     1567 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/README.md
--rw-r--r--   0        0        0    10360 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/__init__.py
--rw-r--r--   0        0        0     7398 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/data_source.py
--rw-r--r--   0        0        0    25056 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/fonts/00TT.TTF
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/clone.bmp
--rw-r--r--   0        0        0     8902 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/colorsonly.bmp
--rw-r--r--   0        0        0     8904 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/hibbeler.bmp
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/icicle.bmp
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/mario.bmp
--rw-r--r--   0        0        0    52760 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/maviz.bmp
--rw-r--r--   0        0        0    52760 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/mine.bmp
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/narkomania.bmp
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/ocean.bmp
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/pacman.bmp
--rw-r--r--   0        0        0     8902 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/predator.bmp
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/scratch.bmp
--rw-r--r--   0        0        0     8902 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/symbol.bmp
--rw-r--r--   0        0        0     8902 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/unknown.bmp
--rw-r--r--   0        0        0    52758 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/vista.bmp
--rw-r--r--   0        0        0     8894 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/win98.bmp
--rw-r--r--   0        0        0     8902 2023-01-31 13:12:47.223544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/winbw.bmp
--rw-r--r--   0        0        0     8902 2023-01-31 13:12:47.227544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/winxp.bmp
--rw-r--r--   0        0        0     2566 2023-01-31 13:12:47.227544 nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/utils.py
--rw-r--r--   0        0        0      630 2023-01-31 13:12:47.227544 nonebot_plugin_minesweeper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 nonebot_plugin_minesweeper-0.2.0/setup.py
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 nonebot_plugin_minesweeper-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1567 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/README.md
+-rw-r--r--   0        0        0     9440 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/__init__.py
+-rw-r--r--   0        0        0     7399 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/data_source.py
+-rw-r--r--   0        0        0    25056 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/fonts/00TT.TTF
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/clone.bmp
+-rw-r--r--   0        0        0     8902 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/colorsonly.bmp
+-rw-r--r--   0        0        0     8904 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/hibbeler.bmp
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/icicle.bmp
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.232679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/mario.bmp
+-rw-r--r--   0        0        0    52760 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/maviz.bmp
+-rw-r--r--   0        0        0    52760 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/mine.bmp
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/narkomania.bmp
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/ocean.bmp
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/pacman.bmp
+-rw-r--r--   0        0        0     8902 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/predator.bmp
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/scratch.bmp
+-rw-r--r--   0        0        0     8902 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/symbol.bmp
+-rw-r--r--   0        0        0     8902 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/unknown.bmp
+-rw-r--r--   0        0        0    52758 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/vista.bmp
+-rw-r--r--   0        0        0     8894 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/win98.bmp
+-rw-r--r--   0        0        0     8902 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/winbw.bmp
+-rw-r--r--   0        0        0     8902 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/winxp.bmp
+-rw-r--r--   0        0        0     2565 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/utils.py
+-rw-r--r--   0        0        0      682 2023-06-21 14:20:47.236679 nonebot_plugin_minesweeper-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 nonebot_plugin_minesweeper-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_minesweeper-0.2.0/LICENSE` & `nonebot_plugin_minesweeper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/README.md` & `nonebot_plugin_minesweeper-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/__init__.py` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,40 @@
+import asyncio
 import re
 import shlex
-import asyncio
-from io import BytesIO
 from asyncio import TimerHandle
 from dataclasses import dataclass, field
-from typing import Dict, List, Tuple, Optional, NoReturn, Union
+from io import BytesIO
+from typing import Dict, List, NoReturn, Optional, Tuple
 
-from nonebot.matcher import Matcher
-from nonebot.rule import ArgumentParser
+from nonebot import on_command, on_shell_command, require
+from nonebot.adapters import Bot, Event, Message
 from nonebot.exception import ParserExit
+from nonebot.matcher import Matcher
+from nonebot.params import CommandArg, CommandStart, EventToMe, ShellCommandArgv
 from nonebot.plugin import PluginMetadata
-from nonebot import on_command, on_shell_command
-from nonebot.params import ShellCommandArgv, CommandArg, CommandStart, EventToMe
+from nonebot.rule import ArgumentParser
 
-from nonebot.adapters.onebot.v11 import Bot as V11Bot
-from nonebot.adapters.onebot.v11 import Message as V11Msg
-from nonebot.adapters.onebot.v11 import MessageSegment as V11MsgSeg
-from nonebot.adapters.onebot.v11 import MessageEvent as V11MEvent
-from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
-
-from nonebot.adapters.onebot.v12 import Bot as V12Bot
-from nonebot.adapters.onebot.v12 import Message as V12Msg
-from nonebot.adapters.onebot.v12 import MessageSegment as V12MsgSeg
-from nonebot.adapters.onebot.v12 import MessageEvent as V12MEvent
-from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12GMEvent
-from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12CMEvent
+require("nonebot_plugin_saa")
+require("nonebot_plugin_session")
 
+from nonebot_plugin_saa import Image, MessageFactory
+from nonebot_plugin_saa import __plugin_meta__ as saa_plugin_meta
+from nonebot_plugin_session import SessionIdType
+from nonebot_plugin_session import __plugin_meta__ as session_plugin_meta
+from nonebot_plugin_session import extract_session
+
+assert saa_plugin_meta.supported_adapters
+assert session_plugin_meta.supported_adapters
+supported_adapters = (
+    saa_plugin_meta.supported_adapters & session_plugin_meta.supported_adapters
+)
+
+from .data_source import GameState, MarkResult, MineSweeper, OpenResult
 from .utils import skin_list
-from .data_source import MineSweeper, GameState, OpenResult, MarkResult
 
 __plugin_meta__ = PluginMetadata(
     name="扫雷",
     description="扫雷游戏",
     usage=(
         "@我 + 扫雷 开始游戏；\n"
         "@我 + 扫雷初级 / 扫雷中级 / 扫雷高级 可开始不同难度的游戏；\n"
@@ -39,19 +42,22 @@
         "可使用 -s/--skin SKIN 指定皮肤，默认为 winxp；\n"
         "使用 挖开/open + 位置 来挖开方块，可同时指定多个位置；\n"
         "使用 标记/mark + 位置 来标记方块，可同时指定多个位置；\n"
         "位置为 字母+数字 的组合，如“A1”；\n"
         "发送 查看游戏 查看当前游戏状态；\n"
         "发送 结束 结束游戏；\n"
     ),
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-minesweeper",
+    supported_adapters=supported_adapters,
     extra={
         "unique_name": "minesweeper",
         "example": "@小Q 扫雷\n挖开 A1\n标记 B2 C3",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.2.0",
+        "version": "0.3.0",
     },
 )
 
 
 parser = ArgumentParser("minesweeper", description="扫雷")
 parser.add_argument("-r", "--row", type=int, default=8, help="行数")
 parser.add_argument("-c", "--col", type=int, default=8, help="列数")
@@ -79,59 +85,42 @@
 timers: Dict[str, TimerHandle] = {}
 
 minesweeper = on_shell_command("minesweeper", parser=parser, block=True, priority=13)
 
 
 @minesweeper.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
-    matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
-    argv: List[str] = ShellCommandArgv(),
+    bot: Bot, matcher: Matcher, event: Event, argv: List[str] = ShellCommandArgv()
 ):
     await handle_minesweeper(bot, matcher, event, argv)
 
 
-def get_cid(bot: Union[V11Bot, V12Bot], event: Union[V11MEvent, V12MEvent]):
-    if isinstance(event, V11MEvent):
-        cid = f"{bot.self_id}_{event.sub_type}_"
-    else:
-        cid = f"{bot.self_id}_{event.detail_type}_"
-
-    if isinstance(event, V11GMEvent) or isinstance(event, V12GMEvent):
-        cid += str(event.group_id)
-    elif isinstance(event, V12CMEvent):
-        cid += f"{event.guild_id}_{event.channel_id}"
-    else:
-        cid += str(event.user_id)
-
-    return cid
-
-
-def game_running(
-    bot: Union[V11Bot, V12Bot], event: Union[V11MEvent, V12MEvent]
-) -> bool:
+def get_cid(bot: Bot, event: Event):
+    return extract_session(bot, event).get_id(SessionIdType.GROUP)
+
+
+def game_running(bot: Bot, event: Event) -> bool:
     cid = get_cid(bot, event)
     return bool(games.get(cid, None))
 
 
 # 命令前缀为空则需要to_me，否则不需要
 def smart_to_me(command_start: str = CommandStart(), to_me: bool = EventToMe()) -> bool:
     return bool(command_start) or to_me
 
 
 def shortcut(cmd: str, argv: List[str] = [], **kwargs):
     command = on_command(cmd, **kwargs, block=True, priority=12)
 
     @command.handle()
     async def _(
-        bot: Union[V11Bot, V12Bot],
+        bot: Bot,
         matcher: Matcher,
-        event: Union[V11MEvent, V12MEvent],
-        msg: Union[V11Msg, V12Msg] = CommandArg(),
+        event: Event,
+        msg: Message = CommandArg(),
     ):
         try:
             args = shlex.split(msg.extract_plain_text().strip())
         except:
             args = []
         await handle_minesweeper(bot, matcher, event, argv + args)
 
@@ -142,18 +131,14 @@
 shortcut("扫雷高级", ["--row", "16", "--col", "30", "--num", "99"], rule=smart_to_me)
 shortcut("挖开", ["--open"], aliases={"open", "wk"}, rule=game_running)
 shortcut("标记", ["--mark"], aliases={"mark", "bj"}, rule=game_running)
 shortcut("查看游戏", ["--show"], aliases={"查看游戏盘", "显示游戏", "显示游戏盘"}, rule=game_running)
 shortcut("结束", ["--stop"], aliases={"停", "停止游戏", "结束游戏"}, rule=game_running)
 
 
-def is_qq(msg: str):
-    return msg.isdigit() and 11 >= len(msg) >= 5
-
-
 async def stop_game(matcher: Matcher, cid: str):
     timers.pop(cid, None)
     if games.get(cid, None):
         games.pop(cid)
         await matcher.finish("扫雷超时，游戏结束")
 
 
@@ -165,42 +150,34 @@
     timer = loop.call_later(
         timeout, lambda: asyncio.ensure_future(stop_game(matcher, cid))
     )
     timers[cid] = timer
 
 
 async def handle_minesweeper(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     argv: List[str],
 ):
     async def send(
         message: Optional[str] = None, image: Optional[BytesIO] = None
     ) -> NoReturn:
         if not (message or image):
             await matcher.finish()
 
-        if isinstance(bot, V11Bot):
-            msg = V11Msg()
-            if message:
-                msg.append(message)
-            if image:
-                msg.append(V11MsgSeg.image(image))
-        else:
-            msg = V12Msg()
-            if message:
-                msg.append(message)
+        msg_builder = MessageFactory([])
+        if message:
             if image:
-                resp = await bot.upload_file(
-                    type="data", name="minesweeper", data=image.getvalue()
-                )
-                file_id = resp["file_id"]
-                msg.append(V12MsgSeg.image(file_id))
-        await matcher.finish(msg)
+                message += "\n"
+            msg_builder.append(message)
+        if image:
+            msg_builder.append(Image(image))
+        await msg_builder.send()
+        await matcher.finish()
 
     try:
         args = parser.parse_args(argv)
     except ParserExit as e:
         if e.status == 0:
             await send(__plugin_meta__.usage)
         await send()
```

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/data_source.py` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import time
 import random
+import time
+from dataclasses import dataclass
 from enum import Enum
 from io import BytesIO
-from dataclasses import dataclass
-from typing import Tuple, Optional, Iterator
+from typing import Iterator, Optional, Tuple
+
 from PIL import Image, ImageDraw
 from PIL.Image import Image as IMG
 
-from .utils import load_skin, load_font, save_png
+from .utils import load_font, load_skin, save_png
 
 
 class GameState(Enum):
     PREPARE = 0
     GAMING = 1
     WIN = 2
     FAIL = 3
```

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/fonts/00TT.TTF` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/fonts/00TT.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/clone.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/clone.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/colorsonly.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/colorsonly.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/hibbeler.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/hibbeler.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/icicle.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/icicle.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/mario.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/mario.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/maviz.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/maviz.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/mine.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/mine.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/narkomania.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/narkomania.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/ocean.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/ocean.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/pacman.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/pacman.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/predator.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/predator.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/scratch.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/scratch.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/symbol.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/symbol.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/unknown.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/unknown.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/vista.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/vista.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/win98.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/win98.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/winbw.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/winbw.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/resources/skins/winxp.bmp` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/resources/skins/winxp.bmp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_minesweeper-0.2.0/nonebot_plugin_minesweeper/utils.py` & `nonebot_plugin_minesweeper-0.3.0/nonebot_plugin_minesweeper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from dataclasses import dataclass
 from io import BytesIO
 from pathlib import Path
 from typing import List, Tuple
-from dataclasses import dataclass
+
 from PIL import Image, ImageFont
 from PIL.Image import Image as IMG
 from PIL.ImageFont import FreeTypeFont
 
 data_dir = Path(__file__).parent / "resources"
 skins_dir = data_dir / "skins"
 fonts_dir = data_dir / "fonts"
@@ -51,15 +52,15 @@
         ((15, 108, 27, 109), (12 + w * 16, 55, 24 + w * 16, 55 + h * 16)),
         ((0, 110, 12, 121), (0, 55 + h * 16, 12, 66 + h * 16)),
         ((13, 110, 14, 121), (12, 55 + h * 16, 12 + w * 16, 66 + h * 16)),
         ((15, 110, 27, 121), (12 + w * 16, 55 + h * 16, 24 + w * 16, 66 + h * 16)),
         ((28, 82, 69, 107), (16, 15, 57, 40)),
         ((28, 82, 69, 107), (w * 16 - 33, 15, 8 + w * 16, 40)),
     ]
-    for (s, t) in b:
+    for s, t in b:
         background.paste(image.crop(s).resize((t[2] - t[0], t[3] - t[1])), t)
 
     return Skin(numbers, icons, digits, faces, background)
 
 
 def save_png(frame: IMG) -> BytesIO:
     output = BytesIO()
```

### Comparing `nonebot_plugin_minesweeper-0.2.0/PKG-INFO` & `nonebot_plugin_minesweeper-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-minesweeper
-Version: 0.2.0
+Version: 0.3.0
 Summary: Nonebot2 扫雷插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-minesweeper
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
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.5,<0.1.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-minesweeper
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-minesweeper
 
 适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的 扫雷插件
```

