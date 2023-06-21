# Comparing `tmp/microservicebus-py-0.9.5.tar.gz` & `tmp/microservicebus-py-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-0.9.5.tar", last modified: Fri Jun  9 06:45:29 2023, max compression
+gzip compressed data, was "microservicebus-py-0.9.7.tar", last modified: Wed Jun 21 15:55:54 2023, max compression
```

## Comparing `microservicebus-py-0.9.5.tar` & `microservicebus-py-0.9.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-09 06:45:29.326264 microservicebus-py-0.9.5/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-09 06:45:29.317804 microservicebus-py-0.9.5/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.5/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-09 06:45:28.646693 microservicebus-py-0.9.5/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-09 06:45:29.329259 microservicebus-py-0.9.5/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.5/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-09 06:45:29.260140 microservicebus-py-0.9.5/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.5/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.5/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1609 2023-06-08 22:01:37.000000 microservicebus-py-0.9.5/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    30523 2023-06-07 20:46:51.000000 microservicebus-py-0.9.5/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6541 2023-06-09 06:40:37.000000 microservicebus-py-0.9.5/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.5/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.5/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.5/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.5/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.5/src/test.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.5/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.5/src/vpn_helper.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-21 15:55:54.766540 microservicebus-py-0.9.7/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-21 15:55:54.755114 microservicebus-py-0.9.7/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.7/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-21 15:55:53.724276 microservicebus-py-0.9.7/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-21 15:55:53.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-21 15:55:54.771607 microservicebus-py-0.9.7/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.7/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-21 15:55:54.645519 microservicebus-py-0.9.7/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.7/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.7/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1609 2023-06-08 22:01:37.000000 microservicebus-py-0.9.7/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    31975 2023-06-21 15:52:13.000000 microservicebus-py-0.9.7/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6541 2023-06-09 06:40:37.000000 microservicebus-py-0.9.7/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.7/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.7/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.7/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.7/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.7/src/test.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.7/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.7/src/vpn_helper.py
```

### Comparing `microservicebus-py-0.9.5/PKG-INFO` & `microservicebus-py-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.5
+Version: 0.9.7
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.5/README.md` & `microservicebus-py-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-0.9.7/microservicebus_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.5
+Version: 0.9.7
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.5/setup.py` & `microservicebus-py-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/axians.py` & `microservicebus-py-0.9.7/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/base_service.py` & `microservicebus-py-0.9.7/src/base_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/logger_service.py` & `microservicebus-py-0.9.7/src/logger_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/msb_handler.py` & `microservicebus-py-0.9.7/src/msb_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 class microServiceBusHandler(BaseService):
     # region Constructor
     def __init__(self, id, queue):
         self.ready = False
         self._connected = False
         self._reconnect = False
+        self.signed_in = False
         self._missedheartbeat = 0
 
         self.base_uri = os.getenv('MSB_HOST') if os.getenv('MSB_HOST') != None else "https://microservicebus.com"
                 
         home = str(Path.home())
         self.msb_dir = f"{os.environ['HOME']}/msb-py"
         
@@ -83,15 +84,15 @@
         if "nodeName" in self.settings and self._connected == True:
             self.connection.send("logMessage", [ self.settings["nodeName"], message.message[0], self.settings["organizationId"]])
 
     # endregion
     # region Private methods
     def debug_sync(self, message):
         self.printf(message)
-        #asyncio.run(self.Debug(message))
+        ##asyncio.run(self.Debug(message))
 
     def get_settings(self):
         settings = {
             "hubUri": self.base_uri
         }
         # Check if directory exists
         if os.path.isdir(self.msb_dir) == False:
@@ -253,21 +254,21 @@
         self.connection.on_reconnect(lambda: self.debug_sync(f"Reconnected to {self.base_uri}"))
 
         # mSB.com listeners
         self.connection.on("nodeCreated", lambda sign_in_info: self.sign_in_sync(sign_in_info[0], True))
         self.connection.on("signInMessage", lambda sign_in_response: self.successful_sign_in(sign_in_response[0]))
         self.connection.on("updatedToken", lambda args: self.update_token(args[0]))
         self.connection.on("ping", lambda conn_id: self.ping_response(conn_id[0]))
-        self.connection.on("errorMessage", lambda arg: self.debug_sync(arg[0]))
+        self.connection.on("errorMessage", lambda arg: self.handle_error(arg))
         self.connection.on("restart", lambda args: self.restart())
         self.connection.on("reboot", lambda args: self.reboot())
         self.connection.on("reset", lambda args: self.reset(args[0]))
         self.connection.on("changeState", lambda args: self.change_state(args[0]))
         self.connection.on("changeDebug", lambda args: self.change_debug(args[0]))
-        self.connection.on("heartBeat", lambda messageList: self.printf("Heartbeat received: " + " ".join(messageList)))
+        self.connection.on("heartBeat", lambda args: self.receive_heartbeat(args[0]))
         self.connection.on("reportState", lambda id: self.report_state(id[0]))
         self.connection.on("updateFirmware", lambda firmware_response: self.update_firmware(
             firmware_response[0], firmware_response[1]))
         self.connection.on("setBootPartition", lambda boot_info: self.set_boot_partition(
             boot_info[0], boot_info[1]))
         self.connection.on("getVpnSettingsResponse", lambda vpn_response: self.get_vpn_settings_response(
             vpn_response[0], vpn_response[1], vpn_response[2]))
@@ -341,16 +342,23 @@
         self.connection.on(
             "downloadFile", lambda response: self.not_implemented("downloadFile"))
         self.connection.on(
             "uploadFile", lambda response: self.not_implemented("uploadFile"))
         # endregion
 
         self.connection.start()
-        time.sleep(1)
-        self.set_interval(self.sendHeartbeat, 60 * 3)
+        time.sleep(2)
+        print(self.settings)
+
+        if "policies" not in self.settings:
+            self.settings["policies"] = { "disconnectPolicy": { "heartbeatTimeout": 30, "missedHearbeatLimit": 3}}
+
+        heartbeatTimeout = self.settings["policies"]["disconnectPolicy"]["heartbeatTimeout"]
+        self.set_interval(self.send_heartbeat, heartbeatTimeout)
+        await self.Debug(f"Start hearbeat at {heartbeatTimeout} seconds interval")
     # endregion
     # region SignalR callback functions
     def successful_sign_in(self, sign_in_response):
         try:
             node_name = sign_in_response["nodeName"]
             tag_list = sign_in_response["tags"]
 
@@ -417,15 +425,16 @@
                                 print(f"Unable to load {module_name}service: Error: {loadEx}")
 
                         except Exception as ex:
                             print("Unable to start service")
 
             settings = self.get_settings()
             self.connection.send("signedIn", [ settings["nodeName"], socket.gethostname(), "Online", settings["organizationId"], False])
-            self.sendHeartbeat()
+            self.send_heartbeat()
+            self.signed_in = True
             asyncio.run(self.Debug(f"Node {node_name} signed in successfully"))
             
         except Exception as ex:
             asyncio.run(self.Debug(f"sign_in_response error: {ex}"))
             asyncio.run(self.Debug(f"sign_in_response: {sign_in_response}"))
 
     def update_token(self, token):
@@ -447,28 +456,48 @@
         except Exception as e:
             asyncio.run(self.Debug(f"Error in ping_response: {e}"))
     
     def connected(self):
         self.debug_sync("Connection opened and handshake received ready to send messages")
         self._connected = True
 
-        if(self._reconnect is True):
+        if(self._reconnect is True and "id" in self.settings):
             id = self.settings["id"]
-            # self.debug_sync(f"Waiting to reconnect")
-            # time.sleep(10)
             self.debug_sync(f"Reconnecting: {id}")
             self.connection.send("reconnected", [self.settings["id"]])
 
     def disconnected(self):
         self.debug_sync("Connection closed")
         self._connected = False
         self._reconnect = True
 
-    def sendHeartbeat(self):
+    def send_heartbeat(self):
+        if self._missedheartbeat > 1:
+            asyncio.run(self.Debug(f"MISSING HEARTBEAT"))
+            missedHearbeatLimit = self.settings["policies"]["disconnectPolicy"]["missedHearbeatLimit"]
+            if self._missedheartbeat >= missedHearbeatLimit or self.signed_in == False:
+                asyncio.run(self.Debug(f"\033[93m{self._missedheartbeat} missing heartbeats exceeding limit ({missedHearbeatLimit}). Restarting process\033[0m"))
+                self.restart()
+        
+        #asyncio.run(self.Debug(f"Send heatbeat"))        
+        self._missedheartbeat += 1
         self.connection.send("heartBeat", ["echo"])
+    
+    def receive_heartbeat(self, message):
+        self._missedheartbeat = 0
+        #asyncio.run(self.Debug(f"Received heatbeat"))
+
+    def handle_error(self, message):
+        asyncio.run(self.ThrowError(f"HUB ERROR: {message[0]}"))
+        if len(message) > 1 and message[1] == 9: #Secret is not valid
+            settings = {
+                "hubUri": self.base_uri
+            }
+            self.save_settings(settings)
+            os.execv(sys.executable, ['python'] + sys.argv)
 
     def report_state(self, id):
         node_name = self.settings["nodeName"]
         self.printf(f'Fetching environment state from {node_name}')
         self.connection.send(
             'notify', [id, f'Fetching environment state from {node_name}', 'INFO'])
```

### Comparing `microservicebus-py-0.9.5/src/orchestrator_service.py` & `microservicebus-py-0.9.7/src/orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/rauc_handler.py` & `microservicebus-py-0.9.7/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/start.py` & `microservicebus-py-0.9.7/src/start.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/terminal_service.py` & `microservicebus-py-0.9.7/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/test.py` & `microservicebus-py-0.9.7/src/test.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/utils.py` & `microservicebus-py-0.9.7/src/utils.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.5/src/vpn_helper.py` & `microservicebus-py-0.9.7/src/vpn_helper.py`

 * *Files identical despite different names*

