# Comparing `tmp/aioarp-0.0.7.tar.gz` & `tmp/aioarp-0.0.8.tar.gz`

## Comparing `aioarp-0.0.7.tar` & `aioarp-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aioarp-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 aioarp-0.0.7/mkdocs.yml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aioarp-0.0.7/requirements.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.7/unasync.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.7/.github/workflows/main.yml
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 aioarp-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/__about__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/__init__.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_arp.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_async.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_cli.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_client.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_exceptions.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_mock.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_sync.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/defaults.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_backends/__init__.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_backends/_async.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_backends/_base.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_backends/_mock.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.7/aioarp/_backends/_sync.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 aioarp-0.0.7/docs/client.md
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 aioarp-0.0.7/docs/index.md
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 aioarp-0.0.7/scripts/check
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.7/scripts/lint
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 aioarp-0.0.7/scripts/publish
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.7/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioarp-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.7/tests/test_async.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.7/tests/test_client.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.7/tests/test_proto.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.7/tests/test_sync.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.7/tests/test_utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aioarp-0.0.7/README.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 aioarp-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 aioarp-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aioarp-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 aioarp-0.0.8/mkdocs.yml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aioarp-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.8/unasync.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 aioarp-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/__init__.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_arp.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_async.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_cli.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_client.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_exceptions.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_mock.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_sync.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/defaults.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/__init__.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_async.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_base.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_mock.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_sync.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 aioarp-0.0.8/docs/client.md
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 aioarp-0.0.8/docs/index.md
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/check
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/lint
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/publish
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/publish-docs
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/conftest.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_async.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_client.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_proto.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_sync.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_utils.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aioarp-0.0.8/README.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 aioarp-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aioarp-0.0.8/PKG-INFO
```

### Comparing `aioarp-0.0.7/unasync.py` & `aioarp-0.0.8/unasync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/.github/workflows/main.yml` & `aioarp-0.0.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/aioarp/_arp.py` & `aioarp-0.0.8/aioarp/_arp.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/aioarp/_async.py` & `aioarp-0.0.8/aioarp/_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import time
 import typing
 
 from aioarp import _exceptions as exc
 from aioarp._arp import ARP_HEADER_SIZE, ETHERNET_HEADER_SIZE, ArpPacket, EthPacket, Protocol
+from aioarp._backends import AsyncStream
 from aioarp._utils import is_valid_ipv4
 from aioarp.defaults import DEFAULT_READ_TIMEOUT, DEFAULT_REPLY_MISSING_TIME, DEFAULT_WRITE_TIMEOUT
 
-from ._backends._async import AsyncStream
-
 __all__ = (
     'async_send_arp',
 )
 
 
 async def receive_arp(sock: AsyncStream, timeout: float) -> ArpPacket:
     start_time = time.time()
@@ -42,21 +41,24 @@
         except BaseException:  # pragma: no cover
             # TODO: catch concrete errors
             ...
 
 
 async def async_send_arp(arp_packet: ArpPacket,
                          stream: AsyncStream,
-                         timeout: typing.Optional[float] = None) -> ArpPacket:
+                         timeout: typing.Optional[float] = None,
+                         wait_response: bool = True) -> typing.Optional[ArpPacket]:
     ethernet_packet = EthPacket(
         target_mac=arp_packet.target_mac,
         sender_mac=arp_packet.sender_mac,
         proto=Protocol.arp
     )
 
     try:
         frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
         await stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
     except exc.WriteTimeoutError as e:  # pragma: no cover
         raise exc.NotFoundError from e
-
-    return await receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
+    
+    if wait_response:
+        return await receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
+    return None  # pragma: no cover
```

### Comparing `aioarp-0.0.7/aioarp/_cli.py` & `aioarp-0.0.8/aioarp/_cli.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/aioarp/_client.py` & `aioarp-0.0.8/aioarp/_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,31 +43,33 @@
     return request_packet
 
 
 def request(
         interface: str,
         target_ip: str,
         timeout: typing.Optional[float] = None,
-        sock: typing.Optional[SocketInterface] = None
-) -> ArpPacket:
+        sock: typing.Optional[SocketInterface] = None,
+        wait_response: bool = True
+) -> typing.Optional[ArpPacket]:
     if not sock:  # pragma: no cover
         sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
     with Stream(interface=interface,
                     sock=sock) as stream:
         request_packet = build_arp_packet(interface, target_ip)
-        arp_response = sync_send_arp(request_packet, stream, timeout)
+        arp_response = sync_send_arp(request_packet, stream, timeout, wait_response)
         return arp_response
 
 
 async def arequest(
         interface: str,
         target_ip: str,
         timeout: typing.Optional[float] = None,
-        sock: typing.Optional[SocketInterface] = None
-) -> ArpPacket:
+        sock: typing.Optional[SocketInterface] = None,
+        wait_response: bool = True
+) -> typing.Optional[ArpPacket]:
     if not sock:  # pragma: no cover
         sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
     with AsyncStream(interface=interface,
                     sock=sock) as stream:
         request_packet = build_arp_packet(interface, target_ip)
-        arp_response = await async_send_arp(request_packet, stream, timeout)
+        arp_response = await async_send_arp(request_packet, stream, timeout, wait_response)
         return arp_response
```

### Comparing `aioarp-0.0.7/aioarp/_sync.py` & `aioarp-0.0.8/aioarp/_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 import typing
 
-from aioarp import Stream, _exceptions as exc
+from aioarp import _exceptions as exc
 from aioarp._arp import ARP_HEADER_SIZE, ETHERNET_HEADER_SIZE, ArpPacket, EthPacket, Protocol
+from aioarp._backends import Stream
 from aioarp._utils import is_valid_ipv4
 from aioarp.defaults import DEFAULT_READ_TIMEOUT, DEFAULT_REPLY_MISSING_TIME, DEFAULT_WRITE_TIMEOUT
 
 __all__ = (
     'sync_send_arp',
 )
 
@@ -40,21 +41,24 @@
         except BaseException:  # pragma: no cover
             # TODO: catch concrete errors
             ...
 
 
 def sync_send_arp(arp_packet: ArpPacket,
                          stream: Stream,
-                         timeout: typing.Optional[float] = None) -> ArpPacket:
+                         timeout: typing.Optional[float] = None,
+                         wait_response: bool = True) -> typing.Optional[ArpPacket]:
     ethernet_packet = EthPacket(
         target_mac=arp_packet.target_mac,
         sender_mac=arp_packet.sender_mac,
         proto=Protocol.arp
     )
 
     try:
         frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
         stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
     except exc.WriteTimeoutError as e:  # pragma: no cover
         raise exc.NotFoundError from e
-
-    return receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
+    
+    if wait_response:
+        return receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
+    return None  # pragma: no cover
```

### Comparing `aioarp-0.0.7/aioarp/_utils.py` & `aioarp-0.0.8/aioarp/_utils.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/aioarp/_backends/_async.py` & `aioarp-0.0.8/aioarp/_backends/_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/aioarp/_backends/_mock.py` & `aioarp-0.0.8/aioarp/_backends/_mock.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/aioarp/_backends/_sync.py` & `aioarp-0.0.8/aioarp/_backends/_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/docs/client.md` & `aioarp-0.0.8/docs/client.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 This is simply sending the arp packet that searches the network for a mac address of the `10.0.2.2` ip using the interface that you provided.
 You can also use a `timeout` to ensure that waiting for a response does not go on indefinitely.
 
 ```py title="timeout request"
 aioarp.request("enp0s3", "10.0.2.2", timeout=0.5)
 ```
 
+You can also use the `wait_response` parameter to tell aioarp whether you need the response or not.
+```py title="without waiting for a response"
+aioarp.request("enp0s3", "10.0.2.2", wait_response=False)
+```
+
+!!! note
+
+    When the `wait_response` argument is false, the `timeout` argument has no effect.
+
+
 This method can also take the `sock` argument, which is a socket connection that will be used for IO operations. (useful for mocking)
 
 ## Asynchronous requests
 
 It is very simple to switch from synchronous to asynchronous aioarp; simply use the await keyword and change request to arequest.
 
 ```py title="async request"
```

### Comparing `aioarp-0.0.7/docs/index.md` & `aioarp-0.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/tests/test_async.py` & `aioarp-0.0.8/tests/test_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     b"\x11\x11\x7f\x00\x00\x01"
     b"\x11\x11\x11\x11\x11\x11"
     b"\x7f\x00\x00\x01"
 )
 
 
 @pytest.mark.anyio
-async def test_async_send_arp():
+def test_async_send_arp():
     msocket = MockSocket(eth_header_arp + arp_header)
-    response = await aioarp.arequest('null', '100.100.100.100', sock=msocket)
+    response = aioarp.request('null', '100.100.100.100', sock=msocket)
+    assert response
     assert response.sender_mac == '11:11:11:11:11:11'
 
 
 @pytest.mark.anyio
-async def test_async_send_arp_timeout():
+def test_async_send_arp_timeout():
     with MockSocket(eth_header_no_arp + arp_header) as msocket:
         with pytest.raises(aioarp.NotFoundError):
-            await aioarp.arequest('null', '100.100.100.100', sock=msocket, timeout=0.5)
+            aioarp.request('null', '100.100.100.100', sock=msocket, timeout=0.5)
```

### Comparing `aioarp-0.0.7/tests/test_client.py` & `aioarp-0.0.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/tests/test_proto.py` & `aioarp-0.0.8/tests/test_proto.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/tests/test_sync.py` & `aioarp-0.0.8/tests/test_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     b"\x11\x11\x7f\x00\x00\x01"
     b"\x11\x11\x11\x11\x11\x11"
     b"\x7f\x00\x00\x01"
 )
 
 
 @pytest.mark.anyio
-def test_async_send_arp():
+async def test_async_send_arp():
     msocket = MockSocket(eth_header_arp + arp_header)
-    response = aioarp.request('null', '100.100.100.100', sock=msocket)
+    response = await aioarp.arequest('null', '100.100.100.100', sock=msocket)
+    assert response
     assert response.sender_mac == '11:11:11:11:11:11'
 
 
 @pytest.mark.anyio
-def test_async_send_arp_timeout():
+async def test_async_send_arp_timeout():
     with MockSocket(eth_header_no_arp + arp_header) as msocket:
         with pytest.raises(aioarp.NotFoundError):
-            aioarp.request('null', '100.100.100.100', sock=msocket, timeout=0.5)
+            await aioarp.arequest('null', '100.100.100.100', sock=msocket, timeout=0.5)
```

### Comparing `aioarp-0.0.7/.gitignore` & `aioarp-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/LICENSE.txt` & `aioarp-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.7/pyproject.toml` & `aioarp-0.0.8/pyproject.toml`

 * *Files identical despite different names*

