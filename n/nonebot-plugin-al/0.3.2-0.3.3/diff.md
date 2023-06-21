# Comparing `tmp/nonebot_plugin_al-0.3.2.tar.gz` & `tmp/nonebot_plugin_al-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.3.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.2.tar` & `nonebot_plugin_al-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/LICENSE
--rw-r--r--   0        0        0     3778 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/README.md
--rw-r--r--   0        0        0     6487 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    70845 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3348 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0    69109 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10152 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7691 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13667 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     6878 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1028 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4912 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4110 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/README.md
+-rw-r--r--   0        0        0     6357 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    70845 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3348 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0     1790 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/config.py
+-rw-r--r--   0        0        0    69109 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10152 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7691 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13687 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5972 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1055 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.2/LICENSE` & `nonebot_plugin_al-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.2/README.md` & `nonebot_plugin_al-0.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -122,11 +122,18 @@
 
 命令示范：blhx皮肤 光辉 0
 
 12.建造模拟
 
 命令示范：blhx大建 轻型/重型/特型
 
+## 🙈 其他
+
+- 本项目仅供学习使用，请勿用于商业用途
+- 喜欢该项目可以Star或者提供PR，你的支持就是我持续维护的动力
+- [爱发电](https://afdian.net/a/agnes_digital)
+- [MIT License](https://github.com/Agnes4m/nonebot_plugin_AL/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
+
 ## 感谢
 
 - [AzurAPI](https://github.com/AzurAPI/azurapi-js-setup)持续更新的碧蓝航线数据库
 - [blhx_wiki](https://github.com/Gaylone/blhx_wiki) - hoshino碧蓝航线项目（已停止维护）
```

#### html2text {}

```diff
@@ -29,11 +29,15 @@
 (ç®åå·²ä½¿ç¨ä»£çæ´æ°apiæ°æ®ä¸ºç¦»çº¿æ¨¡å¼æç¨ï¼å¦æåºé®é¢åæ¶issue)
 å½ä»¤ç¤ºèï¼blhx å¼ºå¶æ´æ° 8.è·åææ°æ´»å¨ä¿¡æ¯
 (æé®é¢åæ¶issue) å½ä»¤ç¤ºèï¼blhx ææ°æ´»å¨ 9.ä¸ºè°è¹åæµç§°
 (ä»¥åä½ å°±å¯ä»¥ç¨æµç§°æ¥è¯¢äº) å½ä»¤ç¤ºèï¼blhxå¤æ³¨ åè¾ å¤ªå¤ª
 ä»¥åå°±å¯ä»¥ç¨ blhx å¤ªå¤ª å©çº± è¿ç§æµç§°åä»£æ­£å¼åç§°æ¥è¯¢
 10.å é¤è°è¹æµç§° å½ä»¤ç¤ºèï¼blhxç§»é¤å¤æ³¨ åè¾ å¤ªå¤ª
 11.è°è¹æµç§°å¿«æ·æ¥è¯¢ å½ä»¤ç¤ºèï¼blhxç®è¤ åè¾ 0 12.å»ºé æ¨¡æ
-å½ä»¤ç¤ºèï¼blhxå¤§å»º è½»å/éå/ç¹å ## æè°¢ - [AzurAPI](https://
-github.com/AzurAPI/azurapi-js-setup)æç»­æ´æ°çç¢§èèªçº¿æ°æ®åº -
-[blhx_wiki](https://github.com/Gaylone/blhx_wiki) -
-hoshinoç¢§èèªçº¿é¡¹ç®ï¼å·²åæ­¢ç»´æ¤ï¼
+å½ä»¤ç¤ºèï¼blhxå¤§å»º è½»å/éå/ç¹å ## ð å¶ä» -
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é -
+åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PRï¼ä½ çæ¯æå°±æ¯ææç»­ç»´æ¤çå¨å
+- [ç±åçµ](https://afdian.net/a/agnes_digital) - [MIT License](https://
+github.com/Agnes4m/nonebot_plugin_AL/blob/main/LICENSE) Â©[@Agnes4m](https://
+github.com/Agnes4m) ## æè°¢ - [AzurAPI](https://github.com/AzurAPI/azurapi-
+js-setup)æç»­æ´æ°çç¢§èèªçº¿æ°æ®åº - [blhx_wiki](https://github.com/
+Gaylone/blhx_wiki) - hoshinoç¢§èèªçº¿é¡¹ç®ï¼å·²åæ­¢ç»´æ¤ï¼
```

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,25 @@
 from nonebot.adapters.onebot.v11 import (
     Message,
     MessageSegment,
     Bot,
     Event,
     GroupMessageEvent,
 )
-from nonebot.adapters.onebot.v11.permission import (
-    GROUP_ADMIN,
-    GROUP_OWNER,
-    PRIVATE_FRIEND,
-)
 import traceback
 from pathlib import Path
 try:
     import ujson as json
 except:
     import json
 
 
 from .bili import jinghao,get_data, get_ship_msg
 from .send_message import blhx
+from .config import ADMIN
 
 
 __version__ = "0.3"
 __plugin_meta__ = PluginMetadata(
     name="碧蓝航线攻略",
     description='碧蓝航线井号榜等等攻略',
     usage="""
@@ -72,15 +68,14 @@
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
-ADMIN = SUPERUSER | GROUP_ADMIN | GROUP_OWNER 
 al_command = on_command('al',aliases={'碧蓝'},priority=50,block=True)
 tag_ser = on_command('alhelp',aliases={'碧蓝指令','碧蓝帮助'},priority=30,block=False)
 tags = ['强度榜','装备榜','金部件榜','萌新榜','兵器榜','专武榜',
         '兑换榜','研发榜','改造榜','跨队榜','pt榜','氪金榜','打捞主线榜','打捞作战榜']
 
 
 @tag_ser.handle()
```

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/send_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                     msg = "舰船信息\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_info.png"))) \
                         + "\n此船可改\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_retrofit.png"))) \
                         + "\n推荐出装\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_weapon.png")))\
                         + "\n此船备注昵称有：\n"+nickname_list
 
                 msg_list = []
                 msg_list.append(msg)
-                forward_msg = render_forward_msg(msg_list)
+                forward_msg = render_forward_msg(msg_list,bot=bot)
                 if isinstance(event,GroupMessageEvent):
                     await bot.call_api('send_group_forward_msg',group_id=event.group_id, messages=forward_msg)
                     return
             if len(args) == 0:
                 await bot.send(event=event,message='请在命令之后提供精确舰船名称和皮肤昵称哦~', at_sender=True)
         except Exception as e:
             traceback.print_exc()
@@ -124,16 +124,16 @@
         #             "兵装推荐榜\n", "专武推荐榜\n", "兑换装备推荐榜\n", "研发装备推荐榜\n", "改造推荐榜\n", "跨队舰船推荐榜\n",
         #             "氪金榜\n" , "打捞主线榜\n","打捞作战榜'\n"]
         msg = "仅代表个人观点，完全不等于绝对客观，可能存在各种主观评判或者真爱加成，不过目标是努力去进行符合环境需求的客观评定\n"
         msg_list = []
         if len(div_list) != 0:
             for i in range(0, len(div_list)):
                 msg += Message(str(div_list[i].find('img')['alt']) + MessageSegment.image(file=str(div_list[i].find('img')['src'])) + "\n")
-            msg_list.append(msg)
-            forward_msg = render_forward_msg(msg_list)
+                msg_list.append(msg)
+            forward_msg = render_forward_msg(msg_list,bot=bot)
             if isinstance(event,GroupMessageEvent):
                 await bot.call_api('send_group_forward_msg',group_id=event.group_id, messages=forward_msg)
                 return
         else:
             await bot.send(event=event,message='暂无信息', at_sender=True)
```

### Comparing `nonebot_plugin_al-0.3.2/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.3/nonebot_plugin_al/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import cv2
 import pypinyin
 import json
 import aiofiles
 
 from typing import Optional
 from pathlib import Path
+from nonebot import get_bot
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot_plugin_htmlrender import html_to_pic
+from nonebot.log import logger
 
 SAVE_PATH = Path().joinpath('data/al')
 tool_path = SAVE_PATH.joinpath('wkhtmltopdf', 'bin', 'wkhtmltoimage.exe')
 """
 方法名：print_img
 参数列表：无
 用处：调用打印工具，打印ship_info.html成图片
@@ -29,27 +31,14 @@
     else:
         with open(SAVE_PATH.joinpath('ship_html', f'ship_{tag}.html'),'r',encoding='utf-8')as f:
             html = f.read()
         pic = await html_to_pic(html=html)
         with open(SAVE_PATH.joinpath('ship_html','images', f'ship_{tag}{tep}.png'),'wb')as f:
             f.write(pic)
             
-def print_img_ship():
-    # path_wkimg = SAVE_PATH + '/\\wkhtmltopdf/\\bin/\\wkhtmltoimage.exe'  # 工具路径
-    path_wkimg = tool_path
-    cfg = imgkit.config(wkhtmltoimage=path_wkimg)
-    options = {
-        "encoding": "UTF-8",
-        "enable-local-file-access": None
-    }
-    print("开始")
-    imgkit.from_file(SAVE_PATH.joinpath('ship_html', 'ship_info.html'),
-                     SAVE_PATH.joinpath('images', 'ship_temp.png'),
-                     options=options, config=cfg)  # 不管怎么样都打印这张图片
-    print("结束")
 
 def print_img_ship_retrofit():
     # path_wkimg = SAVE_PATH + '/\\wkhtmltopdf/\\bin/\\wkhtmltoimage.exe'  # 工具路径
     path_wkimg = tool_path
     cfg = imgkit.config(wkhtmltoimage=path_wkimg)
     options = {
         "encoding": "UTF-8",
@@ -59,15 +48,14 @@
     imgkit.from_file(SAVE_PATH.joinpath('ship_html', 'ship_retrofit.html'),
                      SAVE_PATH.joinpath('images', 'ship_retrofit_temp.png'),
                      options=options, config=cfg)  # 不管怎么样都打印这张图片
     print("结束")
 
 
 
-
 def img_process_ship_retrofit():
     # SAVE_PATH.joinpath('images', 'ship_temp.png'))
     img = cv2.imread(SAVE_PATH.joinpath('ship_html','images', 'ship_retrofit_temp.png'))
     image = img.shape
     cropped = img[0:image[0], 0:620]  # 裁剪坐标为[y0:y1, x0:x1]
     cv2.imwrite(SAVE_PATH.joinpath('ship_html','images', 'ship_retrofit.png'), cropped)
 
@@ -87,27 +75,14 @@
         "enable-local-file-access": None
     }
     imgkit.from_file(SAVE_PATH.joinpath('ship_html', 'ship_skin.html'),
                      SAVE_PATH.joinpath('ship_html', 'images','ship_skin.png'),
                      options=options, config=cfg)  # 不管怎么样都打印这张图片
 
 
-def print_img_ship_weapon():
-    path_wkimg = tool_path  # 工具路径
-    cfg = imgkit.config(wkhtmltoimage=path_wkimg)
-    options = {
-        "encoding": "UTF-8",
-        "enable-local-file-access": None
-    }
-    imgkit.from_file(SAVE_PATH.joinpath('ship_html', 'ship_weapon.html'),
-                     SAVE_PATH.joinpath('ship_html', 'images', 'ship_weapon_temp.png'),
-                     options=options, config=cfg)  # 不管怎么样都打印这张图片
-
-
-
 """
 方法名：img_process_ship_info
 参数列表：无
 用处：裁剪图片
 返回值：无返回值
 """
 
@@ -181,16 +156,16 @@
         load_dict:dict = json.loads(load_dict) # 别删除，否则会有类型错误
     return load_dict['ships']
 
 def render_forward_msg(msg_list: list, uid=1916714922, name='小加加(VC装甲钢36D版)',bot:Bot = None):
     try:
         uid = bot.self_id
         name = list(bot.config.nickname)[0]
-    except:
-        pass
+    except Exception as e:
+        logger.warning(f'获取bot信息错误\n{e}')
     forward_msg = []
     for msg in msg_list:
         forward_msg.append({
             "type": "node",
             "data": {
                 "name": str(name),
                 "uin": str(uid),
```

### Comparing `nonebot_plugin_al-0.3.2/pyproject.toml` & `nonebot_plugin_al-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.2"
+version = "0.3.3"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
@@ -27,11 +27,12 @@
 nonebot_plugin_htmlrender = "^0.2.0.3"
 aiohttp = ">=3.8.3"
 bs4 = "^0.0.1"
 aiofiles = "^23.1.0"
 pypinyin = "^0.49.0"
 imgkit = "^1.2.3"
 opencv-python = "^4.7.0"
+"ruamel.yaml" = "^0.17.21"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_al-0.3.2/PKG-INFO` & `nonebot_plugin_al-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.2
+Version: 0.3.3
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -20,14 +20,15 @@
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: imgkit (>=1.2.3,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0)
 Requires-Dist: opencv-python (>=4.7.0,<5.0.0)
 Requires-Dist: pypinyin (>=0.49.0,<0.50.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
                 <br>
@@ -151,12 +152,19 @@
 
 命令示范：blhx皮肤 光辉 0
 
 12.建造模拟
 
 命令示范：blhx大建 轻型/重型/特型
 
+## 🙈 其他
+
+- 本项目仅供学习使用，请勿用于商业用途
+- 喜欢该项目可以Star或者提供PR，你的支持就是我持续维护的动力
+- [爱发电](https://afdian.net/a/agnes_digital)
+- [MIT License](https://github.com/Agnes4m/nonebot_plugin_AL/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
+
 ## 感谢
 
 - [AzurAPI](https://github.com/AzurAPI/azurapi-js-setup)持续更新的碧蓝航线数据库
 - [blhx_wiki](https://github.com/Gaylone/blhx_wiki) - hoshino碧蓝航线项目（已停止维护）
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.2 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.3 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
 Dist: aiohttp (>=3.8.3) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist:
 imgkit (>=1.2.3,<2.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
 nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist: opencv-python
-(>=4.7.0,<5.0.0) Requires-Dist: pypinyin (>=0.49.0,<0.50.0) Project-URL:
-Repository, https://github.com/Agnes4m/nonebot_plugin_AL Description-Content-
-Type: text/markdown
+(>=4.7.0,<5.0.0) Requires-Dist: pypinyin (>=0.49.0,<0.50.0) Requires-Dist:
+ruamel.yaml (>=0.17.21,<0.18.0) Project-URL: Repository, https://github.com/
+Agnes4m/nonebot_plugin_AL Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_al 0.3.0 __â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨__ [GitHub_stars]
            [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## åè½ 1ãbç«wikiäºå·æ¦ä¸å¾æµ 2ãè°è¹è£å¤å¾é´ 3ã
 (70%å®æ)ç§»æ¤å¤§é¨å[blhx](https://github.com/Gaylone/
 blhx_wiki)ï¼åhoshinoæ¹é¡¹ç®ï¼çå¤§é¨ååè½ ## å®è£
@@ -45,11 +45,15 @@
 (ç®åå·²ä½¿ç¨ä»£çæ´æ°apiæ°æ®ä¸ºç¦»çº¿æ¨¡å¼æç¨ï¼å¦æåºé®é¢åæ¶issue)
 å½ä»¤ç¤ºèï¼blhx å¼ºå¶æ´æ° 8.è·åææ°æ´»å¨ä¿¡æ¯
 (æé®é¢åæ¶issue) å½ä»¤ç¤ºèï¼blhx ææ°æ´»å¨ 9.ä¸ºè°è¹åæµç§°
 (ä»¥åä½ å°±å¯ä»¥ç¨æµç§°æ¥è¯¢äº) å½ä»¤ç¤ºèï¼blhxå¤æ³¨ åè¾ å¤ªå¤ª
 ä»¥åå°±å¯ä»¥ç¨ blhx å¤ªå¤ª å©çº± è¿ç§æµç§°åä»£æ­£å¼åç§°æ¥è¯¢
 10.å é¤è°è¹æµç§° å½ä»¤ç¤ºèï¼blhxç§»é¤å¤æ³¨ åè¾ å¤ªå¤ª
 11.è°è¹æµç§°å¿«æ·æ¥è¯¢ å½ä»¤ç¤ºèï¼blhxç®è¤ åè¾ 0 12.å»ºé æ¨¡æ
-å½ä»¤ç¤ºèï¼blhxå¤§å»º è½»å/éå/ç¹å ## æè°¢ - [AzurAPI](https://
-github.com/AzurAPI/azurapi-js-setup)æç»­æ´æ°çç¢§èèªçº¿æ°æ®åº -
-[blhx_wiki](https://github.com/Gaylone/blhx_wiki) -
-hoshinoç¢§èèªçº¿é¡¹ç®ï¼å·²åæ­¢ç»´æ¤ï¼
+å½ä»¤ç¤ºèï¼blhxå¤§å»º è½»å/éå/ç¹å ## ð å¶ä» -
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é -
+åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PRï¼ä½ çæ¯æå°±æ¯ææç»­ç»´æ¤çå¨å
+- [ç±åçµ](https://afdian.net/a/agnes_digital) - [MIT License](https://
+github.com/Agnes4m/nonebot_plugin_AL/blob/main/LICENSE) Â©[@Agnes4m](https://
+github.com/Agnes4m) ## æè°¢ - [AzurAPI](https://github.com/AzurAPI/azurapi-
+js-setup)æç»­æ´æ°çç¢§èèªçº¿æ°æ®åº - [blhx_wiki](https://github.com/
+Gaylone/blhx_wiki) - hoshinoç¢§èèªçº¿é¡¹ç®ï¼å·²åæ­¢ç»´æ¤ï¼
```

