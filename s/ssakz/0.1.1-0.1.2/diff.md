# Comparing `tmp/ssakz-0.1.1.tar.gz` & `tmp/ssakz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssakz-0.1.1.tar", last modified: Tue Jun 20 06:30:29 2023, max compression
+gzip compressed data, was "ssakz-0.1.2.tar", last modified: Wed Jun 21 05:20:21 2023, max compression
```

## Comparing `ssakz-0.1.1.tar` & `ssakz-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 max      (1000003) max       (1000)        0 2023-06-20 06:30:29.486944 ssakz-0.1.1/
--rw-r--r--   0 max      (1000003) max       (1000)     1078 2023-06-18 15:39:54.000000 ssakz-0.1.1/LICENSE
--rw-r--r--   0 max      (1000003) max       (1000)       35 2023-06-20 06:24:11.000000 ssakz-0.1.1/MANIFEST.in
--rw-r--r--   0 max      (1000003) max       (1000)     1362 2023-06-20 06:30:29.486944 ssakz-0.1.1/PKG-INFO
--rw-r--r--   0 max      (1000003) max       (1000)     1123 2023-06-20 06:30:03.000000 ssakz-0.1.1/README.rst
--rw-r--r--   0 max      (1000003) max       (1000)       38 2023-06-20 06:30:29.486944 ssakz-0.1.1/setup.cfg
--rw-r--r--   0 max      (1000003) max       (1000)      501 2023-06-20 06:30:24.000000 ssakz-0.1.1/setup.py
-drwxr-xr-x   0 max      (1000003) max       (1000)        0 2023-06-20 06:30:29.486944 ssakz-0.1.1/ssakz.egg-info/
--rw-r--r--   0 max      (1000003) max       (1000)     1362 2023-06-20 06:30:29.000000 ssakz-0.1.1/ssakz.egg-info/PKG-INFO
--rw-r--r--   0 max      (1000003) max       (1000)      220 2023-06-20 06:30:29.000000 ssakz-0.1.1/ssakz.egg-info/SOURCES.txt
--rw-r--r--   0 max      (1000003) max       (1000)        1 2023-06-20 06:30:29.000000 ssakz-0.1.1/ssakz.egg-info/dependency_links.txt
--rw-r--r--   0 max      (1000003) max       (1000)        1 2023-06-20 06:24:43.000000 ssakz-0.1.1/ssakz.egg-info/not-zip-safe
--rw-r--r--   0 max      (1000003) max       (1000)        6 2023-06-20 06:30:29.000000 ssakz-0.1.1/ssakz.egg-info/requires.txt
--rw-r--r--   0 max      (1000003) max       (1000)        6 2023-06-20 06:30:29.000000 ssakz-0.1.1/ssakz.egg-info/top_level.txt
--rw-r--r--   0 max      (1000003) max       (1000)     3819 2023-06-20 06:07:30.000000 ssakz-0.1.1/ssakz.py
+drwxr-xr-x   0 max      (1000003) max       (1000)        0 2023-06-21 05:20:21.518146 ssakz-0.1.2/
+-rw-r--r--   0 max      (1000003) max       (1000)     1078 2023-06-18 15:39:54.000000 ssakz-0.1.2/LICENSE
+-rw-r--r--   0 max      (1000003) max       (1000)       35 2023-06-20 06:24:11.000000 ssakz-0.1.2/MANIFEST.in
+-rw-r--r--   0 max      (1000003) max       (1000)     1362 2023-06-21 05:20:21.518146 ssakz-0.1.2/PKG-INFO
+-rw-r--r--   0 max      (1000003) max       (1000)     1123 2023-06-20 06:30:03.000000 ssakz-0.1.2/README.rst
+-rw-r--r--   0 max      (1000003) max       (1000)       38 2023-06-21 05:20:21.518146 ssakz-0.1.2/setup.cfg
+-rw-r--r--   0 max      (1000003) max       (1000)      501 2023-06-21 05:18:36.000000 ssakz-0.1.2/setup.py
+drwxr-xr-x   0 max      (1000003) max       (1000)        0 2023-06-21 05:20:21.518146 ssakz-0.1.2/ssakz.egg-info/
+-rw-r--r--   0 max      (1000003) max       (1000)     1362 2023-06-21 05:20:21.000000 ssakz-0.1.2/ssakz.egg-info/PKG-INFO
+-rw-r--r--   0 max      (1000003) max       (1000)      220 2023-06-21 05:20:21.000000 ssakz-0.1.2/ssakz.egg-info/SOURCES.txt
+-rw-r--r--   0 max      (1000003) max       (1000)        1 2023-06-21 05:20:21.000000 ssakz-0.1.2/ssakz.egg-info/dependency_links.txt
+-rw-r--r--   0 max      (1000003) max       (1000)        1 2023-06-21 05:20:21.000000 ssakz-0.1.2/ssakz.egg-info/not-zip-safe
+-rw-r--r--   0 max      (1000003) max       (1000)        6 2023-06-21 05:20:21.000000 ssakz-0.1.2/ssakz.egg-info/requires.txt
+-rw-r--r--   0 max      (1000003) max       (1000)        6 2023-06-21 05:20:21.000000 ssakz-0.1.2/ssakz.egg-info/top_level.txt
+-rw-r--r--   0 max      (1000003) max       (1000)     4286 2023-06-21 05:12:04.000000 ssakz-0.1.2/ssakz.py
```

### Comparing `ssakz-0.1.1/LICENSE` & `ssakz-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssakz-0.1.1/PKG-INFO` & `ssakz-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssakz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Client API for ssa.fai.kz
 Home-page: https://github.com/fai-kz/ssakz
 Author: FAI
 Author-email: ssakz@fai.kz
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `ssakz-0.1.1/README.rst` & `ssakz-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `ssakz-0.1.1/ssakz.egg-info/PKG-INFO` & `ssakz-0.1.2/ssakz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssakz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Client API for ssa.fai.kz
 Home-page: https://github.com/fai-kz/ssakz
 Author: FAI
 Author-email: ssakz@fai.kz
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `ssakz-0.1.1/ssakz.py` & `ssakz-0.1.2/ssakz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 import zmq
 import json
 
 SERVER_PUBLIC_KEY = b"82M+$O0^qkJRj8/nWi[cma-4916*miCcALuf2-&e"
 
+
+class ssaError(Exception):
+    pass
+
+
+def ssa_error(func):
+    def wrapper(self, *args, **kwargs):
+        try:
+            return func(self, *args, **kwargs)
+        except zmq.error.ZMQError:
+            raise ConnectionError("Failed to connect to SSA server")
+    return wrapper
+
+
 class Client(object):
     def __init__(self, api_key):
         self.client_public_key = api_key[:40].encode('ascii')
         self.client_secret_key = api_key[40:].encode('ascii')
-        self.server_public_key = SERVER_PUBLIC_KEY
         self.context = zmq.Context()
         self.socket = self.context.socket(zmq.REQ)
         self.socket.curve_secretkey = self.client_secret_key
         self.socket.curve_publickey = self.client_public_key
-        self.socket.curve_serverkey = self.server_public_key
-        self.socket.connect("tcp://ssa.fai.kz:5555")
+        self.socket.curve_serverkey = SERVER_PUBLIC_KEY
+        try:
+            self.socket.connect("tcp://ssa.fai.kz:5555")
+        except zmq.error.ZMQError:
+            raise ConnectionError("Cannot connect to SSA server")
 
     def __del__(self):
         self.socket.close()
         self.context.term()
 
+    @ssa_error
     def get_nme(self, rlow=None, rhigh=None, since=None, until=None, id=None, id2=None, name=None, name2=None):
         request = {
             "type": "nme",
             "filter": {
                 "rlow": rlow,
                 "rhigh": rhigh,
                 "since": since,
@@ -32,86 +49,93 @@
                 "name": name,
                 "name2": name2
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
     
+    @ssa_error
     def get_sw_solar(self, since, until=None, rate=None):
         request = {
             "type": "sw_solar",
             "filter": {
                 "since": since,
                 "until": until,
                 "rate": rate
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
 
+    @ssa_error
     def get_sw_neutrons(self, since, until=None, rate=None):
         request = {
             "type": "sw_neutrons",
             "filter": {
                 "since": since,
                 "until": until,
                 "rate": rate
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
 
+    @ssa_error
     def get_sw_geomag(self, since, until=None, rate=None):
         request = {
             "type": "sw_geomag",
             "filter": {
                 "since": since,
                 "until": until,
                 "rate": rate
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
 
+    @ssa_error
     def get_sw_geomag_x(self, since, until=None, rate=None):
         request = {
             "type": "sw_geomag_x",
             "filter": {
                 "since": since,
                 "until": until,
                 "rate": rate
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
 
+    @ssa_error
     def get_sw_geomag_y(self, since, until=None, rate=None):
         request = {
             "type": "sw_geomag_y",
             "filter": {
                 "since": since,
                 "until": until,
                 "rate": rate
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
 
+    @ssa_error
     def get_sw_geomag_z(self, since, until=None, rate=None):
         request = {
             "type": "sw_geomag_z",
             "filter": {
                 "since": since,
                 "until": until,
                 "rate": rate
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
 
+    @ssa_error
     def get_sw_k_index(self, since, until=None, rate=None):
         request = {
             "type": "sw_k_index",
             "filter": {
                 "since": since,
                 "until": until,
                 "rate": rate
```

