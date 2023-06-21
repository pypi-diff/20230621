# Comparing `tmp/nonebot_plugin_7s_roll-0.2.0a1.tar.gz` & `tmp/nonebot_plugin_7s_roll-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_7s_roll-0.2.0a1.tar", max compression
+gzip compressed data, was "nonebot_plugin_7s_roll-0.2.0a2.tar", max compression
```

## Comparing `nonebot_plugin_7s_roll-0.2.0a1.tar` & `nonebot_plugin_7s_roll-0.2.0a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1059 2023-06-15 14:37:09.263085 nonebot_plugin_7s_roll-0.2.0a1/LICENSE
--rw-r--r--   0        0        0      317 2023-06-15 15:20:26.275167 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/__init__.py
--rw-r--r--   0        0        0     2067 2023-06-15 15:16:46.889258 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/command.py
--rw-r--r--   0        0        0      212 2023-06-15 15:04:46.601369 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/common.py
--rw-r--r--   0        0        0      178 2023-06-15 14:37:09.264086 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/config.py
--rw-r--r--   0        0        0     5736 2023-06-15 15:12:01.427116 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/expr.py
--rw-r--r--   0        0        0     2003 2023-06-15 14:37:09.265086 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/roll.py
--rw-r--r--   0        0        0     1123 2023-06-15 15:20:50.587710 nonebot_plugin_7s_roll-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     1701 2023-06-15 14:38:13.472977 nonebot_plugin_7s_roll-0.2.0a1/README.md
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 nonebot_plugin_7s_roll-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-15 14:37:09.263085 nonebot_plugin_7s_roll-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0      317 2023-06-15 16:06:13.014479 nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/__init__.py
+-rw-r--r--   0        0        0     2108 2023-06-15 16:05:28.659183 nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/command.py
+-rw-r--r--   0        0        0      212 2023-06-15 15:04:46.601369 nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/common.py
+-rw-r--r--   0        0        0      178 2023-06-15 14:37:09.264086 nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/config.py
+-rw-r--r--   0        0        0     5736 2023-06-15 15:12:01.427116 nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/expr.py
+-rw-r--r--   0        0        0     2132 2023-06-15 16:04:18.995280 nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/roll.py
+-rw-r--r--   0        0        0     1157 2023-06-15 16:06:16.760147 nonebot_plugin_7s_roll-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1701 2023-06-15 14:38:13.472977 nonebot_plugin_7s_roll-0.2.0a2/README.md
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 nonebot_plugin_7s_roll-0.2.0a2/PKG-INFO
```

### Comparing `nonebot_plugin_7s_roll-0.2.0a1/LICENSE` & `nonebot_plugin_7s_roll-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/command.py` & `nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/command.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from typing import Annotated
 
+import nonebot.adapters.onebot.v11 as onebot11
 from nonebot import on_command, on_message
 from nonebot.adapters import Event
 from nonebot.consts import REGEX_MATCHED
 from nonebot.log import logger
 from nonebot.params import EventPlainText
 from nonebot.rule import regex
 from nonebot.typing import T_State
@@ -20,44 +21,43 @@
     + CONF.i7s_roll_trigger
     #      2                     3  4      5                                    6
     + r" )([0-9adgimnsuvx+\- ]+)( ?(结果)?(大于|小于|大于等于|小于等于|>=|>|<|<=) ?(-?\d{1,10}))?"
 )
 
 RE_ROLL_CMD = re.compile(RE_ROLL_STR)
 
-
 async def roll_command_handler(event: Event, msg: Annotated[str, EventPlainText()], state: T_State):
-    messages = []
+    messages = onebot11.Message() 
 
     logger.info(f"[7sRoll] received roll command: {msg}")
 
-    if event.get_event_name().startswith("message.group"): # onebot v11
-        messages.append(f"[CQ:at,qq={event.user_id}]") # type: ignore
+    if isinstance(event, onebot11.GroupMessageEvent):
+        messages.append(onebot11.MessageSegment.at(event.user_id))
+        messages.append('\n')
 
     match = None
     if REGEX_MATCHED in state:
         match = state[REGEX_MATCHED]
     else:
         args = msg.strip()
         match = RE_ROLL_CMD.match(args)
         if not match:
-            messages.append("roll 命令格式错误")
-            messages.append("格式为：roll <表达式>[ <判断方式><目标>]")
-            messages.append("表达式举例：3d6+1d3-1")
-            messages.append("判断方式可选：>, <, <=, >=, 或对应中文")
+            messages.append("roll 命令格式错误\n")
+            messages.append("格式为：roll <表达式>[ <判断方式><目标>]\n")
+            messages.append("表达式举例：3d6+1d3-1\n")
+            messages.append("判断方式可选：>, <, <=, >=, 或对应中文\n")
             messages.append("目标：需要达成的点数")
-            return await cmd_roll.finish("\n".join(messages))
-        if match.group(1) is None:
+        elif match.group(1) is None:
             return
 
-    expr_str, op_str, target = match.group(2, 5, 6)
-
-    messages.extend(roll(expr_str, op_str, target))
+    if match:
+        expr_str, op_str, target = match.group(2, 5, 6)
+        messages.append('\n'.join(roll(expr_str, op_str, target)))
 
-    return await cmd_roll.finish("\n".join(messages))
+    return await cmd_roll.finish(messages)
 
 
 cmd_roll = on_command(CONF.i7s_roll_command, priority=1, block=True)
 cmd_roll.handle()(roll_command_handler)
 
 message_cmd_roll = on_message(rule=regex(RE_ROLL_STR), priority=2, block=True)
 message_cmd_roll.handle()(roll_command_handler)
```

### Comparing `nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/expr.py` & `nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/expr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/roll.py` & `nonebot_plugin_7s_roll-0.2.0a2/nonebot_plugin_7s_roll/roll.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-import re
 import operator
+from typing import List, Optional
 
-from .expr import compile, Roll
+from .expr import Roll, compile
 
 OP_MAP = {
     ">": operator.gt,
     ">=": operator.ge,
     "<": operator.lt,
     "<=": operator.le,
     "大于": operator.gt,
     "大于等于": operator.ge,
     "小于": operator.lt,
     "小于等于": operator.le,
 }
 
 
-def roll(expr_str: str, op_str: str = None, target_str: str = None) -> [str]:
+def roll(expr_str: str, op_str: Optional[str] = None, target_str: Optional[str] = None) -> List[str]:
     messages = []
 
     try:
         expr = compile(expr_str)
     except:
         expr = None
 
     if expr is None:
         messages.append("roll 命令表达式错误")
         messages.append("表达式举例：3d6+1d3-1")
         return messages
 
-    op = None
+    op = target = None
     if op_str:
         op = OP_MAP[op_str]
+        assert(target_str is not None)
         target = int(target_str)
 
     message = [f"{expr_str.strip()} 投掷结果"]
     if op:
         message.append(f"(目标 {op_str} {target})：")
     messages.append("".join(message))
 
@@ -44,34 +45,34 @@
         roll: Roll = expr
         dices = roll.values
 
         messages.append("")
 
         for i, dice in enumerate(dices):
             message = [f"第 {i+1} 颗：{dice}"]
-            if op:
+            if op and target:
                 if op(dice, target):
                     message.append("，通过")
                 else:
                     message.append("，未通过")
             messages.append("".join(message))
 
         if len(dices) > 1:
             prefix = roll.post_processor.prefix
             messages.append("")
             message = [f"{prefix} {result}"]
-            if op:
+            if op and target:
                 if op(result, target):
                     message.append("，通过")
                 else:
                     message.append("，未通过")
             messages.append("".join(message))
     else:
         message = [display, " = ", str(result)]
-        if op:
+        if op and target:
             if op(result, target):
                 message.append("，通过")
             else:
                 message.append("，未通过")
         messages.append("".join(message))
 
     return messages
```

### Comparing `nonebot_plugin_7s_roll-0.2.0a1/pyproject.toml` & `nonebot_plugin_7s_roll-0.2.0a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-7s-roll"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "A roll dice plugin for nonebot"
 authors = ["7sDream <i@7sdre.am>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/7sDream/nonebot_plugin_7s_roll"
 repository = "https://github.com/7sDream/nonebot_plugin_7s_roll"
 keywords = ["nonebot", "dice", "roll", "trpg"]
@@ -21,14 +21,15 @@
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
+nonebot-adapter-onebot = "^2.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 black = "^23.3.0"
 rope = "^1.8.0"
 pytest = "^7.3.2"
 nonebot-adapter-console = "^0.3.2"
```

### Comparing `nonebot_plugin_7s_roll-0.2.0a1/README.md` & `nonebot_plugin_7s_roll-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_7s_roll-0.2.0a1/PKG-INFO` & `nonebot_plugin_7s_roll-0.2.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-7s-roll
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A roll dice plugin for nonebot
 Home-page: https://github.com/7sDream/nonebot_plugin_7s_roll
 License: MIT
 Keywords: nonebot,dice,roll,trpg
 Author: 7sDream
 Author-email: i@7sdre.am
 Requires-Python: >=3.9,<4.0
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/7sDream/nonebot_plugin_7s_roll
 Description-Content-Type: text/markdown
 
 # Roll Dice
 
 扔骰子小工具。
```

