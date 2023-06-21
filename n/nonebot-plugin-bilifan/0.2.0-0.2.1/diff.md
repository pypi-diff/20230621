# Comparing `tmp/nonebot_plugin_bilifan-0.2.0.tar.gz` & `tmp/nonebot_plugin_bilifan-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.2.0.tar` & `nonebot_plugin_bilifan-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/LICENSE
--rw-r--r--   0        0        0     2125 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/README.md
--rw-r--r--   0        0        0     9299 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     4844 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     4331 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       52 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    16963 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    16706 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2197 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     2647 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/utils.py
--rw-r--r--   0        0        0     1078 2023-06-21 01:32:13.639103 nonebot_plugin_bilifan-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2125 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/README.md
+-rw-r--r--   0        0        0     9316 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     4844 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     4331 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       52 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    16963 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    16706 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2197 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     2647 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/utils.py
+-rw-r--r--   0        0        0     1078 2023-06-21 02:15:05.082303 nonebot_plugin_bilifan-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.2.0/LICENSE` & `nonebot_plugin_bilifan-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/README.md` & `nonebot_plugin_bilifan-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/__init__.py` & `nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,15 @@
 
 logger.opt(colors=True).info(
     "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
     if scheduler
     else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>"
 )
 
-driver = get_driver()
-__version__ = "0.2.0"
-__plugin_meta__ = PluginMetadata(
-    name="bilifan",
-    description='b站粉丝牌~',
-    usage="""
+logo ="""
     ......                  ` .]]@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......                ,/@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......            /O@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     `.....           ,@^=.OOO\/\@@@@@@@@@@@@@@@@@@@@OO//@@@@@/OO\]]]OO\]
     ``....          ,@@/=^OOOOOOOO@@@@@@@@@@@\]OOOOOOO^^=@@@@OOOOOOOOOOO
     `.....          O@O^==OOOOOOOO@@@/.,@@@OOOOOOOOOOO\O,@@@@OOOOOOOOO@@
     ......    ,    .@@@^=`OOOOOOOOO/  ,O@@OOOOOOOOOOOOOO.O@@@OO/[[[[[[[.
@@ -62,17 +57,24 @@
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
+driver = get_driver()
+__version__ = "0.2.0"
+__plugin_meta__ = PluginMetadata(
+    name="bilifan",
+    description='b站粉丝牌~',
+    usage=logo,
     type="application",
-    homepage="https://github.com/Agnes4m/nonebot_plugin_AL",
+    homepage="https://github.com/Agnes4m/nonebot_plugin_bilifan",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
```

### Comparing `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/login/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/src/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/src/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/users.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/nonebot_plugin_bilifan/utils.py` & `nonebot_plugin_bilifan-0.2.1/nonebot_plugin_bilifan/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.2.0/pyproject.toml` & `nonebot_plugin_bilifan-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.2.0"
+version = "0.2.1"
 description = "刷站粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 repository = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 keywords = ["bilibili", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_bilifan-0.2.0/PKG-INFO` & `nonebot_plugin_bilifan-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilifan
-Version: 0.2.0
+Version: 0.2.1
 Summary: 刷站粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_bilifan
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.2.1 Summary:
 å·ç«ç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_bilifan License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

