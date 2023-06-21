# Comparing `tmp/nonebot_plugin_handle-0.2.0.tar.gz` & `tmp/nonebot_plugin_handle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_handle-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_handle-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_handle-0.2.0.tar` & `nonebot_plugin_handle-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1063 2023-01-29 06:55:55.489167 nonebot_plugin_handle-0.2.0/LICENSE
--rw-r--r--   0        0        0     1500 2023-01-29 06:55:55.489167 nonebot_plugin_handle-0.2.0/README.md
--rw-r--r--   0        0        0     8272 2023-01-29 06:55:55.489167 nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/__init__.py
--rw-r--r--   0        0        0     8118 2023-01-29 06:55:55.489167 nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/data_source.py
--rw-r--r--   0        0        0   211859 2023-01-29 06:55:55.493167 nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/data/answers.json
--rw-r--r--   0        0        0   383525 2023-01-29 06:55:55.493167 nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/data/idioms.txt
--rw-r--r--   0        0        0   383844 2023-01-29 06:55:55.497167 nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/fonts/NotoSansMono-Regular.ttf
--rw-r--r--   0        0        0 11214632 2023-01-29 06:55:55.589168 nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/fonts/NotoSerifSC-Regular.otf
--rw-r--r--   0        0        0     2193 2023-01-29 06:55:55.589168 nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/utils.py
--rw-r--r--   0        0        0      644 2023-01-29 06:55:55.589168 nonebot_plugin_handle-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 nonebot_plugin_handle-0.2.0/setup.py
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 nonebot_plugin_handle-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 08:18:26.615289 nonebot_plugin_handle-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1500 2023-06-21 08:18:26.615289 nonebot_plugin_handle-0.3.0/README.md
+-rw-r--r--   0        0        0     7434 2023-06-21 08:18:26.615289 nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/__init__.py
+-rw-r--r--   0        0        0     8119 2023-06-21 08:18:26.615289 nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/data_source.py
+-rw-r--r--   0        0        0   211859 2023-06-21 08:18:26.619289 nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/data/answers.json
+-rw-r--r--   0        0        0   383525 2023-06-21 08:18:26.623289 nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/data/idioms.txt
+-rw-r--r--   0        0        0   383844 2023-06-21 08:18:26.627289 nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/fonts/NotoSansMono-Regular.ttf
+-rw-r--r--   0        0        0 11214632 2023-06-21 08:18:26.731290 nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/fonts/NotoSerifSC-Regular.otf
+-rw-r--r--   0        0        0     2194 2023-06-21 08:18:26.731290 nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/utils.py
+-rw-r--r--   0        0        0      703 2023-06-21 08:18:26.731290 nonebot_plugin_handle-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 nonebot_plugin_handle-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_handle-0.2.0/LICENSE` & `nonebot_plugin_handle-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_handle-0.2.0/README.md` & `nonebot_plugin_handle-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/__init__.py` & `nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,47 @@
+import asyncio
 import re
 import shlex
-import asyncio
-from io import BytesIO
 from asyncio import TimerHandle
 from dataclasses import dataclass
-from typing import Dict, List, Optional, NoReturn, Union
+from io import BytesIO
+from typing import Dict, List, NoReturn, Optional
 
-from nonebot.typing import T_State
-from nonebot.matcher import Matcher
+from nonebot import on_command, on_message, on_shell_command, require
+from nonebot.adapters import Bot, Event, Message
 from nonebot.exception import ParserExit
-from nonebot.plugin import PluginMetadata
-from nonebot.rule import Rule, ArgumentParser
-from nonebot import on_command, on_shell_command, on_message
+from nonebot.matcher import Matcher
 from nonebot.params import (
-    ShellCommandArgv,
     CommandArg,
     CommandStart,
     EventPlainText,
     EventToMe,
+    ShellCommandArgv,
 )
+from nonebot.plugin import PluginMetadata
+from nonebot.rule import ArgumentParser, Rule
+from nonebot.typing import T_State
+
+require("nonebot_plugin_saa")
+require("nonebot_plugin_session")
 
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
 
+from .data_source import GuessResult, Handle
 from .utils import random_idiom
-from .data_source import Handle, GuessResult
 
 __plugin_meta__ = PluginMetadata(
     name="猜成语",
     description="汉字Wordle 猜成语",
     usage=(
         "@我 + “猜成语”开始游戏；\n"
         "你有十次的机会猜一个四字词语；\n"
@@ -46,19 +49,22 @@
         "青色 表示其出现在答案中且在正确的位置；\n"
         "橙色 表示其出现在答案中但不在正确的位置；\n"
         "每个格子的 汉字、声母、韵母、声调 都会独立进行颜色的指示。\n"
         "当四个格子都为青色时，你便赢得了游戏！\n"
         "可发送“结束”结束游戏；可发送“提示”查看提示。\n"
         "使用 --strict 选项开启成语检查，即猜测的短语必须是成语，如：@我 猜成语 --strict"
     ),
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-handle",
+    supported_adapters=supported_adapters,
     extra={
         "unique_name": "handle",
         "example": "@小Q 猜成语",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.2.0",
+        "version": "0.3.0",
     },
 )
 
 
 parser = ArgumentParser("handle", description="猜成语")
 parser.add_argument("--hint", action="store_true", help="提示")
 parser.add_argument("--stop", action="store_true", help="结束游戏")
@@ -78,41 +84,27 @@
 timers: Dict[str, TimerHandle] = {}
 
 handle = on_shell_command("handle", parser=parser, block=True, priority=13)
 
 
 @handle.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     argv: List[str] = ShellCommandArgv(),
 ):
     await handle_handle(bot, matcher, event, argv)
 
 
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
 
 
 def match_idiom(msg: str) -> bool:
     return bool(re.fullmatch(r"[\u4e00-\u9fa5]{4}", msg))
 
@@ -129,42 +121,37 @@
     return bool(command_start) or to_me
 
 
 def shortcut(cmd: str, argv: List[str] = [], **kwargs):
     command = on_command(cmd, **kwargs, block=True, priority=12)
 
     @command.handle()
-    async def _(
-        bot: Union[V11Bot, V12Bot],
-        matcher: Matcher,
-        event: Union[V11MEvent, V12MEvent],
-        msg: Union[V11Msg, V12Msg] = CommandArg(),
-    ):
+    async def _(bot: Bot, matcher: Matcher, event: Event, msg: Message = CommandArg()):
         try:
             args = shlex.split(msg.extract_plain_text().strip())
         except:
             args = []
         await handle_handle(bot, matcher, event, argv + args)
 
 
 shortcut("猜成语", rule=smart_to_me)
 shortcut("提示", ["--hint"], aliases={"给个提示"}, rule=game_running)
-shortcut("结束", ["--stop"], aliases={"停止游戏", "结束游戏"}, rule=game_running)
+shortcut("结束", ["--stop"], aliases={"结束游戏", "停止游戏"}, rule=game_running)
 
 
 idiom_matcher = on_message(
     Rule(game_running) & get_idiom_input, block=True, priority=14
 )
 
 
 @idiom_matcher.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     state: T_State,
 ):
     idiom: str = state["idiom"]
     await handle_handle(bot, matcher, event, [idiom])
 
 
 async def stop_game(matcher: Matcher, cid: str):
@@ -185,41 +172,34 @@
     timer = loop.call_later(
         timeout, lambda: asyncio.ensure_future(stop_game(matcher, cid))
     )
     timers[cid] = timer
 
 
 async def handle_handle(
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
-            if image:
-                msg.append(V11MsgSeg.image(image))
-        else:
-            msg = V12Msg()
-            if image:
-                resp = await bot.upload_file(
-                    type="data", name="wordle", data=image.getvalue()
-                )
-                file_id = resp["file_id"]
-                msg.append(V12MsgSeg.image(file_id))
-
+        msg_builder = MessageFactory([])
+        if image:
+            msg_builder.append(Image(image))
         if message:
-            msg.append(message)
-        await matcher.finish(msg)
+            if image:
+                message = "\n" + message
+            msg_builder.append(message)
+        await msg_builder.send()
+        await matcher.finish()
 
     try:
         args = parser.parse_args(argv)
     except ParserExit as e:
         if e.status == 0:
             await send(__plugin_meta__.usage)
         await send()
```

### Comparing `nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/data_source.py` & `nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from io import BytesIO
+from typing import Iterable, List, Optional, Tuple
+
 from PIL import Image, ImageDraw
 from PIL.Image import Image as IMG
-from typing import Iterable, Tuple, List, Optional
 
-from .utils import get_pinyin, load_font, save_jpg, legal_idiom
+from .utils import get_pinyin, legal_idiom, load_font, save_jpg
 
 
 class GuessResult(Enum):
     WIN = 0  # 猜出正确成语
     LOSS = 1  # 达到最大可猜次数，未猜出正确成语
     DUPLICATE = 2  # 成语重复
     ILLEGAL = 3  # 成语不合法
```

### Comparing `nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/data/answers.json` & `nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/data/answers.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/data/idioms.txt` & `nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/data/idioms.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/fonts/NotoSansMono-Regular.ttf` & `nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/fonts/NotoSansMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/resources/fonts/NotoSerifSC-Regular.otf` & `nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/resources/fonts/NotoSerifSC-Regular.otf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_handle-0.2.0/nonebot_plugin_handle/utils.py` & `nonebot_plugin_handle-0.3.0/nonebot_plugin_handle/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import random
 from io import BytesIO
 from pathlib import Path
-from typing import List, Dict, Tuple
-from pypinyin import pinyin, Style
+from typing import Dict, List, Tuple
+
 from PIL import ImageFont
 from PIL.Image import Image as IMG
 from PIL.ImageFont import FreeTypeFont
+from pypinyin import Style, pinyin
 
 resource_dir = Path(__file__).parent / "resources"
 fonts_dir = resource_dir / "fonts"
 data_dir = resource_dir / "data"
 idiom_path = data_dir / "idioms.txt"
 answer_path = data_dir / "answers.json"
```

### Comparing `nonebot_plugin_handle-0.2.0/pyproject.toml` & `nonebot_plugin_handle-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "nonebot_plugin_handle"
-version = "0.2.0"
+version = "0.3.0"
 description = "Nonebot2 汉字Wordle 插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-handle"
 repository = "https://github.com/noneplugin/nonebot-plugin-handle"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
+nonebot-plugin-session = ">=0.0.5,<0.1.0"
 Pillow = "^9.0.0"
-pypinyin = ">=0.40.0"
+pypinyin = ">=0.40.0,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_handle-0.2.0/PKG-INFO` & `nonebot_plugin_handle-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-handle
-Version: 0.2.0
+Version: 0.3.0
 Summary: Nonebot2 汉字Wordle 插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-handle
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
-Requires-Dist: pypinyin (>=0.40.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.5,<0.1.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
+Requires-Dist: pypinyin (>=0.40.0,<1.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-handle
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-handle
 
 适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的 汉字Wordle 猜成语插件
```

