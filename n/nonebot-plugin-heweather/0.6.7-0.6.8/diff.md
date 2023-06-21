# Comparing `tmp/nonebot_plugin_heweather-0.6.7.tar.gz` & `tmp/nonebot_plugin_heweather-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_heweather-0.6.7.tar", last modified: Wed Jun 21 07:52:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_heweather-0.6.8.tar", last modified: Wed Jun 21 08:41:15 2023, max compression
```

## Comparing `nonebot_plugin_heweather-0.6.7.tar` & `nonebot_plugin_heweather-0.6.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1062 2023-06-21 07:52:36.993460 nonebot_plugin_heweather-0.6.7/LICENSE
--rw-r--r--   0        0        0     2272 2023-06-21 07:52:36.993460 nonebot_plugin_heweather-0.6.7/README.md
--rw-r--r--   0        0        0     1867 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/__init__.py
--rw-r--r--   0        0        0      435 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/config.py
--rw-r--r--   0        0        0     1104 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/model.py
--rw-r--r--   0        0        0     1785 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/render_pic.py
--rwxr-xr-x   0        0        0    69948 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
--rwxr-xr-x   0        0        0    27920 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
--rwxr-xr-x   0        0        0    19688 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
--rwxr-xr-x   0        0        0    20240 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.css
--rwxr-xr-x   0        0        0     9784 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.json
--rw-r--r--   0        0        0     2850 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/weather.css
--rw-r--r--   0        0        0     5219 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/weather.html
--rw-r--r--   0        0        0     4978 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/weather_data.py
--rw-r--r--   0        0        0      831 2023-06-21 07:52:51.905481 nonebot_plugin_heweather-0.6.7/pyproject.toml
--rw-r--r--   0        0        0        6 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/.gitignore
--rw-r--r--   0        0        0        0 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/__init__.py
--rw-r--r--   0        0        0      487 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/conftest.py
--rw-r--r--   0        0        0      784 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/test_heweather.py
--rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-21 08:41:07.723333 nonebot_plugin_heweather-0.6.8/LICENSE
+-rw-r--r--   0        0        0     2272 2023-06-21 08:41:07.723333 nonebot_plugin_heweather-0.6.8/README.md
+-rw-r--r--   0        0        0     1975 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/config.py
+-rw-r--r--   0        0        0     1104 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/model.py
+-rw-r--r--   0        0        0     1785 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/render_pic.py
+-rwxr-xr-x   0        0        0    69948 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
+-rwxr-xr-x   0        0        0    27920 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
+-rwxr-xr-x   0        0        0    19688 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
+-rwxr-xr-x   0        0        0    20240 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.css
+-rwxr-xr-x   0        0        0     9784 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.json
+-rw-r--r--   0        0        0     2850 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/weather.css
+-rw-r--r--   0        0        0     5219 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/weather.html
+-rw-r--r--   0        0        0     4978 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/weather_data.py
+-rw-r--r--   0        0        0      993 2023-06-21 08:41:15.807415 nonebot_plugin_heweather-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/__init__.py
+-rw-r--r--   0        0        0      487 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/conftest.py
+-rw-r--r--   0        0        0      784 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/test_heweather.py
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.8/PKG-INFO
```

### Comparing `nonebot_plugin_heweather-0.6.7/LICENSE` & `nonebot_plugin_heweather-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/README.md` & `nonebot_plugin_heweather-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/__init__.py` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from .config import DEBUG, QWEATHER_APIKEY, QWEATHER_APITYPE, Config
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-heweather",
     description="和风天气图片显示插件",
     usage="天气地名 / 地名天气",
     type="application",
+    homepage="https://github.com/kexue-z/nonebot-plugin-heweather",
     config=Config,
     extra={},
+    supported_adapters={"~onebot.v11"},
 )
 
 
 if DEBUG:
     logger.debug("将会保存图片到 weather.png")
```

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/model.py` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/render_pic.py` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/render_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.css` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.json` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/weather.css` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/weather.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/weather.html` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/weather.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/weather_data.py` & `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/weather_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.7/pyproject.toml` & `nonebot_plugin_heweather-0.6.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-heweather"
-version = "0.6.7"
+version = "0.6.8"
 description = "Get Heweather information and convert to pictures"
 authors = [
     { name = "kexue", email = "xana278@foxmail.com" },
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot-plugin-htmlrender>=0.0.4.3",
@@ -12,15 +12,19 @@
     "pydantic>=1.5.0",
     "nonebot2[fastapi]>=2.0.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
-text = "MIT"
+file = "LICENSE"
+
+[project.urls]
+Homepage = "https://github.com/kexue-z/nonebot-plugin-heweather"
+"Bug Tracker" = "https://github.com/kexue-z/nonebot-plugin-heweather/issues"
 
 [tool.pdm.build]
 includes = []
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pillow>=9.5.0",
```

### Comparing `nonebot_plugin_heweather-0.6.7/tests/test_heweather.py` & `nonebot_plugin_heweather-0.6.8/tests/test_heweather.py`

 * *Files identical despite different names*

