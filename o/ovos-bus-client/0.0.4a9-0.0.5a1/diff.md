# Comparing `tmp/ovos-bus-client-0.0.4a9.tar.gz` & `tmp/ovos-bus-client-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.4a9.tar", last modified: Sat May  6 01:20:15 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.5a1.tar", last modified: Wed Jun 21 01:30:16 2023, max compression
```

## Comparing `ovos-bus-client-0.0.4a9.tar` & `ovos-bus-client-0.0.5a1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15910 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22546 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/setup.py
```

### Comparing `ovos-bus-client-0.0.4a9/LICENSE.md` & `ovos-bus-client-0.0.5a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a9/PKG-INFO` & `ovos-bus-client-0.0.5a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a9
+Version: 0.0.5a1
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import time
 import traceback
 from os import getpid
 from threading import Event, Thread
+from typing import Union, Callable, Any, List, Optional
 from uuid import uuid4
 
-from ovos_utils.log import LOG
+from ovos_utils.log import LOG, deprecated
 from pyee import ExecutorEventEmitter
 from websocket import (WebSocketApp,
                        WebSocketConnectionClosedException,
                        WebSocketException)
 
 from ovos_bus_client.client.collector import MessageCollector
 from ovos_bus_client.client.waiter import MessageWaiter
@@ -56,51 +57,53 @@
         self.client = self.create_client()
         self.retry = 5
         self.connected_event = Event()
         self.started_running = False
         self.wrapped_funcs = {}
 
     @staticmethod
-    def build_url(host, port, route, ssl):
-        """Build a websocket url."""
-        return '{scheme}://{host}:{port}{route}'.format(
-            scheme='wss' if ssl else 'ws',
-            host=host,
-            port=str(port),
-            route=route)
-
-    def create_client(self):
-        """Setup websocket client."""
-        url = MessageBusClient.build_url(ssl=self.config.ssl,
-                                         host=self.config.host,
-                                         port=self.config.port,
-                                         route=self.config.route)
+    def build_url(host: str, port: int, route: str, ssl: bool) -> str:
+        """
+        Build a websocket url.
+        """
+        return f"{'wss' if ssl else 'ws'}://{host}:{port}{route}"
+
+    def create_client(self) -> WebSocketApp:
+        """
+        Setup websocket client.
+        """
+        url = self.build_url(ssl=self.config.ssl,
+                             host=self.config.host,
+                             port=self.config.port,
+                             route=self.config.route)
         return WebSocketApp(url, on_open=self.on_open, on_close=self.on_close,
                             on_error=self.on_error, on_message=self.on_message)
 
     def on_open(self, *args):
-        """Handle the "open" event from the websocket.
-
+        """
+        Handle the "open" event from the websocket.
         A Basic message with the name "open" is forwarded to the emitter.
         """
-        LOG.info("Connected")
+        LOG.debug("Connected")
         self.connected_event.set()
         self.emitter.emit("open")
         # Restore reconnect timer to 5 seconds on sucessful connect
         self.retry = 5
 
     def on_close(self, *args):
-        """Handle the "close" event from the websocket.
-
+        """
+        Handle the "close" event from the websocket.
         A Basic message with the name "close" is forwarded to the emitter.
         """
         self.emitter.emit("close")
 
     def on_error(self, *args):
-        """On error start trying to reconnect to the websocket."""
+        """
+        On error start trying to reconnect to the websocket.
+        """
         if len(args) == 1:
             error = args[0]
         else:
             error = args[1]
         if isinstance(error, WebSocketConnectionClosedException):
             LOG.warning('Could not send message because connection has closed')
         elif isinstance(error, ConnectionRefusedError):
@@ -123,30 +126,31 @@
             self.emitter.emit('reconnecting')
             self.client = self.create_client()
             self.run_forever()
         except WebSocketException:
             pass
 
     def on_message(self, *args):
-        """Handle incoming websocket message.
-
-        Args:
-            message (str): serialized Mycroft Message
+        """
+        Handle an incoming websocket message
+        @param args:
+            message (str): serialized Message
         """
         if len(args) == 1:
             message = args[0]
         else:
             message = args[1]
         parsed_message = Message.deserialize(message)
         SessionManager.update(Session.from_message(parsed_message))
         self.emitter.emit('message', message)
         self.emitter.emit(parsed_message.msg_type, parsed_message)
 
-    def emit(self, message):
-        """Send a message onto the message bus.
+    def emit(self, message: Message):
+        """
+        Send a message onto the message bus.
 
         This will both send the message to the local process using the
         event emitter and onto the Mycroft websocket for other processes.
 
         Args:
             message (Message): Message to send
         """
@@ -166,18 +170,21 @@
                 self.client.send(message.serialize())
             else:
                 self.client.send(json.dumps(message.__dict__))
         except WebSocketConnectionClosedException:
             LOG.warning('Could not send %s message because connection '
                         'has been closed', message.msg_type)
 
-    def collect_responses(self, message,
-                          min_timeout=0.2, max_timeout=3.0,
-                          direct_return_func=lambda msg: False):
-        """Collect responses from multiple handlers.
+    def collect_responses(self, message: Message,
+                          min_timeout: Union[int, float] = 0.2,
+                          max_timeout: Union[int, float] = 3.0,
+                          direct_return_func: Callable[[Message], Any] =
+                          lambda msg: False) -> List[Message]:
+        """
+        Collect responses from multiple handlers.
 
         This sets up a collect-call (pun intended) expecting multiple handlers
         to respond.
 
         Args:
             message (Message): message to send
             min_timeout (int/float): Minimum time to wait for a response
@@ -189,16 +196,19 @@
                 (list) collected response messages.
         """
         collector = MessageCollector(self, message,
                                      min_timeout, max_timeout,
                                      direct_return_func)
         return collector.collect()
 
-    def on_collect(self, event_name, func, timeout=2):
-        """Create a handler for a collect_responses call.
+    def on_collect(self, event_name: str,
+                   func: Callable[[CollectionMessage], Any],
+                   timeout: Union[int, float] = 2):
+        """
+        Create a handler for a collect_responses call.
 
         This immeditely responds with an ack to register the handler with
         the caller, promising to return a response.
 
         The handler function then needs to send a response.
 
         Args:
@@ -218,29 +228,35 @@
                                           'timeout': timeout})
             self.emit(acknowledge)
             func(CollectionMessage.from_message(msg, handler_id, collect_id))
 
         self.wrapped_funcs[func] = wrapper
         self.on(event_name, wrapper)
 
-    def wait_for_message(self, message_type, timeout=3.0):
-        """Wait for a message of a specific type.
+    def wait_for_message(self, message_type: str,
+                         timeout: Union[int, float] = 3.0) -> Optional[Message]:
+        """
+        Wait for a message of a specific type.
 
         Arguments:
             message_type (str): the message type of the expected message
             timeout: seconds to wait before timeout, defaults to 3
 
         Returns:
             The received message or None if the response timed out
         """
 
         return MessageWaiter(self, message_type).wait(timeout)
 
-    def wait_for_response(self, message, reply_type=None, timeout=3.0):
-        """Send a message and wait for a response.
+    def wait_for_response(self, message: Message,
+                          reply_type: Optional[str] = None,
+                          timeout: Union[float, int] = 3.0) -> \
+            Optional[Message]:
+        """
+        Send a message and wait for a response.
 
         Arguments:
             message (Message): message to send
             reply_type (str): the message type of the expected reply.
                               Defaults to "<message.msg_type>.response".
             timeout: seconds to wait before timeout, defaults to 3
 
@@ -249,33 +265,33 @@
         """
         message_type = reply_type or message.msg_type + '.response'
         waiter = MessageWaiter(self, message_type)  # Setup response handler
         # Send message and wait for it's response
         self.emit(message)
         return waiter.wait(timeout)
 
-    def on(self, event_name, func):
+    def on(self, event_name: str, func: Callable[[Message], Any]):
         """Register callback with event emitter.
 
         Args:
             event_name (str): message type to map to the callback
             func (callable): callback function
         """
         self.emitter.on(event_name, func)
 
-    def once(self, event_name, func):
+    def once(self, event_name: str, func: Callable[[Message], Any]):
         """Register callback with event emitter for a single call.
 
         Args:
             event_name (str): message type to map to the callback
             func (callable): callback function
         """
         self.emitter.once(event_name, func)
 
-    def remove(self, event_name, func):
+    def remove(self, event_name: str, func: Callable[[Message], Any]):
         """Remove registered event.
 
         Args:
             event_name (str): message type to map to the callback
             func (callable): callback function
         """
         if func in self.wrapped_funcs:
@@ -308,31 +324,36 @@
                 LOG.warning("       %s", repr(self.emitter._events[evt]))
             if event_name in self.emitter._events:
                 LOG.debug("Removing found '%s'", event_name)
             else:
                 LOG.debug("Not able to find '%s'", event_name)
             LOG.warning('----- End dump -----')
 
-    def remove_all_listeners(self, event_name):
-        """Remove all listeners connected to event_name.
+    def remove_all_listeners(self, event_name: str):
+        """
+        Remove all listeners connected to event_name.
 
-            Arguments:
-                event_name: event from which to remove listeners
+        Arguments:
+            event_name: event from which to remove listeners
         """
         if event_name is None:
             raise ValueError
         self.emitter.remove_all_listeners(event_name)
 
     def run_forever(self):
-        """Start the websocket handling."""
+        """
+        Start the websocket handling.
+        """
         self.started_running = True
         self.client.run_forever()
 
     def close(self):
-        """Close the websocket connection."""
+        """
+        Close the websocket connection.
+        """
         self.client.close()
         self.connected_event.clear()
 
     def run_in_thread(self):
         """Launches the run_forever in a separate daemon thread."""
         t = Thread(target=self.run_forever)
         t.daemon = True
@@ -346,16 +367,17 @@
                  emitter=None, cache=False, client_name="ovos-gui-client"):
         self.gui_id = f"{client_name}_{getpid()}"
         config_overrides = dict(host=host, port=port, route=route, ssl=ssl)
         config = load_gui_message_bus_config(**config_overrides)
         super().__init__(host=config.host, port=config.port, route=config.route,
                          ssl=config.ssl, emitter=emitter, cache=cache)
 
-    def emit(self, message):
-        """Send a message onto the message bus.
+    def emit(self, message: GUIMessage):
+        """
+        Send a message onto the message bus.
 
         This will both send the message to the local process using the
         event emitter and onto the Mycroft websocket for other processes.
 
         Args:
             message (GUIMessage): Message to send
         """
@@ -377,38 +399,38 @@
 
     def on_open(self, *args):
         super().on_open(*args)
         self.emit(GUIMessage("mycroft.gui.connected",
                              gui_id=self.gui_id))
 
     def on_message(self, *args):
-        """Handle incoming websocket message.
-
-        Args:
-            message (str): GUI protocol bus message
+        """
+        Handle an incoming websocket message
+        @param args:
+            message (str): serialized Message
         """
         if len(args) == 1:
             message = args[0]
         else:
             message = args[1]
 
         self.emitter.emit('message', message)
 
         parsed_message = GUIMessage.deserialize(message)
         self.emitter.emit(parsed_message.msg_type, parsed_message)
 
 
+@deprecated("No direct replacement", "0.1.0")
 def echo():
-    """Echo function repeating all input from a user."""
+    """
+    Echo function repeating all input from a user.
+    """
+    # TODO: Deprecate in 0.1.0
     message_bus_client = MessageBusClient()
 
     def repeat_utterance(message):
         message.msg_type = 'speak'
         message_bus_client.emit(message)
 
     message_bus_client.on('message', create_echo_function(None))
     message_bus_client.on('recognizer_loop:utterance', repeat_utterance)
     message_bus_client.run_forever()
-
-
-if __name__ == "__main__":
-    echo()
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/message.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import inspect
 import json
 import re
 from copy import deepcopy
 from typing import Optional
 from binascii import hexlify, unhexlify
 from ovos_utils.gui import _GUIDict
-from ovos_utils.log import LOG
+from ovos_utils.log import LOG, deprecated
 from ovos_utils.security import encrypt, decrypt
 from ovos_config.config import Configuration
 
 try:
     from lingua_franca.parse import normalize
 except ImportError:
     # optional LF import
@@ -81,15 +81,15 @@
             destination or domain.
     """
     # if set all messages are AES encrypted
     _secret_key = Configuration().get("websocket", {}).get("secret_key")
     # if set to False, will refuse to deserialize unencrypted messages for processing
     _allow_unencrypted = Configuration().get("websocket", {}).get("allow_unencrypted", _secret_key is None)
 
-    def __init__(self, msg_type, data=None, context=None):
+    def __init__(self, msg_type: str, data: dict = None, context: dict = None):
         """Used to construct a message object
 
         Message objects will be used to send information back and forth
         between processes of mycroft service, voice, skill and cli
         """
         data = data or {}
         context = context or {}
@@ -102,35 +102,35 @@
     def __eq__(self, other):
         if not isinstance(other, Message):
             return False
         return other.msg_type == self.msg_type and \
             other.data == self.data and \
             other.context == self.context
 
-    def serialize(self):
+    def serialize(self) -> str:
         """This returns a string of the message info.
 
         This makes it easy to send over a websocket. This uses
         json dumps to generate the string with type, data and context
 
         Returns:
             str: a json string representation of the message.
         """
         # handle Session and Message objects
         data = self._json_dump(self.data)
         ctxt = self._json_dump(self.context)
 
         msg = json.dumps({'type': self.msg_type, 'data': data, 'context': ctxt})
         if self._secret_key:
-            payload = encrypt_as_dict(msg)
+            payload = encrypt_as_dict(self._secret_key, msg)
             return json.dumps(payload)
         return msg
 
     @property
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return json.loads(self.serialize())
 
     @staticmethod
     def _json_dump(value):
         def serialize_item(x):
             try:
                 if hasattr(x, "serialize"):
@@ -153,22 +153,23 @@
         if isinstance(value, str):
             obj = json.loads(value)
         else:
             obj = value
         assert isinstance(obj, dict)
         if Message._secret_key:
             if 'ciphertext' in obj:
-                obj = decrypt_from_dict(obj)
+                obj = decrypt_from_dict(Message._secret_key, obj)
             elif not Message._allow_unencrypted:
                 raise RuntimeError("got an unencrypted message, configured to refuse")
         return obj
 
     @staticmethod
-    def deserialize(value):
-        """This takes a string and constructs a message object.
+    def deserialize(value: str) -> _MsgBase:
+        """
+        This takes a string and constructs a message object.
 
         This makes it easy to take strings from the websocket and create
         a message object.  This uses json loads to get the info and generate
         the message object.
 
         Args:
             value(str): This is the json string received from the websocket
@@ -179,16 +180,17 @@
             value(str): This is the string received from the websocket
         """
         obj = Message._json_load(value)
         return Message(obj.get('type') or '',
                        obj.get('data') or {},
                        obj.get('context') or {})
 
-    def forward(self, msg_type, data=None):
-        """ Keep context and forward message
+    def forward(self, msg_type: str, data: dict = None) -> _MsgBase:
+        """
+        Keep context and forward message
 
         This will take the same parameters as a message object but use
         the current message object as a reference.  It will copy the context
         from the existing message object.
 
         Args:
             msg_type (str): type of message
@@ -196,16 +198,18 @@
 
         Returns:
             Message: Message object to be used on the reply to the message
         """
         data = data or {}
         return Message(msg_type, data, context=self.context)
 
-    def reply(self, msg_type, data=None, context=None):
-        """Construct a reply message for a given message
+    def reply(self, msg_type: str, data: dict = None,
+              context: dict = None) -> _MsgBase:
+        """
+        Construct a reply message for a given message
 
         This will take the same parameters as a message object but use
         the current message object as a reference.  It will copy the context
         from the existing message object and add any context passed in to
         the function.  Check for a destination passed in to the function from
         the data object and add that to the context as a destination.  If the
         context has a source then that will be swapped with the destination
@@ -230,37 +234,39 @@
             new_context['destination'] = data['destination']
         if 'source' in new_context and 'destination' in new_context:
             s = new_context['destination']
             new_context['destination'] = new_context['source']
             new_context['source'] = s
         return Message(msg_type, data, context=new_context)
 
-    def response(self, data=None, context=None):
-        """Construct a response message for the message
+    def response(self, data: dict = None, context: dict = None) -> _MsgBase:
+        """
+        Construct a response message for the message
 
         Constructs a reply with the data and appends the expected
         ".response" to the message
 
         Args:
             data (dict): message data
             context (dict): message context
         Returns
             (Message) message with the type modified to match default response
         """
         return self.reply(self.msg_type + '.response', data, context)
 
-    def publish(self, msg_type, data, context=None):
+    def publish(self, msg_type: str, data: dict,
+                context: dict = None) -> _MsgBase:
         """
         Copy the original context and add passed in context.  Delete
         any target in the new context. Return a new message object with
         passed in data and new context.  Type remains unchanged.
 
         Args:
             msg_type (str): type of message
-            data (dict): date to send with message
+            data (dict): data to send with message
             context: context added to existing context
 
         Returns:
             Message: Message object to publish
         """
         context = context or {}
         new_context = self.context.copy()
@@ -268,51 +274,51 @@
             new_context[key] = context[key]
 
         if 'target' in new_context:
             del new_context['target']
 
         return Message(msg_type, data, context=new_context)
 
+    @deprecated("This method is deprecated with no replacement", "0.1.0")
     def utterance_remainder(self):
         """
         DEPRECATED - mycroft-core hack, used by some skills in the wild
 
         For intents get the portion not consumed by Adapt.
 
         For example: if they say 'Turn on the family room light' and there are
         entity matches for "turn on" and "light", then it will leave behind
         " the family room " which is then normalized to "family room".
 
         Returns:
             str: Leftover words or None if not an utterance.
         """
-        LOG.warning("Message.utterance_remainder has been deprecated!")
         utt = normalize(self.data.get("utterance", ""))
         if utt and "__tags__" in self.data:
             for token in self.data["__tags__"]:
                 # Substitute only whole words matching the token
                 utt = re.sub(r'\b' + token.get("key", "") + r"\b", "", utt)
         return normalize(utt)
 
 
-def encrypt_as_dict(data, nonce=None):
-    ciphertext, tag, nonce = encrypt(data, nonce=nonce)
+def encrypt_as_dict(key: str, data: str, nonce=None) -> dict:
+    ciphertext, tag, nonce = encrypt(key, data, nonce=nonce)
     return {"ciphertext": hexlify(ciphertext).decode('utf-8'),
             "tag": hexlify(tag).decode('utf-8'),
             "nonce": hexlify(nonce).decode('utf-8')}
 
 
-def decrypt_from_dict(data):
+def decrypt_from_dict(key: str, data: dict) -> str:
     ciphertext = unhexlify(data["ciphertext"])
     if data.get("tag") is None:  # web crypto
         ciphertext, tag = ciphertext[:-16], ciphertext[-16:]
     else:
         tag = unhexlify(data["tag"])
     nonce = unhexlify(data["nonce"])
-    return decrypt(ciphertext, tag, nonce)
+    return decrypt(key, ciphertext, tag, nonce)
 
 
 def dig_for_message(max_records: int = 10) -> Optional[Message]:
     """
     Dig Through the stack for message. Looks at the current stack
     for a passed argument of type 'Message'.
     Args:
@@ -436,30 +442,16 @@
 
         Returns:
             str: a json string representation of the message.
         """
         data = self._json_dump(self.data)
         msg = json.dumps({'type': self.msg_type, **data})
         if self._secret_key:
-            payload = encrypt_as_dict(msg)
+            payload = encrypt_as_dict(self._secret_key, msg)
             return json.dumps(payload)
         return msg
 
     @staticmethod
     def deserialize(value):
         value = Message._json_load(value)
         msg_type = value.pop("type")
         return GUIMessage(msg_type, **value)
-
-
-if __name__ == "__main__":
-    from mycroft_bus_client.message import Message as _MycroftMessage
-
-    m1 = _MycroftMessage("")
-    m2 = Message("")
-    print(m1 == m2)
-    print(m2 == m1)
-    print(isinstance(m1, _MycroftMessage))
-    print(isinstance(m1, Message))
-    print(isinstance(m2,
-                     _MycroftMessage))  # can't fix this one without the monkey patching, its defined in the class at mycroft_bus_client
-    print(isinstance(m2, Message))
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # each corresponds to a cli util
 from ovos_bus_client import MessageBusClient, Message
 from ovos_config import Configuration
 import sys
 
 
 def ovos_speak():
-    if (args_count := len(sys.argv)) == 2:
+    args_count = len(sys.argv)
+    if args_count == 2:
         utt = sys.argv[1]
         lang = Configuration().get("lang", "en-us")
     elif args_count == 3:
         utt = sys.argv[1]
         lang = sys.argv[2]
     else:
         print("USAGE: ovos-speak {utterance} [lang]")
@@ -19,15 +20,16 @@
     client = MessageBusClient()
     client.run_in_thread()
     client.emit(Message("speak", {"utterance": utt, "lang": lang}))
     client.close()
 
 
 def ovos_say_to():
-    if (args_count := len(sys.argv)) == 2:
+    args_count = len(sys.argv)
+    if args_count == 2:
         utt = sys.argv[1]
         lang = Configuration().get("lang", "en-us")
     elif args_count == 3:
         utt = sys.argv[1]
         lang = sys.argv[2]
     else:
         print("USAGE: ovos-say-to {utterance} [lang]")
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/send_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from websocket import create_connection
 
 from ovos_config.config import Configuration
 from ovos_bus_client.client import MessageBusClient
 from ovos_bus_client.message import Message
 
 
-def send(message_to_send, data_to_send=None):
+def send(message_to_send: str, data_to_send: dict = None):
     """Send a single message over the websocket.
 
     Args:
         message_to_send (str): Message to send
         data_to_send (dict): data structure to go along with the
             message, defaults to empty dict.
     """
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/session.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,59 @@
 import enum
 import time
+import json
 from threading import Lock
 from uuid import uuid4
+from typing import Optional, List, Tuple, Union, Iterable
 
-from ovos_bus_client.message import dig_for_message
-from ovos_utils.log import LOG
+from ovos_bus_client.message import dig_for_message, Message
+from ovos_utils.log import LOG, log_deprecation
 from ovos_config.config import Configuration
 from ovos_config.locale import get_default_lang
 
 
 class UtteranceState(str, enum.Enum):
     INTENT = "intent"  # includes converse
     RESPONSE = "response"
 
 
-def _get_valid_langs():
-    return list(set([get_default_lang()] + Configuration().get("secondary_langs'", [])))
-
-
-class Session:
-    """
-    An class representing a Mycroft Session Identifier
-    """
-
-    def __init__(self, session_id=None, expiration_seconds=None, active_skills=None, history=None,
-                 max_time=5, max_messages=5, utterance_states=None, lang=None, context=None, valid_langs=None):
-        self.session_id = session_id or str(uuid4())
-        self.lang = lang or get_default_lang()
-
-        self.valid_languages = valid_langs or _get_valid_langs()
-        self.active_skills = active_skills or []  # [skill_id , timestamp]
-        self.history = history or []  # [Message , timestamp]
-        self.utterance_states = utterance_states or {}  # {skill_id: UtteranceState}
-        self.max_time = max_time  # minutes
-        self.max_messages = max_messages
-        self.touch_time = int(time.time())
-        if expiration_seconds is None:
-            expiration_seconds = Configuration().get('session', {}).get("ttl", -1)
-        self.expiration_seconds = expiration_seconds
-        self.context = context or IntentContextManager(timeout=self.touch_time + expiration_seconds)
-
-    @property
-    def active(self):
-        # NOTE: skills without converse implemented never
-        # get added here unless using get_response
-        return len(self.active_skills) > 0
-
-    def touch(self):
-        """
-        update the touch_time on the session
-
-        :return:
-        """
-        self.touch_time = int(time.time())
-
-    def expired(self):
-        """
-        determine if the session has expired
-
-        :return:
-        """
-        if self.expiration_seconds < 0:
-            return False
-        return int(time.time()) - self.touch_time > self.expiration_seconds
-
-    def __str__(self):
-        return "{%s,%d}" % (str(self.session_id), self.touch_time)
-
-    def enable_response_mode(self, skill_id):
-        self.utterance_states[skill_id] = UtteranceState.RESPONSE.value
-
-    def disable_response_mode(self, skill_id):
-        self.utterance_states[skill_id] = UtteranceState.INTENT.value
-
-    def activate_skill(self, skill_id):
-        # remove it from active list
-        self.deactivate_skill(skill_id)
-        # add skill with timestamp to start of active list
-        self.active_skills.insert(0, [skill_id, time.time()])
-
-    def deactivate_skill(self, skill_id):
-        active_ids = [s[0] for s in self.active_skills]
-        if skill_id in active_ids:
-            idx = active_ids.index(skill_id)
-            self.active_skills.pop(idx)
-
-    def is_active(self, skill_id):
-        self._prune_history()
-        active_ids = [s[0] for s in self.active_skills]
-        return skill_id in active_ids
-
-    def _prune_history(self):
-        # filter old messages from history
-        now = time.time()
-        self.history = [m for m in self.history
-                        if now - m[1] < 60 * self.max_time]
-        # keep only self.max_messages
-        if len(self.history) > self.max_messages:
-            self.history = self.history[self.max_messages * -1:]
-
-    def clear(self):
-        self.active_skills = []  # [skill_id , timestamp]
-        self.history = []  # [Message , timestamp]
-
-    def serialize(self):
-        # safe for json dumping
-        return {
-            "active_skills": self.active_skills,
-            "utterance_states": self.utterance_states,
-            "session_id": self.session_id,
-            "history": self.history,
-            "lang": self.lang,
-            "valid_languages": self.valid_languages,
-            "context": self.context.serialize()
-        }
-
-    def update_history(self, message=None):
-        message = message or dig_for_message()
-        if message:
-            m = message.as_dict
-            m["context"] = {}  # clear personal data
-            self.history.append((m, time.time()))
-        self._prune_history()
-
-    @staticmethod
-    def deserialize(data):
-        uid = data.get("session_id")
-        active = data.get("active_skills") or []
-        history = data.get("history") or []
-        max_time = data.get("max_time") or 5
-        max_messages = data.get("max_messages") or 5
-        states = data.get("utterance_states") or {}
-        lang = data.get("lang")
-        valid_langs = data.get("valid_languages") or _get_valid_langs()
-        context = IntentContextManager.deserialize(data["context"])
-        return Session(uid,
-                       active_skills=active,
-                       utterance_states=states,
-                       history=history,
-                       max_time=max_time,
-                       lang=lang,
-                       valid_langs=valid_langs,
-                       max_messages=max_messages,
-                       context=context)
-
-    @staticmethod
-    def from_message(message=None):
-        message = message or dig_for_message()
-        if message:
-            lang = message.context.get("lang") or \
-                   message.data.get("lang")
-            sid = None
-            if "session_id" in message.context:
-                sid = message.context["session_id"]
-            if "session" in message.context:
-                sess = message.context["session"]
-                if sid and "session_id" not in sess:
-                    sess["session_id"] = sid
-                if "lang" not in sess:
-                    sess["lang"] = lang
-                sess = Session.deserialize(sess)
-            elif sid:
-                sess = SessionManager.sessions.get(sid) or \
-                       Session(sid)
-                if lang:
-                    sess.lang = lang
-            else:
-                sess = Session(lang=lang)
-        else:
-            # new session
-            sess = Session()
-        return sess
-
-
-class SessionManager:
-    """ Keeps track of the current active session. """
-    default_session = None
-    __lock = Lock()
-    sessions = {}
-
-    @staticmethod
-    def reset_default_session():
-        with SessionManager.__lock:
-            sess = Session()
-            LOG.info(f"New Default Session Start: {sess.session_id}")
-            SessionManager.default_session = sess
-            SessionManager.sessions[sess.session_id] = sess
-        return SessionManager.default_session
-
-    @staticmethod
-    def update(sess: Session, make_default: bool = False):
-        """
-        Update the last_touch timestamp on the current session
-
-        :return: None
-        """
-        sess.touch()
-        SessionManager.sessions[sess.session_id] = sess
-        if make_default:
-            SessionManager.default_session = sess
-
-    @staticmethod
-    def get(message=None):
-        """
-        get the active session.
-
-        :return: An active session
-        """
-        sess = SessionManager.default_session
-        message = message or dig_for_message()
-
-        if not sess or sess.expired():
-            if sess is not None and sess.session_id in SessionManager.sessions:
-                SessionManager.sessions.pop(sess.session_id)
-            sess = SessionManager.reset_default_session()
-        if message:
-            sess = Session.from_message(message)
-            SessionManager.sessions[sess.session_id] = sess
-        return sess
-
-    @staticmethod
-    def touch(message=None):
-        """
-        Update the last_touch timestamp on the current session
-
-        :return: None
-        """
-        SessionManager.get(message).touch()
+def _get_valid_langs() -> List[str]:
+    return list(set([get_default_lang()] +
+                    Configuration().get("secondary_langs'", [])))
 
 
 class IntentContextManagerFrame:
-    """
-    Manages entities and context for a single frame of conversation.
-    Provides simple equality querying.
-    Attributes:
-        entities(list): Entities that belong to ContextManagerFrame
-        metadata(object): metadata to describe context belonging to ContextManagerFrame
-    """
-
-    def __init__(self, entities=None, metadata=None):
+    def __init__(self, entities: List[dict] = None, metadata: dict = None):
         """
-        Initialize ContextManagerFrame
-        Args:
-            entities(list): List of Entities...
-            metadata(object): metadata to describe context?
+        Manages entities and context for a single frame of conversation.
+        Provides simple equality querying.
+        Attributes:
+            entities(list): Entities that belong to ContextManagerFrame
+            metadata(object): metadata to describe context belonging to ContextManagerFrame
         """
         self.entities = entities or []
         self.metadata = metadata or {}
 
-    def serialize(self):
+    def serialize(self) -> dict:
+        """
+        Get a dict representation of this frame
+        """
         return {"entities": self.entities,
                 "metadata": self.metadata}
 
     @staticmethod
-    def deserialize(data):
+    def deserialize(data: dict):
+        """
+        Build an IntentContextManagerFrame from serialized data
+        @param data: serialized (dict) frame data
+        @return: IntentContextManagerFrame for the specified data
+        """
         return IntentContextManagerFrame(**data)
 
-    def metadata_matches(self, query=None):
+    def metadata_matches(self, query: dict = None) -> bool:
         """
         Returns key matches to metadata
         Asserts that the contents of query exist within (logical subset of)
         metadata in this frame.
         Args:
             query(dict): metadata for matching
         Returns:
@@ -273,38 +66,42 @@
         query = query or {}
         result = len(query.keys()) > 0
         for key in query.keys():
             result = result and query[key] == self.metadata.get(key)
 
         return result
 
-    def merge_context(self, tag, metadata):
+    def merge_context(self, tag: dict, metadata: dict):
         """
         merge into contextManagerFrame new entity and metadata.
         Appends tag as new entity and adds keys in metadata to keys in
         self.metadata.
         Args:
-            tag(str): entity to be added to self.entities
+            tag(dict): entity to be added to self.entities
             metadata(dict): metadata contains keys to be added to self.metadata
         """
         self.entities.append(tag)
         for k, v in metadata.items():
             if k not in self.metadata:
                 self.metadata[k] = v
 
 
 class IntentContextManager:
-    """Context Manager
+    """
+    Context Manager
 
     Use to track context throughout the course of a conversational session.
     How to manage a session's lifecycle is not captured here.
     """
 
-    def __init__(self, timeout=None, frame_stack=None,
-                 greedy=None, keywords=None, max_frames=None):
+    def __init__(self, timeout: int = None,
+                 frame_stack: List[Tuple[IntentContextManagerFrame,
+                                         float]] = None,
+                 greedy: bool = None, keywords: List[str] = None,
+                 max_frames: int = None):
 
         config = Configuration().get('context', {})
         if timeout is None:
             timeout = config.get('timeout', 2)
         if greedy is None:
             greedy = config.get('greedy', False)
         if keywords is None:
@@ -314,61 +111,70 @@
 
         self.frame_stack = frame_stack or []
         self.timeout = timeout * 60  # minutes to seconds
         self.context_keywords = keywords
         self.context_max_frames = max_frames
         self.context_greedy = greedy
 
-    def serialize(self):
+    def serialize(self) -> dict:
+        """
+        Get a dict representation of this IntentContextManager
+        """
         return {"timeout": self.timeout,
-                "frame_stack": [s.serialize() for s in self.frame_stack]}
+                "frame_stack": [(s.serialize(), t) for (s, t)
+                                in self.frame_stack]}
 
     @staticmethod
-    def deserialize(data):
-        timeout = data["timeout"]
-        framestack = [IntentContextManagerFrame.deserialize(f) for f in data["frame_stack"]]
+    def deserialize(data: dict):
+        """
+        Build an IntentContextManager from serialized data
+        @param data: serialized (dict) data
+        @return: IntentContextManager for the specified data
+        """
+        timeout = data.get("timeout", 2)
+        framestack = [(IntentContextManagerFrame.deserialize(f), t)
+                      for (f, t) in data.get("frame_stack", [])]
         return IntentContextManager(timeout, framestack)
 
-    def update_context(self, entities):
-        """Updates context with keyword from the intent.
+    def update_context(self, entities: dict):
+        """
+        Updates context with keyword from the intent.
 
         entity(dict): Format example...
                    {'data': 'Entity tag as <str>',
                     'key': 'entity proper name as <str>',
                     'confidence': <float>'
                    }
-                               
+
         Args:
             entities (list): Intent to scan for keywords
         """
         for context_entity in entities:
-            #  entity(dict): Format example...
-            #   {'data': 'Entity tag as <str>',
-            #   'key': 'entity proper name as <str>',
-            #   'confidence': <float>' }
             if self.context_greedy:
                 self.inject_context(context_entity)
             elif context_entity['data'][0][1] in self.context_keywords:
                 self.inject_context(context_entity)
 
     def clear_context(self):
         """Remove all contexts."""
         self.frame_stack = []
 
-    def remove_context(self, context_id):
+    def remove_context(self, context_id: str):
         """Remove a specific context entry.
 
         Args:
             context_id (str): context entry to remove
         """
         self.frame_stack = [(f, t) for (f, t) in self.frame_stack
                             if context_id in f.entities[0].get('data', [])]
 
-    def inject_context(self, entity, metadata=None):
+    def inject_context(self, entity: dict, metadata: dict = None):
         """
+        Add context to the first frame in the stack. If no frame metadata
+        doesn't match the passed metadata then a new one is inserted.
         Args:
             entity(dict): Format example...
                        {'data': 'Entity tag as <str>',
                         'key': 'entity proper name as <str>',
                         'confidence': <float>'
                        }
             metadata(dict): arbitrary metadata about entity injected
@@ -385,31 +191,33 @@
                 frame = IntentContextManagerFrame(entities=[entity],
                                                   metadata=metadata.copy())
                 self.frame_stack.insert(0, (frame, time.time()))
         except (IndexError, KeyError):
             pass
 
     @staticmethod
-    def _strip_result(context_features):
+    def _strip_result(context_features: Iterable):
         """Keep only the latest instance of each keyword.
 
         Arguments
             context_features (iterable): context features to check.
         """
         stripped = []
         processed = []
         for feature in context_features:
             keyword = feature['data'][0][1]
             if keyword not in processed:
                 stripped.append(feature)
                 processed.append(keyword)
         return stripped
 
-    def get_context(self, max_frames=None, missing_entities=None):
-        """ Constructs a list of entities from the context.
+    def get_context(self, max_frames: int = None,
+                    missing_entities: List[str] = None):
+        """
+        Constructs a list of entities from the context.
 
         Args:
             max_frames(int): maximum number of frames to look back
             missing_entities(list of str): a list or set of tag names,
             as strings
 
         Returns:
@@ -451,7 +259,340 @@
                     # an arbitrary number of an entity kind.
                     missing_entities.remove(entity.get('data'))
         else:
             result = context
 
         # Only use the latest  keyword
         return self._strip_result(result)
+
+
+class Session:
+    def __init__(self, session_id: str = None, expiration_seconds: int = None,
+                 active_skills: List[List[Union[str, float]]] = None,
+                 history: List[Tuple[Message, float]] = None,
+                 max_time: int = 5, max_messages: int = 5,
+                 utterance_states: dict = None, lang: str = None,
+                 context: IntentContextManager = None,
+                 valid_langs: List[str] = None):
+        """
+        Construct a session identifier
+        @param session_id: string UUID for the session
+        @param expiration_seconds: TTL for session (-1 for no expiration)
+        @param active_skills: List of list skill_id, last reference
+        @param history: List of tuple Message, timestamp
+        @param max_time: maximum time for history in minutes
+        @param max_messages: maximum number of messages to retain
+        @param utterance_states: dict of skill_id to UtteranceState
+        @param lang: language associated with this Session
+        @param context: IntentContextManager for this Session
+        @param valid_langs: list of configured valid languages
+        """
+        self.session_id = session_id or str(uuid4())
+        self.lang = lang or get_default_lang()
+
+        self.valid_languages = valid_langs or _get_valid_langs()
+        self.active_skills = active_skills or []  # [skill_id , timestamp]
+        # TODO: Can active_skills be a list of tuples like history?
+        self.history = history or []  # (Message , timestamp)
+        self.utterance_states = utterance_states or {}  # {skill_id: UtteranceState}
+        self.max_time = max_time  # minutes
+        self.max_messages = max_messages
+        self.touch_time = int(time.time())
+        if expiration_seconds is None:
+            expiration_seconds = Configuration().get('session', {}).get("ttl",
+                                                                        -1)
+        self.expiration_seconds = expiration_seconds
+        self.context = context or IntentContextManager(timeout=self.touch_time +
+                                                       expiration_seconds)
+
+    @property
+    def active(self) -> bool:
+        """
+        Return true if any skills attached to this session are active.
+        NOTE: skills without converse implemented never get added here unless
+        using get_response
+        """
+        return len(self.active_skills) > 0
+
+    def touch(self):
+        """
+        update the touch_time on the session
+        """
+        self.touch_time = int(time.time())
+
+    def expired(self) -> bool:
+        """
+        Return True if the session has expired
+        """
+        if self.expiration_seconds < 0:
+            return False
+        return int(time.time()) - self.touch_time > self.expiration_seconds
+
+    def __str__(self):
+        return "{%s,%d}" % (str(self.session_id), self.touch_time)
+
+    def enable_response_mode(self, skill_id: str):
+        """
+        Mark a skill as expecting a response
+        @param skill_id: ID of skill expecting a response
+        """
+        self.utterance_states[skill_id] = UtteranceState.RESPONSE.value
+
+    def disable_response_mode(self, skill_id: str):
+        """
+        Mark a skill as not expecting a response (handling intents normally)
+        @param skill_id: ID of skill expecting a response
+        """
+        self.utterance_states[skill_id] = UtteranceState.INTENT.value
+
+    def activate_skill(self, skill_id: str):
+        """
+        Add a skill to the front of the active_skills list
+        @param skill_id: ID of skill to activate
+        """
+        # remove it from active list
+        self.deactivate_skill(skill_id)
+        # add skill with timestamp to start of active list
+        self.active_skills.insert(0, [skill_id, time.time()])
+
+    def deactivate_skill(self, skill_id: str):
+        """
+        Remove a skill from the active_skills list
+        @param skill_id: ID of skill to deactivate
+        """
+        active_ids = [s[0] for s in self.active_skills]
+        if skill_id in active_ids:
+            idx = active_ids.index(skill_id)
+            self.active_skills.pop(idx)
+
+    def is_active(self, skill_id: str) -> bool:
+        """
+        Check if a skill is active
+        @param skill_id: ID of skill to check
+        @return: True if the requested skill is active
+        """
+        self._prune_history()  # TODO: Is this necessary or useful?
+        active_ids = [s[0] for s in self.active_skills]
+        return skill_id in active_ids
+
+    def _prune_history(self):
+        """
+        Remove messages from history that are too old or exceed max_messages
+        """
+        # filter old messages from history
+        now = time.time()
+        self.history = [m for m in self.history
+                        if now - m[1] < 60 * self.max_time]
+        # keep only self.max_messages
+        if len(self.history) > self.max_messages:
+            self.history = self.history[self.max_messages * -1:]
+
+    def clear(self):
+        """
+        Clear history and active_skills
+        """
+        self.active_skills = []
+        self.history = []
+
+    def serialize(self) -> dict:
+        """
+        Get a json-serializable dict representation of this session
+        """
+        # safe for json dumping
+        return {
+            "active_skills": self.active_skills,
+            "utterance_states": self.utterance_states,
+            "session_id": self.session_id,
+            "history": self.history,
+            "lang": self.lang,
+            "valid_languages": self.valid_languages,
+            "context": self.context.serialize()
+        }
+
+    def update_history(self, message: Message = None):
+        """
+        Add a message to history and then prune history
+        @param message: Message to append to history
+        """
+        message = message or dig_for_message()
+        if message:
+            try:
+                m = message.as_dict
+            except AttributeError:
+                log_deprecation("mycroft-bus-client has been deprecated, please"
+                                " update your imports to use ovos-bus-client",
+                                "0.0.4",
+                                excluded_package_refs=["ovos_bus_client"])
+                m = json.loads(message.serialize())
+            except Exception as e:
+                LOG.exception(e)
+                m = json.loads(message.serialize())
+            m["context"] = {}  # clear personal data
+            self.history.append((m, time.time()))
+        self._prune_history()
+
+    @staticmethod
+    def deserialize(data: dict):
+        """
+        Build a Session object from dict data
+        @param data: dict serialized Session object
+        @return: Session representation of data
+        """
+        uid = data.get("session_id")
+        active = data.get("active_skills") or []
+        history = data.get("history") or []
+        max_time = data.get("max_time") or 5
+        max_messages = data.get("max_messages") or 5
+        states = data.get("utterance_states") or {}
+        lang = data.get("lang")
+        valid_langs = data.get("valid_languages") or _get_valid_langs()
+        context = IntentContextManager.deserialize(data.get("context", {}))
+        return Session(uid,
+                       active_skills=active,
+                       utterance_states=states,
+                       history=history,
+                       max_time=max_time,
+                       lang=lang,
+                       valid_langs=valid_langs,
+                       max_messages=max_messages,
+                       context=context)
+
+    @staticmethod
+    def from_message(message: Message = None):
+        """
+        Get a Session for the given message. If no session in message context,
+        SessionManager.default_session is returned.
+        If SessionManager.default_session is None, a default session is created
+        @param message: Message to get session for
+        @return: Session object
+        """
+        message = message or dig_for_message()
+        if message:
+            lang = message.context.get("lang") or \
+                   message.data.get("lang")
+            sid = None
+            if "session_id" in message.context:
+                sid = message.context["session_id"]
+            if "session" in message.context:
+                sess = message.context["session"]
+                if sid and "session_id" not in sess:
+                    sess["session_id"] = sid
+                if "lang" not in sess:
+                    sess["lang"] = lang
+                sess = Session.deserialize(sess)
+            elif sid:
+                sess = SessionManager.sessions.get(sid) or \
+                       Session(sid)
+                if lang:
+                    sess.lang = lang
+            else:
+                sess = SessionManager.default_session
+                if not sess:
+                    LOG.debug(f"Creating default session on reference")
+                    sess = SessionManager.reset_default_session()
+                if sess and lang and sess.lang != lang:
+                    sess.lang = lang
+                    LOG.info(f"Updated default session lang to: {lang}")
+        else:
+            # new session
+            LOG.warning(f"No message found, using default session")
+            sess = SessionManager.default_session
+        if sess and sess.expired():
+            LOG.debug(f"Resolved session expired {sess.session_id}")
+            sess.touch()
+        return sess
+
+
+class SessionManager:
+    """ Keeps track of the current active session. """
+    default_session: Session = None
+    __lock = Lock()
+    sessions = {}
+
+    @staticmethod
+    def prune_sessions():
+        """
+        Discard any expired sessions
+        """
+        # TODO: Consider when to prune sessions; an event or callback scheduled
+        #   on `touch`, periodically scheduled event, or triggered on some
+        #   interaction with `SessionManager` (ideally threaded to not slow
+        #   down references)
+        SessionManager.sessions = {sid: s for sid, s in
+                                   SessionManager.sessions.items()
+                                   if not s.expired}
+
+    @staticmethod
+    def reset_default_session() -> Session:
+        """
+        Define and return a new default_session
+        """
+        with SessionManager.__lock:
+            sess = Session()
+            LOG.info(f"New Default Session Start: {sess.session_id}")
+            if not SessionManager.default_session:
+                SessionManager.default_session = sess
+            if SessionManager.default_session.session_id in \
+                    SessionManager.sessions:
+                LOG.debug(f"Removing expired default session from sessions")
+                SessionManager.sessions.pop(
+                    SessionManager.default_session.session_id)
+            SessionManager.default_session = sess
+            SessionManager.sessions[sess.session_id] = sess
+        return SessionManager.default_session
+
+    @staticmethod
+    def update(sess: Session, make_default: bool = False):
+        """
+        Update the last_touch timestamp on the current session
+        @param sess: Session to update
+        @param make_default: if true, set default_session to sess
+        """
+        if not sess:
+            raise ValueError(f"Expected Session and got None")
+        sess.touch()
+        SessionManager.sessions[sess.session_id] = sess
+        if make_default:
+            SessionManager.default_session = sess
+
+    @staticmethod
+    def get(message: Optional[Message] = None) -> Session:
+        """
+        Get the active session for a given Message
+
+        @param message: Message to get session for
+        @return: Session from message or default_session
+        """
+        sess = SessionManager.default_session
+        message = message or dig_for_message()
+
+        # A message exists, get a real session
+        if message:
+            msg_sess = Session.from_message(message)
+            if msg_sess:
+                SessionManager.sessions[msg_sess.session_id] = msg_sess
+                return msg_sess
+            else:
+                LOG.debug(f"No session from message.")
+        else:
+            LOG.debug(f"No message, use default session")
+
+        # Default session, check if it needs to be (re)-created
+        if not sess or sess.expired():
+            if sess is not None and sess.session_id in SessionManager.sessions:
+                LOG.debug(f"Removing expired default: {sess.session_id}")
+                SessionManager.sessions.pop(sess.session_id)
+            sess = SessionManager.reset_default_session()
+        else:
+            # Existing default, make sure lang is in sync with Configuration
+            sess.lang = Configuration().get('lang') or sess.lang
+
+        return sess
+
+    @staticmethod
+    def touch(message: Message = None):
+        """
+        Update the last_touch timestamp on the current session
+
+        @param message: Message to get Session for to update
+        """
+        SessionManager.get(message).touch()
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/util/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,29 +17,34 @@
 
 A scheduled message will be kept and not sent until the system clock time
 criteria is met.
 """
 
 import json
 import shutil
+
 import time
+
+from typing import Optional, Callable, Union
+from threading import Event
 from datetime import datetime, timedelta
 from os.path import isfile, join, expanduser
 from threading import Thread, Lock
 
 from ovos_config.config import Configuration
 from ovos_config.locations import get_xdg_data_save_path, get_xdg_config_save_path
-from ovos_utils.log import LOG
+from ovos_utils.log import LOG, log_deprecation, deprecated
 from ovos_utils.messagebus import FakeBus
 from ovos_utils.events import create_basic_wrapper
 from ovos_bus_client.message import Message
 
 
-def repeat_time(sched_time, repeat):
-    """Next scheduled time for repeating event. Guarantees that the
+def repeat_time(sched_time: float, repeat: float) -> float:
+    """
+    Next scheduled time for repeating event. Guarantees that the
     time is not in the past (but could skip interim events)
 
     Args:
         sched_time (float): Scheduled unix time for the event
         repeat (float):     Repeat period in seconds
 
     Returns: (float) time for next event
@@ -48,31 +53,33 @@
     while next_time < time.time():
         # Schedule at an offset to assure no doubles
         next_time = time.time() + abs(repeat)
     return next_time
 
 
 class EventScheduler(Thread):
-    """Create an event scheduler thread. Will send messages at a
-     predetermined time to the registered targets.
+    """
+    Create an event scheduler thread. Will send messages at a
+    predetermined time to the registered targets.
 
     Arguments:
-        bus:            Mycroft messagebus (mycroft.messagebus)
-        schedule_file:  Path to file used to store pending events to on
-                        shutdown.
+        bus:            Mycroft messagebus client
+        schedule_file:  filename used to store pending events to on
+                        shutdown. File is created in XDG_DATA_HOME
+        autostart: if True, start scheduler on init
     """
 
-    def __init__(self, bus, schedule_file='schedule.json', autostart=True):
+    def __init__(self, bus,
+                 schedule_file: str = 'schedule.json', autostart: bool = True):
         super().__init__()
 
         self.events = {}
         self.event_lock = Lock()
 
         self.bus = bus
-        self.is_running = True
 
         core_conf = Configuration()
         data_dir = core_conf.get('data_dir') or get_xdg_data_save_path()
         old_schedule_path = join(expanduser(data_dir), schedule_file)
 
         self.schedule_file = join(get_xdg_config_save_path(), schedule_file)
         if isfile(old_schedule_path):
@@ -88,16 +95,34 @@
         self.bus.on('mycroft.scheduler.update_event',
                     self.update_event_handler)
         self.bus.on('mycroft.scheduler.get_event',
                     self.get_event_handler)
         if autostart:
             self.start()
 
+        self._stopping = Event()
+
+    @property
+    def is_running(self) -> bool:
+        """
+        Return True while scheduler is running
+        """
+        return not self._stopping.is_set()
+
+    @is_running.setter
+    def is_running(self, value: bool):
+        if value is True:
+            self._stopping.clear()
+        elif value is False:
+            self._stopping.set()
+
     def load(self):
-        """Load json data with active events from json file."""
+        """
+        Load json data with active events from json file.
+        """
         if isfile(self.schedule_file):
             json_data = {}
             with open(self.schedule_file) as schedule_file:
                 try:
                     json_data = json.load(schedule_file)
                 except Exception as exc:
                     LOG.error(exc)
@@ -106,77 +131,87 @@
                 for key in json_data:
                     event_list = json_data[key]
                     # discard non repeating events that has already happened
                     self.events[key] = [tuple(evt) for evt in event_list
                                         if evt[0] > current_time or evt[1]]
 
     def run(self):
-        while self.is_running:
+        """
+        Check events periodically until stopped
+        """
+        while not self._stopping.wait(0.5):
             self.check_state()
-            time.sleep(0.5)
+        LOG.info(f"Stopped")
 
     def check_state(self):
-        """Check if an event should be triggered."""
+        """
+        Check if any event should be triggered.
+        """
         with self.event_lock:
             # Check all events
             pending_messages = []
             for event in self.events:
                 current_time = time.time()
                 e = self.events[event]
                 # Get scheduled times that has passed
-                passed = [(t, r, d, c) for
-                          (t, r, d, c) in e if t <= current_time]
+                passed = ((t, r, d, c) for
+                          (t, r, d, c) in e if t <= current_time)
                 # and remaining times that we're still waiting for
                 remaining = [(t, r, d, c) for
                              t, r, d, c in e if t > current_time]
                 # Trigger registered methods
                 for sched_time, repeat, data, context in passed:
                     pending_messages.append(Message(event, data, context))
                     # if this is a repeated event add a new trigger time
                     if repeat:
                         next_time = repeat_time(sched_time, repeat)
                         remaining.append((next_time, repeat, data, context))
                 # update list of events
                 self.events[event] = remaining
 
-        # Remove events have are now completed
+        # Remove events that are now completed
         self.clear_empty()
 
         # Finally, emit the queued up events that triggered
         for msg in pending_messages:
             self.bus.emit(msg)
 
-    def schedule_event(self, event, sched_time, repeat=None,
-                       data=None, context=None):
-        """Add event to pending event schedule.
+    def schedule_event(self, event: str, sched_time: float,
+                       repeat: Optional[float] = None,
+                       data: Optional[dict] = None,
+                       context: Optional[dict] = None):
+        """
+        Add event to pending event schedule.
 
         Arguments:
             event (str): Handler for the event
-            sched_time ([type]): [description]
+            sched_time (float): epoch time of event
             repeat ([type], optional): Defaults to None. [description]
             data ([type], optional): Defaults to None. [description]
             context (dict, optional): context (dict, optional): message
                                       context to send when the
                                       handler is called
         """
         data = data or {}
         with self.event_lock:
             # get current list of scheduled times for event, [] if missing
             event_list = self.events.get(event, [])
 
             # Don't schedule if the event is repeating and already scheduled
             if repeat and event in self.events:
-                LOG.debug(f'Repeating event {event} is already scheduled, discarding')
+                LOG.debug(f'Repeating event {event} is already scheduled, '
+                          f'discarding')
             else:
                 # add received event and time
                 event_list.append((sched_time, repeat, data, context))
                 self.events[event] = event_list
 
-    def schedule_event_handler(self, message):
-        """Messagebus interface to the schedule_event method.
+    def schedule_event_handler(self, message: Message):
+        """
+        Messagebus interface to the schedule_event method.
         Required data in the message envelope is
             event: event to emit
             time:  time to emit the event
 
         Optional data is
             repeat: repeat interval
             data:   data to send along with the event
@@ -189,115 +224,132 @@
         if event and sched_time:
             self.schedule_event(event, sched_time, repeat, data, context)
         elif not event:
             LOG.error('Scheduled event name not provided')
         else:
             LOG.error('Scheduled event time not provided')
 
-    def remove_event(self, event):
-        """Remove an event from the list of scheduled events.
+    def remove_event(self, event: str):
+        """
+        Remove an event from the list of scheduled events.
 
         Arguments:
             event (str): event identifier
         """
         with self.event_lock:
             if event in self.events:
                 self.events.pop(event)
 
-    def remove_event_handler(self, message):
-        """Messagebus interface to the remove_event method."""
+    def remove_event_handler(self, message: Message):
+        """
+        Messagebus interface to the remove_event method.
+        """
         event = message.data.get('event')
         self.remove_event(event)
 
-    def update_event(self, event, data):
-        """Change an existing events data.
+    def update_event(self, event: str, data: dict):
+        """
+        Change an existing event's data.
 
         This will only update the first call if multiple calls are registered
         to the same event identifier.
 
         Arguments:
             event (str): event identifier
             data (dict): new data
         """
         with self.event_lock:
             # if there is an active event with this name
             if len(self.events.get(event, [])) > 0:
-                time, repeat, _, context = self.events[event][0]
-                self.events[event][0] = (time, repeat, data, context)
+                event_time, repeat, _, context = self.events[event][0]
+                self.events[event][0] = (event_time, repeat, data, context)
 
-    def update_event_handler(self, message):
-        """Messagebus interface to the update_event method."""
+    def update_event_handler(self, message: Message):
+        """
+        Messagebus interface to the update_event method.
+        """
         event = message.data.get('event')
         data = message.data.get('data')
         self.update_event(event, data)
 
-    def get_event_handler(self, message):
-        """Messagebus interface to get_event.
+    def get_event_handler(self, message: Message):
+        """
+        Messagebus interface to get_event.
 
         Emits another event sending event status.
         """
         event_name = message.data.get("name")
         event = None
         with self.event_lock:
             if event_name in self.events:
                 event = self.events[event_name]
         emitter_name = f'mycroft.event_status.callback.{event_name}'
         self.bus.emit(message.reply(emitter_name, data=event))
 
     def store(self):
-        """Write current schedule to disk."""
+        """
+        Write current schedule to disk.
+        """
         with self.event_lock:
             with open(self.schedule_file, 'w') as schedule_file:
                 json.dump(self.events, schedule_file)
 
     def clear_repeating(self):
-        """Remove repeating events from events dict."""
+        """
+        Remove repeating events from events dict.
+        """
         with self.event_lock:
             for evt in self.events:
                 self.events[evt] = [tup for tup in self.events[evt]
                                     if tup[1] is None]
 
     def clear_empty(self):
-        """Remove empty event entries from events dict."""
+        """
+        Remove empty event entries from events dict.
+        """
         with self.event_lock:
             self.events = {k: self.events[k] for k in self.events
                            if self.events[k] != []}
 
     def shutdown(self):
-        """Stop the running thread."""
-        self.is_running = False
+        """
+        Stop the running thread.
+        """
+        self._stopping.set()
         # Remove listeners
         self.bus.remove_all_listeners('mycroft.scheduler.schedule_event')
         self.bus.remove_all_listeners('mycroft.scheduler.remove_event')
         self.bus.remove_all_listeners('mycroft.scheduler.update_event')
         # Wait for thread to finish
         self.join()
         # Prune event list in preparation for saving
         self.clear_repeating()
         self.clear_empty()
         # Store all pending scheduled events
         self.store()
 
 
 class EventContainer:
-    """Container tracking messagbus handlers.
+    """
+    Container tracking messagbus handlers.
 
     This container tracks events added by a skill, allowing unregistering
     all events on shutdown.
     """
 
     def __init__(self, bus=None):
         self.bus = bus or FakeBus()
         self.events = []
 
     def set_bus(self, bus):
         self.bus = bus
 
-    def add(self, name, handler, once=False):
-        """Create event handler for executing intent or other event.
+    def add(self, name: str, handler: Callable, once: bool = False):
+        """
+        Create event handler for executing intent or other event.
 
         Arguments:
             name (string): IntentParser name
             handler (func): Method to call
             once (bool, optional): Event handler will be removed after it has
                                    been run once.
         """
@@ -314,16 +366,17 @@
                 self.events.append((name, once_wrapper))
             else:
                 self.bus.on(name, handler)
                 self.events.append((name, handler))
 
             LOG.debug('Added event: {}'.format(name))
 
-    def remove(self, name):
-        """Removes an event from bus emitter and events list.
+    def remove(self, name: str):
+        """
+        Removes an event from bus emitter and events list.
 
         Args:
             name (string): Name of Intent or Scheduler Event
         Returns:
             bool: True if found and removed, False if not found
         """
         LOG.debug("Removing event {}".format(name))
@@ -348,69 +401,79 @@
             self.bus.remove_all_listeners(name)
         return removed
 
     def __iter__(self):
         return iter(self.events)
 
     def clear(self):
-        """Unregister all registered handlers and clear the list of registered
+        """
+        Unregister all registered handlers and clear the list of registered
         events.
         """
         for e, f in self.events:
             self.bus.remove(e, f)
         self.events = []  # Remove reference to wrappers
 
 
 class EventSchedulerInterface:
-    """Interface for accessing the event scheduler over the message bus."""
+    """
+    Interface for accessing the event scheduler over the message bus.
+    """
 
     def __init__(self, name=None, sched_id=None, bus=None, skill_id=None):
         # NOTE: can not rename or move sched_id/name arguments to keep api compatibility
         if name:
-            LOG.warning("name argument has been deprecated! use skill_id instead")
+            log_deprecation("name argument has been deprecated! "
+                            "use skill_id instead", "0.1.0")
         if sched_id:
-            LOG.warning("sched_id argument has been deprecated! use skill_id instead")
+            log_deprecation("sched_id argument has been deprecated! "
+                            "use skill_id instead", "0.1.0")
 
         self.skill_id = skill_id or sched_id or name or self.__class__.__name__
         self.bus = bus
         self.events = EventContainer(bus)
         self.scheduled_repeats = []
 
     def set_bus(self, bus):
-        """Attach the messagebus of the parent skill
+        """
+        Attach the messagebus of the parent skill
 
         Args:
             bus (MessageBusClient): websocket connection to the messagebus
         """
         self.bus = bus
         self.events.set_bus(bus)
 
-    def set_id(self, sched_id):
-        """Attach the skill_id of the parent skill
+    def set_id(self, sched_id: str):
+        """
+        Attach the skill_id of the parent skill
 
         Args:
             sched_id (str): skill_id of the parent skill
         """
         # NOTE: can not rename sched_id kwarg to keep api compatibility
         self.skill_id = sched_id
 
-    def _create_unique_name(self, name):
-        """Return a name unique to this skill using the format
+    def _create_unique_name(self, name: str) -> str:
+        """
+        Return a name unique to this skill using the format
         [skill_id]:[name].
 
         Args:
             name:   Name to use internally
 
         Returns:
             str: name unique to this skill
         """
         return self.skill_id + ':' + (name or '')
 
-    def _schedule_event(self, handler, when, data, name,
-                        repeat_interval=None, context=None):
+    def _schedule_event(self, handler: Callable, when: datetime,
+                        data: dict, name: str,
+                        repeat_interval: Optional[float] = None,
+                        context: Optional[dict] = None):
         """Underlying method for schedule_event and schedule_repeating_event.
 
         Takes scheduling information and sends it off on the message bus.
 
         Args:
             handler:                method to be called
             when (datetime):        time (in system timezone) for first
@@ -430,30 +493,35 @@
         unique_name = self._create_unique_name(name)
         if repeat_interval:
             self.scheduled_repeats.append(name)  # store "friendly name"
 
         data = data or {}
 
         def on_error(e):
-            LOG.exception(f'An error occurred executing the scheduled event {e}')
+            LOG.exception(f'An error occurred executing the scheduled event: '
+                          f'{e}')
 
         wrapped = create_basic_wrapper(handler, on_error)
         self.events.add(unique_name, wrapped, once=not repeat_interval)
-        event_data = {'time': time.mktime(when.timetuple()),
+        event_data = {'time': when.timestamp(),  # Epoch timestamp
                       'event': unique_name,
                       'repeat': repeat_interval,
                       'data': data}
         context = context or {}
         context["skill_id"] = self.skill_id
         self.bus.emit(Message('mycroft.scheduler.schedule_event',
                               data=event_data, context=context))
 
-    def schedule_event(self, handler, when, data=None, name=None,
-                       context=None):
-        """Schedule a single-shot event.
+    def schedule_event(self, handler: Callable,
+                       when: datetime,
+                       data: Optional[dict] = None,
+                       name: Optional[str] = None,
+                       context: Optional[dict] = None):
+        """
+        Schedule a single-shot event.
 
         Args:
             handler:               method to be called
             when (datetime/int/float):   datetime (in system timezone) or
                                    number of seconds in the future when the
                                    handler should be called
             data (dict, optional): data to send when the handler is called
@@ -462,17 +530,22 @@
                                    previously scheduled event of the same
                                    name.
             context (dict, optional): message context to send
                                       when the handler is called
         """
         self._schedule_event(handler, when, data, name, context=context)
 
-    def schedule_repeating_event(self, handler, when, interval,
-                                 data=None, name=None, context=None):
-        """Schedule a repeating event.
+    def schedule_repeating_event(self, handler: Callable,
+                                 when: Optional[datetime],
+                                 interval: Union[float, int],
+                                 data: Optional[dict] = None,
+                                 name: Optional[str] = None,
+                                 context: Optional[dict] = None):
+        """
+        Schedule a repeating event.
 
         Args:
             handler:                method to be called
             when (datetime):        time (in system timezone) for first
                                     calling the handler, or None to
                                     initially trigger <frequency> seconds
                                     from now
@@ -490,46 +563,49 @@
                 when = datetime.now() + timedelta(seconds=interval)
             self._schedule_event(handler, when, data, name, interval,
                                  context=context)
         else:
             LOG.debug('The event is already scheduled, cancel previous '
                       'event if this scheduling should replace the last.')
 
-    def update_scheduled_event(self, name, data=None):
-        """Change data of event.
+    def update_scheduled_event(self, name: str, data: Optional[dict] = None):
+        """
+        Change data of event.
 
         Args:
             name (str): reference name of event (from original scheduling)
+            data (dict): new data to update event with
         """
         data = data or {}
         data = {
             'event': self._create_unique_name(name),
             'data': data
         }
         self.bus.emit(Message('mycroft.schedule.update_event',
                               data=data, context={"skill_id": self.skill_id}))
 
-    def cancel_scheduled_event(self, name):
-        """Cancel a pending event. The event will no longer be scheduled
-        to be executed
+    def cancel_scheduled_event(self, name: str):
+        """
+        Cancel a pending event. The event will no longer be scheduled.
 
         Args:
             name (str): reference name of event (from original scheduling)
         """
         unique_name = self._create_unique_name(name)
         data = {'event': unique_name}
         if name in self.scheduled_repeats:
             self.scheduled_repeats.remove(name)
         if self.events.remove(unique_name):
             self.bus.emit(Message('mycroft.scheduler.remove_event',
                                   data=data,
                                   context={"skill_id": self.skill_id}))
 
-    def get_scheduled_event_status(self, name):
-        """Get scheduled event data and return the amount of time left
+    def get_scheduled_event_status(self, name: str) -> int:
+        """
+        Get scheduled event data and return the amount of time left
 
         Args:
             name (str): reference name of event (from original scheduling)
 
         Returns:
             int: the time left in seconds
 
@@ -550,50 +626,58 @@
             time_left_in_seconds = event_time - current_time
             LOG.info(time_left_in_seconds)
             return time_left_in_seconds
         else:
             raise Exception("Event Status Messagebus Timeout")
 
     def cancel_all_repeating_events(self):
-        """Cancel any repeating events started by the skill."""
+        """
+        Cancel any repeating events started by the skill.
+        """
         # NOTE: Gotta make a copy of the list due to the removes that happen
         #       in cancel_scheduled_event().
         for e in list(self.scheduled_repeats):
             self.cancel_scheduled_event(e)
 
     def shutdown(self):
-        """Shutdown the interface unregistering any event handlers."""
+        """
+        Shutdown the interface unregistering any event handlers.
+        """
         self.cancel_all_repeating_events()
         self.events.clear()
 
     @property
+    @deprecated("self.sched_id has been deprecated! use self.skill_id instead",
+                "0.1.0")
     def sched_id(self):
         """DEPRECATED: do not use, method only for api backwards compatibility
         Logs a warning and returns self.skill_id
         """
-        LOG.warning("self.sched_id has been deprecated! use self.skill_id instead")
         return self.skill_id
 
     @sched_id.setter
+    @deprecated("self.sched_id has been deprecated! use self.skill_id instead",
+                "0.1.0")
     def sched_id(self, skill_id):
         """DEPRECATED: do not use, method only for api backwards compatibility
         Logs a warning and sets self.skill_id
         """
-        LOG.warning("self.sched_id has been deprecated! use self.skill_id instead")
         self.skill_id = skill_id
 
     @property
+    @deprecated("self.name has been deprecated! use self.skill_id instead",
+                "0.1.0")
     def name(self):
         """DEPRECATED: do not use, method only for api backwards compatibility
         Logs a warning and returns self.skill_id
         """
-        LOG.warning("self.name has been deprecated! use self.skill_id instead")
         return self.skill_id
 
     @name.setter
+    @deprecated("self.name has been deprecated! use self.skill_id instead",
+                "0.1.0")
     def name(self, skill_id):
         """DEPRECATED: do not use, method only for api backwards compatibility
         Logs a warning and sets self.skill_id
         """
-        LOG.warning("self.name has been deprecated! use self.skill_id instead")
         self.skill_id = skill_id
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.5a1/ovos_bus_client/util/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,37 +11,45 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
 Small utils and tools to use with the Messagebus.
 """
-import json
+
 import logging
+from typing import Callable, Optional, Union
+from ovos_bus_client.message import Message
+from ovos_utils.log import deprecated
 
 
-def create_echo_function(name):
-    """Standard logging mechanism for Mycroft processes.
+@deprecated("No direct replacement", "0.1.0")
+def create_echo_function(name: Optional[str]) -> \
+        Callable[[Union[Message, str]], None]:
+    """
+    Standard logging mechanism for Mycroft processes.
 
-    This creats
     Arguments:
         name (str): Reference name of the process
 
     Returns:
         func: The echo function
     """
+    # TODO: Deprecate in 0.1.0
     log = logging.getLogger(name)
 
-    def echo(message):
+    def echo(message: Union[Message, str]):
         try:
-            msg = json.loads(message)
-            msg_type = msg.get("type", "")
+            if isinstance(message, str):
+                msg = Message.deserialize(message)
+            else:
+                msg = message
             # do not log tokens from registration messages
-            if msg_type == "registration":
-                msg["data"]["token"] = None
-                message = json.dumps(msg)
+            if msg.msg_type == "registration":
+                msg.data["token"] = None
+                message = msg.serialize()
         except Exception as exc:
-            log.info("Error: %s", repr(exc), exc_info=True)
+            log.info(f"Error: {exc}", exc_info=True)
 
         # Listen for messages and echo them for logging
-        log.info("BUS: %s", repr(message))
+        log.info(f"BUS: {message}")
     return echo
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a9
+Version: 0.0.5a1
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a9/setup.py` & `ovos-bus-client-0.0.5a1/setup.py`

 * *Files identical despite different names*

