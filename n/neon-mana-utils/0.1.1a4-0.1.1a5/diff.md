# Comparing `tmp/neon-mana-utils-0.1.1a4.tar.gz` & `tmp/neon-mana-utils-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-mana-utils-0.1.1a4.tar", last modified: Wed Jun 21 13:20:39 2023, max compression
+gzip compressed data, was "neon-mana-utils-0.1.1a5.tar", last modified: Wed Jun 21 14:27:23 2023, max compression
```

## Comparing `neon-mana-utils-0.1.1a4.tar` & `neon-mana-utils-0.1.1a5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:20:39.125173 neon-mana-utils-0.1.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-21 13:20:39.125173 neon-mana-utils-0.1.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:20:39.125173 neon-mana-utils-0.1.1a4/neon_mana_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/bus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/core_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/skills.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/neon_mana_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:20:39.125173 neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-21 13:20:39.000000 neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 13:20:39.000000 neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:20:39.000000 neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 13:20:39.000000 neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 13:20:39.000000 neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 13:20:39.000000 neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:20:39.125173 neon-mana-utils-0.1.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-21 13:20:34.000000 neon-mana-utils-0.1.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:23.709061 neon-mana-utils-0.1.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-21 14:27:23.709061 neon-mana-utils-0.1.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:23.709061 neon-mana-utils-0.1.1a5/neon_mana_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/bus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/core_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/skills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/neon_mana_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:23.709061 neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-21 14:27:23.000000 neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 14:27:23.000000 neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:27:23.000000 neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 14:27:23.000000 neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 14:27:23.000000 neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 14:27:23.000000 neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:27:23.709061 neon-mana-utils-0.1.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-21 14:27:17.000000 neon-mana-utils-0.1.1a5/setup.py
```

### Comparing `neon-mana-utils-0.1.1a4/LICENSE.md` & `neon-mana-utils-0.1.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/PKG-INFO` & `neon-mana-utils-0.1.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mana-utils
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: Message Application for Neon AI
 Home-page: https://github.com/neongeckocom/neon-mana-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-mana-utils-0.1.1a4/README.md` & `neon-mana-utils-0.1.1a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/__init__.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/bus_api.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/bus_api.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/cli.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,18 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import click
 import json
 
 from pprint import pformat
-
-import click
 from click_default_group import DefaultGroup
 from mycroft_bus_client.client import MessageBusClient
 
 from neon_mana_utils.config import get_messagebus_config
 from neon_mana_utils.version import __version__
 
 
@@ -80,24 +79,27 @@
               help="host to connect to (IP or hostname)")
 @click.option('--port', '-p', default=None,
               help="port to connect to")
 @click.option('--ssl', default=False,
               help="Connect using secured websocket")
 @click.option('--route', '-r', default=None,
               help="websocket route to connect to")
-def tail_messagebus(host, port, route, ssl, format, include, exclude):
+@click.option('--include-session', '-s', is_flag=True,
+              help="Include session context in output")
+def tail_messagebus(host, port, route, ssl, format, include, exclude,
+                    include_session):
     from neon_mana_utils.messagebus import tail_messagebus
     default = get_messagebus_config()
     config = {"host": host or default["host"],
               "port": port or default["port"],
               "route": route or default["route"],
               "ssl": ssl or default["ssl"]}
     client = MessageBusClient(**config)
     client.run_in_thread()
-    tail_messagebus(include, exclude, format, True, client)
+    tail_messagebus(include, exclude, format, True, client, include_session)
     click.echo("Exiting")
 
 
 @neon_mana_cli.command(help="Start listening immediately")
 def listen():
     from neon_mana_utils.core_commands import start_listening
     client = MessageBusClient(**get_messagebus_config())
@@ -134,25 +136,29 @@
 
 
 @neon_mana_cli.command(help="Get an STT response")
 @click.option('--file', '-f', default=None,
               help="File to transcribe")
 @click.option('--lang', '-l', default="en-us",
               help="Language of audio in file")
-def get_stt(file, lang):
+@click.option('--include-session', '-s', is_flag=True,
+              help="Include session context in output")
+def get_stt(file, lang, include_session):
     from neon_mana_utils.bus_api import get_stt
 
     if not file:
         click.echo("No audio file specified")
         return
 
     client = MessageBusClient(**get_messagebus_config())
     client.run_in_thread()
     message = get_stt(client, audio_path=file, lang=lang)
     if message:
+        if not include_session:
+            message.context.pop("session", None)
         click.echo(pformat(json.loads(message.serialize())))
     else:
         click.echo("No Response")
 
 
 @neon_mana_cli.command(help="Get a TTS response")
 @click.option('--text', '-t', default=None,
@@ -194,56 +200,76 @@
 
 
 @neon_mana_cli.command(help="Get a skill response")
 @click.option('--utterance', '-u',
               help="Input utterance to send to skills")
 @click.option('--lang', '-l', default="en-us",
               help="Language of the input utterance")
-def get_response(utterance, lang):
+@click.option('--include-session', '-s', is_flag=True,
+              help="Include session context in output")
+def get_response(utterance, lang, include_session):
     from neon_mana_utils.bus_api import get_response
     # TODO: Handle message loading DM
     if not utterance:
         click.echo("Empty utterance received")
     client = MessageBusClient(**get_messagebus_config())
     client.run_in_thread()
     message = get_response(client, utterance, lang)
     if message:
+        if not include_session:
+            message.context.pop("session", None)
         click.echo(pformat(json.loads(message.serialize())))
     else:
         click.echo("No Response")
 
 
 @neon_mana_cli.command(help="Send a json or yaml serialized message")
 @click.option('--response', '-r', default=None,
               help="Optional response message type to listen to")
+@click.option('--include-session', '-s', is_flag=True,
+              help="Include session context in output")
 @click.argument('file')
-def send_message_file(response, file):
+def send_message_file(response, include_session, file):
     from neon_mana_utils.messagebus import send_message_file
     client = MessageBusClient(**get_messagebus_config())
     client.run_in_thread()
     try:
         response = send_message_file(file, client, response)
         if response:
+            if not include_session:
+                response.context.pop('session', None)
             click.echo(pformat(json.loads(response.serialize())))
         elif response:
             click.echo("No Response")
         else:
             click.echo("Message Sent")
     except Exception as e:
         click.echo(e)
 
 
 @neon_mana_cli.command(help="Send a simple message with no data or context")
+@click.option('--response', '-r', is_flag=True,
+              help="Listen for `.response` message")
+@click.option('--include-session', '-s', is_flag=True,
+              help="Include session context in output")
 @click.argument('message')
-def send_message(message):
+def send_message(response, include_session, message):
     from neon_mana_utils.messagebus import send_message_simple
     client = MessageBusClient(**get_messagebus_config())
     client.run_in_thread()
-    send_message_simple(message, client)
-    click.echo(f"Sent: {message}")
+    resp = send_message_simple(message, client, response)
+    if response:
+        if not resp:
+            click.echo("No Response")
+            return
+        if not include_session:
+            resp.context.pop('session', None)
+        click.echo(pformat(json.loads(resp.serialize())))
+    else:
+        click.echo(f"Sent: {message}")
 
 
 @neon_mana_cli.command(help="Check if a core service is alive")
 @click.option('--namespace', '-n', default="mycroft",
               help="Namespace of service to query")
 @click.argument("service")
 def check_service_alive(namespace, service):
```

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/config.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/config.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/constants.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import json
-
-from mycroft_bus_client.message import Message as _Message
-
-BASE_CONTEXT = {
-    "client_name": "mana",
-    "client": "mana",
-    "source": ["mana"],
-}
-
-
-class Message(_Message):
-    def as_dict(self):
-        return json.loads(self.serialize())
+__version__ = "0.1.1a5"
```

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/core_commands.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/core_commands.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/messagebus.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/messagebus.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,36 +38,43 @@
 
 from neon_mana_utils.config import get_event_filters
 from neon_mana_utils.constants import BASE_CONTEXT, Message
 
 
 def tail_messagebus(include: Set[str] = None, exclude: Set[str] = None,
                     format_output: bool = False, block: bool = False,
-                    client: MessageBusClient = None):
+                    client: MessageBusClient = None,
+                    include_session: bool = False):
     """
     Follow Messagebus activity like you would a logger
     :param include: set of msg_type prefixes to include in output (None to include all)
     :param exclude: set of msg_type prefixes to exclude in output (None to exclude none)
     :param format_output: if True, pformat logged messages
     :param block: if True, block this thread until keyboard interrupt
     :param client: MessageBusClient object to connect and use to monitor
+    :param include_session: if True, include message.context['session']
     """
     def handle_message(serial_message: str):
         message = Message.deserialize(serial_message)
-        if include and not any([x for x in include if message.msg_type.startswith(x)]):
+        if include and not any([x for x in include
+                                if message.msg_type.startswith(x)]):
             # Message not specified in included types
             return
-        if exclude and any([x for x in exclude if message.msg_type.startswith(x)]):
+        if exclude and any([x for x in exclude
+                            if message.msg_type.startswith(x)]):
             # Message is specified in excluded types
             return
+        if not include_session:
+            message.context.pop("session", None)
+        serialized = message.as_dict()
         if format_output:
-            pprint(json.loads(message.serialize()))
+            pprint(serialized)
             print('---')
         else:
-            print(message.serialize())
+            print(serialized)
 
     default_filters = get_event_filters()
     include = include or default_filters.get("include", [])
     exclude = exclude or default_filters.get("exclude", [])
 
     print(f"Connecting to "
           f"{client.config.host}:{client.config.port}{client.config.route}")
@@ -111,13 +118,16 @@
 
     if response:
         return bus.wait_for_response(message, response, 10)
     else:
         bus.emit(message)
 
 
-def send_message_simple(msg_type: str, bus: MessageBusClient):
+def send_message_simple(msg_type: str, bus: MessageBusClient,
+                        expect_response: bool = False):
     """
     Send a message with no data or context. This can be useful for mocking
     ready messages or audio status changes.
     """
+    if expect_response:
+        return bus.wait_for_response(Message(msg_type))
     bus.emit(Message(msg_type))
```

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/skills.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/skills.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/status.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/status.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils/version.py` & `neon-mana-utils-0.1.1a5/neon_mana_utils/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,8 +22,28 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a4"
+import json
+
+from mycroft_bus_client.message import Message as _Message
+
+BASE_CONTEXT = {
+    "client_name": "mana",
+    "client": "mana",
+    "source": ["mana"],
+}
+
+
+class Message(_Message):
+    @staticmethod
+    def deserialize(value):
+        obj = json.loads(value)
+        return Message(obj.get('type') or '',
+                       obj.get('data') or {},
+                       obj.get('context') or {})
+
+    def as_dict(self):
+        return json.loads(self.serialize())
```

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/PKG-INFO` & `neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mana-utils
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: Message Application for Neon AI
 Home-page: https://github.com/neongeckocom/neon-mana-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-mana-utils-0.1.1a4/neon_mana_utils.egg-info/SOURCES.txt` & `neon-mana-utils-0.1.1a5/neon_mana_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.1.1a4/setup.py` & `neon-mana-utils-0.1.1a5/setup.py`

 * *Files identical despite different names*

