# Comparing `tmp/serial_packets-0.1.2.tar.gz` & `tmp/serial_packets-0.1.3.tar.gz`

## Comparing `serial_packets-0.1.2.tar` & `serial_packets-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/__init__.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_interval_tracker.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/client.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.2/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.2/LICENSE
--rw-r--r--   0        0        0    16077 2020-02-02 00:00:00.000000 serial_packets-0.1.2/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 serial_packets-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_interval_tracker.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17965 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.3/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.3/LICENSE
+-rw-r--r--   0        0        0    16077 2020-02-02 00:00:00.000000 serial_packets-0.1.3/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 serial_packets-0.1.3/PKG-INFO
```

### Comparing `serial_packets-0.1.2/src/serial_packets/_interval_tracker.py` & `serial_packets-0.1.3/src/serial_packets/_interval_tracker.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.2/src/serial_packets/_packet_decoder.py` & `serial_packets-0.1.3/src/serial_packets/_packet_decoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.2/src/serial_packets/_packet_encoder.py` & `serial_packets-0.1.3/src/serial_packets/_packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.2/src/serial_packets/_packets.py` & `serial_packets-0.1.3/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.2/src/serial_packets/client.py` & `serial_packets-0.1.3/src/serial_packets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         # NOTE: Deleting dict elements inside a dict iteration is not allowed.
         # Using a workaround instead.
         keys = list(self.__tx_cmd_contexts.keys())
         for cmd_id in keys:
             tx_context = self.__tx_cmd_contexts.get(cmd_id)
             if tx_context.is_expired():
                 logger.error("Command [%d] timeout", cmd_id)
-                tx_context.set_command_result(0xff, PacketData())
+                tx_context.set_command_result(PacketStatus.TIMEOUT.value, PacketData())
                 self.__tx_cmd_contexts.pop(cmd_id)
 
     async def __worker_task_loop(self, task_name):
         """Body of the worker tasks to serve incoming packets."""
         # task_name = asyncio.current_task().get_name()
         # print(f"RX task '{task_name}' started", flush=True)
         # logger.debug("RX worker task [%s] started", task_name)
```

### Comparing `serial_packets-0.1.2/src/serial_packets/packets.py` & `serial_packets-0.1.3/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.2/LICENSE` & `serial_packets-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.2/README.md` & `serial_packets-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.2/pyproject.toml` & `serial_packets-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.2/PKG-INFO` & `serial_packets-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

