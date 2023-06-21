# Comparing `tmp/nonebot_plugin_rename-1.5.1.tar.gz` & `tmp/nonebot_plugin_rename-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.5.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.5.5.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.5.1.tar` & `nonebot_plugin_rename-1.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/LICENSE
--rw-r--r--   0        0        0     5790 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/README.md
--rw-r--r--   0        0        0      550 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      479 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/exam_time.py
--rw-r--r--   0        0        0      689 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      450 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0     1500 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/mhy_time.py
--rw-r--r--   0        0        0      607 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      604 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      697 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/year_time.py
--rw-r--r--   0        0        0      551 2023-06-10 13:40:51.972372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0  1878036 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/fonts/draw.ttf
--rw-r--r--   0        0        0     8723 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      264 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      964 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1528 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      400 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      700 2023-06-10 13:40:51.988372 nonebot_plugin_rename-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     6695 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/LICENSE
+-rw-r--r--   0        0        0     5775 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/README.md
+-rw-r--r--   0        0        0      550 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/exam_time.py
+-rw-r--r--   0        0        0      689 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0     1161 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      450 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0     1500 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/mhy_time.py
+-rw-r--r--   0        0        0      607 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      307 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      697 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/year_time.py
+-rw-r--r--   0        0        0      551 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8733 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      264 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      970 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1528 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      400 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      700 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6680 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.5.5/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.5.1/LICENSE` & `nonebot_plugin_rename-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/README.md` & `nonebot_plugin_rename-1.5.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 |-------------------------------|-----------------------------|------|
 | set_group_card_hour           | 间隔时间(小时)                    | int  |
 | set_group_card_minute         | 间隔时间(分钟)                    | int  |
 | use_nickname_front            | 是否在群名片前加上bot名称              | bool |
 | self_name                     | 自定义前缀(需开启上一个配置)             | str  |
 | is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
  | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
- | zk_time_start                 | 设置当地中考时间                    | str  |
-    | zk_time_end                   | 设置当地中考时间                    | str  |
+ | zk_time_start                 | 中考开始时间                    | str  |
+ | zk_time_end                   | 中考结束时间                    | str  |
 
 **如果要使用中考剩余时间，由于每个地方中考时间并不统一，请务必填写`zk_time`系列配置项，否则获取的时间并不是你们当地的中考时间节点（开始和结束时间），参考配置如下**
 ```dotenv
 zk_time_start="06-12 09:00:00"
 zk_time_end="06-14 11:00:00"
 ```
```

#### html2text {}

```diff
@@ -29,16 +29,16 @@
 -------|-----------------------------|------| | set_group_card_hour |
 é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
 int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
 self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
 is_one_bot_set_all_group_card |
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
 | is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool | |
-zk_time_start | è®¾ç½®å½å°ä¸­èæ¶é´ | str | | zk_time_end |
-è®¾ç½®å½å°ä¸­èæ¶é´ | str |
+zk_time_start | ä¸­èå¼å§æ¶é´ | str | | zk_time_end | ä¸­èç»ææ¶é´ |
+str |
 **å¦æè¦ä½¿ç¨ä¸­èå©ä½æ¶é´ï¼ç±äºæ¯ä¸ªå°æ¹ä¸­èæ¶é´å¹¶ä¸ç»ä¸ï¼è¯·å¡å¿å¡«å`zk_time`ç³»åéç½®é¡¹ï¼å¦åè·åçæ¶é´å¹¶ä¸æ¯ä½ ä»¬å½å°çä¸­èæ¶é´èç¹ï¼å¼å§åç»ææ¶é´ï¼ï¼åèéç½®å¦ä¸**
 ```dotenv zk_time_start="06-12 09:00:00" zk_time_end="06-14 11:00:00" ```
 **è¯·æ³¨æä¸è¦å°`set_group_card_hour`å`set_group_card_minute`é½è®¾ä¸º0**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- ä¸­èæ¶é´
```

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/__init__.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot.plugin import PluginMetadata
 
 from .config import env_config
 from .main import *  # noqa
 
-__version__ = "1.5.1"
+__version__ = "1.5.5"
 __plugin_meta__ = PluginMetadata(
     name="nonebot_plugin_rename",
     description="用于更改qq机器人的群名片，内置多种有趣名片",
     usage="查看本仓库readme",
     supported_adapters={"~onebot.v11"},
     type="application",
     config=env_config,
```

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/exam_time.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/exam_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/hot_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 
 import random
 from typing import Optional
 
 import httpx
 from nonebot import logger
 
+# URL = {
+#     "1": "https://tenapi.cn/v2/bilihot/",  # B站
+#     "2": "https://tenapi.cn/v2/weibohot",  # 微博
+#     "3": "https://tenapi.cn/v2/douyinhot",  # 抖音
+#     "4": "https://tenapi.cn/v2/baiduhot/",  # 百度
+#     "5": "https://tenapi.cn/v2/zhihuhot",  # 知乎
+#     "6": "https://tenapi.cn/v2/toutiaohot",  # 今日头条
+# }
 URL = {
-    "1": "https://tenapi.cn/v2/bilihot/",  # B站
-    "2": "https://tenapi.cn/v2/weibohot",  # 微博
-    "3": "https://tenapi.cn/v2/douyinhot",  # 抖音
-    "4": "https://tenapi.cn/v2/baiduhot/",  # 百度
-    "5": "https://tenapi.cn/v2/zhihuhot",  # 知乎
-    "6": "https://tenapi.cn/v2/toutiaohot",  # 今日头条
+    "1": "bilibili",  # B站
+    "2": "weibo",  # 微博
+    "3": "newsqq",  # 腾讯新闻
+    "4": "baidu",  # 百度
+    "5": "zhihu",  # 知乎
+    "6": "toutiao",  # 今日头条
 }
 
 
 async def hot(num: int) -> Optional[str]:
     async with httpx.AsyncClient(follow_redirects=True) as client:
         try:
-            res = await client.get(URL[str(num)])
+            res = await client.get(f"https://hot.zhenxun.buzz/{URL[str(num)]}")
             if res.status_code != 200:
                 return "热搜api失效"
             data = res.json()["data"]
-            result = random.choice(data)["name"]
-            return result[:16]
+            result = random.choice(data)["title"]
+            return result
         except Exception as e:
             logger.warning(f"获取热搜失败: {e}")
             return None
```

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/mhy_time.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/mhy_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/card/year_time.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/year_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/config.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/fonts/draw.ttf` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/fonts/draw.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     elif card_number not in map(str, range(1, len(card_list) + 1)):
         await set_card_now.finish("没有这种类型的群名片哦，可以发送[查看群名片列表]命令查看吧")
     card_names = await choice_card(card_number)
     if env_config.use_nickname_front:
         card_names = f"{NICKNAME}|{card_names}"
     try:
         await bot.set_group_card(
-            group_id=event.group_id, user_id=int(bot.self_id), card=card_names
+            group_id=event.group_id, user_id=int(bot.self_id), card=card_names[:20]
         )
         logger.info(f"群组{event.group_id}成功设置名片 >> {card_names}")
     except (AttributeError, ActionFailed):
         logger.warning("更改群名片失败，可能是机器人不存在或被风控")
 
 
 # on_command "删除群名片"
@@ -208,15 +208,15 @@
         if env_config.use_nickname_front:
             card_names = f"{NICKNAME}|{card_names}"
         if card_names:
             tasks.append(
                 bot_case.set_group_card(
                     group_id=group_id,
                     user_id=int(bot_id),
-                    card=card_names,
+                    card=card_names[:20],
                 )
             )
             if env_config.is_show_aps_info_log:
                 logger.info(f"即将为群{group_id}的bot设置群名片后缀{card_names}")
     return tasks
```

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/card_name.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 card_list = {
     "1": ("每日一言", get_one_speak),
     "2": ("北京时间(小时)", now_time),
     "3": ("当前时间(古代计时制)", old_time),
     "4": ("B站热搜", hot),
     "5": ("微博热搜", hot),
-    "6": ("抖音热搜", hot),
+    "6": ("腾讯新闻热搜", hot),
     "7": ("百度热搜", hot),
     "8": ("知乎热搜", hot),
     "9": ("今日头条热搜", hot),
     "10": ("原神版本剩余时间", genshin),
     "11": ("崩铁版本剩余时间", starrail),
     "12": ("bot系统运行状态", system_status),
     "13": ("bot收发消息统计", get_msg),
```

### Comparing `nonebot_plugin_rename-1.5.1/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.1/pyproject.toml` & `nonebot_plugin_rename-1.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.5.1"
+version = "1.5.5"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
```

### Comparing `nonebot_plugin_rename-1.5.1/PKG-INFO` & `nonebot_plugin_rename-1.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.5.1
+Version: 1.5.5
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -107,16 +107,16 @@
 |-------------------------------|-----------------------------|------|
 | set_group_card_hour           | 间隔时间(小时)                    | int  |
 | set_group_card_minute         | 间隔时间(分钟)                    | int  |
 | use_nickname_front            | 是否在群名片前加上bot名称              | bool |
 | self_name                     | 自定义前缀(需开启上一个配置)             | str  |
 | is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
  | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
- | zk_time_start                 | 设置当地中考时间                    | str  |
-    | zk_time_end                   | 设置当地中考时间                    | str  |
+ | zk_time_start                 | 中考开始时间                    | str  |
+ | zk_time_end                   | 中考结束时间                    | str  |
 
 **如果要使用中考剩余时间，由于每个地方中考时间并不统一，请务必填写`zk_time`系列配置项，否则获取的时间并不是你们当地的中考时间节点（开始和结束时间），参考配置如下**
 ```dotenv
 zk_time_start="06-12 09:00:00"
 zk_time_end="06-14 11:00:00"
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.5.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.5.5 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
@@ -41,16 +41,16 @@
 -------|-----------------------------|------| | set_group_card_hour |
 é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
 int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
 self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
 is_one_bot_set_all_group_card |
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
 | is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool | |
-zk_time_start | è®¾ç½®å½å°ä¸­èæ¶é´ | str | | zk_time_end |
-è®¾ç½®å½å°ä¸­èæ¶é´ | str |
+zk_time_start | ä¸­èå¼å§æ¶é´ | str | | zk_time_end | ä¸­èç»ææ¶é´ |
+str |
 **å¦æè¦ä½¿ç¨ä¸­èå©ä½æ¶é´ï¼ç±äºæ¯ä¸ªå°æ¹ä¸­èæ¶é´å¹¶ä¸ç»ä¸ï¼è¯·å¡å¿å¡«å`zk_time`ç³»åéç½®é¡¹ï¼å¦åè·åçæ¶é´å¹¶ä¸æ¯ä½ ä»¬å½å°çä¸­èæ¶é´èç¹ï¼å¼å§åç»ææ¶é´ï¼ï¼åèéç½®å¦ä¸**
 ```dotenv zk_time_start="06-12 09:00:00" zk_time_end="06-14 11:00:00" ```
 **è¯·æ³¨æä¸è¦å°`set_group_card_hour`å`set_group_card_minute`é½è®¾ä¸º0**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- ä¸­èæ¶é´
```

