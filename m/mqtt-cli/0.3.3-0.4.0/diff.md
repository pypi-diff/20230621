# Comparing `tmp/mqtt-cli-0.3.3.tar.gz` & `tmp/mqtt-cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-cli-0.3.3.tar", last modified: Fri Jun 16 12:37:01 2023, max compression
+gzip compressed data, was "mqtt-cli-0.4.0.tar", last modified: Wed Jun 21 20:54:22 2023, max compression
```

## Comparing `mqtt-cli-0.3.3.tar` & `mqtt-cli-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:37:01.727618 mqtt-cli-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-16 12:36:41.000000 mqtt-cli-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 12:37:01.727618 mqtt-cli-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-16 12:36:41.000000 mqtt-cli-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 12:37:01.723618 mqtt-cli-0.3.3/mqtt_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-16 12:37:01.000000 mqtt-cli-0.3.3/mqtt_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-16 12:37:01.000000 mqtt-cli-0.3.3/mqtt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 12:37:01.000000 mqtt-cli-0.3.3/mqtt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-16 12:37:01.000000 mqtt-cli-0.3.3/mqtt_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 12:37:01.000000 mqtt-cli-0.3.3/mqtt_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-16 12:37:01.000000 mqtt-cli-0.3.3/mqtt_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7777 2023-06-16 12:36:41.000000 mqtt-cli-0.3.3/mqtt_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 12:37:01.727618 mqtt-cli-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-16 12:36:41.000000 mqtt-cli-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 20:54:22.420711 mqtt-cli-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-21 20:54:04.000000 mqtt-cli-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-21 20:54:22.420711 mqtt-cli-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-21 20:54:04.000000 mqtt-cli-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 20:54:22.420711 mqtt-cli-0.4.0/mqtt_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-21 20:54:22.000000 mqtt-cli-0.4.0/mqtt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-21 20:54:22.000000 mqtt-cli-0.4.0/mqtt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 20:54:22.000000 mqtt-cli-0.4.0/mqtt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-21 20:54:22.000000 mqtt-cli-0.4.0/mqtt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-21 20:54:22.000000 mqtt-cli-0.4.0/mqtt_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-21 20:54:22.000000 mqtt-cli-0.4.0/mqtt_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-21 20:54:04.000000 mqtt-cli-0.4.0/mqtt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 20:54:22.420711 mqtt-cli-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-21 20:54:04.000000 mqtt-cli-0.4.0/setup.py
```

### Comparing `mqtt-cli-0.3.3/LICENSE` & `mqtt-cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt-cli-0.3.3/PKG-INFO` & `mqtt-cli-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-cli
-Version: 0.3.3
+Version: 0.4.0
 Summary: CLI for Paho MQTT
 Home-page: https://github.com/MO-RISE/mqtt-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
```

### Comparing `mqtt-cli-0.3.3/mqtt_cli.egg-info/PKG-INFO` & `mqtt-cli-0.4.0/mqtt_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-cli
-Version: 0.3.3
+Version: 0.4.0
 Summary: CLI for Paho MQTT
 Home-page: https://github.com/MO-RISE/mqtt-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
```

### Comparing `mqtt-cli-0.3.3/mqtt_cli.py` & `mqtt-cli-0.4.0/mqtt_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Main entrypoint for this application"""
 import sys
 import time
+import json
 import atexit
 import logging
 import warnings
 import argparse
 from pathlib import Path
 from threading import Thread
 
@@ -16,15 +17,14 @@
 
 
 def connect(mq: Client, args: argparse.Namespace):
     @mq.disconnect_callback()
     def _(
         client, userdata, flags, reason_code, props=None
     ):  # pylint: disable=unused-argument
-        """Subscribe on connect"""
         if reason_code != 0:
             logger.error(
                 "Disconnected from %s with reason code: %s", client, reason_code
             )
 
     if args.transport == "websockets":
         mq.ws_set_options(path=args.path)
@@ -54,14 +54,21 @@
             parser.error("A topic and a message must be specified on the command line.")
         if args.queue:
             parser.error("--queue may only be used together with --line")
 
     if args.queue and args.qos > 0:
         parser.error("--queue is only suitable for use together with qos=0")
 
+    @mq.connect_callback()
+    def _(client, userdata, flags, reason_code, properties):
+        if reason_code != 0:
+            logger.error(
+                "Connection failed to %s with reason code: %s", client, reason_code
+            )
+
     # Connect and start loop
     connect(mq, args)
     mq.loop_start()
 
     # Dont start publishing until we are actually connected
     logger.debug("Waiting for client to connect...")
     while not mq.is_connected():
@@ -146,14 +153,21 @@
 
         try:
             payload = message.payload.decode()
         except UnicodeDecodeError:
             logger.exception(f"Could not decode payload: {message.payload}")
             return
 
+        if args.json:
+            try:
+                payload = json.dumps(json.loads(payload))
+            except json.JSONDecodeError:
+                logger.exception(f"Could not decode payload as JSON: {payload}")
+                return
+
         sys.stdout.write(f"{args.line.format(topic=topic, message=payload)}\n")
         sys.stdout.flush()
 
     connect(mq, args)
     mq.loop_forever()
 
 
@@ -170,15 +184,15 @@
     parser.add_argument("--user", type=str, default=None)
     parser.add_argument("--password", type=str, default=None)
     parser.add_argument(
         "--protocol", type=int, choices=[MQTTv31, MQTTv311, MQTTv5], default=MQTTv5
     )
     parser.add_argument("--path", type=str, default="/mqtt")
     parser.add_argument("--tls", action="store_true", default=False)
-    parser.add_argument("--clean-start", action="store_true", default=False)
+    parser.add_argument("--clean-start", action="store_true", default=True)
     parser.add_argument("--log-level", type=int, default=logging.WARNING)
 
     ## Subcommands
     subparsers = parser.add_subparsers(required=True)
 
     ## Common parser for all subcommands
     common_parser = argparse.ArgumentParser(add_help=False)
@@ -196,14 +210,15 @@
 
     ## Subscribe subcommand
     subscribe_parser = subparsers.add_parser("subscribe", parents=[common_parser])
     subscribe_parser.add_argument(
         "-t", "--topic", type=str, action="append", required=True
     )
     subscribe_parser.add_argument("--line", type=str, default="{message}")
+    subscribe_parser.add_argument("--json", action="store_true", default=False)
     subscribe_parser.set_defaults(func=subscribe)
 
     ## Parse arguments and start doing our thing
     args = parser.parse_args()
 
     # Setup logger
     logging.basicConfig(
```

### Comparing `mqtt-cli-0.3.3/setup.py` & `mqtt-cli-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="mqtt-cli",
-    version="0.3.3",
+    version="0.4.0",
     license="Apache License 2.0",
     description="CLI for Paho MQTT",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/MO-RISE/mqtt-cli",
     author="Fredrik Olsson",
     author_email="fredrik.x.olsson@ri.se",
```

