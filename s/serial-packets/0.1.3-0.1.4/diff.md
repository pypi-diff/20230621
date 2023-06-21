# Comparing `tmp/serial_packets-0.1.3.tar.gz` & `tmp/serial_packets-0.1.4.tar.gz`

## Comparing `serial_packets-0.1.3.tar` & `serial_packets-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/__init__.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_interval_tracker.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17965 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/client.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.3/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.3/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.3/LICENSE
--rw-r--r--   0        0        0    16077 2020-02-02 00:00:00.000000 serial_packets-0.1.3/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 serial_packets-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.4/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.4/LICENSE
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.4/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.4/PKG-INFO
```

### Comparing `serial_packets-0.1.3/src/serial_packets/_packet_decoder.py` & `serial_packets-0.1.4/src/serial_packets/_packet_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import asyncio
 from PyCRC.CRCCCITT import CRCCCITT
 from typing import Optional, Callable
 
-from ._packets import PacketType, PACKET_FLAG, PACKET_ESC, MIN_PACKET_LEN, MAX_PACKET_LEN
+from ._packets import PacketType, PACKET_START_FLAG, PACKET_END_FLAG, PACKET_ESC, MIN_PACKET_LEN, MAX_PACKET_LEN
 from .packets import PacketData, MAX_DATA_LEN
 # from .packets import  PACKET_MAX_LEN
 
 logger = logging.getLogger(__name__)
 
 
 class DecodedCommandPacket:
@@ -54,89 +54,95 @@
         self.__in_packet = False
         self.__pending_escape = False
         self.__decoded_packet_callback = decoded_packet_callback
 
     def __str__(self):
         return f"In_packet ={self.__in_packet}, pending_escape={self.__pending_escape}, len={len(self.__packet_bytes)}"
 
-    def __reset_packet(self):
-        # self.__state = state
-        self.__in_packet = False
+    def __reset_packet(self, in_packet: bool):
+        self.__in_packet = in_packet
         self.__pending_escape = False
         self.__packet_bfr.clear()
 
     # async def get_next_packet(self):
     #     """Blocking asyncio fetch of next pending packet."""
     #     return await self.__packets_queue.get()
 
     def receive(self, data: bytes):
         for b in data:
             self.__receive_byte(b)
 
     def __receive_byte(self, b: int):
         # If not already in a packet, wait for next flag.
         if not self.__in_packet:
-            if b == PACKET_FLAG:
+            if b == PACKET_START_FLAG:
                 # Start collecting a packet.
-                self.__in_packet = True
-                self.__pending_escape = False
-                self.__packet_bfr.clear()
+                self.__reset_packet(True)
+            else:
+                # Here we drop bytes until next packet start. Should not
+                # happen in normal operation.
+                logger.error(f"Dropping byte {b:02x}")
+                pass
             return
 
-        # Here collecting packet bytes. Handle end of packet.
+        # Here collecting packet bytes.
         assert (self.__in_packet)
-        if b == PACKET_FLAG and not self.__pending_escape:
-            self.__process_packet()
-            self.__reset_packet()
-            # No need to wait for additional flag byte before next packet.
-            self.__in_packet = True
+
+        if b == PACKET_START_FLAG:
+            # Abort current packet and start a new one.
+            logger.error(f"Dropping partial packet of size {len(self.__packet_bfr)}.")
+            self.__reset_packet(True)
+            return
+
+        if b == PACKET_END_FLAG:
+            # Process current packet.
+            if self.__pending_escape:
+                logger.error("Packet has a pending escape, dropping.")
+            else:
+                self.__process_packet()
+            self.__reset_packet(False)
             return
 
         # Check for size overrun. At this point, we know that the packet will
-        # have at least one more additional byte.
+        # have at least one more additional byte, either normal or escaped.
         if len(self.__packet_bfr) >= MAX_PACKET_LEN:
             logger.error("Packet is too long (%d), dropping", len(self.__packet_bfr))
-            self.__reset_packet()
+            self.__reset_packet(False)
             return
 
-        # Handle escape byte
+        # Handle escape byte.
         if b == PACKET_ESC:
             if self.__pending_escape:
                 logger.error("Two consecutive escape chars, dropping packet")
-                self.__reset_packet()
+                self.__reset_packet(False)
             else:
                 self.__pending_escape = True
             return
 
-        # Handle escaped byte.
+        # Handle an escaped byte.
         if self.__pending_escape:
+            # Flip back for 5x to 7x.
             b1 = b ^ 0x20
-            if b1 != PACKET_FLAG and b1 != PACKET_ESC:
-                logger.error("Invalid escaped byte (%02x, %02x), dropping packet", b1, b)
-                self.__reset_packet()
+            if b1 != PACKET_START_FLAG and b1 != PACKET_END_FLAG and b1 != PACKET_ESC:
+                logger.error(f"Invalid escaped byte ({b1:02x}, {b:02x}), dropping packet")
+                self.__reset_packet(False)
             else:
                 self.__packet_bfr.append(b1)
                 self.__pending_escape = False
             return
 
-        # Handle normal byte
+        # Handle a normal byte
         self.__packet_bfr.append(b)
 
     def __process_packet(self):
         rx_bfr = self.__packet_bfr
 
-        # Ignore empty packets
-        n = len(rx_bfr)
-        if not n:
-            # Zero length packet can occur normally when we insert
-            # a pre packet flag.
-            return
-
         # Check for minimum length. A minimum we should
         # have a type byte and two CRC bytes.
+        n = len(rx_bfr)
         if n < MIN_PACKET_LEN:
             logger.error("Packet too short (%d), dropping", n)
             return
 
         # Check CRC
         packet_crc = int.from_bytes(rx_bfr[-2:], byteorder='big', signed=False)
         computed_crc = self.__crc_calc.calculate(bytes(rx_bfr[:-2]))
@@ -161,14 +167,15 @@
             data = PacketData().add_bytes(rx_bfr[2:-2])
             decoded_packet = DecodedMessagePacket(endpoint, data)
         else:
             logger.error("Invalid packet type %02x, dropping packet", type.value)
             return
 
         if data.size() > MAX_DATA_LEN:
-            logger.error("Packet data too long (type=%d, len=%d), dropping", type_value, data.size())
+            logger.error("Packet data too long (type=%d, len=%d), dropping", type_value,
+                         data.size())
             return
 
         # Inform the user about the new packet.
         self.__decoded_packet_callback(decoded_packet)
 
         # self.__packets_queue.put_nowait(decoded_packet)
```

### Comparing `serial_packets-0.1.3/src/serial_packets/_packet_encoder.py` & `serial_packets-0.1.4/src/serial_packets/_packet_encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 import time
 
 from PyCRC.CRCCCITT import CRCCCITT
-from ._packets import PacketType, PACKET_FLAG, PACKET_ESC, MAX_DATA_LEN, MAX_PACKET_LEN,  PRE_FLAG_TIMEOUT
+from ._packets import PacketType, PACKET_START_FLAG, PACKET_END_FLAG, PACKET_ESC, MAX_DATA_LEN, MAX_PACKET_LEN
 
 logger = logging.getLogger(__name__)
 
 
 class PacketEncoder:
 
     def __init__(self):
@@ -34,62 +34,52 @@
         packet.extend(cmd_id.to_bytes(4, 'big'))
         packet.append(status)
         packet.extend(data)
         crc = self.__crc_calc.calculate(bytes(packet))
         packet.extend(crc.to_bytes(2, 'big'))
         assert (len(packet) <= MAX_PACKET_LEN)
         return packet
-      
+
     def __construct_message_packet(self, endpoint: int, data: bytearray):
         """Constructs a message packet, before byte stuffing"""
         packet = bytearray()
         packet.append(PacketType.MESSAGE.value)
         packet.append(endpoint)
         packet.extend(data)
         crc = self.__crc_calc.calculate(bytes(packet))
         packet.extend(crc.to_bytes(2, 'big'))
         assert (len(packet) <= MAX_PACKET_LEN)
         return packet
 
-    def __byte_stuffing(self, packet: bytearray, insert_pre_flag: bool):
+    def __byte_stuffing(self, packet: bytearray):
         """Byte stuff the packet using HDLC format. Also adds packet flag(s)"""
         result = bytearray()
-        if insert_pre_flag:
-            result.append(PACKET_FLAG)
+        result.append(PACKET_START_FLAG)
         for byte in packet:
-            if byte == PACKET_FLAG or byte == PACKET_ESC:
+            if byte == PACKET_START_FLAG or byte == PACKET_END_FLAG or byte == PACKET_ESC:
                 result.append(PACKET_ESC)
                 result.append(byte ^ 0x20)
             else:
                 result.append(byte)
-        result.append(PACKET_FLAG)
+        result.append(PACKET_END_FLAG)
         return result
 
-    # def __track_packet_interval(self):
-    #     last_packet_time = self.__last_packet_time
-    #     self.__last_packet_time = time.time()
-    #     elapsed = self.__last_packet_time - last_packet_time
-    #     # We insert a pre packet flag only if the packets are sparse.
-    #     insert_pre_flag = elapsed > PRE_FLAG_TIMEOUT
-    #     return insert_pre_flag
-
-    def encode_command_packet(self, cmd_id: int, endpoint: int, data: bytearray, insert_pre_flag: bool):
+    def encode_command_packet(self, cmd_id: int, endpoint: int, data: bytearray):
         """Returns the command packet in wire format"""
         assert (len(data) <= MAX_DATA_LEN)
         packet = self.__construct_command_packet(cmd_id, endpoint, data)
-        stuffed_packet = self.__byte_stuffing(packet, insert_pre_flag)
+        stuffed_packet = self.__byte_stuffing(packet)
         return stuffed_packet
 
-    def encode_response_packet(self, cmd_id: int, status: int, data: bytearray, insert_pre_flag: bool):
+    def encode_response_packet(self, cmd_id: int, status: int, data: bytearray):
         """Returns the packet in wire format."""
         assert (len(data) <= MAX_DATA_LEN)
         packet = self.__construct_response_packet(cmd_id, status, data)
-        stuffed_packet = self.__byte_stuffing(packet, insert_pre_flag)
+        stuffed_packet = self.__byte_stuffing(packet)
         return stuffed_packet
-      
-    def encode_message_packet(self,  endpoint: int, data: bytearray, insert_pre_flag: bool):
+
+    def encode_message_packet(self, endpoint: int, data: bytearray):
         """Returns the message packet in wire format"""
         assert (len(data) <= MAX_DATA_LEN)
         packet = self.__construct_message_packet(endpoint, data)
-        stuffed_packet = self.__byte_stuffing(packet, insert_pre_flag)
-        return stuffed_packet  
- 
+        stuffed_packet = self.__byte_stuffing(packet)
+        return stuffed_packet
```

### Comparing `serial_packets-0.1.3/src/serial_packets/_packets.py` & `serial_packets-0.1.4/src/serial_packets/_packets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 from enum import Enum
 from .packets import MAX_DATA_LEN
 
-# Flag and escape bytes per HDLC specification.
-PACKET_FLAG = 0x7E
+# Flag and escape bytes. Inspired by the HDLC specification.
+PACKET_START_FLAG = 0x7C
 PACKET_ESC = 0X7D
+PACKET_END_FLAG = 0x7E
 
 # Prefix a packet with a flag byte only if interval from previous
 # encoded packet is longer that this time in secs.
-PRE_FLAG_TIMEOUT = 1.0
+# PRE_FLAG_TIMEOUT = 1.0
 
 # Packet sizes in bytes, with zero data length, and before
 # byte stuffing, and flagging.
 MIN_PACKET_OVERHEAD = 4
 MAX_PACKET_OVERHEAD = 8
 
 MIN_PACKET_LEN = MIN_PACKET_OVERHEAD
```

### Comparing `serial_packets-0.1.3/src/serial_packets/client.py` & `serial_packets-0.1.4/src/serial_packets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import traceback
 
 from enum import Enum
 from typing import Optional, Tuple, Dict, Callable
 from asyncio.transports import BaseTransport
 from ._packet_encoder import PacketEncoder
 from ._packet_decoder import PacketDecoder, DecodedCommandPacket, DecodedResponsePacket, DecodedMessagePacket
-from ._packets import PacketType, MAX_DATA_LEN, MIN_CMD_TIMEOUT, MAX_CMD_TIMEOUT, DEFAULT_CMD_TIMEOUT, MIN_WORKERS_COUNT, MAX_WORKERS_COUNT, DEFAULT_WORKERS_COUNT, PRE_FLAG_TIMEOUT
-from ._interval_tracker import IntervalTracker
+from ._packets import PacketType, MAX_DATA_LEN, MIN_CMD_TIMEOUT, MAX_CMD_TIMEOUT, DEFAULT_CMD_TIMEOUT, MIN_WORKERS_COUNT, MAX_WORKERS_COUNT, DEFAULT_WORKERS_COUNT
+# from ._interval_tracker import IntervalTracker
 from .packets import PacketStatus, PacketsEvent, PacketsEventType, PacketsEvent, PacketData, MAX_USER_ENDPOINT
 
 logger = logging.getLogger(__name__)
 
 # pyserial_asyncio is documented at
 # https://github.com/pyserial/pyserial-asyncio
 
@@ -129,15 +129,15 @@
         self.__message_async_callback = message_async_callback
         self.__event_async_callback = event_async_callback
         self.__transport = None
         self.__protocol = None
         self.__packet_encoder = PacketEncoder()
         self.__packet_decoder = PacketDecoder(self.__on_decoded_packet)
         self.__command_id_counter = 0
-        self.__interval_tracker = IntervalTracker(PRE_FLAG_TIMEOUT)
+        # self.__interval_tracker = IntervalTracker(PRE_FLAG_TIMEOUT)
         self.__tx_cmd_contexts: Dict[int, _TxCommandContext] = {}
         # Work items types:
         # * PacketsEvent: call user's event handler.
         # * DecodedCommandPacket: handle incoming command packet.
         # * DecodedResponsePacket: handle incoming response packet.
         # * DecodedMessagePacket: handle incoming message packet.
         self.__work_queue = asyncio.Queue()
@@ -238,15 +238,15 @@
                                                                decoded_cmd_packet.data)
             if data.size() > MAX_DATA_LEN:
                 logger.error("Command response data too long (%d), failing command", data.size9)
                 status, data = (PacketStatus.LENGTH_ERROR.value, PacketData())
         else:
             status, data = (PacketStatus.UNHANDLED.value, PacketData())
         response_packet = self.__packet_encoder.encode_response_packet(
-            decoded_cmd_packet.cmd_id, status, data._internal_bytes_buffer(), self.__interval_tracker.track_packet())
+            decoded_cmd_packet.cmd_id, status, data._internal_bytes_buffer())
         self.__transport.write(response_packet)
 
     async def __handle_incoming_response_packet(self, decoded_rsp_packet: DecodedResponsePacket):
         # print(f"Handling resp packet ({len(self.__tx_cmd_contexts)} tx contexts)", flush=True)
         assert (isinstance(decoded_rsp_packet, DecodedResponsePacket))
         tx_context: _TxCommandContext = self.__tx_cmd_contexts.pop(decoded_rsp_packet.cmd_id, None)
         if not tx_context:
@@ -331,15 +331,15 @@
             return future
         # Allocate a 32 bit fresh command id. Wrap around are ok since
         # commands are short living.
         self.__command_id_counter = (self.__command_id_counter + 1) & 0xffffffff
         cmd_id = self.__command_id_counter
         assert (not cmd_id in self.__tx_cmd_contexts)
         # Encode packet bytes
-        packet = self.__packet_encoder.encode_command_packet(cmd_id, endpoint, data._internal_bytes_buffer(), self.__interval_tracker.track_packet())
+        packet = self.__packet_encoder.encode_command_packet(cmd_id, endpoint, data._internal_bytes_buffer())
         logger.debug("TX command packet [%d]: %s", endpoint, packet.hex(sep=' '))
         # Create command tx context
         expiration_time = time.time() + timeout
         future = asyncio.Future()
         tx_cmd_context = _TxCommandContext(cmd_id, expiration_time, future)
         self.__tx_cmd_contexts[cmd_id] = tx_cmd_context
         # Start sending
@@ -359,11 +359,11 @@
             """
         assert (endpoint >= 0 and endpoint <= MAX_USER_ENDPOINT)
         assert (data.size() <= MAX_DATA_LEN)
         if not self.is_connected():
             logger.warn("Client not connected, ignoring message send")
             return
         # Encode packet bytes
-        packet = self.__packet_encoder.encode_message_packet(endpoint, data._internal_bytes_buffer(), self.__interval_tracker.track_packet())
+        packet = self.__packet_encoder.encode_message_packet(endpoint, data._internal_bytes_buffer())
         logger.debug("TX message packet [%d]: %s", endpoint, packet.hex(sep=' '))
         # Start sending
         self.__transport.write(packet)
```

### Comparing `serial_packets-0.1.3/src/serial_packets/packets.py` & `serial_packets-0.1.4/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.3/LICENSE` & `serial_packets-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.3/README.md` & `serial_packets-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Python Serial Packets
 
+**NOTE**: As of June 21 2023, the **wire format changed** to have distinct
+packet start and stop flag bytes.
+
 Python implementations of the Serial Packets protocol.
 
 * PYPI: <https://pypi.org/project/serial-packets/>
 * Github: <https://github.com/zapta/serial_packets_py>
 
 Related works:
 
@@ -34,31 +37,31 @@
 Commands are round-trip interactions where one node send a 'command' packet receives as 'response' packet from the other node. Commands can be used for example the device and to retrieve information selected
 information.
 
 The following tables lists the fields of command request and response  packets respectively. Note that this is not the exact wire representation since the packets are subject to flagging and byte stuffing as explained later.
 
 #### Command packet
 
-| Field     | Size [bytes] | Source   | Description                                            |
-| :-------- | :----------- | :------- | :----------------------------------------------------- |
-| PACKET_TYPE      | 1            | Auto     | The value 0x01                                         |
-| CMD_ID    | 4            | Auto     | A unique command id for response matching. Big Endian. |
-| END_POINT | 1            | **User** | The target endpoint of this command.                   |
-| DATA      | 0 to 1024    | **User** | Command data.                                          |
-| CRC       | 2            | Auto     | Packet CRC. Big endian.                                |
+| Field       | Size [bytes] | Source   | Description                                            |
+| :---------- | :----------- | :------- | :----------------------------------------------------- |
+| PACKET_TYPE | 1            | Auto     | The value 0x01                                         |
+| CMD_ID      | 4            | Auto     | A unique command id for response matching. Big Endian. |
+| END_POINT   | 1            | **User** | The target endpoint of this command.                   |
+| DATA        | 0 to 1024    | **User** | Command data.                                          |
+| CRC         | 2            | Auto     | Packet CRC. Big endian.                                |
 
 #### Response packet
 
-| Field  | Size [bytes] | Source   | Description                                 |
-| :----- | :----------- | :------- | :------------------------------------------ |
-| PACKET_TYPE   | 1            | Auto     | The value 0x02                              |
-| CMD_ID | 4            | Auto     | The ID of the original command. Big Endian. |
-| STATUS | 1            | **User** | Response status.                            |
-| DATA   | 0 to 1024    | **User** | Response data.                              |
-| CRC    | 2            | Auto     | Packet CRC. Big endian.                     |
+| Field       | Size [bytes] | Source   | Description                                 |
+| :---------- | :----------- | :------- | :------------------------------------------ |
+| PACKET_TYPE | 1            | Auto     | The value 0x02                              |
+| CMD_ID      | 4            | Auto     | The ID of the original command. Big Endian. |
+| STATUS      | 1            | **User** | Response status.                            |
+| DATA        | 0 to 1024    | **User** | Response data.                              |
+| CRC         | 2            | Auto     | Packet CRC. Big endian.                     |
 
 #### Sending a command
 
 The SerialPacketsClient class provides two methods for sending commands.
 *send_command_future(...)* for sending using a future that provides the response and *send_command_blocking(...)* which is a convenience method that blocks internally on the future.
 
 Future base command sending:
@@ -119,20 +122,20 @@
 
 ### Messages
 
 Messages are a simpler case of a commands with no response. They are useful for periodic notifications, for example for data reporting, and have lower overhead than commands.
 
 #### Message packet
 
-| Field     | Size [bytes] | Source   | Description                          |
-| :-------- | :----------- | :------- | :----------------------------------- |
-| PACKET_TYPE      | 1            | Auto     | The value 0x03                       |
-| END_POINT | 1            | **User** | The target endpoint of this command. |
-| DATA      | 0 to 1024    | **User** | Command data.                        |
-| CRC       | 2            | Auto     | Packet CRC. Big endian.              |
+| Field       | Size [bytes] | Source   | Description                          |
+| :---------- | :----------- | :------- | :----------------------------------- |
+| PACKET_TYPE | 1            | Auto     | The value 0x03                       |
+| END_POINT   | 1            | **User** | The target endpoint of this command. |
+| DATA        | 0 to 1024    | **User** | Command data.                        |
+| CRC         | 2            | Auto     | Packet CRC. Big endian.              |
 
 #### Sending a message
 
 The *SerialPacketsClient* class provides a method for sending a command. The method is non blocking and merely queues the message for sending.
 two methods for sending commands.
 
 ```python
@@ -237,50 +240,50 @@
 data_bytes() -> bytearray  # Returns a copy of the data bytes.
 size() -> int  # Returns the number of data bytes.
 clear() -> None # Clear the data and reset the read location and error flag..
 ```
 
 ## Wire representation
 
-### Packet flag byte
+### Packet start/stop flags
 
-The Serial Packets protocol uses packet flags similar to the HDLC protocol, with the special flag byte 0x7E inserted in the serial stream to mark packet ends. A flag byte is always inserted immediately after the
-last byte of each packet, and also optionally just before the first byte of packets, if the interval from the previous packet was longer than a certain time period.
+The Serial Packets protocol uses packet flags inspired from the HDLC protocol, with the special flag bytes 0X7C, 0x7E indicating the beginning and end of a packet, respectively.
 
 ### Byte stuffing
 
-To make the flag byte 0x7E unique in the serial stream, the Serial Packet uses 'byte stuffing' borrowed from the HDLC protocol. This allows the protocol to resync on next packet boundary, in case of line errors. This byte stuffing is done using the escape byte 0X7D
+To make the flag bytes 0X7C, 0x7E unique in the serial stream, the Serial Packet uses 'byte stuffing' borrowed from the HDLC protocol. This allows the protocol to resync on next packet boundary, in case of line errors. This byte stuffing is done using the escape byte 0X7D
 
 | Packet byte | Wire bytes | Comments            |
 | :---------- | :--------- | :------------------ |
-| 0x7E        | 0x7D, 0x5E | Escaped flag byte   |
+| 0x7C        | 0x7D, 0x5C | Escaped start flag  |
 | 0x7D        | 0x7D, 0x5D | Escaped escape byte |
+| 0x7E        | 0x7D, 0x5E | Escaped end flag    |
 | Other bytes | No change  | The common case     |
 
 Example of a command packet:
 
 ```python
 
 Stuffed command packet:
-0x7e, 0x01, 0xff, 0x12, 0x34, 0x56, 0x20, 0xff, 
-0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99, 0x09,
-0x8c, 0x7e
+ 0x7c, 0x01, 0xff, 0x12, 0x34, 0x56, 0x20, 0xff, 
+ 0x00, 0x7d, 0x5c, 0x11, 0x7d, 0x5e, 0x22, 0x7d, 
+ 0x5d, 0x99, 0x7a, 0xa7, 0x7e
 
 Breakdown into parts:
-flag:         0x7e
+start flag:   0x7c
 packet_type:  0x01
 cmd_id:       0xff, 0x12, 0x34, 0x56
 endpoint:     0x20
-data:         0xff, 0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99
-crc:          0x09, 0x8c
+data:         0xff, 0x00, 0x7d, 0x5c, 0x11, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99
+crc:          0x7a, 0xa7
 flag:         0x7e
 
 # In this examples, only the data part contains escaped bytes and its
 # unescaped version is:
-data:   0xff, 0x00, 0x7e, 0x22, 0x7d, 0x99
+data:  0xff, 0x00, 0x7c, 0x11, 0x7e, 0x22, 0x7d, 0x99
 ```
 
 ## Status codes
 
 The Serial Packets protocol uses 1 byte status codes where 0x00 indicates success and all other values indicate errors. These status codes are used in the command responses, and optionally also by the implementation API for other reasons.
 
 As of May 2023, these are the predefined status codes. For the updated list, look at the *serial_packets.packets.PacketStatus* enum.
```

### Comparing `serial_packets-0.1.3/pyproject.toml` & `serial_packets-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.3/PKG-INFO` & `serial_packets-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,17 @@
 Requires-Python: >=3.7
 Requires-Dist: pyserial-asyncio>=0.6.0
 Requires-Dist: pythoncrc>=1.21.0
 Description-Content-Type: text/markdown
 
 # Python Serial Packets
 
+**NOTE**: As of June 21 2023, the **wire format changed** to have distinct
+packet start and stop flag bytes.
+
 Python implementations of the Serial Packets protocol.
 
 * PYPI: <https://pypi.org/project/serial-packets/>
 * Github: <https://github.com/zapta/serial_packets_py>
 
 Related works:
 
@@ -50,31 +53,31 @@
 Commands are round-trip interactions where one node send a 'command' packet receives as 'response' packet from the other node. Commands can be used for example the device and to retrieve information selected
 information.
 
 The following tables lists the fields of command request and response  packets respectively. Note that this is not the exact wire representation since the packets are subject to flagging and byte stuffing as explained later.
 
 #### Command packet
 
-| Field     | Size [bytes] | Source   | Description                                            |
-| :-------- | :----------- | :------- | :----------------------------------------------------- |
-| PACKET_TYPE      | 1            | Auto     | The value 0x01                                         |
-| CMD_ID    | 4            | Auto     | A unique command id for response matching. Big Endian. |
-| END_POINT | 1            | **User** | The target endpoint of this command.                   |
-| DATA      | 0 to 1024    | **User** | Command data.                                          |
-| CRC       | 2            | Auto     | Packet CRC. Big endian.                                |
+| Field       | Size [bytes] | Source   | Description                                            |
+| :---------- | :----------- | :------- | :----------------------------------------------------- |
+| PACKET_TYPE | 1            | Auto     | The value 0x01                                         |
+| CMD_ID      | 4            | Auto     | A unique command id for response matching. Big Endian. |
+| END_POINT   | 1            | **User** | The target endpoint of this command.                   |
+| DATA        | 0 to 1024    | **User** | Command data.                                          |
+| CRC         | 2            | Auto     | Packet CRC. Big endian.                                |
 
 #### Response packet
 
-| Field  | Size [bytes] | Source   | Description                                 |
-| :----- | :----------- | :------- | :------------------------------------------ |
-| PACKET_TYPE   | 1            | Auto     | The value 0x02                              |
-| CMD_ID | 4            | Auto     | The ID of the original command. Big Endian. |
-| STATUS | 1            | **User** | Response status.                            |
-| DATA   | 0 to 1024    | **User** | Response data.                              |
-| CRC    | 2            | Auto     | Packet CRC. Big endian.                     |
+| Field       | Size [bytes] | Source   | Description                                 |
+| :---------- | :----------- | :------- | :------------------------------------------ |
+| PACKET_TYPE | 1            | Auto     | The value 0x02                              |
+| CMD_ID      | 4            | Auto     | The ID of the original command. Big Endian. |
+| STATUS      | 1            | **User** | Response status.                            |
+| DATA        | 0 to 1024    | **User** | Response data.                              |
+| CRC         | 2            | Auto     | Packet CRC. Big endian.                     |
 
 #### Sending a command
 
 The SerialPacketsClient class provides two methods for sending commands.
 *send_command_future(...)* for sending using a future that provides the response and *send_command_blocking(...)* which is a convenience method that blocks internally on the future.
 
 Future base command sending:
@@ -135,20 +138,20 @@
 
 ### Messages
 
 Messages are a simpler case of a commands with no response. They are useful for periodic notifications, for example for data reporting, and have lower overhead than commands.
 
 #### Message packet
 
-| Field     | Size [bytes] | Source   | Description                          |
-| :-------- | :----------- | :------- | :----------------------------------- |
-| PACKET_TYPE      | 1            | Auto     | The value 0x03                       |
-| END_POINT | 1            | **User** | The target endpoint of this command. |
-| DATA      | 0 to 1024    | **User** | Command data.                        |
-| CRC       | 2            | Auto     | Packet CRC. Big endian.              |
+| Field       | Size [bytes] | Source   | Description                          |
+| :---------- | :----------- | :------- | :----------------------------------- |
+| PACKET_TYPE | 1            | Auto     | The value 0x03                       |
+| END_POINT   | 1            | **User** | The target endpoint of this command. |
+| DATA        | 0 to 1024    | **User** | Command data.                        |
+| CRC         | 2            | Auto     | Packet CRC. Big endian.              |
 
 #### Sending a message
 
 The *SerialPacketsClient* class provides a method for sending a command. The method is non blocking and merely queues the message for sending.
 two methods for sending commands.
 
 ```python
@@ -253,50 +256,50 @@
 data_bytes() -> bytearray  # Returns a copy of the data bytes.
 size() -> int  # Returns the number of data bytes.
 clear() -> None # Clear the data and reset the read location and error flag..
 ```
 
 ## Wire representation
 
-### Packet flag byte
+### Packet start/stop flags
 
-The Serial Packets protocol uses packet flags similar to the HDLC protocol, with the special flag byte 0x7E inserted in the serial stream to mark packet ends. A flag byte is always inserted immediately after the
-last byte of each packet, and also optionally just before the first byte of packets, if the interval from the previous packet was longer than a certain time period.
+The Serial Packets protocol uses packet flags inspired from the HDLC protocol, with the special flag bytes 0X7C, 0x7E indicating the beginning and end of a packet, respectively.
 
 ### Byte stuffing
 
-To make the flag byte 0x7E unique in the serial stream, the Serial Packet uses 'byte stuffing' borrowed from the HDLC protocol. This allows the protocol to resync on next packet boundary, in case of line errors. This byte stuffing is done using the escape byte 0X7D
+To make the flag bytes 0X7C, 0x7E unique in the serial stream, the Serial Packet uses 'byte stuffing' borrowed from the HDLC protocol. This allows the protocol to resync on next packet boundary, in case of line errors. This byte stuffing is done using the escape byte 0X7D
 
 | Packet byte | Wire bytes | Comments            |
 | :---------- | :--------- | :------------------ |
-| 0x7E        | 0x7D, 0x5E | Escaped flag byte   |
+| 0x7C        | 0x7D, 0x5C | Escaped start flag  |
 | 0x7D        | 0x7D, 0x5D | Escaped escape byte |
+| 0x7E        | 0x7D, 0x5E | Escaped end flag    |
 | Other bytes | No change  | The common case     |
 
 Example of a command packet:
 
 ```python
 
 Stuffed command packet:
-0x7e, 0x01, 0xff, 0x12, 0x34, 0x56, 0x20, 0xff, 
-0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99, 0x09,
-0x8c, 0x7e
+ 0x7c, 0x01, 0xff, 0x12, 0x34, 0x56, 0x20, 0xff, 
+ 0x00, 0x7d, 0x5c, 0x11, 0x7d, 0x5e, 0x22, 0x7d, 
+ 0x5d, 0x99, 0x7a, 0xa7, 0x7e
 
 Breakdown into parts:
-flag:         0x7e
+start flag:   0x7c
 packet_type:  0x01
 cmd_id:       0xff, 0x12, 0x34, 0x56
 endpoint:     0x20
-data:         0xff, 0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99
-crc:          0x09, 0x8c
+data:         0xff, 0x00, 0x7d, 0x5c, 0x11, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99
+crc:          0x7a, 0xa7
 flag:         0x7e
 
 # In this examples, only the data part contains escaped bytes and its
 # unescaped version is:
-data:   0xff, 0x00, 0x7e, 0x22, 0x7d, 0x99
+data:  0xff, 0x00, 0x7c, 0x11, 0x7e, 0x22, 0x7d, 0x99
 ```
 
 ## Status codes
 
 The Serial Packets protocol uses 1 byte status codes where 0x00 indicates success and all other values indicate errors. These status codes are used in the command responses, and optionally also by the implementation API for other reasons.
 
 As of May 2023, these are the predefined status codes. For the updated list, look at the *serial_packets.packets.PacketStatus* enum.
```

