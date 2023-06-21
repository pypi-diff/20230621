# Comparing `tmp/nonebot-plugin-gw2-0.0.1.tar.gz` & `tmp/nonebot_plugin_gw2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-gw2-0.0.1.tar", last modified: Fri Mar 31 17:16:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_gw2-0.0.2.tar", max compression
```

## Comparing `nonebot-plugin-gw2-0.0.1.tar` & `nonebot_plugin_gw2-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 17:16:58.799055 nonebot-plugin-gw2-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-02-08 00:46:07.000000 nonebot-plugin-gw2-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      401 2023-03-31 17:16:58.799055 nonebot-plugin-gw2-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2023-03-31 16:07:20.000000 nonebot-plugin-gw2-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 17:16:58.795069 nonebot-plugin-gw2-0.0.1/nonebot-plugin-gw2/
--rw-rw-rw-   0        0        0      759 2023-03-31 16:04:22.000000 nonebot-plugin-gw2-0.0.1/nonebot-plugin-gw2/__init__.py
--rw-rw-rw-   0        0        0     2779 2023-03-31 16:02:20.000000 nonebot-plugin-gw2-0.0.1/nonebot-plugin-gw2/api.py
-drwxrwxrwx   0        0        0        0 2023-03-31 17:16:58.798063 nonebot-plugin-gw2-0.0.1/nonebot_plugin_gw2.egg-info/
--rw-rw-rw-   0        0        0      401 2023-03-31 17:16:58.000000 nonebot-plugin-gw2-0.0.1/nonebot_plugin_gw2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-03-31 17:16:58.000000 nonebot-plugin-gw2-0.0.1/nonebot_plugin_gw2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 17:16:58.000000 nonebot-plugin-gw2-0.0.1/nonebot_plugin_gw2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-03-31 17:16:58.000000 nonebot-plugin-gw2-0.0.1/nonebot_plugin_gw2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-31 17:16:58.000000 nonebot-plugin-gw2-0.0.1/nonebot_plugin_gw2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      970 2023-03-31 17:14:27.000000 nonebot-plugin-gw2-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-31 17:16:58.800052 nonebot-plugin-gw2-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      691 2023-03-31 17:03:10.000000 nonebot-plugin-gw2-0.0.1/setup.py
+-rw-r--r--   0        0        0     1068 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1714 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/README.md
+-rw-r--r--   0        0        0     3556 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/nonebot_plugin_gw2/__init__.py
+-rw-r--r--   0        0        0     2704 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/nonebot_plugin_gw2/api.py
+-rw-r--r--   0        0        0      949 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 nonebot_plugin_gw2-0.0.2/PKG-INFO
```

### Comparing `nonebot-plugin-gw2-0.0.1/LICENSE` & `nonebot_plugin_gw2-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Diving-Fish
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Diving-Fish
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot-plugin-gw2-0.0.1/README.md` & `nonebot_plugin_gw2-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-<div align="center">
-  <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
-  <br>
-  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot_plugin_gw2
-_✨激战2 星岬岛查询✨_
-
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_gw2/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_gw2" alt="stars">
-</a>
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_gw2//issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_gw2" alt="issues">
-</a>
-<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
-        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_gw2">
-        <img src="https://img.shields.io/pypi/v/nonebot_plugin_gw2/.svg" alt="pypi">
-</a>
-    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
-</div>
-
-## 安装
-
-        pip3 install nonebot_plugin_gw2
-
-## 指令
-| 指令 | 功能 | 备注 |
-|:-----:|:----:|:----:|
-| gw2日常 | 日常信息 | 【gw2日常明日】 可以查看第二天
-| gw2活动 | 空中网活动和近日公告 | 暂无
-| gw2资讯 | 第三方咨询 | 接口暂时不更新... 
-
-## 备注
-本信息数据均来自[激战2 星岬岛](https://gw2.wishingstarmoye.com/gw2api)侵删
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_gw2
+_✨激战2 星岬岛查询✨_
+
+<a href="https://github.com/Agnes4m/nonebot_plugin_gw2/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_gw2" alt="stars">
+</a>
+<a href="https://github.com/Agnes4m/nonebot_plugin_gw2//issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_gw2" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_gw2">
+        <img src="https://img.shields.io/pypi/v/nonebot_plugin_gw2/.svg" alt="pypi">
+</a>
+    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
+</div>
+
+## 安装
+
+以下指令任意一个即可
+
+        pip3 install nonebot_plugin_gw2
+        nb plugin install nonebot_plugin_gw2
+
+## 指令
+
+| 指令 | 功能 | 备注 |
+|:-----:|:----:|:----:|
+| gw2日常 | 日常信息 | 【gw2日常明日】 可以查看第二天
+| gw2活动 | 空中网活动和近日公告 | 暂无
+| gw2资讯 | 第三方咨询 | 接口暂时不更新... 
+
+## 备注
+
+本信息数据均来自[激战2 星岬岛](https://gw2.wishingstarmoye.com/gw2api)侵删
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_gw2 _â¨æ¿æ2 æå²¬å²æ¥è¯¢â¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
-## å®è£ pip3 install nonebot_plugin_gw2 ## æä»¤ | æä»¤ | åè½ | å¤æ³¨
-| |:-----:|:----:|:----:| | gw2æ¥å¸¸ | æ¥å¸¸ä¿¡æ¯ | ãgw2æ¥å¸¸ææ¥ã
+## å®è£ ä»¥ä¸æä»¤ä»»æä¸ä¸ªå³å¯ pip3 install nonebot_plugin_gw2 nb
+plugin install nonebot_plugin_gw2 ## æä»¤ | æä»¤ | åè½ | å¤æ³¨ | |:----
+-:|:----:|:----:| | gw2æ¥å¸¸ | æ¥å¸¸ä¿¡æ¯ | ãgw2æ¥å¸¸ææ¥ã
 å¯ä»¥æ¥çç¬¬äºå¤© | gw2æ´»å¨ | ç©ºä¸­ç½æ´»å¨åè¿æ¥å¬å | ææ  |
 gw2èµè®¯ | ç¬¬ä¸æ¹å¨è¯¢ | æ¥å£ææ¶ä¸æ´æ°... ## å¤æ³¨
 æ¬ä¿¡æ¯æ°æ®åæ¥èª[æ¿æ2 æå²¬å²](https://gw2.wishingstarmoye.com/
 gw2api)ä¾µå
```

### Comparing `nonebot-plugin-gw2-0.0.1/nonebot-plugin-gw2/api.py` & `nonebot_plugin_gw2-0.0.2/nonebot_plugin_gw2/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-import httpx
-import asyncio
-try:
-    import ujson as json
-except:
-    import json
-from nonebot.log import logger
-
-async def get_json(mode):
-    if mode=='today':
-        url = 'https://gw2.wishingstarmoye.com/gw2api/daily'
-    elif mode == 'tom':
-        url = 'https://gw2.wishingstarmoye.com/gw2api/daily/tomorrow'
-    elif mode == 'activity':
-        url = 'https://gw2.wishingstarmoye.com/gw2api/activity'
-    elif mode == 'news':
-        url = 'https://gw2.wishingstarmoye.com/gw2api/news'
-    headers = {
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0',
-    }
-    data:dict = json.loads(httpx.get(url=url,headers=headers).text)
-    return data
-
-async def daily(day:str):
-    # 日常
-    data = await get_json(day)
-    date = data['date']
-    data_pve = data['pve']
-    data_pvp = data['pvp']
-    data_wvw = data['wvw']
-    data_fac = data['fractals']
-
-
-    msg:str = '[+] 游戏每日日常\n'
-    msg = msg + '[-] PvE\n'
-    for pve in data_pve:
-     msg = msg + pve['zh'] + '  '
-    msg = msg.strip('  ') + '\n'
-    msg = msg + '[-] PvP\n'
-    for pvp in data_pvp:
-     msg = msg + pvp['zh'] + '  '
-    msg = msg.strip('  ') + '\n'
-    msg = msg + '[-] WvW\n'
-    for wvw in data_wvw:
-        msg = msg + wvw['zh'] + '  '
-    msg = msg.strip('  ') + '\n'
-    msg = msg + '[-] 碎层\n'
-    msg_tuijian = '推荐：'
-    msg_4ji = '4级：'
-    for fac in data_fac:
-        if '推荐' in fac['zh']:
-            msg_tuijian = msg_tuijian + fac['zh'][9:] + '  '
-        elif '4级' in fac['zh']:
-            msg_4ji = msg_4ji + fac['zh'][:-2] + '  '
-    msg = msg + msg_tuijian.strip('') + '\n' + msg_4ji.strip('')
-    msg = "当前时间为"+ date+'\n'+msg
-    return msg
-
-async def activity():
-    # 活动
-    data = await get_json('activity')
-    activitys = data['activitys']
-    disactivitys = data['disactivitys']
-    msg:str = '[+] 当前可参与活动或公告\n'
-    for act in activitys:
-        msg = msg + "[" + act['public_date'] + "] " + act['title'] + "\n" + act['url'] + "\n"
-    msg = msg + '[x] 最近已失效活动或公告\n'
-    for act in disactivitys:
-        msg = msg + "[已失效] " + act['title'] + "\n" + act['url'] + "\n"
-    msg = msg.strip('\n')
-    return msg
-
-async def zixuns():
-    # 咨询
-    json_data = await get_json('news')
-    msg1:str = '[+] 第三方资讯，包括小邋遢、明眸游戏、和风议会(NGA)\n'
-    for act in json_data:
-        msg1 = msg1 + "[" + act['date'] + "] " + act['title'] + "\n" + act['url'] + '数据来源'+act['type'] + "\n"
-    msg1 = msg1.strip('\n')
-    return msg1
-
-if __name__ == '__main__':
-    # asyncio.run(daily('tom'))
-    asyncio.run(activity())
+import httpx
+# import asyncio
+try:
+    import ujson as json
+except:
+    import json
+from nonebot.log import logger
+
+async def get_json(mode):
+    if mode=='today':
+        url = 'https://gw2.wishingstarmoye.com/gw2api/daily'
+    elif mode == 'tom':
+        url = 'https://gw2.wishingstarmoye.com/gw2api/daily/tomorrow'
+    elif mode == 'activity':
+        url = 'https://gw2.wishingstarmoye.com/gw2api/activity'
+    elif mode == 'news':
+        url = 'https://gw2.wishingstarmoye.com/gw2api/news'
+    headers = {
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0',
+    }
+    data:dict = json.loads(httpx.get(url=url,headers=headers).text)
+    return data
+
+async def daily(day:str):
+    # 日常
+    data = await get_json(day)
+    date = data['date']
+    data_pve = data['pve']
+    data_pvp = data['pvp']
+    data_wvw = data['wvw']
+    data_fac = data['fractals']
+
+
+    msg:str = '[+] 游戏每日日常\n'
+    msg = msg + '[-] PvE\n'
+    for pve in data_pve:
+     msg = msg + pve['zh'] + '  '
+    msg = msg.strip('  ') + '\n'
+    msg = msg + '[-] PvP\n'
+    for pvp in data_pvp:
+     msg = msg + pvp['zh'] + '  '
+    msg = msg.strip('  ') + '\n'
+    msg = msg + '[-] WvW\n'
+    for wvw in data_wvw:
+        msg = msg + wvw['zh'] + '  '
+    msg = msg.strip('  ') + '\n'
+    msg = msg + '[-] 碎层\n'
+    msg_tuijian = '推荐：'
+    msg_4ji = '4级：'
+    for fac in data_fac:
+        if '推荐' in fac['zh']:
+            msg_tuijian = msg_tuijian + fac['zh'][9:] + '  '
+        elif '4级' in fac['zh']:
+            msg_4ji = msg_4ji + fac['zh'][:-2] + '  '
+    msg = msg + msg_tuijian.strip('') + '\n' + msg_4ji.strip('')
+    msg = "当前时间为"+ date+'\n'+msg
+    return msg
+
+async def activity():
+    # 活动
+    data = await get_json('activity')
+    activitys = data['activitys']
+    disactivitys = data['disactivitys']
+    msg:str = '[+] 当前可参与活动或公告\n'
+    for act in activitys:
+        msg = msg + "[" + act['public_date'] + "] " + act['title'] + "\n" + act['url'] + "\n"
+    msg = msg + '[x] 最近已失效活动或公告\n'
+    for act in disactivitys:
+        msg = msg + "[已失效] " + act['title'] + "\n" + act['url'] + "\n"
+    msg = msg.strip('\n')
+    return msg
+
+async def zixuns():
+    # 咨询
+    json_data = await get_json('news')
+    msg1:str = '[+] 第三方资讯，包括小邋遢、明眸游戏、和风议会(NGA)\n'
+    for act in json_data:
+        msg1 = msg1 + "[" + act['date'] + "] " + act['title'] + "\n" + act['url'] + '数据来源'+act['type'] + "\n"
+    msg1 = msg1.strip('\n')
+    return msg1
+
+# if __name__ == '__main__':
+#     # asyncio.run(daily('tom'))
+#     asyncio.run(activity())
```

### Comparing `nonebot-plugin-gw2-0.0.1/pyproject.toml` & `nonebot_plugin_gw2-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-[tool.poetry]
-name = "nonebot-plugin-gw2"
-version = "0.0.1"
-description = "gw2 plugin for NoneBot"
-authors = ["Agnes_Digital <Z735803792@163.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_gw2"
-repository = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_gw2"
-keywords = ["game", "gw2", "nonebot2", "plugin"]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Operating System :: OS Independent",
-]
-include = [
-    "LICENSE","README.md"
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-nonebot2 = "^2.0.0rc3"
-nonebot-adapter-onebot = ">=2.1.5"
-asyncio = ">=3.4.3"
-httpx = "^0.23.3"
-
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot-plugin-gw2"
+version = "0.0.2"
+description = "gw2 plugin for NoneBot"
+authors = ["Agnes_Digital <Z735803792@163.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/Agnes4m/nonebot_plugin_gw2"
+repository = "https://github.com/Agnes4m/nonebot_plugin_gw2"
+keywords = ["game", "gw2", "nonebot2", "plugin"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+]
+include = [
+    "LICENSE","README.md"
+]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+nonebot2 = "^2.0.0"
+nonebot-adapter-onebot = ">=2.1.5"
+asyncio = ">=3.4.3"
+httpx = ">=0.23.3"
+
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

