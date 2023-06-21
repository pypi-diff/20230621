# Comparing `tmp/whatsapp-chatbot-python-0.3.0.tar.gz` & `tmp/whatsapp-chatbot-python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.3.0.tar", last modified: Tue Jun 20 08:37:10 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.4.0.tar", last modified: Wed Jun 21 17:38:48 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.3.0.tar` & `whatsapp-chatbot-python-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.542245 whatsapp-chatbot-python-0.3.0/
--rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    10908 2023-06-20 08:37:10.541448 whatsapp-chatbot-python-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     9883 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 08:37:10.542245 whatsapp-chatbot-python-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-06-20 08:34:37.000000 whatsapp-chatbot-python-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.530419 whatsapp-chatbot-python-0.3.0/tests/
--rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.533427 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-06-18 19:42:33.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     3673 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.540447 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     3289 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     1881 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-06-15 14:08:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/router.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.537438 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0    10908 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.245029 whatsapp-chatbot-python-0.4.0/
+-rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    10908 2023-06-21 17:38:48.244027 whatsapp-chatbot-python-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9883 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 17:38:48.245029 whatsapp-chatbot-python-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.230992 whatsapp-chatbot-python-0.4.0/tests/
+-rw-rw-rw-   0        0        0     1416 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.234001 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     3783 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.243024 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     3289 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     1881 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-06-15 14:08:46.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/router.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.240017 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0    10908 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.3.0/LICENSE` & `whatsapp-chatbot-python-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.3.0/PKG-INFO` & `whatsapp-chatbot-python-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.3.0
+Version: 0.4.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.3.0/README.md` & `whatsapp-chatbot-python-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.3.0/setup.py` & `whatsapp-chatbot-python-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.3.0",
+    version="0.4.0",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-chatbot-python-0.3.0/tests/test_manager.py` & `whatsapp-chatbot-python-0.4.0/tests/test_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+from unittest.mock import patch
 
 from whatsapp_chatbot_python import GreenAPIBot, Notification
 
 event_example = {
     "typeWebhook": "incomingMessageReceived",
     "messageData": {
         "typeMessage": "textMessage",
@@ -11,42 +12,44 @@
         }
     }
 }
 
 
 class ManagerTestCase(unittest.TestCase):
     def test_router(self):
-        bot = self.bot
+        bot = self.create_bot()
 
         @bot.router.message()
         def message_handler(notification: Notification):
             self.assertEqual(notification.event, event_example)
 
         bot.router.route_event(event_example)
 
     def test_filters(self):
-        bot = self.bot
+        bot = self.create_bot()
 
         @bot.router.message(command="help")
         def command_handler(_):
             raise Exception("filters do not filter messages")
 
         bot.router.route_event(event_example)
 
     def test_observers(self):
-        bot = self.bot
+        bot = self.create_bot()
 
         @bot.router.message()
         def handler(_):
             pass
 
         bot.router.message.add_handler(handler)
 
         self.assertEqual(len(bot.router.message.handlers), 2)
 
-    @property
-    def bot(self):
+    @patch("whatsapp_chatbot_python.bot.Bot._update_settings")
+    def create_bot(self, mock__update_settings):
+        mock__update_settings.return_value = None
+
         return GreenAPIBot("", "")
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/filters.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,61 +12,63 @@
     def check_event(self, event: dict) -> bool:
         pass
 
 
 class ChatIDFilter(AbstractFilter):
     def __init__(self, chat: Union[str, List[str]]):
         self.chat = chat
+        if isinstance(chat, str):
+            self.chat = [chat]
 
     def check_event(self, event: dict) -> bool:
         chat = event["senderData"]["chatId"]
 
-        if chat == self.chat or chat in self.chat:
+        if chat in self.chat:
             return True
         return False
 
 
 class SenderFilter(AbstractFilter):
     def __init__(self, sender: Union[str, List[str]]):
         self.sender = sender
+        if isinstance(sender, str):
+            self.sender = [sender]
 
     def check_event(self, event: dict) -> bool:
         sender = event["senderData"]["sender"]
 
-        if sender == self.sender or sender in self.sender:
+        if sender in self.sender:
             return True
         return False
 
 
 class TypeMessageFilter(AbstractFilter):
     def __init__(self, type_message: Union[str, List[str]]):
         self.type_message = type_message
+        if isinstance(type_message, str):
+            self.type_message = [type_message]
 
     def check_event(self, event: dict) -> bool:
         type_message = event["messageData"]["typeMessage"]
 
-        if (
-                type_message == self.type_message
-                or type_message in self.type_message
-        ):
+        if type_message in self.type_message:
             return True
         return False
 
 
 class TextMessageFilter(AbstractFilter):
     def __init__(self, text_message: Union[str, List[str]]):
         self.text_message = text_message
+        if isinstance(text_message, str):
+            self.text_message = [text_message]
 
     def check_event(self, event: dict) -> bool:
         text_message = self.get_text_message(event)
 
-        if (
-                text_message == self.text_message
-                or text_message in self.text_message
-        ):
+        if text_message in self.text_message:
             return True
         return False
 
     @staticmethod
     def get_text_message(event: dict) -> Optional[str]:
         message_data = event["messageData"]
 
@@ -79,14 +81,15 @@
 
 class RegExpFilter(AbstractFilter):
     def __init__(self, pattern: str):
         self.pattern = pattern
 
     def check_event(self, event: dict) -> bool:
         text_message = TextMessageFilter.get_text_message(event)
+
         if fullmatch(self.pattern, text_message):
             return True
         return False
 
 
 class CommandFilter(AbstractFilter):
     def __init__(self, command: str, prefixes: str = "/"):
```

### Comparing `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/handler.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.3.0
+Version: 0.4.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

