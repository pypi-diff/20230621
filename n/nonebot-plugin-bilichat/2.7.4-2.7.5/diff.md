# Comparing `tmp/nonebot_plugin_bilichat-2.7.4.tar.gz` & `tmp/nonebot_plugin_bilichat-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.7.4.tar", last modified: Tue Jun 20 03:47:19 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.7.5.tar", last modified: Wed Jun 21 16:07:04 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.7.4.tar` & `nonebot_plugin_bilichat-2.7.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    34523 2023-06-20 03:47:09.348728 nonebot_plugin_bilichat-2.7.4/LICENSE
--rw-r--r--   0        0        0    13120 2023-06-20 03:47:09.348728 nonebot_plugin_bilichat-2.7.4/README.md
--rw-r--r--   0        0        0     9598 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5513 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    16205 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    14952 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
--rw-r--r--   0        0        0    93905 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7279 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     1363 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6899 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-20 03:47:19.361150 nonebot_plugin_bilichat-2.7.4/pyproject.toml
--rw-r--r--   0        0        0    14695 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-21 16:06:54.416686 nonebot_plugin_bilichat-2.7.5/LICENSE
+-rw-r--r--   0        0        0    13120 2023-06-21 16:06:54.416686 nonebot_plugin_bilichat-2.7.5/README.md
+-rw-r--r--   0        0        0     9690 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5513 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-21 16:06:54.436687 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16205 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    14952 2023-06-21 16:06:54.440688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
+-rw-r--r--   0        0        0    93905 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7279 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     1363 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6899 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-21 16:06:54.444688 nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-21 16:07:04.985378 nonebot_plugin_bilichat-2.7.5/pyproject.toml
+-rw-r--r--   0        0        0    14695 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.5/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.7.4/LICENSE` & `nonebot_plugin_bilichat-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/README.md` & `nonebot_plugin_bilichat-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 require("nonebot_plugin_segbuilder")
 
 
 from nonebot_plugin_segbuilder import SegmentBuilder
 
 BOT = Union[V11_Bot, V12_Bot, QG_Bot, Mirai_Bot]
 MESSAGE_EVENT = Union[V11_ME, V12_ME, QG_ME, Mirai_ME]
+INGNORE_TYPE = ("image",)
 
 if plugin_config.bilichat_openai_token or plugin_config.bilichat_newbing_cookie:
     ENABLE_SUMMARY = True
     from .summary import summarization
 else:
     ENABLE_SUMMARY = False
 
@@ -69,32 +70,34 @@
 )
 
 
 async def _bili_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     # 检查并提取 raw_bililink
     if plugin_config.bilichat_only_self and isinstance(event, V11_ME) and event.reply:
         # 仅自身的情况下，检查是否是回复，是的话则取被回复的消息
-        _msg = event.reply.message
+        _msgs = event.reply.message
     else:
         # 其余情况取该条消息
-        _msg = event.get_message()
+        _msgs = event.get_message()
 
-    # 如果是 B23 格式的链接，先转为正常的链接
-    _msg_str = str(_msg)
-    if "b23" in _msg_str:
-        if b23 := re.search(r"b23.(tv|wtf)[\\/]+(\w+)", _msg_str):  # type: ignore
-            state["_bililink_"] = await b23_extract(list(b23.groups()))
-            return True
-
-    # av bv cv 仅匹配纯文本部分，防止误触
-    _msg_str = _msg.extract_plain_text()
-    for seg in ("av", "AV", "bv", "BV", "cv", "CV"):
-        if seg in _msg_str:
-            state["_bililink_"] = _msg_str
-            return True
+    for _msg in _msgs:
+        # 如果是图片格式则忽略
+        if _msg.type in INGNORE_TYPE:
+            continue
+        # b23 格式的链接
+        _msg_str = str(_msg)
+        if "b23" in _msg_str:
+            if b23 := re.search(r"b23.(tv|wtf)[\\/]+(\w+)", _msg_str):  # type: ignore
+                state["_bililink_"] = await b23_extract(list(b23.groups()))
+                return True
+        # av bv cv 格式的链接
+        for seg in ("av", "AV", "bv", "BV", "cv", "CV"):
+            if seg in _msg_str:
+                state["_bililink_"] = _msg_str
+                return True
     return False
 
 
 async def _permission_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     # 检查权限
     # check if self msg
     if str(event.get_user_id()) == str(bot.self_id):
```

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.7.5/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.4/pyproject.toml` & `nonebot_plugin_bilichat-2.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.7.4"
+version = "2.7.5"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.7.4/PKG-INFO` & `nonebot_plugin_bilichat-2.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.7.4
+Version: 2.7.5
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.5 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

