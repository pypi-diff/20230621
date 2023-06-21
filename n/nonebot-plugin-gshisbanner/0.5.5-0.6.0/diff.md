# Comparing `tmp/nonebot_plugin_gshisbanner-0.5.5.tar.gz` & `tmp/nonebot_plugin_gshisbanner-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-0.5.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-0.6.0.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-0.5.5.tar` & `nonebot_plugin_gshisbanner-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-06-11 14:06:12.602589 nonebot_plugin_gshisbanner-0.5.5/LICENSE
--rw-r--r--   0        0        0     5295 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/README.md
--rw-r--r--   0        0        0      593 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0     1030 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      427 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      300 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0     3276 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1231 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     5270 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/main.py
--rw-r--r--   0        0        0     2640 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0      600 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     5987 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5510 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/README.md
+-rw-r--r--   0        0        0      595 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0     1030 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      427 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      300 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0     3621 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1231 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     4979 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/main.py
+-rw-r--r--   0        0        0     2640 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0      600 2023-06-21 10:31:30.041371 nonebot_plugin_gshisbanner-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6202 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.6.0/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-0.5.5/LICENSE` & `nonebot_plugin_gshisbanner-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.5/README.md` & `nonebot_plugin_gshisbanner-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     plugins = ["nonebot_plugin_gshisbanner"]
 </details>
 
 ## ⚙️ 配置
 ```
 gshisbanner_forward_length: int
 # 单次合并转发消息长度（int）,默认为10
+# 仅为角色/武器卡池转发内容长度，不包括版本卡池
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
 
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
 ·· 1."banners.52v6.com/data" 
@@ -60,20 +61,21 @@
 ·· 2."genshin-gacha-banners.vercel.app/data" 
      #vercel代理，国内可能无法直连
 ·· 3."genshin-gacha-banners.52v6.com/data" 
      #cloudfare代理，可能会被墙
 ·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
      ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
-·· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/gacha"
+·· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
      ##jsdelivr代理的文件，大多数情况可用，推荐
 ```
 
 ## 🎉 使用
 ### 指令表
+#### 用前提示，本插件采用on_keyword，不需要带你设置的command_start，当然，如果你非要带，本插件做了一定的处理
 |        指令        |  权限   | 需要@ | 范围  |                                说明                                |
 |:----------------:|:-----:|:---:|:---:|:----------------------------------------------------------------:|
 | [name]历史卡池(num)  |  ALL  |  否  | ALL | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
 | [version]卡池[num] |  ALL  |  否  | ALL |    version为版本号，如1.3，2.6等，num为1-3，对应上半（中）下半，可不填，如不填则发送该版本全部卡池     |
 |  刷新(更新)历史卡池/别名   | 管理员以上 |  否  | ALL |                            刷新历史卡池或别名                             |
 ### 效果图
 <details>
```

#### html2text {}

```diff
@@ -8,30 +8,33 @@
 æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ï¼å½åä»éç¨äºqqï¼
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-gshisbanner   pip pip install nonebot-plugin-gshisbanner
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"]  ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
-åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 #
+åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 # ä»ä¸ºè§è²/
+æ­¦å¨å¡æ± è½¬ååå®¹é¿åº¦ï¼ä¸åæ¬çæ¬å¡æ±  #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
 # ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸²
 gshisbanner_json_url: str # åå²å¡æ± jsonåè¡¨ä¸è½½ä½ç½® # å¯éå¼ Â·Â·
 1."banners.52v6.com/data" #é»è®¤ï¼æ¨è Â·Â· 2."genshin-gacha-
 banners.vercel.app/data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â·
 3."genshin-gacha-banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â·
 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/
 gacha" ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
-(éè¦æ¯æhttps) Â·Â· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/
-gacha" ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:--------
---------:|:-----:|:---:|:---:|:------------------------------------------------
-----------------:| | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+(éè¦æ¯æhttps) Â·Â· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
+##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ## ð ä½¿ç¨
+### æä»¤è¡¨ ####
+ç¨åæç¤ºï¼æ¬æä»¶éç¨on_keywordï¼ä¸éè¦å¸¦ä½ è®¾ç½®çcommand_startï¼å½ç¶ï¼å¦æä½ éè¦å¸¦ï¼æ¬æä»¶åäºä¸å®çå¤ç
+| æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:----------------:|:-----:|:--
+-:|:---:|:----------------------------------------------------------------:| |
+[name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°(æ´æ°)åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
```

### Comparing `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/__init__.py` & `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from nonebot.plugin import PluginMetadata
 
 from .config import plugin_config
 from .main import *  # noqa: F403
 
-__version__ = "0.5.5"
+__version__ = "0.6.0"
 __plugin_meta__ = PluginMetadata(
     name="gshisbanner",
     description="这是一个在机器人上获取原神历史卡池的插件",
-    usage="XX历史卡池,XX版本卡池，详细查看本仓库readme",
+    usage="XX历史卡池,XX卡池(版本)，详细查看本仓库readme",
     type="application",
     homepage="https://github.com/forchannot/nonebot-plugin-gshisbanner",
     config=plugin_config,
     supported_adapters={"~onebot.v11"},
     extra={
         "author": "forchannot",
         "version": __version__,
```

### Comparing `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from pathlib import Path
 from typing import Dict, List, Union
 
+from nonebot import get_driver
+
 from .config import plugin_config
 from .deal_json import load_json_from_url
 
 path = Path.cwd() / "data" / "genshin_history"
+command_start = get_driver().config.command_start
 
 
 async def get_info_from_url(
     cha: bool, cache_dir: Path = path
 ) -> Union[Dict, List[Dict]]:
     """
     :param cha: 类型
@@ -64,15 +67,20 @@
     :param version: 版本号
     :param is_all: 是否获取全部卡池
     :return: 获取到的历史卡池数据
     """
     # 获取所有卡池信息
     json = await get_info_from_url(True) + await get_info_from_url(False)
     # 卡池类型列表
-    type_list = ["five_character", "four_character", "five_weapon", "four_weapon"]
+    type_list = [
+        "five_character",
+        "four_character",
+        "five_weapon",
+        "four_weapon",
+    ]
     result = []
     for data in json:
         # 判断是否为指定版本
         if data["version"][:3] == version if is_all else data["version"] == version:
             # 构造卡池信息字典
             temp = {
                 "start": data["start"],
@@ -87,7 +95,15 @@
                     for x in data["items"]
                     if x.get("rankType") == (5 if "five" in item else 4)
                     and x.get("itemType") == item.split("_")[1].capitalize()
                 ]
             result.append(temp)
     # 去除空值
     return [{k: v for k, v in data.items() if v} for data in result]
+
+
+def delete_command_start(text: str) -> str:
+    """
+    :param text: 原始文本
+    :return: 删除文本开头的指令符
+    """
+    return text[1:] if any(text.startswith(cs) for cs in command_start if cs) else text
```

### Comparing `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/main.py` & `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,129 @@
 import contextlib
 from pathlib import Path
 from typing import Union
 
-from nonebot import get_driver, logger, on_regex
+from nonebot import get_driver, logger
 from nonebot.adapters.onebot.v11 import (
     GROUP_ADMIN,
     GROUP_OWNER,
     Bot,
     GroupMessageEvent,
-    MessageEvent,
     PrivateMessageEvent,
 )
-from nonebot.params import RegexDict
+from nonebot.params import Keyword
 from nonebot.permission import SUPERUSER
+from nonebot.plugin.on import on_keyword
 
 from .alias import find_name
 from .api import get
 from .config import plugin_config
-from .deal import deal_info_from_name, deal_info_from_version
+from .deal import deal_info_from_name, deal_info_from_version, delete_command_start
 from .deal_json import load_json_from_url, save_json
 from .send import word_send_from_name, word_send_from_version
 
-old_gacha = on_regex(
-    r"(?<!\w)(?P<name>[\u4e00-\u9fa5]+)(?<!刷新)(历史卡池|历史up)(?P<len>\d{0,2})(?!.)",
-    priority=35,
-    block=False,
+old_gacha = on_keyword(
+    {"历史卡池", "历史up"},
+    priority=45,
+    block=True,
 )
-version_gacha = on_regex(
-    r"(?<!.)(?P<version>\d\.\d)(卡池|up)(?P<upordown>(1|2|3)?)(?!.)",
-    priority=35,
+version_gacha = on_keyword(
+    {"卡池", "up"},
+    priority=47,
     block=False,
 )
-refresh = on_regex(
-    r"(?<!.)(刷新|更新)(?P<name>历史卡池|别名)(?!.)",
+refresh = on_keyword(
+    {"刷新", "更新"},
     permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
-    priority=13,
-    block=False,
+    priority=40,
+    block=True,
 )
 
+
 DRIVER = get_driver()
 gacha_info_path = Path.cwd() / "data" / "genshin_history"
 special_version = ["1.3"]  # 特殊三卡池版本
 forward_length = plugin_config.gshisbanner_forward_length  # 合并转发长度
 
 
 @old_gacha.handle()
 async def _(
     bot: Bot,
     event: Union[GroupMessageEvent, PrivateMessageEvent],
-    regex_dict: dict = RegexDict(),  # noqa: B008
+    key: str = Keyword(),  # noqa: B008
 ):
-    type_name = regex_dict["name"]
-    if not isinstance(forward_length, int) or forward_length <= 0:
-        await old_gacha.finish("合并转发长度设置错误")
-    # regex_dict["len"]：表示合并转发的长度,由用户输入获取，未获取到则为默认值
-    length = (
-        int(regex_dict["len"])
-        if regex_dict["len"]
-        else plugin_config.gshisbanner_forward_length
-    )
-    # 获取角色真实名字
-    real_name, real_type = find_name(type_name)
+    name, length = event.get_plaintext().split(key)
+    name = delete_command_start(name)
+    if name in ["刷新", "更新"]:
+        return
+    if length and not length.isdigit():
+        return
+    real_name, real_type = find_name(name)
     if real_name is None or real_type not in ["角色", "武器"]:
         await old_gacha.finish("该角色/武器不存在或是从未up过")
     # 获取up信息
     info = await deal_info_from_name(real_name, "cha" if real_type == "角色" else "wep")
-    if length > 0:
+    if length := int(length) if length else plugin_config.gshisbanner_forward_length:
         await word_send_from_name(bot, event, real_name, info, length)
-    await old_gacha.finish()
 
 
 @version_gacha.handle()
 async def _(
-    bot: Bot, event: MessageEvent, regex_dict: dict = RegexDict()  # noqa: B008
-):  # noqa: B008
-    # 判断是否为三卡池的版本
-    if regex_dict["version"] not in special_version and regex_dict["upordown"] == "3":
-        await version_gacha.finish()
-    # 获取版本信息
-    real_version = (
-        f"{regex_dict['version']}.{regex_dict['upordown']}"
-        if regex_dict["upordown"]
-        else regex_dict["version"]
-    )
-    # 根据版本获取up信息
-    info = await deal_info_from_version(real_version, not regex_dict["upordown"])
-    if info:
+    bot: Bot,
+    event: Union[GroupMessageEvent, PrivateMessageEvent],
+    key: str = Keyword(),  # noqa: B008
+):
+    version, upordown = event.get_plaintext().split(key)
+    version = delete_command_start(version)
+    if version in ["刷新", "更新"]:
+        return
+    if upordown and not (
+        upordown.isdigit() and all(part.isdigit() for part in version.split("."))
+    ):
+        return
+    if upordown == "3" and version not in special_version:
+        return
+    real_version = f"{version}.{upordown}" if upordown else version
+    if info := await deal_info_from_version(real_version, not upordown):
         await word_send_from_version(bot, event, real_version, info)
-    await version_gacha.finish()
 
 
 @refresh.handle()
 async def _(
-    event: MessageEvent,
-    regex_dict: dict = RegexDict(),  # noqa: B008
+    event: Union[GroupMessageEvent, PrivateMessageEvent],
+    key: str = Keyword(),  # noqa: B008
 ):
-    type_name = regex_dict["name"]
-    types = ["character", "weapon"]
-    if type_name == "历史卡池":
-        for i in types:
+    args = event.get_plaintext().split(key)
+    _arg = delete_command_start(args[0])
+    if _arg:
+        return
+    choose = args[1]
+    if choose in ["历史卡池", "历史up", "卡池", "up"]:
+        for i in ["character", "weapon"]:
             url = f"https://{plugin_config.gshisbanner_json_url}/{i}.json"
             path = gacha_info_path / f"{i}.json"
             result = await load_json_from_url(url, path, True)
             if not result:
-                await refresh.finish(f"刷新{type_name}失败,可能是网络问题或api失效")
+                await refresh.send(f"刷新{i}.json失败,可能是网络问题或api失效")
+                continue
             save_json(result, path)
             logger.info(f"{i}.json文件保存成功")
-    elif type_name == "别名":
+    elif choose == "别名":
         if (await init_group_card(True)) is False:
-            await refresh.finish(f"刷新{type_name}失败,可能是网络问题或api失效")
-    await refresh.finish(f"刷新{type_name}成功")
+            await refresh.finish(f"刷新{choose}失败,可能是网络问题或api失效")
+    await refresh.finish(f"刷新{choose}成功")
 
 
 @DRIVER.on_startup
 async def init_group_card(force_refresh: bool = False) -> bool:
     if not gacha_info_path.exists():
         gacha_info_path.mkdir(parents=True)
     urls = [
         "https://jsd.cdn.zzko.cn/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
         "https://raw.fastgit.org/forchannot/nonebot-plugin-gshisbanner/main/data/genshin_history/alias.json",
-        "https://cdn.jsdelivr.net/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
         "https://cdn.staticaly.com/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
         "https://fastly.jsdelivr.net/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
     ]
     if (gacha_info_path / "alias.json").exists() and not force_refresh:
         logger.info("alias.json文件已存在，跳过下载，如需更新请使用刷新别名功能")
         return False
     for url in urls:
```

### Comparing `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-0.6.0/nonebot_plugin_gshisbanner/send.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.5/pyproject.toml` & `nonebot_plugin_gshisbanner-0.6.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gshisbanner"
-version = "0.5.5"
+version = "0.6.0"
 description = "Nonebot2查询原神历史卡池小插件"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_gshisbanner"}]
```

### Comparing `nonebot_plugin_gshisbanner-0.5.5/PKG-INFO` & `nonebot_plugin_gshisbanner-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 0.5.5
+Version: 0.6.0
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -64,14 +64,15 @@
     plugins = ["nonebot_plugin_gshisbanner"]
 </details>
 
 ## ⚙️ 配置
 ```
 gshisbanner_forward_length: int
 # 单次合并转发消息长度（int）,默认为10
+# 仅为角色/武器卡池转发内容长度，不包括版本卡池
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
 
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
 ·· 1."banners.52v6.com/data" 
@@ -79,20 +80,21 @@
 ·· 2."genshin-gacha-banners.vercel.app/data" 
      #vercel代理，国内可能无法直连
 ·· 3."genshin-gacha-banners.52v6.com/data" 
      #cloudfare代理，可能会被墙
 ·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
      ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
-·· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/gacha"
+·· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
      ##jsdelivr代理的文件，大多数情况可用，推荐
 ```
 
 ## 🎉 使用
 ### 指令表
+#### 用前提示，本插件采用on_keyword，不需要带你设置的command_start，当然，如果你非要带，本插件做了一定的处理
 |        指令        |  权限   | 需要@ | 范围  |                                说明                                |
 |:----------------:|:-----:|:---:|:---:|:----------------------------------------------------------------:|
 | [name]历史卡池(num)  |  ALL  |  否  | ALL | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
 | [version]卡池[num] |  ALL  |  否  | ALL |    version为版本号，如1.3，2.6等，num为1-3，对应上半（中）下半，可不填，如不填则发送该版本全部卡池     |
 |  刷新(更新)历史卡池/别名   | 管理员以上 |  否  | ALL |                            刷新历史卡池或别名                             |
 ### 效果图
 <details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.5.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.6.0 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
@@ -18,30 +18,33 @@
 æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ï¼å½åä»éç¨äºqqï¼
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-gshisbanner   pip pip install nonebot-plugin-gshisbanner
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"]  ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
-åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 #
+åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 # ä»ä¸ºè§è²/
+æ­¦å¨å¡æ± è½¬ååå®¹é¿åº¦ï¼ä¸åæ¬çæ¬å¡æ±  #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
 # ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸²
 gshisbanner_json_url: str # åå²å¡æ± jsonåè¡¨ä¸è½½ä½ç½® # å¯éå¼ Â·Â·
 1."banners.52v6.com/data" #é»è®¤ï¼æ¨è Â·Â· 2."genshin-gacha-
 banners.vercel.app/data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â·
 3."genshin-gacha-banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â·
 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/
 gacha" ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
-(éè¦æ¯æhttps) Â·Â· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/
-gacha" ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:--------
---------:|:-----:|:---:|:---:|:------------------------------------------------
-----------------:| | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+(éè¦æ¯æhttps) Â·Â· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
+##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ## ð ä½¿ç¨
+### æä»¤è¡¨ ####
+ç¨åæç¤ºï¼æ¬æä»¶éç¨on_keywordï¼ä¸éè¦å¸¦ä½ è®¾ç½®çcommand_startï¼å½ç¶ï¼å¦æä½ éè¦å¸¦ï¼æ¬æä»¶åäºä¸å®çå¤ç
+| æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:----------------:|:-----:|:--
+-:|:---:|:----------------------------------------------------------------:| |
+[name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°(æ´æ°)åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
```

