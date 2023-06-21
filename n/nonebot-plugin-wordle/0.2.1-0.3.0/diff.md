# Comparing `tmp/nonebot_plugin_wordle-0.2.1.tar.gz` & `tmp/nonebot_plugin_wordle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wordle-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_wordle-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_wordle-0.2.1.tar` & `nonebot_plugin_wordle-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/LICENSE
--rw-r--r--   0        0        0     1302 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/README.md
--rw-r--r--   0        0        0     9033 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/__init__.py
--rw-r--r--   0        0        0     5997 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/data_source.py
--rw-r--r--   0        0        0   139252 2023-04-13 04:13:05.000661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf
--rw-r--r--   0        0        0   695923 2023-04-13 04:13:05.004661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET4.json
--rw-r--r--   0        0        0   443930 2023-04-13 04:13:05.008662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET6.json
--rw-r--r--   0        0        0   480469 2023-04-13 04:13:05.008662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GMAT.json
--rw-r--r--   0        0        0  1021713 2023-04-13 04:13:05.016662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GRE.json
--rw-r--r--   0        0        0   521446 2023-04-13 04:13:05.016662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/IELTS.json
--rw-r--r--   0        0        0   637594 2023-04-13 04:13:05.020662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/SAT.json
--rw-r--r--   0        0        0  1252663 2023-04-13 04:13:05.028663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/TOEFL.json
--rw-r--r--   0        0        0  1750255 2023-04-13 04:13:05.036663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专八.json
--rw-r--r--   0        0        0   620016 2023-04-13 04:13:05.040663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专四.json
--rw-r--r--   0        0        0   675299 2023-04-13 04:13:05.044663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/考研.json
--rw-r--r--   0        0        0     1193 2023-04-13 04:13:05.044663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/utils.py
--rw-r--r--   0        0        0      650 2023-04-13 04:13:05.044663 nonebot_plugin_wordle-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 nonebot_plugin_wordle-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 07:18:53.822752 nonebot_plugin_wordle-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1302 2023-06-21 07:18:53.822752 nonebot_plugin_wordle-0.3.0/README.md
+-rw-r--r--   0        0        0     8229 2023-06-21 07:18:53.822752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/__init__.py
+-rw-r--r--   0        0        0     5997 2023-06-21 07:18:53.822752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/data_source.py
+-rw-r--r--   0        0        0   139252 2023-06-21 07:18:53.822752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf
+-rw-r--r--   0        0        0   695923 2023-06-21 07:18:53.826752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/CET4.json
+-rw-r--r--   0        0        0   443930 2023-06-21 07:18:53.830752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/CET6.json
+-rw-r--r--   0        0        0   480469 2023-06-21 07:18:53.830752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/GMAT.json
+-rw-r--r--   0        0        0  1021713 2023-06-21 07:18:53.838752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/GRE.json
+-rw-r--r--   0        0        0   521446 2023-06-21 07:18:53.842752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/IELTS.json
+-rw-r--r--   0        0        0   637594 2023-06-21 07:18:53.846752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/SAT.json
+-rw-r--r--   0        0        0  1252663 2023-06-21 07:18:53.854752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/TOEFL.json
+-rw-r--r--   0        0        0  1750255 2023-06-21 07:18:53.866752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/专八.json
+-rw-r--r--   0        0        0   620016 2023-06-21 07:18:53.870752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/专四.json
+-rw-r--r--   0        0        0   675299 2023-06-21 07:18:53.874752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/考研.json
+-rw-r--r--   0        0        0     1193 2023-06-21 07:18:53.874752 nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/utils.py
+-rw-r--r--   0        0        0      702 2023-06-21 07:18:53.874752 nonebot_plugin_wordle-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 nonebot_plugin_wordle-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_wordle-0.2.1/LICENSE` & `nonebot_plugin_wordle-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/README.md` & `nonebot_plugin_wordle-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/__init__.py` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import asyncio
 import re
 import shlex
 from asyncio import TimerHandle
 from dataclasses import dataclass
 from io import BytesIO
-from typing import Dict, List, NoReturn, Optional, Union
+from typing import Dict, List, NoReturn, Optional
 
-from nonebot import on_command, on_message, on_shell_command
-from nonebot.adapters.onebot.v11 import Bot as V11Bot
-from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
-from nonebot.adapters.onebot.v11 import Message as V11Msg
-from nonebot.adapters.onebot.v11 import MessageEvent as V11MEvent
-from nonebot.adapters.onebot.v11 import MessageSegment as V11MsgSeg
-from nonebot.adapters.onebot.v12 import Bot as V12Bot
-from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12CMEvent
-from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12GMEvent
-from nonebot.adapters.onebot.v12 import Message as V12Msg
-from nonebot.adapters.onebot.v12 import MessageEvent as V12MEvent
-from nonebot.adapters.onebot.v12 import MessageSegment as V12MsgSeg
+from nonebot import on_command, on_message, on_shell_command, require
+from nonebot.adapters import Bot, Event, Message
 from nonebot.exception import ParserExit
 from nonebot.matcher import Matcher
 from nonebot.params import (
     CommandArg,
     CommandStart,
     EventPlainText,
     EventToMe,
     ShellCommandArgv,
 )
 from nonebot.plugin import PluginMetadata
 from nonebot.rule import ArgumentParser, Rule
 from nonebot.typing import T_State
 
+require("nonebot_plugin_saa")
+require("nonebot_plugin_session")
+
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
 from .data_source import GuessResult, Wordle
 from .utils import dic_list, random_word
 
 __plugin_meta__ = PluginMetadata(
     name="猜单词",
     description="wordle猜单词游戏",
     usage=(
@@ -45,19 +50,22 @@
         "灰色块代表此单词中没有此字母；\n"
         "猜出单词或用光次数则游戏结束；\n"
         "发送“结束”结束游戏；发送“提示”查看提示；\n"
         "可使用 -l/--length 指定单词长度，默认为5；\n"
         "可使用 -d/--dic 指定词典，默认为CET4\n"
         f"支持的词典：{'、'.join(dic_list)}"
     ),
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-wordle",
+    supported_adapters=supported_adapters,
     extra={
         "unique_name": "wordle",
         "example": "@小Q 猜单词\nwordle -l 6 -d CET6",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.2.1",
+        "version": "0.3.0",
     },
 )
 
 
 parser = ArgumentParser("wordle", description="猜单词")
 parser.add_argument("-l", "--length", type=int, default=5, help="单词长度")
 parser.add_argument("-d", "--dic", default="CET4", help="词典")
@@ -79,41 +87,27 @@
 timers: Dict[str, TimerHandle] = {}
 
 wordle = on_shell_command("wordle", parser=parser, block=True, priority=13)
 
 
 @wordle.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     argv: List[str] = ShellCommandArgv(),
 ):
     await handle_wordle(bot, matcher, event, argv)
 
 
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
 
 
 def get_word_input(state: T_State, msg: str = EventPlainText()) -> bool:
     if re.fullmatch(r"^[a-zA-Z]{3,8}$", msg):
         state["word"] = msg
@@ -122,18 +116,18 @@
 
 
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
         await handle_wordle(bot, matcher, event, argv + args)
 
@@ -141,25 +135,25 @@
 # 命令前缀为空则需要to_me，否则不需要
 def smart_to_me(command_start: str = CommandStart(), to_me: bool = EventToMe()) -> bool:
     return bool(command_start) or to_me
 
 
 shortcut("猜单词", ["--length", "5", "--dic", "CET4"], rule=smart_to_me)
 shortcut("提示", ["--hint"], aliases={"给个提示"}, rule=game_running)
-shortcut("结束", ["--stop"], aliases={"停", "停止游戏", "结束游戏"}, rule=game_running)
+shortcut("结束", ["--stop"], aliases={"结束游戏", "停止游戏"}, rule=game_running)
 
 
 word_matcher = on_message(Rule(game_running) & get_word_input, block=True, priority=12)
 
 
 @word_matcher.handle()
 async def _(
-    bot: Union[V11Bot, V12Bot],
+    bot: Bot,
     matcher: Matcher,
-    event: Union[V11MEvent, V12MEvent],
+    event: Event,
     state: T_State,
 ):
     word: str = state["word"]
     await handle_wordle(bot, matcher, event, [word])
 
 
 async def stop_game(matcher: Matcher, cid: str):
@@ -180,41 +174,34 @@
     timer = loop.call_later(
         timeout, lambda: asyncio.ensure_future(stop_game(matcher, cid))
     )
     timers[cid] = timer
 
 
 async def handle_wordle(
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

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/data_source.py` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/data_source.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,22 +36,22 @@
         self.exist_color = (198, 182, 109)  # 存在但位置不正确时的颜色
         self.wrong_color = (123, 123, 124)  # 不存在时颜色
         self.border_color = (123, 123, 124)  # 边框颜色
         self.bg_color = (255, 255, 255)  # 背景颜色
         self.font_color = (255, 255, 255)  # 文字颜色
 
     def guess(self, word: str) -> Optional[GuessResult]:
-        if not legal_word(word):
-            return GuessResult.ILLEGAL
         word = word.lower()
+        if word == self.word_lower:
+            return GuessResult.WIN
         if word in self.guessed_words:
             return GuessResult.DUPLICATE
+        if not legal_word(word):
+            return GuessResult.ILLEGAL
         self.guessed_words.append(word)
-        if word == self.word_lower:
-            return GuessResult.WIN
         if len(self.guessed_words) == self.rows:
             return GuessResult.LOSS
 
     def draw_block(self, color: Tuple[int, int, int], letter: str) -> IMG:
         block = Image.new("RGB", self.block_size, self.border_color)
         inner_w = self.block_size[0] - self.border_width * 2
         inner_h = self.block_size[1] - self.border_width * 2
```

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET4.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/CET4.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET6.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/CET6.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GMAT.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/GMAT.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GRE.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/GRE.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/IELTS.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/IELTS.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/SAT.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/SAT.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/TOEFL.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/TOEFL.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专八.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/专八.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专四.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/专四.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/考研.json` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/resources/words/考研.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/utils.py` & `nonebot_plugin_wordle-0.3.0/nonebot_plugin_wordle/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.1/pyproject.toml` & `nonebot_plugin_wordle-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "nonebot_plugin_wordle"
-version = "0.2.1"
+version = "0.3.0"
 description = "Nonebot2 wordle猜单词插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-wordle"
 repository = "https://github.com/noneplugin/nonebot-plugin-wordle"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
+nonebot-plugin-session = ">=0.0.5,<0.1.0"
 Pillow = "^9.0.0"
 pyspellchecker = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 
 [build-system]
```

### Comparing `nonebot_plugin_wordle-0.2.1/PKG-INFO` & `nonebot_plugin_wordle-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-wordle
-Version: 0.2.1
+Version: 0.3.0
 Summary: Nonebot2 wordle猜单词插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-wordle
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
 Requires-Dist: pyspellchecker (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-wordle
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-wordle
 
 适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的 wordle 猜单词插件
```

