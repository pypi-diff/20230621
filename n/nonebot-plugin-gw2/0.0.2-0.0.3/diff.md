# Comparing `tmp/nonebot_plugin_gw2-0.0.2.tar.gz` & `tmp/nonebot_plugin_gw2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gw2-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_gw2-0.0.3.tar", max compression
```

## Comparing `nonebot_plugin_gw2-0.0.2.tar` & `nonebot_plugin_gw2-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/LICENSE
--rw-r--r--   0        0        0     1714 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/README.md
--rw-r--r--   0        0        0     3556 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/nonebot_plugin_gw2/__init__.py
--rw-r--r--   0        0        0     2704 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/nonebot_plugin_gw2/api.py
--rw-r--r--   0        0        0      949 2023-06-21 01:46:25.020985 nonebot_plugin_gw2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 nonebot_plugin_gw2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1714 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/README.md
+-rw-r--r--   0        0        0     3572 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/__init__.py
+-rw-r--r--   0        0        0     2704 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/api.py
+-rw-r--r--   0        0        0      949 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 nonebot_plugin_gw2-0.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_gw2-0.0.2/LICENSE` & `nonebot_plugin_gw2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gw2-0.0.2/README.md` & `nonebot_plugin_gw2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gw2-0.0.2/nonebot_plugin_gw2/__init__.py` & `nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message,Bot, Event
 from nonebot.plugin import PluginMetadata
 
 from .api import activity , daily,zixuns
 
-__version__ = "0.0.2"
-__plugin_meta__ = PluginMetadata(
-    name="激战2",
-    description='使用api获取星岬岛信息',
-    usage="""
+logo ="""
     ......                  ` .]]@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......                ,/@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......            /O@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     `.....           ,@^=.OOO\/\@@@@@@@@@@@@@@@@@@@@OO//@@@@@/OO\]]]OO\]
     ``....          ,@@/=^OOOOOOOO@@@@@@@@@@@\]OOOOOOO^^=@@@@OOOOOOOOOOO
     `.....          O@O^==OOOOOOOO@@@/.,@@@OOOOOOOOOOO\O,@@@@OOOOOOOOO@@
     ......    ,    .@@@^=`OOOOOOOOO/  ,O@@OOOOOOOOOOOOOO.O@@@OO/[[[[[[[.
@@ -39,15 +35,21 @@
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
+__version__ = "0.0.3"
+__plugin_meta__ = PluginMetadata(
+    name="激战2",
+    description='使用api获取星岬岛信息',
+    usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_gw2",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
```

### Comparing `nonebot_plugin_gw2-0.0.2/nonebot_plugin_gw2/api.py` & `nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gw2-0.0.2/pyproject.toml` & `nonebot_plugin_gw2-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gw2"
-version = "0.0.2"
+version = "0.0.3"
 description = "gw2 plugin for NoneBot"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_gw2"
 repository = "https://github.com/Agnes4m/nonebot_plugin_gw2"
 keywords = ["game", "gw2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_gw2-0.0.2/PKG-INFO` & `nonebot_plugin_gw2-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gw2
-Version: 0.0.2
+Version: 0.0.3
 Summary: gw2 plugin for NoneBot
 Home-page: https://github.com/Agnes4m/nonebot_plugin_gw2
 License: MIT
 Keywords: game,gw2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gw2 Version: 0.0.2 Summary: gw2
+Metadata-Version: 2.1 Name: nonebot-plugin-gw2 Version: 0.0.3 Summary: gw2
 plugin for NoneBot Home-page: https://github.com/Agnes4m/nonebot_plugin_gw2
 License: MIT Keywords: game,gw2,nonebot2,plugin Author: Agnes_Digital Author-
 email: Z735803792@163.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

