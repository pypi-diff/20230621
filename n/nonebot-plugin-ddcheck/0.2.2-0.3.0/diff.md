# Comparing `tmp/nonebot_plugin_ddcheck-0.2.2.tar.gz` & `tmp/nonebot_plugin_ddcheck-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ddcheck-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_ddcheck-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_ddcheck-0.2.2.tar` & `nonebot_plugin_ddcheck-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-05-12 13:20:56.298534 nonebot_plugin_ddcheck-0.2.2/LICENSE
--rw-r--r--   0        0        0     1029 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/README.md
--rw-r--r--   0        0        0     1967 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/__init__.py
--rw-r--r--   0        0        0      115 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/config.py
--rw-r--r--   0        0        0     6768 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/data_source.py
--rw-r--r--   0        0        0     4860 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/template/info.html
--rw-r--r--   0        0        0      753 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 nonebot_plugin_ddcheck-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 09:30:36.939043 nonebot_plugin_ddcheck-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1029 2023-06-21 09:30:36.939043 nonebot_plugin_ddcheck-0.3.0/README.md
+-rw-r--r--   0        0        0     1661 2023-06-21 09:30:36.939043 nonebot_plugin_ddcheck-0.3.0/nonebot_plugin_ddcheck/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-21 09:30:36.939043 nonebot_plugin_ddcheck-0.3.0/nonebot_plugin_ddcheck/config.py
+-rw-r--r--   0        0        0     6768 2023-06-21 09:30:36.939043 nonebot_plugin_ddcheck-0.3.0/nonebot_plugin_ddcheck/data_source.py
+-rw-r--r--   0        0        0     4860 2023-06-21 09:30:36.939043 nonebot_plugin_ddcheck-0.3.0/nonebot_plugin_ddcheck/template/info.html
+-rw-r--r--   0        0        0      769 2023-06-21 09:30:36.939043 nonebot_plugin_ddcheck-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 nonebot_plugin_ddcheck-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_ddcheck-0.2.2/LICENSE` & `nonebot_plugin_ddcheck-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ddcheck-0.2.2/README.md` & `nonebot_plugin_ddcheck-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/data_source.py` & `nonebot_plugin_ddcheck-0.3.0/nonebot_plugin_ddcheck/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/template/info.html` & `nonebot_plugin_ddcheck-0.3.0/nonebot_plugin_ddcheck/template/info.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ddcheck-0.2.2/pyproject.toml` & `nonebot_plugin_ddcheck-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nonebot_plugin_ddcheck"
-version = "0.2.2"
+version = "0.3.0"
 description = "Nonebot2 成分姬插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-ddcheck"
 repository = "https://github.com/noneplugin/nonebot-plugin-ddcheck"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.0"
-nonebot-plugin-htmlrender = ">=0.0.4"
-nonebot-plugin-apscheduler = "^0.2.0"
-nonebot-plugin-localstore = "^0.4.0"
-httpx = ">=0.19.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
+nonebot-plugin-htmlrender = "^0.2.0"
+nonebot-plugin-apscheduler = "^0.3.0"
+nonebot-plugin-localstore = "^0.5.0"
+httpx = ">=0.19.0,<1.0.0"
 Jinja2 = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_ddcheck-0.2.2/PKG-INFO` & `nonebot_plugin_ddcheck-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ddcheck
-Version: 0.2.2
+Version: 0.3.0
 Summary: Nonebot2 成分姬插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-ddcheck
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
-Requires-Dist: httpx (>=0.19.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.0.4)
-Requires-Dist: nonebot-plugin-localstore (>=0.4.0,<0.5.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: httpx (>=0.19.0,<1.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.5.0,<0.6.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-ddcheck
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-ddcheck
 
 NoneBot2 成分姬插件
```

