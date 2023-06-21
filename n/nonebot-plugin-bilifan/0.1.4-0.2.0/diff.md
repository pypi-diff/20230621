# Comparing `tmp/nonebot_plugin_bilifan-0.1.4.tar.gz` & `tmp/nonebot_plugin_bilifan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.1.4.tar` & `nonebot_plugin_bilifan-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/LICENSE
--rw-r--r--   0        0        0     2083 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/README.md
--rw-r--r--   0        0        0     6358 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     4844 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     4331 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       52 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    16963 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    16706 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2197 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     2068 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/utils.py
--rw-r--r--   0        0        0     1100 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2125 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/README.md
+-rw-r--r--   0        0        0     9299 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     4844 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     4331 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       52 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    16963 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    16706 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2197 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     2647 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/utils.py
+-rw-r--r--   0        0        0     1078 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.1.4/LICENSE` & `nonebot_plugin_bilifan-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.4/README.md` & `nonebot_plugin_bilifan-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,14 @@
 - 删除全部的定时任务 - [超管]删除全部的定时任务
 
 
 </details>
 
 ## 🙈 其他
 
-- 本项目仅供学习使用，请勿用于商业用途
+- 本项目仅供学习使用，请勿用于商业用途，喜欢该项目可以Star或者提供PR
 - [爱发电](https://afdian.net/a/agnes_digital)
 - [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
 
 ## 🌐 感谢
 
 - [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他
```

#### html2text {}

```diff
@@ -5,12 +5,12 @@
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å é¤ç»å½ä¿¡æ¯ -
 å é¤ç»å½ä¿¡æ¯åç»å® - å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤ -
 èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ - åæ¶èªå¨å·çå­ -
 åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
 [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡  ## ð å¶ä» -
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [ç±åçµ](https://
-afdian.net/a/agnes_digital) - [GPL-3.0 License](https://github.com/Agnes4m/
-nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
-Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
-XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PR
+- [ç±åçµ](https://afdian.net/a/agnes_digital) - [GPL-3.0 License](https://
+github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m]
+(https://github.com/Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https:
+//github.com/XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

### Comparing `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/login/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/users.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/utils.py` & `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import yaml
 import os
 import shutil
 import asyncio
 
 from nonebot.log import logger
 from nonebot import get_bot
+from nonebot.adapters.onebot.v11 import Bot
 
 from .main import main
 
 config_dir = Path('data/bilifan')
 config_dir.mkdir(parents=True, exist_ok=True)
 CONFIG_PATH = config_dir / 'config.yaml'
 if not os.path.exists(Path().joinpath('data/bilifan/users.yaml')):
@@ -62,8 +63,26 @@
     if message_str:
         for user_id, group_id in config.items():
             if user_id == group_id:
                 await get_bot().send_private_msg(user_id=user_id, message=message_str)
                 continue
             else:
                 count_value = count.get(group_id, 0)
-                count[group_id] = count_value + 1 
+                count[group_id] = count_value + 1 
+                
+def render_forward_msg(msg_list: list, uid=2711142767, name='宁宁',bot:Bot = None):
+    try:
+        uid = bot.self_id
+        name = list(bot.config.nickname)[0]
+    except Exception as e:
+        logger.warning(f'获取bot信息错误\n{e}')
+    forward_msg = []
+    for msg in msg_list:
+        forward_msg.append({
+            "type": "node",
+            "data": {
+                "name": str(name),
+                "uin": str(uid),
+                "content": msg
+            }
+        })
+    return forward_msg
```

### Comparing `nonebot_plugin_bilifan-0.1.4/pyproject.toml` & `nonebot_plugin_bilifan-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.1.4"
-description = "刷bili粉丝牌子的机器人插件"
+version = "0.2.0"
+description = "刷站粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 repository = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 keywords = ["bilibili", "nonebot2", "plugin"]
 classifiers = [
@@ -19,20 +19,19 @@
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot2 = "^2.0.0rc4"
+nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.1.5"
 nonebot_plugin_apscheduler = ">=0.2.0"
 
-pillow = "^9.3.0"
-aiohttp = "^3.8.3"
+pillow = ">=9.3.0"
 aiohttp-socks = "^0.8.0"
 pyyaml = "^6.0"
 qrcode = "^7.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_bilifan-0.1.4/PKG-INFO` & `nonebot_plugin_bilifan-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilifan
-Version: 0.1.4
-Summary: 刷bili粉丝牌子的机器人插件
+Version: 0.2.0
+Summary: 刷站粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_bilifan
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
-Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0)
-Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: pillow (>=9.3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_bilifan
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
@@ -68,15 +67,15 @@
 - 删除全部的定时任务 - [超管]删除全部的定时任务
 
 
 </details>
 
 ## 🙈 其他
 
-- 本项目仅供学习使用，请勿用于商业用途
+- 本项目仅供学习使用，请勿用于商业用途，喜欢该项目可以Star或者提供PR
 - [爱发电](https://afdian.net/a/agnes_digital)
 - [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
 
 ## 🌐 感谢
 
 - [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.4 Summary:
-å·biliç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
+Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.2.0 Summary:
+å·ç«ç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_bilifan License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist: nonebot-adapter-
-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist:
-nonebot_plugin_apscheduler (>=0.2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0)
-Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_bilifan
-Description-Content-Type: text/markdown
+Programming Language :: Python :: 3.11 Requires-Dist: aiohttp-socks
+(>=0.8.0,<0.9.0) Requires-Dist: nonebot-adapter-onebot (>=2.1.5) Requires-Dist:
+nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0)
+Requires-Dist: pillow (>=9.3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-
+Dist: qrcode (>=7.4.2,<8.0.0) Project-URL: Repository, https://github.com/
+Agnes4m/nonebot_plugin_bilifan Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å é¤ç»å½ä¿¡æ¯ -
 å é¤ç»å½ä¿¡æ¯åç»å® - å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤ -
 èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ - åæ¶èªå¨å·çå­ -
 åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
 [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡  ## ð å¶ä» -
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [ç±åçµ](https://
-afdian.net/a/agnes_digital) - [GPL-3.0 License](https://github.com/Agnes4m/
-nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
-Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
-XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PR
+- [ç±åçµ](https://afdian.net/a/agnes_digital) - [GPL-3.0 License](https://
+github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m]
+(https://github.com/Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https:
+//github.com/XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

