# Comparing `tmp/neon-skill-fallback_llm-0.0.3a2.tar.gz` & `tmp/neon-skill-fallback_llm-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-fallback_llm-0.0.3a2.tar", last modified: Thu Jun 15 22:14:48 2023, max compression
+gzip compressed data, was "neon-skill-fallback_llm-0.0.3a3.tar", last modified: Wed Jun 21 03:25:44 2023, max compression
```

## Comparing `neon-skill-fallback_llm-0.0.3a2.tar` & `neon-skill-fallback_llm-0.0.3a3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.642590 neon-skill-fallback_llm-0.0.3a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.642590 neon-skill-fallback_llm-0.0.3a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/end_chat.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/fallback_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/fallback_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/no_chat_history.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/no_chatgpt.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/no_email_address.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/notify_llm_active.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/sending_chat_history.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/dialog/start_chat.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/intent/ask_chatgpt.intent
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/intent/chat_with_llm.intent
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/intent/disable_fallback.intent
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/intent/email_chat_history.intent
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/intent/enable_fallback.intent
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/intent/llm.entity
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/vocab/chat_gpt.voc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/locale/en-us/vocab/exit.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-15 22:14:48.000000 neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 22:14:48.000000 neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:14:48.000000 neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 22:14:48.000000 neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:14:48.000000 neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:14:48.000000 neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:14:48.646590 neon-skill-fallback_llm-0.0.3a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:14:44.000000 neon-skill-fallback_llm-0.0.3a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.578086 neon-skill-fallback_llm-0.0.3a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 03:25:44.578086 neon-skill-fallback_llm-0.0.3a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.570086 neon-skill-fallback_llm-0.0.3a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.570086 neon-skill-fallback_llm-0.0.3a3/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.574086 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/end_chat.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/fallback_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/fallback_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/no_chat_history.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/no_chatgpt.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/no_email_address.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/notify_llm_active.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/sending_chat_history.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/dialog/start_chat.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.574086 neon-skill-fallback_llm-0.0.3a3/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/intent/ask_llm.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/intent/chat_with_llm.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/intent/disable_fallback.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/intent/email_chat_history.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/intent/enable_fallback.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/intent/llm.entity
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.574086 neon-skill-fallback_llm-0.0.3a3/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/vocab/chat_gpt.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/vocab/exit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/locale/en-us/vocab/fastchat.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.578086 neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 03:25:44.000000 neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-21 03:25:44.000000 neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:25:44.000000 neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 03:25:44.000000 neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 03:25:44.000000 neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 03:25:44.000000 neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:25:44.578086 neon-skill-fallback_llm-0.0.3a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:25:44.578086 neon-skill-fallback_llm-0.0.3a3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 03:25:41.000000 neon-skill-fallback_llm-0.0.3a3/version.py
```

### Comparing `neon-skill-fallback_llm-0.0.3a2/LICENSE` & `neon-skill-fallback_llm-0.0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_llm-0.0.3a2/LICENSE.md` & `neon-skill-fallback_llm-0.0.3a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_llm-0.0.3a2/PKG-INFO` & `neon-skill-fallback_llm-0.0.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback_llm
-Version: 0.0.3a2
+Version: 0.0.3a3
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_llm
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-fallback_llm-0.0.3a2/README.md` & `neon-skill-fallback_llm-0.0.3a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_llm-0.0.3a2/__init__.py` & `neon-skill-fallback_llm-0.0.3a3/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,35 +26,38 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from enum import Enum
 from threading import Thread
 from time import time
 
 from lingua_franca.format import nice_duration
+from ovos_bus_client import Message
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 # from ovos_workshop.skills.fallback import FallbackSkill
 from neon_utils.skills.neon_fallback_skill import NeonFallbackSkill, NeonSkill
 from neon_utils.message_utils import get_message_user
 from neon_utils.user_utils import get_user_prefs
 from neon_mq_connector.utils.client_utils import send_mq_request
 
 from mycroft.skills.mycroft_skill.decorators import intent_handler
 
 
 class LLM(Enum):
     GPT = "Chat GPT"
+    FASTCHAT = "FastChat"
 
 
 class LLMSkill(NeonFallbackSkill):
     def __init__(self, **kwargs):
         NeonFallbackSkill.__init__(self, **kwargs)
         self.chat_history = dict()
         self._default_user = "local"
+        self._default_llm = LLM.FASTCHAT
         self.chatting = dict()
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(internet_before_load=True,
                                    network_before_load=True,
                                    gui_before_load=False,
@@ -79,15 +82,15 @@
         # TODO: Resolve Padatious entity file handling bug
         if self.fallback_enabled:
             self.register_fallback(self.fallback_llm, 85)
 
     def fallback_llm(self, message):
         utterance = message.data['utterance']
         user = get_message_user(message) or self._default_user
-        answer = self._get_llm_response(utterance, user)
+        answer = self._get_llm_response(utterance, user, self._default_llm)
         if not answer:
             LOG.info(f"No fallback response")
             return False
         self.speak(answer)
         return True
 
     @intent_handler("enable_fallback.intent")
@@ -100,41 +103,37 @@
     @intent_handler("disable_fallback.intent")
     def handle_disable_fallback(self, message):
         if self.fallback_enabled:
             self.settings['fallback_enabled'] = False
             self.remove_fallback(self.fallback_llm)
         self.speak_dialog("fallback_disabled")
 
-    @intent_handler("ask_chatgpt.intent")
+    @intent_handler("ask_llm.intent")
     def handle_ask_chatgpt(self, message):
         utterance = message.data['utterance']
+        llm = self._get_requested_llm(message)
         user = get_message_user(message) or self._default_user
         try:
-            resp = self._get_llm_response(utterance, user)
+            resp = self._get_llm_response(utterance, user, llm)
             self.speak(resp)
         except Exception as e:
             LOG.exception(e)
             self.speak_dialog("no_chatgpt")
 
     @intent_handler("chat_with_llm.intent")
     def handle_chat_with_llm(self, message):
         user = get_message_user(message) or self._default_user
         self.gui.show_controlled_notification(
             self.translate("notify_llm_active"))
-        llm = message.data.get('llm')
-        if self.voc_match(llm, "chat_gpt"):
-            llm = LLM.GPT
-        else:
-            LOG.warning(f"Requested invalid LLM: {llm}")
-            llm = LLM.GPT
+        llm = self._get_requested_llm(message)
         timeout_duration = nice_duration(self.chat_timeout_seconds)
         self.speak_dialog("start_chat", {"llm": llm.value,
                                          "timeout": timeout_duration},
                           private=True)
-        self._reset_expiration(user)
+        self._reset_expiration(user, llm)
 
     @intent_handler("email_chat_history.intent")
     def handle_email_chat_history(self, message):
         user_prefs = get_user_prefs(message)['user']
         username = user_prefs['username']
         email_addr = user_prefs['email']
         if username not in self.chat_history:
@@ -163,60 +162,78 @@
         user = get_message_user(message) or self._default_user
         self.gui.remove_controlled_notification()
         self.chatting.pop(user)
         self.speak_dialog("end_chat")
         event_name = f"end_converse.{user}"
         self.cancel_scheduled_event(event_name)
 
-    def _get_llm_response(self, query: str, user: str) -> str:
+    def _get_llm_response(self, query: str, user: str, llm: LLM) -> str:
         """
         Get a response from an LLM
         :param query: User utterance to generate a response to
         :param user: Username making the request
         :returns: Speakable response to the user's query
         """
-        # TODO: support multiple LLM backends?
+        if llm == LLM.GPT:
+            queue = "chat_gpt_input"
+        elif llm == LLM.FASTCHAT:
+            queue = "fastchat_input"
+        else:
+            raise ValueError(f"Expected LLM, got: {llm}")
         self.chat_history.setdefault(user, list())
         mq_resp = send_mq_request("/llm", {"query": query,
                                            "history": self.chat_history[user]},
-                                  "chat_gpt_input")
+                                  queue)
         resp = mq_resp.get("response") or ""
         if resp:
             username = "user" if user == self._default_user else user
             self.chat_history[user].append((username, query))
             self.chat_history[user].append(("llm", resp))
         LOG.debug(f"Got LLM response: {resp}")
         return resp
 
+    def _get_requested_llm(self, message: Message) -> LLM:
+        request = message.data.get('llm') or message.data.get('utterance')
+        if self.voc_match(request, "chat_gpt"):
+            llm = LLM.GPT
+        elif self.voc_match(request, "fastchat"):
+            llm = LLM.FASTCHAT
+        else:
+            LOG.warning(f"No valid LLM in request: {request}")
+            llm = LLM.GPT
+        return llm
+
     def converse(self, message=None):
         user = get_message_user(message) or self._default_user
         if user not in self.chatting:
             return False
-        last_message = self.chatting[user]
+        last_message = self.chatting[user][0]
         if time() - last_message > self.chat_timeout_seconds:
             LOG.info(f"Chat session timed out")
             self._stop_chatting(message)
             return False
         # Take final utterance as one that wasn't normalized
         utterance = message.data.get('utterances', [""])[-1]
-        if self.voc_match(utterance, "exit"):
+        if self.voc_match(utterance, "exit") and len(utterance.split()) < 4:
+            # TODO: Imperfect check for "stop" or "exit"
             self._stop_chatting(message)
             return True
         Thread(target=self._threaded_converse, args=(utterance, user),
                daemon=True).start()
         return True
 
     def _threaded_converse(self, utterance, user):
         try:
-            resp = self._get_llm_response(utterance, user)
+            llm = self.chatting[user][1]
+            resp = self._get_llm_response(utterance, user, llm)
             self.speak(resp)
-            self._reset_expiration(user)
+            self._reset_expiration(user, llm)
         except Exception as e:
             LOG.exception(e)
             self.speak_dialog("no_chatgpt")
 
-    def _reset_expiration(self, user):
-        self.chatting[user] = time()
+    def _reset_expiration(self, user, llm):
+        self.chatting[user] = (time(), llm)
         event_name = f"end_converse.{user}"
         self.cancel_scheduled_event(event_name)
         self.schedule_event(self._stop_chatting, self.chat_timeout_seconds,
                             {'user': user}, event_name)
```

### Comparing `neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/PKG-INFO` & `neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback-llm
-Version: 0.0.3a2
+Version: 0.0.3a3
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_llm
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-fallback_llm-0.0.3a2/neon_skill_fallback_llm.egg-info/SOURCES.txt` & `neon-skill-fallback_llm-0.0.3a3/neon_skill_fallback_llm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 locale/en-us/dialog/fallback_enabled.dialog
 locale/en-us/dialog/no_chat_history.dialog
 locale/en-us/dialog/no_chatgpt.dialog
 locale/en-us/dialog/no_email_address.dialog
 locale/en-us/dialog/notify_llm_active.dialog
 locale/en-us/dialog/sending_chat_history.dialog
 locale/en-us/dialog/start_chat.dialog
-locale/en-us/intent/ask_chatgpt.intent
+locale/en-us/intent/ask_llm.intent
 locale/en-us/intent/chat_with_llm.intent
 locale/en-us/intent/disable_fallback.intent
 locale/en-us/intent/email_chat_history.intent
 locale/en-us/intent/enable_fallback.intent
 locale/en-us/intent/llm.entity
 locale/en-us/vocab/chat_gpt.voc
 locale/en-us/vocab/exit.voc
+locale/en-us/vocab/fastchat.voc
 neon_skill_fallback_llm.egg-info/PKG-INFO
 neon_skill_fallback_llm.egg-info/SOURCES.txt
 neon_skill_fallback_llm.egg-info/dependency_links.txt
 neon_skill_fallback_llm.egg-info/entry_points.txt
 neon_skill_fallback_llm.egg-info/requires.txt
 neon_skill_fallback_llm.egg-info/top_level.txt
 test/test_skill.py
```

### Comparing `neon-skill-fallback_llm-0.0.3a2/setup.py` & `neon-skill-fallback_llm-0.0.3a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_llm-0.0.3a2/skill.json` & `neon-skill-fallback_llm-0.0.3a3/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_llm-0.0.3a2/test/test_skill.py` & `neon-skill-fallback_llm-0.0.3a3/test/test_skill.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from os.path import dirname, join, exists
 from mock import Mock
 from ovos_utils.messagebus import FakeBus
 from ovos_bus_client import Message
 from lingua_franca import load_language
 from mycroft.skills.skill_loader import SkillLoader
 
+from skill_fallback_llm import LLM
+
 
 class TestSkill(unittest.TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         bus = FakeBus()
         bus.run_in_thread()
         skill_loader = SkillLoader(bus, dirname(dirname(__file__)))
@@ -85,15 +87,21 @@
         mock = Mock()
         self.skill._get_llm_response = mock
         mock.return_value = "test"
 
         fake_msg = Message("test", {"utterance": "testing"},
                            {"username": "test_user"})
         self.skill.handle_ask_chatgpt(fake_msg)
-        mock.assert_called_once_with("testing", "test_user")
+        mock.assert_called_once()
+        args = mock.call_args[0]
+        self.assertEqual(args[0], 'testing')
+        self.assertEqual(args[1], 'test_user')
+        self.assertEqual(args[2].value, LLM.GPT.value)
+        # TODO: Diagnose failure
+        # mock.assert_called_once_with("testing", "test_user", LLM.GPT)
         self.skill.speak.assert_called_once_with("test")
 
         def raise_exception():
             raise Exception()
 
         mock.side_effect = raise_exception
         self.skill.handle_ask_chatgpt(fake_msg)
@@ -105,15 +113,18 @@
     def test_handle_chat_with_llm(self):
         self.skill.settings['chat_timeout_seconds'] = 300
         load_language(self.skill.lang)
         fake_msg = Message("test", {},
                            {"username": "test_user"})
         self.skill.chatting = dict()
         self.skill.handle_chat_with_llm(fake_msg)
-        self.assertIsInstance(self.skill.chatting["test_user"], float)
+        self.assertIsInstance(self.skill.chatting["test_user"][0], float)
+        # TODO: Diagnose equality failure
+        self.assertEqual(self.skill.chatting["test_user"][1].value,
+                         LLM.GPT.value)
         self.skill.speak_dialog.assert_called_once_with(
             "start_chat", {"llm": "Chat GPT", "timeout": "five minutes"},
             private=True)
 
     def test_handle_email_chat_history(self):
         real_send_email = self.skill._send_email
         self.skill._send_email = Mock()
```

### Comparing `neon-skill-fallback_llm-0.0.3a2/version.py` & `neon-skill-fallback_llm-0.0.3a3/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.3a2"
+__version__ = "0.0.3a3"
```

