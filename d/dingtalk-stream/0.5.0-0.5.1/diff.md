# Comparing `tmp/dingtalk-stream-0.5.0.tar.gz` & `tmp/dingtalk-stream-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.5.0.tar", last modified: Wed Jun 21 07:31:29 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.5.1.tar", last modified: Wed Jun 21 07:41:04 2023, max compression
```

## Comparing `dingtalk-stream-0.5.0.tar` & `dingtalk-stream-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:41:04.529471 dingtalk-stream-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:41:04.529471 dingtalk-stream-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:41:04.529471 dingtalk-stream-0.5.1/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:41:04.529471 dingtalk-stream-0.5.1/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:41:04.000000 dingtalk-stream-0.5.1/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 07:41:04.000000 dingtalk-stream-0.5.1/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:41:04.000000 dingtalk-stream-0.5.1/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 07:41:04.000000 dingtalk-stream-0.5.1/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 07:41:04.000000 dingtalk-stream-0.5.1/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:41:04.529471 dingtalk-stream-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-21 07:41:03.000000 dingtalk-stream-0.5.1/setup.py
```

### Comparing `dingtalk-stream-0.5.0/LICENSE` & `dingtalk-stream-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.0/PKG-INFO` & `dingtalk-stream-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.5.0/README.md` & `dingtalk-stream-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.0/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.5.1/dingtalk_stream/chatbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             self.sender_nick,
             self.conversation_title,
         )
 
 
 class ChatbotHandler(CallbackHandler):
 
-    def set_off_duty_prompt(self, text: str, title: str, logo: str):
+    def set_off_duty_prompt(self, text: str, title: str = "", logo: str = ""):
         """
         设置离线提示词，需要使用OpenAPI，当前仅支持自建应用。
         :param text: 离线提示词
         :param title: 机器人名称，默认："钉钉Stream机器人"
         :param logo: 机器人logo，默认："@lALPDfJ6V_FPDmvNAfTNAfQ"
         :return:
         """
@@ -297,16 +297,16 @@
             self.logger.error('reply markdown failed, error=%s', e)
             return None
         return response.json()
 
     def reply_card(self,
                    card_data: dict,
                    incoming_message: ChatbotMessage,
-                   at_sender: bool,
-                   at_all: bool) -> str:
+                   at_sender: bool = False,
+                   at_all: bool = False) -> str:
         """
         回复互动卡片。由于sessionWebhook不支持发送互动卡片，所以需要使用OpenAPI，当前仅支持自建应用。
         https://open.dingtalk.com/document/orgapp/robots-send-interactive-cards
         :param card_data: 卡片数据内容，interactive_card.py中有一些简单的样例，高阶需求请至卡片搭建平台：https://card.dingtalk.com/card-builder
         :param incoming_message: 回调数据源
         :param at_sender: 是否at发送人
         :param at_all: 是否at所有人
```

### Comparing `dingtalk-stream-0.5.0/dingtalk_stream/frames.py` & `dingtalk-stream-0.5.1/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.0/dingtalk_stream/handlers.py` & `dingtalk-stream-0.5.1/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.0/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.5.1/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.0/dingtalk_stream/stream.py` & `dingtalk-stream-0.5.1/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.0/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.5.1/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.5.0/setup.py` & `dingtalk-stream-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.5.0',
+    version='0.5.1',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

