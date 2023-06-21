# Comparing `tmp/nonebot_plugin_al-0.3.3.tar.gz` & `tmp/nonebot_plugin_al-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.4.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.3.tar` & `nonebot_plugin_al-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/LICENSE
--rw-r--r--   0        0        0     4110 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/README.md
--rw-r--r--   0        0        0     6357 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    70845 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3348 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0     1790 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/config.py
--rw-r--r--   0        0        0    69109 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10152 2023-06-21 01:35:50.087152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7691 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13687 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     5972 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1055 2023-06-21 01:35:50.091152 nonebot_plugin_al-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4110 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/README.md
+-rw-r--r--   0        0        0     6368 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    70845 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3348 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0     1790 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/config.py
+-rw-r--r--   0        0        0    69109 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10152 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7691 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13687 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5972 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1055 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.4/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.3/LICENSE` & `nonebot_plugin_al-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/README.md` & `nonebot_plugin_al-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,20 +19,15 @@
     import json
 
 
 from .bili import jinghao,get_data, get_ship_msg
 from .send_message import blhx
 from .config import ADMIN
 
-
-__version__ = "0.3"
-__plugin_meta__ = PluginMetadata(
-    name="碧蓝航线攻略",
-    description='碧蓝航线井号榜等等攻略',
-    usage="""
+logo ="""
     ......                  ` .]]@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......                ,/@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......            /O@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     `.....           ,@^=.OOO\/\@@@@@@@@@@@@@@@@@@@@OO//@@@@@/OO\]]]OO\]
     ``....          ,@@/=^OOOOOOOO@@@@@@@@@@@\]OOOOOOO^^=@@@@OOOOOOOOOOO
     `.....          O@O^==OOOOOOOO@@@/.,@@@OOOOOOOOOOO\O,@@@@OOOOOOOOO@@
     ......    ,    .@@@^=`OOOOOOOOO/  ,O@@OOOOOOOOOOOOOO.O@@@OO/[[[[[[[.
@@ -58,15 +53,21 @@
     ...... =.....*.=`..,O`       .O.....=   ... ^.=..OOOOO=O@..=O^..OOO^
     ...... .^...**.O@...\O^ .     \.....`   .^ /.,^.=O@OO`=O@^..OO`.=OO\
     ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
     ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
-    """,
+    """
+
+__version__ = "0.3"
+__plugin_meta__ = PluginMetadata(
+    name="碧蓝航线攻略",
+    description='碧蓝航线井号榜等等攻略',
+    usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_AL",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
```

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/config.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/send_message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.4/nonebot_plugin_al/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.3/pyproject.toml` & `nonebot_plugin_al-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.3"
+version = "0.3.4"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
```

### Comparing `nonebot_plugin_al-0.3.3/PKG-INFO` & `nonebot_plugin_al-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.3
+Version: 0.3.4
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.3 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.4 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

