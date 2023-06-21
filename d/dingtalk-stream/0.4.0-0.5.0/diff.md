# Comparing `tmp/dingtalk-stream-0.4.0.tar.gz` & `tmp/dingtalk-stream-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.4.0.tar", last modified: Fri Jun  9 05:09:00 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.5.0.tar", last modified: Wed Jun 21 07:31:29 2023, max compression
```

## Comparing `dingtalk-stream-0.4.0.tar` & `dingtalk-stream-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 07:31:29.000000 dingtalk-stream-0.5.0/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:31:29.293205 dingtalk-stream-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-21 07:31:28.000000 dingtalk-stream-0.5.0/setup.py
```

### Comparing `dingtalk-stream-0.4.0/LICENSE` & `dingtalk-stream-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.4.0/PKG-INFO` & `dingtalk-stream-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.4.0/README.md` & `dingtalk-stream-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.4.0/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.5.0/dingtalk_stream/chatbot.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import json
 import requests
 import platform
 import hashlib
 from .stream import CallbackHandler, CallbackMessage
 from .frames import AckMessage, Headers
+from .interactive_card import generate_multi_text_line_card_data
+from .utils import DINGTALK_OPENAPI_ENDPOINT
 from concurrent.futures import ThreadPoolExecutor
 import uuid
 
 
 class AtUser(object):
     def __init__(self):
         self.dingtalk_id = None
@@ -189,14 +191,63 @@
             self.sender_nick,
             self.conversation_title,
         )
 
 
 class ChatbotHandler(CallbackHandler):
 
+    def set_off_duty_prompt(self, text: str, title: str, logo: str):
+        """
+        设置离线提示词，需要使用OpenAPI，当前仅支持自建应用。
+        :param text: 离线提示词
+        :param title: 机器人名称，默认："钉钉Stream机器人"
+        :param logo: 机器人logo，默认："@lALPDfJ6V_FPDmvNAfTNAfQ"
+        :return:
+        """
+        access_token = self.dingtalk_client.get_access_token()
+        if not access_token:
+            self.logger.error('send_off_duty_prompt failed, cannot get dingtalk access token')
+            return None
+
+        if title is None or title == "":
+            title = "钉钉Stream机器人"
+
+        if logo is None or logo == "":
+            logo = "@lALPDfJ6V_FPDmvNAfTNAfQ"
+
+        prompt_card_data = generate_multi_text_line_card_data(title=title, logo=logo, texts=[text])
+
+        request_headers = {
+            'Content-Type': 'application/json',
+            'Accept': '*/*',
+            'x-acs-dingtalk-access-token': access_token,
+            'User-Agent': ('DingTalkStream/1.0 SDK/0.1.0 Python/%s '
+                           '(+https://github.com/open-dingtalk/dingtalk-stream-sdk-python)'
+                           ) % platform.python_version(),
+        }
+
+        values = {
+            'robotCode': self.dingtalk_client.credential.client_id,
+            'cardData': json.dumps(prompt_card_data),
+            'cardTemplateId': "StandardCard",
+        }
+
+        url = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/innerApi/robot/stream/away/template/update'
+
+        try:
+            response = requests.post(url,
+                                     headers=request_headers,
+                                     data=json.dumps(values))
+
+            response.raise_for_status()
+        except Exception as e:
+            self.logger.error('set_off_duty_prompt, error=%s, response=%s', e, response.text)
+            return response.status_code
+        return response.json()
+
     def reply_text(self,
                    text: str,
                    incoming_message: ChatbotMessage):
         request_headers = {
             'Content-Type': 'application/json',
             'Accept': '*/*',
         }
@@ -246,21 +297,23 @@
             self.logger.error('reply markdown failed, error=%s', e)
             return None
         return response.json()
 
     def reply_card(self,
                    card_data: dict,
                    incoming_message: ChatbotMessage,
+                   at_sender: bool,
                    at_all: bool) -> str:
         """
         回复互动卡片。由于sessionWebhook不支持发送互动卡片，所以需要使用OpenAPI，当前仅支持自建应用。
         https://open.dingtalk.com/document/orgapp/robots-send-interactive-cards
         :param card_data: 卡片数据内容，interactive_card.py中有一些简单的样例，高阶需求请至卡片搭建平台：https://card.dingtalk.com/card-builder
-        :param at_all: 是否at所有人
         :param incoming_message: 回调数据源
+        :param at_sender: 是否at发送人
+        :param at_all: 是否at所有人
         :return:
         """
         access_token = self.dingtalk_client.get_access_token()
         if not access_token:
             self.logger.error(
                 'simple_reply_interactive_card_only_for_inner_app failed, cannot get dingtalk access token')
             return None
@@ -296,15 +349,24 @@
             body["singleChatReceiver"] = json.dumps(single_chat_receiver)
 
         if at_all:
             body["sendOptions"]["atAll"] = True
         else:
             body["sendOptions"]["atAll"] = False
 
-        url = 'https://api.dingtalk.com/v1.0/im/v1.0/robot/interactiveCards/send'
+        if at_sender:
+            user_list_json = [
+                {
+                    "nickName": incoming_message.sender_nick,
+                    "userId": incoming_message.sender_staff_id
+                }
+            ]
+            body["sendOptions"]["atUserListJson"] = json.dumps(user_list_json, ensure_ascii=False)
+
+        url = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/im/v1.0/robot/interactiveCards/send'
         try:
             response = requests.post(url,
                                      headers=request_headers,
                                      json=body)
             response.raise_for_status()
 
             return card_biz_id
@@ -334,15 +396,15 @@
                            ) % platform.python_version(),
         }
 
         values = {
             'cardBizId': card_biz_id,
             'cardData': json.dumps(card_data),
         }
-        url = 'https://api.dingtalk.com/v1.0/im/robots/interactiveCards'
+        url = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/im/robots/interactiveCards'
         try:
             response = requests.put(url,
                                     headers=request_headers,
                                     data=json.dumps(values))
             response.raise_for_status()
         except Exception as e:
             self.logger.error('update card failed, error=%s, response=%s', e, response.text)
```

### Comparing `dingtalk-stream-0.4.0/dingtalk_stream/frames.py` & `dingtalk-stream-0.5.0/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.4.0/dingtalk_stream/handlers.py` & `dingtalk-stream-0.5.0/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.4.0/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.5.0/dingtalk_stream/interactive_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 这里是卡片模板库，提供一些必要的卡片组件组合。
 INTERACTIVE_CARD_JSON_SAMPLE_1 极简卡片组合：title-text-image-button
 INTERACTIVE_CARD_JSON_SAMPLE_2 较丰富的组件卡片，title-text-image-section-button
 INTERACTIVE_CARD_JSON_SAMPLE_3 较丰富的组件卡片，title-image-markdown-button
 高阶需求请至卡片搭建平台：https://card.dingtalk.com/card-builder
 """
 
+
 '''
 实用卡片模板：多行文本
 '''
 INTERACTIVE_CARD_JSON_SAMPLE_MULTI_TEXT_LINE = {
     "config": {
         "autoLayout": True,
         "enableForward": True
@@ -23,17 +24,17 @@
             "type": "text",
             "text": "钉钉卡片"
         },
         "logo": "@lALPDfJ6V_FPDmvNAfTNAfQ"
     },
     "contents": [
         {
-            "type": "text",
+            "type": "markdown",
             "text": "钉钉正在为各行各业提供专业解决方案，沉淀钉钉1900万企业组织核心业务场景，提供专属钉钉、教育、医疗、新零售等多行业多维度的解决方案。",
-            "id": "text_1686281949314"
+            "id": "markdown_1686281949314"
         },
         {
             "type": "divider",
             "id": "divider_1686281949314"
         }
     ]
 }
@@ -78,17 +79,17 @@
             "type": "text",
             "text": "钉钉卡片"
         },
         "logo": "@lALPDfJ6V_FPDmvNAfTNAfQ"
     },
     "contents": [
         {
-            "type": "text",
+            "type": "markdown",
             "text": "钉钉正在为各行各业提供专业解决方案，沉淀钉钉1900万企业组织核心业务场景，提供专属钉钉、教育、医疗、新零售等多行业多维度的解决方案。",
-            "id": "text_1686281949314"
+            "id": "markdown_1686281949314"
         },
         {
             "type": "divider",
             "id": "divider_1686281949314"
         },
         {
             "type": "imageList",
@@ -149,15 +150,15 @@
             "type": "text",
             "text": "钉钉卡片"
         },
         "logo": "@lALPDfJ6V_FPDmvNAfTNAfQ"
     },
     "contents": [
         {
-            "type": "text",
+            "type": "markdown",
             "text": "钉钉，让进步发生！\n 更新时间：2023-06-06 12:00",
             "id": "text_1686025745169"
         },
         {
             "type": "image",
             "image": "@lADPDetfXH_Pn3HNAbrNBDg",
             "id": "image_1686025745169"
@@ -209,15 +210,15 @@
             "type": "text",
             "text": "钉钉卡片"
         },
         "logo": "@lALPDfJ6V_FPDmvNAfTNAfQ"
     },
     "contents": [
         {
-            "type": "text",
+            "type": "markdown",
             "text": "钉钉正在为各行各业提供专业解决方案，沉淀钉钉1900万企业组织核心业务场景，提供专属钉钉、教育、医疗、新零售等多行业多维度的解决方案。",
             "id": "text_1686025745169"
         },
         {
             "type": "image",
             "image": "@lADPDetfXH_Pn3HNAbrNBDg",
             "id": "image_1686025745169"
```

### Comparing `dingtalk-stream-0.4.0/dingtalk_stream/stream.py` & `dingtalk-stream-0.5.0/dingtalk_stream/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 from .handlers import CallbackHandler
 from .handlers import EventHandler
 from .handlers import SystemHandler
 from .frames import SystemMessage
 from .frames import EventMessage
 from .frames import CallbackMessage
 from .log import setup_default_logger
+from .utils import DINGTALK_OPENAPI_ENDPOINT
 
 
 class DingTalkStreamClient(object):
-    OPEN_CONNECTION_API = 'https://api.dingtalk.com/v1.0/gateway/connections/open'
+    OPEN_CONNECTION_API = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/gateway/connections/open'
     TAG_DISCONNECT = 'disconnect'
 
     def __init__(self, credential: Credential, logger: logging.Logger = None):
         self.credential: Credential = credential
         self.event_handler: EventHandler = EventHandler()
         self.callback_handler_map = {}
         self.system_handler: SystemHandler = SystemHandler()
@@ -97,15 +98,16 @@
             ack = await self.event_handler.raw_process(msg)
         elif msg_type == CallbackMessage.TYPE:
             msg = CallbackMessage.from_dict(json_message)
             handler = self.callback_handler_map.get(msg.headers.topic)
             if handler:
                 ack = await handler.raw_process(msg)
             else:
-                self.logger.warning("unknown callback message topic, topic=%s, message=%s", msg.headers.topic, json_message)
+                self.logger.warning("unknown callback message topic, topic=%s, message=%s", msg.headers.topic,
+                                    json_message)
         else:
             self.logger.warning('unknown message, content=%s', json_message)
         if ack:
             await self.websocket.send(json.dumps(ack.to_dict()))
         return result
 
     def start_forever(self):
@@ -168,15 +170,15 @@
             'Accept': 'application/json',
         }
         values = {
             'appKey': self.credential.client_id,
             'appSecret': self.credential.client_secret,
         }
         try:
-            response = requests.post('https://api.dingtalk.com/v1.0/oauth2/accessToken',
+            response = requests.post(DINGTALK_OPENAPI_ENDPOINT + '/v1.0/oauth2/accessToken',
                                      headers=request_headers,
                                      data=json.dumps(values))
             response.raise_for_status()
         except Exception as e:
             self.logger.error('get dingtalk access token failed, error=%s', e)
             return None
 
@@ -187,18 +189,18 @@
 
     def upload_to_dingtalk(self, image_content, filetype='image', filename='image.png', mimetype='image/png'):
         access_token = self.get_access_token()
         if not access_token:
             self.logger.error('upload_to_dingtalk failed, cannot get dingtalk access token')
             return None
         files = {
-          'media': (filename, image_content, mimetype),
+            'media': (filename, image_content, mimetype),
         }
         values = {
-          'type': filetype,
+            'type': filetype,
         }
         upload_url = ('https://oapi.dingtalk.com/media/upload?access_token=%s'
                       ) % urllib.parse.quote_plus(access_token)
         try:
             response = requests.post(upload_url, data=values, files=files)
             if response.status_code == 401:
                 self.reset_access_token()
```

### Comparing `dingtalk-stream-0.4.0/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.5.0/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.4.0/setup.py` & `dingtalk-stream-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.4.0',
+    version='0.5.0',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

