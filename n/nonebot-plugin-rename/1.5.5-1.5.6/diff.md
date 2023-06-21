# Comparing `tmp/nonebot_plugin_rename-1.5.5.tar.gz` & `tmp/nonebot_plugin_rename-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.5.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.5.6.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.5.5.tar` & `nonebot_plugin_rename-1.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/LICENSE
--rw-r--r--   0        0        0     5775 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/README.md
--rw-r--r--   0        0        0      550 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      479 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/exam_time.py
--rw-r--r--   0        0        0      689 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0     1161 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      450 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0     1500 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/mhy_time.py
--rw-r--r--   0        0        0      607 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      307 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      697 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/year_time.py
--rw-r--r--   0        0        0      551 2023-06-21 06:02:00.870285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0  1878036 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/fonts/draw.ttf
--rw-r--r--   0        0        0     8733 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      264 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      970 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1528 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      400 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      700 2023-06-21 06:02:00.886285 nonebot_plugin_rename-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     6680 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/LICENSE
+-rw-r--r--   0        0        0     6090 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/README.md
+-rw-r--r--   0        0        0      550 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/exam_time.py
+-rw-r--r--   0        0        0      689 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0     1274 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      450 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0     1500 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/mhy_time.py
+-rw-r--r--   0        0        0      607 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      307 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      697 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/year_time.py
+-rw-r--r--   0        0        0      593 2023-06-21 06:24:10.017716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-06-21 06:24:10.033716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8733 2023-06-21 06:24:10.037716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      264 2023-06-21 06:24:10.037716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-21 06:24:10.037716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      970 2023-06-21 06:24:10.037716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1528 2023-06-21 06:24:10.037716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      400 2023-06-21 06:24:10.037716 nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      700 2023-06-21 06:24:10.037716 nonebot_plugin_rename-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     6995 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.5.6/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.5.5/LICENSE` & `nonebot_plugin_rename-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/README.md` & `nonebot_plugin_rename-1.5.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   * [🔐许可](#许可)
   * [💿 安装方法](#-安装方法)
   * [🏷️插件命令](#插件命令)
   * [⚙️插件配置项](#插件配置项)
   * [🎉目前已实现的群名片功能](#目前已实现的群名片功能)
   * [🧐PR需知](#pr需知)
   * [🔥鸣谢](#鸣谢)
-<!-- TOC -->
+  <!-- TOC -->
 
 ## 📖简介
 
 通过定时任务更改bot(s)所在群自己的群名片
 
 ## 🔐许可
 
@@ -76,39 +76,40 @@
 | 查看当前群名片    | 查看当前群名片的设置                       |
 | 立即更改群名片 序号 | 立即更改当前群组bot名片，后面仅可跟一个序号（bot无返回值） |
 | 删除群名片      | 删除当前群组群名片                        |
 | 设置所有群名片    | 为当前机器人所在所有群设置群名片，仅限超管私聊          |
 
 ## ⚙️插件配置项
 
-| 配置项                           | 描述                          | 类型   |
-|-------------------------------|-----------------------------|------|
-| set_group_card_hour           | 间隔时间(小时)                    | int  |
-| set_group_card_minute         | 间隔时间(分钟)                    | int  |
-| use_nickname_front            | 是否在群名片前加上bot名称              | bool |
-| self_name                     | 自定义前缀(需开启上一个配置)             | str  |
-| is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
- | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
- | zk_time_start                 | 中考开始时间                    | str  |
- | zk_time_end                   | 中考结束时间                    | str  |
+| 配置项                           | 描述                          | 类型   | 默认值            |
+|-------------------------------|-----------------------------|------|----------------|
+| set_group_card_hour           | 间隔时间(小时)                    | int  | 0              |
+| set_group_card_minute         | 间隔时间(分钟)                    | int  | 30             |
+| use_nickname_front            | 是否在群名片前加上bot名称              | bool | True           |
+| self_name                     | 自定义前缀(需开启上一个配置)             | str  | None           |
+| is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool | False          |
+| is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool | True           |
+| is_show_hot_search_from       | 热搜是否显示来源                    | bool | False          |
+| zk_time_start                 | 中考开始时间                      | str  | 06-12 09:00:00 |
+| zk_time_end                   | 中考结束时间                      | str  | 06-14 11:00:00 |
 
 **如果要使用中考剩余时间，由于每个地方中考时间并不统一，请务必填写`zk_time`系列配置项，否则获取的时间并不是你们当地的中考时间节点（开始和结束时间），参考配置如下**
 ```dotenv
 zk_time_start="06-12 09:00:00"
 zk_time_end="06-14 11:00:00"
 ```
 
 **请注意不要将`set_group_card_hour`和`set_group_card_minute`都设为0**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
 <summary>一图流</summary>
-<img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230610/image.2cyi74rq30kk.png" alt="help">
+<img src="https://jsd.cdn.zzko.cn/gh/forchannot/mypicgo@main/20230621/e467ea4da8e8bd2c1a30b40daf660c11.14n3cusfflr4.webp" alt="help">
 </details>
 
 <details>
 <summary>时间</summary>
 <pre>
 -- 高考时间
 -- 中考时间
@@ -120,15 +121,15 @@
 </details>
 
 <details>
 <summary>热搜</summary>
 <pre>
 -- B站热搜
 -- 微博热搜
--- 抖音热搜
+-- 腾讯新闻热搜
 -- 百度热搜
 -- 知乎热搜
 -- 今日头条热搜
 </pre>
 </details>
 
 <details>
```

#### html2text {}

```diff
@@ -21,39 +21,41 @@
 è®¾ç½®ç¾¤åç åºå·(éç©ºæ ¼ï¼å¯å¸¦å¤ä¸ªåºå·) | |
 æ¥çç¾¤åçåè¡¨ | æ¥çå½åæ¯æçææç¾¤åçåè¡¨çå¾ç | |
 æ¥çå½åç¾¤åç | æ¥çå½åç¾¤åççè®¾ç½® | |
 ç«å³æ´æ¹ç¾¤åç åºå· |
 ç«å³æ´æ¹å½åç¾¤ç»botåçï¼åé¢ä»å¯è·ä¸ä¸ªåºå·ï¼botæ è¿åå¼ï¼
 | | å é¤ç¾¤åç | å é¤å½åç¾¤ç»ç¾¤åç | | è®¾ç½®ææç¾¤åç |
 ä¸ºå½åæºå¨äººæå¨ææç¾¤è®¾ç½®ç¾¤åçï¼ä»éè¶ç®¡ç§è | ##
-âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | |------------------------
--------|-----------------------------|------| | set_group_card_hour |
-é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
-int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
-self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
+âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | é»è®¤å¼ | |------------
+-------------------|-----------------------------|------|----------------| |
+set_group_card_hour | é´éæ¶é´(å°æ¶) | int | 0 | | set_group_card_minute
+| é´éæ¶é´(åé) | int | 30 | | use_nickname_front |
+æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | True | | self_name |
+èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | None | |
 is_one_bot_set_all_group_card |
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
-| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool | |
-zk_time_start | ä¸­èå¼å§æ¶é´ | str | | zk_time_end | ä¸­èç»ææ¶é´ |
-str |
+False | | is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ |
+bool | True | | is_show_hot_search_from | ç­ææ¯å¦æ¾ç¤ºæ¥æº | bool |
+False | | zk_time_start | ä¸­èå¼å§æ¶é´ | str | 06-12 09:00:00 | |
+zk_time_end | ä¸­èç»ææ¶é´ | str | 06-14 11:00:00 |
 **å¦æè¦ä½¿ç¨ä¸­èå©ä½æ¶é´ï¼ç±äºæ¯ä¸ªå°æ¹ä¸­èæ¶é´å¹¶ä¸ç»ä¸ï¼è¯·å¡å¿å¡«å`zk_time`ç³»åéç½®é¡¹ï¼å¦åè·åçæ¶é´å¹¶ä¸æ¯ä½ ä»¬å½å°çä¸­èæ¶é´èç¹ï¼å¼å§åç»ææ¶é´ï¼ï¼åèéç½®å¦ä¸**
 ```dotenv zk_time_start="06-12 09:00:00" zk_time_end="06-14 11:00:00" ```
 **è¯·æ³¨æä¸è¦å°`set_group_card_hour`å`set_group_card_minute`é½è®¾ä¸º0**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- ä¸­èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
 -- æéçæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
   ç­æ
 -- Bç«ç­æ
 -- å¾®åç­æ
--- æé³ç­æ
+-- è¾è®¯æ°é»ç­æ
 -- ç¾åº¦ç­æ
 -- ç¥ä¹ç­æ
 -- ä»æ¥å¤´æ¡ç­æ
   ä¸è¨
 -- æ¯æ¥(æ¬¡)ä¸è¨
   ç³»ç»ç¶æ
 -- ç³»ç»åå­åcpuä¿¡æ¯
```

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/__init__.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot.plugin import PluginMetadata
 
 from .config import env_config
 from .main import *  # noqa
 
-__version__ = "1.5.5"
+__version__ = "1.5.6"
 __plugin_meta__ = PluginMetadata(
     name="nonebot_plugin_rename",
     description="用于更改qq机器人的群名片，内置多种有趣名片",
     usage="查看本仓库readme",
     supported_adapters={"~onebot.v11"},
     type="application",
     config=env_config,
```

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/exam_time.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/exam_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/hot_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # Description: 获取热搜
 
 import random
-from typing import Optional
 
 import httpx
 from nonebot import logger
 
+from ..config import env_config
+
 # URL = {
 #     "1": "https://tenapi.cn/v2/bilihot/",  # B站
 #     "2": "https://tenapi.cn/v2/weibohot",  # 微博
 #     "3": "https://tenapi.cn/v2/douyinhot",  # 抖音
 #     "4": "https://tenapi.cn/v2/baiduhot/",  # 百度
 #     "5": "https://tenapi.cn/v2/zhihuhot",  # 知乎
 #     "6": "https://tenapi.cn/v2/toutiaohot",  # 今日头条
 # }
 URL = {
-    "1": "bilibili",  # B站
-    "2": "weibo",  # 微博
-    "3": "newsqq",  # 腾讯新闻
-    "4": "baidu",  # 百度
-    "5": "zhihu",  # 知乎
-    "6": "toutiao",  # 今日头条
+    "1": ("bilibili", "B站"),  # B站
+    "2": ("weibo", "微博"),  # 微博
+    "3": ("newsqq", "腾讯"),  # 腾讯新闻
+    "4": ("baidu", "百度"),  # 百度
+    "5": ("zhihu", "知乎"),  # 知乎
+    "6": ("toutiao", "头条"),  # 今日头条
 }
 
 
-async def hot(num: int) -> Optional[str]:
+async def hot(num: int) -> str:
     async with httpx.AsyncClient(follow_redirects=True) as client:
         try:
-            res = await client.get(f"https://hot.zhenxun.buzz/{URL[str(num)]}")
-            if res.status_code != 200:
-                return "热搜api失效"
+            res = await client.get(f"https://hot.zhenxun.buzz/{URL[str(num)][0]}")
             data = res.json()["data"]
             result = random.choice(data)["title"]
+            if env_config.is_show_hot_search_from:
+                result = f"{URL[str(num)][1]}：{result}"
             return result
         except Exception as e:
             logger.warning(f"获取热搜失败: {e}")
-            return None
+            return "热搜获取失败"
```

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/mhy_time.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/mhy_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/card/year_time.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/card/year_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/config.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pydantic import BaseModel, Extra
 
 
 class Config(BaseModel, extra=Extra.ignore):
     set_group_card_hour: int = 0
     set_group_card_minute: int = 30
     use_nickname_front: bool = True
+    is_show_hot_search_from: bool = False
     self_name: Optional[str] = None
     is_one_bot_set_all_group_card: bool = False
     is_show_aps_info_log: bool = True
     zk_time_start: str = "06-12 09:00:00"
     zk_time_end: str = "06-14 11:00:00"
```

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/fonts/draw.ttf` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/fonts/draw.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.5.6/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.5.5/pyproject.toml` & `nonebot_plugin_rename-1.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.5.5"
+version = "1.5.6"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
```

### Comparing `nonebot_plugin_rename-1.5.5/PKG-INFO` & `nonebot_plugin_rename-1.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.5.5
+Version: 1.5.6
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -49,15 +49,15 @@
   * [🔐许可](#许可)
   * [💿 安装方法](#-安装方法)
   * [🏷️插件命令](#插件命令)
   * [⚙️插件配置项](#插件配置项)
   * [🎉目前已实现的群名片功能](#目前已实现的群名片功能)
   * [🧐PR需知](#pr需知)
   * [🔥鸣谢](#鸣谢)
-<!-- TOC -->
+  <!-- TOC -->
 
 ## 📖简介
 
 通过定时任务更改bot(s)所在群自己的群名片
 
 ## 🔐许可
 
@@ -99,39 +99,40 @@
 | 查看当前群名片    | 查看当前群名片的设置                       |
 | 立即更改群名片 序号 | 立即更改当前群组bot名片，后面仅可跟一个序号（bot无返回值） |
 | 删除群名片      | 删除当前群组群名片                        |
 | 设置所有群名片    | 为当前机器人所在所有群设置群名片，仅限超管私聊          |
 
 ## ⚙️插件配置项
 
-| 配置项                           | 描述                          | 类型   |
-|-------------------------------|-----------------------------|------|
-| set_group_card_hour           | 间隔时间(小时)                    | int  |
-| set_group_card_minute         | 间隔时间(分钟)                    | int  |
-| use_nickname_front            | 是否在群名片前加上bot名称              | bool |
-| self_name                     | 自定义前缀(需开启上一个配置)             | str  |
-| is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
- | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
- | zk_time_start                 | 中考开始时间                    | str  |
- | zk_time_end                   | 中考结束时间                    | str  |
+| 配置项                           | 描述                          | 类型   | 默认值            |
+|-------------------------------|-----------------------------|------|----------------|
+| set_group_card_hour           | 间隔时间(小时)                    | int  | 0              |
+| set_group_card_minute         | 间隔时间(分钟)                    | int  | 30             |
+| use_nickname_front            | 是否在群名片前加上bot名称              | bool | True           |
+| self_name                     | 自定义前缀(需开启上一个配置)             | str  | None           |
+| is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool | False          |
+| is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool | True           |
+| is_show_hot_search_from       | 热搜是否显示来源                    | bool | False          |
+| zk_time_start                 | 中考开始时间                      | str  | 06-12 09:00:00 |
+| zk_time_end                   | 中考结束时间                      | str  | 06-14 11:00:00 |
 
 **如果要使用中考剩余时间，由于每个地方中考时间并不统一，请务必填写`zk_time`系列配置项，否则获取的时间并不是你们当地的中考时间节点（开始和结束时间），参考配置如下**
 ```dotenv
 zk_time_start="06-12 09:00:00"
 zk_time_end="06-14 11:00:00"
 ```
 
 **请注意不要将`set_group_card_hour`和`set_group_card_minute`都设为0**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
 <summary>一图流</summary>
-<img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230610/image.2cyi74rq30kk.png" alt="help">
+<img src="https://jsd.cdn.zzko.cn/gh/forchannot/mypicgo@main/20230621/e467ea4da8e8bd2c1a30b40daf660c11.14n3cusfflr4.webp" alt="help">
 </details>
 
 <details>
 <summary>时间</summary>
 <pre>
 -- 高考时间
 -- 中考时间
@@ -143,15 +144,15 @@
 </details>
 
 <details>
 <summary>热搜</summary>
 <pre>
 -- B站热搜
 -- 微博热搜
--- 抖音热搜
+-- 腾讯新闻热搜
 -- 百度热搜
 -- 知乎热搜
 -- 今日头条热搜
 </pre>
 </details>
 
 <details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.5.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.5.6 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
@@ -33,39 +33,41 @@
 è®¾ç½®ç¾¤åç åºå·(éç©ºæ ¼ï¼å¯å¸¦å¤ä¸ªåºå·) | |
 æ¥çç¾¤åçåè¡¨ | æ¥çå½åæ¯æçææç¾¤åçåè¡¨çå¾ç | |
 æ¥çå½åç¾¤åç | æ¥çå½åç¾¤åççè®¾ç½® | |
 ç«å³æ´æ¹ç¾¤åç åºå· |
 ç«å³æ´æ¹å½åç¾¤ç»botåçï¼åé¢ä»å¯è·ä¸ä¸ªåºå·ï¼botæ è¿åå¼ï¼
 | | å é¤ç¾¤åç | å é¤å½åç¾¤ç»ç¾¤åç | | è®¾ç½®ææç¾¤åç |
 ä¸ºå½åæºå¨äººæå¨ææç¾¤è®¾ç½®ç¾¤åçï¼ä»éè¶ç®¡ç§è | ##
-âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | |------------------------
--------|-----------------------------|------| | set_group_card_hour |
-é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
-int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
-self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
+âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | é»è®¤å¼ | |------------
+-------------------|-----------------------------|------|----------------| |
+set_group_card_hour | é´éæ¶é´(å°æ¶) | int | 0 | | set_group_card_minute
+| é´éæ¶é´(åé) | int | 30 | | use_nickname_front |
+æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | True | | self_name |
+èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | None | |
 is_one_bot_set_all_group_card |
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
-| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool | |
-zk_time_start | ä¸­èå¼å§æ¶é´ | str | | zk_time_end | ä¸­èç»ææ¶é´ |
-str |
+False | | is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ |
+bool | True | | is_show_hot_search_from | ç­ææ¯å¦æ¾ç¤ºæ¥æº | bool |
+False | | zk_time_start | ä¸­èå¼å§æ¶é´ | str | 06-12 09:00:00 | |
+zk_time_end | ä¸­èç»ææ¶é´ | str | 06-14 11:00:00 |
 **å¦æè¦ä½¿ç¨ä¸­èå©ä½æ¶é´ï¼ç±äºæ¯ä¸ªå°æ¹ä¸­èæ¶é´å¹¶ä¸ç»ä¸ï¼è¯·å¡å¿å¡«å`zk_time`ç³»åéç½®é¡¹ï¼å¦åè·åçæ¶é´å¹¶ä¸æ¯ä½ ä»¬å½å°çä¸­èæ¶é´èç¹ï¼å¼å§åç»ææ¶é´ï¼ï¼åèéç½®å¦ä¸**
 ```dotenv zk_time_start="06-12 09:00:00" zk_time_end="06-14 11:00:00" ```
 **è¯·æ³¨æä¸è¦å°`set_group_card_hour`å`set_group_card_minute`é½è®¾ä¸º0**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- ä¸­èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
 -- æéçæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
   ç­æ
 -- Bç«ç­æ
 -- å¾®åç­æ
--- æé³ç­æ
+-- è¾è®¯æ°é»ç­æ
 -- ç¾åº¦ç­æ
 -- ç¥ä¹ç­æ
 -- ä»æ¥å¤´æ¡ç­æ
   ä¸è¨
 -- æ¯æ¥(æ¬¡)ä¸è¨
   ç³»ç»ç¶æ
 -- ç³»ç»åå­åcpuä¿¡æ¯
```

