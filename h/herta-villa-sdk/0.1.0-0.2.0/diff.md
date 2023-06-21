# Comparing `tmp/herta_villa_sdk-0.1.0.tar.gz` & `tmp/herta_villa_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.1.0.tar", last modified: Thu Jun  8 09:31:42 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.2.0.tar", last modified: Wed Jun 21 17:12:13 2023, max compression
```

## Comparing `herta_villa_sdk-0.1.0.tar` & `herta_villa_sdk-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-06-08 09:31:14.138365 herta_villa_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0      112 2023-06-08 09:31:14.138365 herta_villa_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      479 2023-06-08 09:31:14.138365 herta_villa_sdk-0.1.0/hertavilla/__init__.py
--rw-r--r--   0        0        0     7154 2023-06-08 09:31:14.138365 herta_villa_sdk-0.1.0/hertavilla/bot.py
--rw-r--r--   0        0        0     4223 2023-06-08 09:31:14.138365 herta_villa_sdk-0.1.0/hertavilla/event.py
--rw-r--r--   0        0        0      738 2023-06-08 09:31:14.142365 herta_villa_sdk-0.1.0/hertavilla/exception.py
--rw-r--r--   0        0        0        0 2023-06-08 09:31:14.142365 herta_villa_sdk-0.1.0/hertavilla/handle.py
--rw-r--r--   0        0        0     6579 2023-06-08 09:31:14.142365 herta_villa_sdk-0.1.0/hertavilla/message.py
--rw-r--r--   0        0        0     2372 2023-06-08 09:31:14.142365 herta_villa_sdk-0.1.0/hertavilla/model.py
--rw-r--r--   0        0        0     2912 2023-06-08 09:31:14.142365 herta_villa_sdk-0.1.0/hertavilla/server.py
--rw-r--r--   0        0        0      416 2023-06-08 09:31:14.142365 herta_villa_sdk-0.1.0/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-06-08 09:31:14.142365 herta_villa_sdk-0.1.0/hertavilla/version.py
--rw-r--r--   0        0        0     1616 2023-06-08 09:31:42.090404 herta_villa_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 herta_villa_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/LICENSE
+-rw-r--r--   0        0        0      112 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0      555 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/__init__.py
+-rw-r--r--   0        0        0     7197 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/bot.py
+-rw-r--r--   0        0        0     4505 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/event.py
+-rw-r--r--   0        0        0      738 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/exception.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/handle.py
+-rw-r--r--   0        0        0      353 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     1060 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1466 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/image.py
+-rw-r--r--   0        0        0      594 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6188 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/text.py
+-rw-r--r--   0        0        0      162 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/types.py
+-rw-r--r--   0        0        0     2372 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/model.py
+-rw-r--r--   0        0        0     2912 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/server.py
+-rw-r--r--   0        0        0      558 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/version.py
+-rw-r--r--   0        0        0     1616 2023-06-21 17:12:13.792804 herta_villa_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 herta_villa_sdk-0.2.0/PKG-INFO
```

### Comparing `herta_villa_sdk-0.1.0/LICENSE` & `herta_villa_sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.1.0/hertavilla/bot.py` & `herta_villa_sdk-0.2.0/hertavilla/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 from hertavilla.exception import raise_exception
 from hertavilla.model import BotMemberAccessInfo, Member, Room, Villa
 from hertavilla.utils import MsgEncoder
 
 if TYPE_CHECKING:
     from hertavilla.event import Event
-    from hertavilla.message import MessageChain, MsgContentInfo
+    from hertavilla.message import MessageChain
+    from hertavilla.message.types import MsgContentInfo
 
 
 from aiohttp import ClientSession
 
 BASE_API = "https://bbs-api.miyoushe.com/vila/api/bot/platform"
 
 TE = TypeVar("TE", bound="Event")
@@ -227,15 +228,15 @@
 
         Returns:
             str: bot_msg_id 机器人所发送消息的唯一标识符
         """
         return await self.send_message(
             villa_id,
             room_id,
-            await chain.to_content_json(self),
+            *(await chain.to_content_json(self)),
         )
 
     # event handle
     def listen(
         self,
         event: type[TE],
     ) -> Callable[
```

### Comparing `herta_villa_sdk-0.1.0/hertavilla/event.py` & `herta_villa_sdk-0.2.0/hertavilla/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from __future__ import annotations
 
 import json
 import sys
 from typing import Any, Literal, Type
 
 from hertavilla.message import (
+    MessageChain,
+)
+from hertavilla.message.text import (
     EntityDict,
     MentionedInfo,
-    MessageChain,
     QuoteInfo,
     Text,
-    _rc,
     entity_types,
 )
+from hertavilla.utils import _rc
 
 from pydantic import BaseModel, Field, create_model_from_typeddict, validator
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
@@ -122,29 +124,35 @@
     @validator("content", pre=True)
     def parse_content(cls, v: Any):
         chain = MessageChain()
         text = v["text"].encode("utf-16")
         entities = v["entities"]
         last_offset = 0
         last_length = 0
+        end_offset = 0
         for entity in entities:
-            end_offset = last_offset + last_length
             entity: EntityDict
             offset = entity["offset"]
             body = entity["entity"]
             type_ = body.pop("type")
             if offset != end_offset:
                 # 两个 Entity 偏移相差为文字
                 chain.append(
                     Text(text[_rc(end_offset) : _rc(offset)].decode("utf-16")),
                 )
             else:
                 chain.append(entity_types[type_](**body))
             last_offset = offset
             last_length = entity["length"]
+            end_offset = last_offset + last_length
+        if _rc(end_offset) != len(text):
+            # 最后一个 Entity 之后是文字
+            chain.append(
+                Text(text[_rc(end_offset) :].decode("utf-16")),
+            )
         return chain
 
 
 class SendMessageEvent(Event):
     type: Literal[2]
 
     content: MessageContent
```

### Comparing `herta_villa_sdk-0.1.0/hertavilla/exception.py` & `herta_villa_sdk-0.2.0/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.1.0/hertavilla/message.py` & `herta_villa_sdk-0.2.0/hertavilla/message/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 from __future__ import annotations
 
 import abc
-from typing import Any, List, Literal, TypedDict, cast
+from typing import Any, Literal, TypedDict, cast
 
 from hertavilla.bot import VillaBot
-
-
-def _c(text: str) -> int:
-    return (len(text.encode("utf-16")) // 2) - 1
-
-
-def _rc(length: int) -> int:
-    return (length + 1) * 2
-
+from hertavilla.message.types import MsgContent, MsgContentInfo, _Segment
+from hertavilla.utils import _c
 
 entity_types: dict[str, type["_TextEntity"]] = {}
 
-# define TypedDicts for typing
+# MsgContentInfo for text
 
 
-class MsgContentInfo(TypedDict):
-    content: MsgContent
+class TextMsgContentInfo(MsgContentInfo):
+    content: TextMsgContent
     mentionedInfo: MentionedInfo | None
     quote: QuoteInfo | None
 
 
 class QuoteInfo(TypedDict):
     quoted_message_id: str
     """引用消息 id"""
@@ -51,22 +44,21 @@
 
 class EntityDict(TypedDict):
     entity: Any
     length: int
     offset: int
 
 
-class MsgContent:
-    ...
+# Segment for text
 
 
-class _TextEntity(abc.ABC):
+class _TextEntity(_Segment, abc.ABC):
     type_: str
 
-    def __init__(self, **kwargs) -> None:  # noqa: B027
+    def __init__(self, **kwargs) -> None:
         ...
 
     @abc.abstractmethod
     async def get_text(self, bot: VillaBot) -> str:
         raise NotImplementedError
 
     def get_mention(self) -> tuple[Literal[1, 2], str] | None:
@@ -159,76 +151,76 @@
         self.message_id = message_id
         self.time = time
 
     async def get_text(self, bot: VillaBot) -> str:
         raise NotImplementedError
 
 
+# MsgContent for text
+
+
 class TextMsgContent(MsgContent):
     def __init__(self, text: str, entities: list[EntityDict]) -> None:
         self.text = text
         self.entities = entities
 
 
-class MessageChain(List[_TextEntity]):
-    def append(self, __object: _TextEntity | str) -> None:
-        if isinstance(__object, str):
-            __object = Text(__object)
-        super().append(__object)
-
-    async def to_content_json(self, bot: VillaBot) -> MsgContentInfo:
-        texts: list[str] = []
-        entities: list[EntityDict] = []
-        mentioned_info: MentionedInfo | None = None
-        quote: QuoteInfo | None = None
-        offset = 0
-        for i, entity in enumerate(self):
-            if isinstance(entity, Quote):
-                # 存在 Quote Entity 转换成 quote
-                message_id = entity.message_id
-                time = entity.time
-                quote = cast(
-                    QuoteInfo,
-                    {
-                        "original_message_id": message_id,
-                        "original_message_send_time": time,
-                        "quoted_message_id": message_id,
-                        "quoted_message_send_time": time,
-                    },
-                )
-                continue
-            # 非文字 entity 尾随空格，最末除外
-            space = "" if i == len(self) - 1 else " "
-            if isinstance(entity, Text):
-                text = str(entity)
-                length = len(text)
-            else:
-                text = f"{await entity.get_text(bot)}{space}"
-                length = _c(text)
-                entities.append(
-                    {
-                        "entity": {"type": entity.type_, **entity.__dict__},
-                        "length": length,
-                        "offset": offset,
-                    },
-                )
-                if mention := entity.get_mention():
-                    type_, id_ = mention
-                    if mentioned_info is None:
-                        user_id_list = []
-                        mentioned_info = cast(
-                            MentionedInfo,
-                            {"type": type_, "userIdList": user_id_list},
-                        )
-                    else:
-                        if mentioned_info["type"] != 1:
-                            mentioned_info["type"] = type_
-                        user_id_list = mentioned_info["userIdList"]
-                    if type_ != 1:
-                        user_id_list.append(id_)
-            offset += len(text)
-            texts.append(text)
-        return {
-            "content": TextMsgContent("".join(texts), entities),
-            "quote": quote,
-            "mentionedInfo": mentioned_info,
-        }
+async def text_to_content(
+    text_entities: list[_TextEntity],
+    bot: VillaBot,
+) -> TextMsgContentInfo:
+    texts: list[str] = []
+    entities: list[EntityDict] = []
+    mentioned_info: MentionedInfo | None = None
+    quote: QuoteInfo | None = None
+    offset = 0
+    for i, entity in enumerate(text_entities):
+        if isinstance(entity, Quote):
+            # 存在 Quote Entity 转换成 quote
+            message_id = entity.message_id
+            time = entity.time
+            quote = cast(
+                QuoteInfo,
+                {
+                    "original_message_id": message_id,
+                    "original_message_send_time": time,
+                    "quoted_message_id": message_id,
+                    "quoted_message_send_time": time,
+                },
+            )
+            continue
+        # 非文字 entity 尾随空格，最末除外
+        space = "" if i == len(text_entities) - 1 else " "
+        if isinstance(entity, Text):
+            text = str(entity)
+            length = len(text)
+        else:
+            text = f"{await entity.get_text(bot)}{space}"
+            length = _c(text)
+            entities.append(
+                {
+                    "entity": {"type": entity.type_, **entity.__dict__},
+                    "length": length,
+                    "offset": offset,
+                },
+            )
+            if mention := entity.get_mention():
+                type_, id_ = mention
+                if mentioned_info is None:
+                    user_id_list = []
+                    mentioned_info = cast(
+                        MentionedInfo,
+                        {"type": type_, "userIdList": user_id_list},
+                    )
+                else:
+                    if mentioned_info["type"] != 1:
+                        mentioned_info["type"] = type_
+                    user_id_list = mentioned_info["userIdList"]
+                if type_ != 1:
+                    user_id_list.append(id_)
+        offset += len(text)
+        texts.append(text)
+    return {
+        "content": TextMsgContent("".join(texts), entities),
+        "quote": quote,
+        "mentionedInfo": mentioned_info,
+    }
```

### Comparing `herta_villa_sdk-0.1.0/hertavilla/model.py` & `herta_villa_sdk-0.2.0/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.1.0/hertavilla/server.py` & `herta_villa_sdk-0.2.0/hertavilla/server.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.1.0/pyproject.toml` & `herta_villa_sdk-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "herta-villa-sdk"
-version = "0.1.0"
+version = "0.2.0"
 description = "大别野「黑塔」Python SDK"
 authors = [
     { name = "MingxuanGame", email = "MingxuanGame@outlook.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.4",
     "pydantic>=1.10.8",
```

