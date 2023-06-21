# Comparing `tmp/MCRP-0.1.8-py3-none-any.whl.zip` & `tmp/MCRP-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 24498 bytes, number of entries: 12
--rw-r--r--  2.0 unx       80 b- defN 23-Mar-18 21:26 MCRP/__init__.py
--rw-r--r--  2.0 unx      611 b- defN 23-Mar-18 21:26 MCRP/iautil.py
--rw-r--r--  2.0 unx    14560 b- defN 23-Mar-18 21:26 MCRP/mcrp.py
--rw-r--r--  2.0 unx     5927 b- defN 23-Mar-18 21:26 MCRP/mcwp.py
--rw-r--r--  2.0 unx     4114 b- defN 23-Mar-18 21:26 MCRP/tcproxy.py
--rw-r--r--  2.0 unx      882 b- defN 23-Mar-18 21:26 MCRP/util.py
--rw-rw-rw-  2.0 unx    35060 b- defN 23-Mar-18 21:27 MCRP-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     7314 b- defN 23-Mar-18 21:27 MCRP-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-18 21:27 MCRP-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Mar-18 21:27 MCRP-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-18 21:27 MCRP-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      883 b- defN 23-Mar-18 21:27 MCRP-0.1.8.dist-info/RECORD
-12 files, 69569 bytes uncompressed, 23040 bytes compressed:  66.9%
+Zip file size: 24513 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       80 b- defN 23-Mar-20 20:43 MCRP/__init__.py
+-rw-r--r--  2.0 unx      611 b- defN 23-Mar-20 20:43 MCRP/iautil.py
+-rw-r--r--  2.0 unx    14614 b- defN 23-Mar-20 20:43 MCRP/mcrp.py
+-rw-r--r--  2.0 unx     5931 b- defN 23-Mar-20 20:43 MCRP/mcwp.py
+-rw-r--r--  2.0 unx     4157 b- defN 23-Mar-20 20:43 MCRP/tcproxy.py
+-rw-r--r--  2.0 unx      882 b- defN 23-Mar-20 20:43 MCRP/util.py
+-rw-rw-rw-  2.0 unx    35060 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7314 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      883 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/RECORD
+12 files, 69670 bytes uncompressed, 23055 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: MCRP/tcproxy.py
 Comment: 
 
 Filename: MCRP/util.py
 Comment: 
 
-Filename: MCRP-0.1.8.dist-info/LICENSE
+Filename: MCRP-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: MCRP-0.1.8.dist-info/METADATA
+Filename: MCRP-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: MCRP-0.1.8.dist-info/WHEEL
+Filename: MCRP-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: MCRP-0.1.8.dist-info/entry_points.txt
+Filename: MCRP-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: MCRP-0.1.8.dist-info/top_level.txt
+Filename: MCRP-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: MCRP-0.1.8.dist-info/RECORD
+Filename: MCRP-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MCRP/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .mcrp import MCRewriteProxy, Relative, ProtocolDecryptor
 
-version = '0.1.8'
+version = '0.1.9'
```

## MCRP/mcrp.py

```diff
@@ -306,15 +306,16 @@
             # Handle EncryptionResponse
             if t is self.PROTOCOL.ServerBound.Login.EncryptionResponse:
                 if self.decryptor:
                     hr = self.decryptor.EncryptionResponse(p.SharedSecret, p.VerifyToken)
                     self.cipher = AESComplex(hr[0])
                     self.logger.info(f"Protocol encryption is set, but you provided a shared secret")
                     self.logger.info(f"Shared secret: {hr[0].hex()}")
-                    self.journal.set_enckey(hr[0])
+                    if self.leave_debug_journals:
+                        self.journal.set_enckey(hr[0])
                     return self.PROTOCOL.ServerBound.Login.EncryptionResponse(*hr[1:])
                 self.logger.warn(f"Minecraft client sent EncryptionResponse! That mean full symmetric encryption enabling, so we can't proceed with protocol analyzing. Just proxying!")
                 self.PASS_THROUGH = True
                 return
 
         # Call a handler if exists        
         return self.HANDLERS[t][1](p) if t in self.HANDLERS else None
```

## MCRP/mcwp.py

```diff
@@ -97,20 +97,20 @@
         ServerBoundFilterList = [find_ap_by_path(proto, "ServerBound.Play." + packet) for packet in conf["ServerBound"]] if "ServerBound" in conf else []
         ClientBoundFilterList = [i for i in ClientBoundFilterList if i is not None]
         ServerBoundFilterList = [i for i in ServerBoundFilterList if i is not None]
 
         logger.debug(f"Filtering mode: {conf['mode']}, filtered packets:")
 
         logger.debug(f"ClientBound [{len(ClientBoundFilterList)}]:")
-        for packet in ClientBoundFilterList:
-            logger.debug(f"    {packet}")
+        for fpacket in ClientBoundFilterList:
+            logger.debug(f"    {fpacket}")
 
         logger.debug(f"ServerBound [{len(ServerBoundFilterList)}]:")
-        for packet in ServerBoundFilterList:
-            logger.debug(f"    {packet}")
+        for fpacket in ServerBoundFilterList:
+            logger.debug(f"    {fpacket}")
 
         return cubelib.proto.ServerBound.Handshaking.Handshake(packet.ProtoVer, *addr_parser(args.u, 25565), packet.NextState)
 
     def log_clientbound(*args):
         logger.info(f'\u001b[96mClientBound   {" ".join([str(a) for a in args])}\u001b[0m')
 
     def log_serverbound(*args):
```

## MCRP/tcproxy.py

```diff
@@ -124,21 +124,22 @@
     def join(self):
 
         while 7:
             self._waiting_for_client()
             self.asyncaccept()
             self._new_client()
             self.Server = socket.socket(self.UpstreamAddr[0], 1)
-            self.Server.settimeout(1)
+            self.Server.settimeout(1.5)
             try:
                 self.Server.connect((self.UpstreamAddr[1], self.UpstreamAddr[2]))
             except Exception as e:
                 self._server_error(e)
                 self.Client.close()
                 continue
+            self.Server.settimeout(None)
             self._new_server()      
 
             CT = threading.Thread(target=self.client_listener, daemon=True)
             ST = threading.Thread(target=self.server_listener, daemon=True)
             CT.start() ; ST.start()
 
             while CT.is_alive() or ST.is_alive():
```

## Comparing `MCRP-0.1.8.dist-info/LICENSE` & `MCRP-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MCRP-0.1.8.dist-info/METADATA` & `MCRP-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCRP
-Version: 0.1.8
+Version: 0.1.9
 Summary: Minecraft MITM proxy with function of rewriting packets, written in pure Python 3
 Home-page: https://gitlab.com/seeklay/MCRP
 Author: seeklay
 Author-email: rudeboy@seeklay.icu
 License: GNU General Public License v3.0
 Download-URL: https://gitlab.com/seeklay/MCRP
 Platform: OS Independent
```

