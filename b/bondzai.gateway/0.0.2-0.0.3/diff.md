# Comparing `tmp/bondzai.gateway-0.0.2.tar.gz` & `tmp/bondzai.gateway-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-0.0.2.tar", last modified: Wed Jun 21 10:30:57 2023, max compression
+gzip compressed data, was "bondzai.gateway-0.0.3.tar", last modified: Wed Jun 21 16:03:27 2023, max compression
```

## Comparing `bondzai.gateway-0.0.2.tar` & `bondzai.gateway-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:15.150751 bondzai.gateway-0.0.2/
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/NOTICE
--rwxrwxrwx   0 root         (0) root         (0)      596 2023-06-21 10:58:15.151752 bondzai.gateway-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      195 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:13.898514 bondzai.gateway-0.0.2/bondzai/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:14.047121 bondzai.gateway-0.0.2/bondzai/gateway/
--rwxrwxrwx   0 root         (0) root         (0)      775 2023-06-21 10:58:03.000000 bondzai.gateway-0.0.2/bondzai/gateway/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:14.287841 bondzai.gateway-0.0.2/bondzai/gateway/core/
--rwxrwxrwx   0 root         (0) root         (0)     8009 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/application.py
--rwxrwxrwx   0 root         (0) root         (0)      328 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/device.py
--rwxrwxrwx   0 root         (0) root         (0)      577 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/events.py
--rwxrwxrwx   0 root         (0) root         (0)      833 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/fsm.py
--rwxrwxrwx   0 root         (0) root         (0)     2127 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2590 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:14.589243 bondzai.gateway-0.0.2/bondzai/gateway/core/message/
--rwxrwxrwx   0 root         (0) root         (0)     5283 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/base.py
--rwxrwxrwx   0 root         (0) root         (0)     4968 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/command.py
--rwxrwxrwx   0 root         (0) root         (0)     6243 2023-06-21 10:58:03.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/enums.py
--rwxrwxrwx   0 root         (0) root         (0)     3942 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/event.py
--rwxrwxrwx   0 root         (0) root         (0)      337 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/payload.py
--rwxrwxrwx   0 root         (0) root         (0)     6376 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/process_dbm.py
--rwxrwxrwx   0 root         (0) root         (0)     7864 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/response.py
--rwxrwxrwx   0 root         (0) root         (0)      942 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/message/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     2276 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/observer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:14.744249 bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/
--rwxrwxrwx   0 root         (0) root         (0)     1768 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/client.py
--rwxrwxrwx   0 root         (0) root         (0)     2652 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/connector.py
--rwxrwxrwx   0 root         (0) root         (0)     1731 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/request.py
--rwxrwxrwx   0 root         (0) root         (0)      171 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:14.849221 bondzai.gateway-0.0.2/bondzai/gateway/device_connectors/
--rwxrwxrwx   0 root         (0) root         (0)      201 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/device_connectors/base.py
--rwxrwxrwx   0 root         (0) root         (0)     4426 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/device_connectors/serial.py
--rwxrwxrwx   0 root         (0) root         (0)     7630 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/device_connectors/socket_server.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:14.915109 bondzai.gateway-0.0.2/bondzai/gateway/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2280 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/bondzai/gateway/tests/test_observer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:58:15.126039 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      596 2023-06-21 10:58:13.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1353 2023-06-21 10:58:13.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:58:13.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-06-21 10:58:13.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-21 10:58:13.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-06-21 10:58:13.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-21 10:58:13.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:58:12.000000 bondzai.gateway-0.0.2/bondzai.gateway.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-21 10:56:50.000000 bondzai.gateway-0.0.2/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      903 2023-06-21 10:58:15.155811 bondzai.gateway-0.0.2/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.605552 bondzai.gateway-0.0.3/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-06-21 16:03:27.605851 bondzai.gateway-0.0.3/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      195 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.579145 bondzai.gateway-0.0.3/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.581435 bondzai.gateway-0.0.3/bondzai/gateway/
+-rw-r--r--   0 theo       (501) staff       (20)      775 2023-06-21 16:01:37.000000 bondzai.gateway-0.0.3/bondzai/gateway/__init__.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.585268 bondzai.gateway-0.0.3/bondzai/gateway/core/
+-rw-r--r--   0 theo       (501) staff       (20)     8002 2023-06-21 15:44:58.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/application.py
+-rw-r--r--   0 theo       (501) staff       (20)      328 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/device.py
+-rw-r--r--   0 theo       (501) staff       (20)      577 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/events.py
+-rw-r--r--   0 theo       (501) staff       (20)      833 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/fsm.py
+-rw-r--r--   0 theo       (501) staff       (20)     2127 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/logger.py
+-rw-r--r--   0 theo       (501) staff       (20)     2590 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/manager.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.593735 bondzai.gateway-0.0.3/bondzai/gateway/core/message/
+-rw-r--r--   0 theo       (501) staff       (20)     5283 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4968 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/command.py
+-rw-r--r--   0 theo       (501) staff       (20)     6243 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)     3942 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/event.py
+-rw-r--r--   0 theo       (501) staff       (20)      337 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/payload.py
+-rw-r--r--   0 theo       (501) staff       (20)     6376 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/process_dbm.py
+-rw-r--r--   0 theo       (501) staff       (20)     7864 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/response.py
+-rw-r--r--   0 theo       (501) staff       (20)      942 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/message/utils.py
+-rw-r--r--   0 theo       (501) staff       (20)     2276 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.596499 bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/
+-rw-r--r--   0 theo       (501) staff       (20)     1768 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/client.py
+-rw-r--r--   0 theo       (501) staff       (20)     2652 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/connector.py
+-rw-r--r--   0 theo       (501) staff       (20)     1731 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/request.py
+-rw-r--r--   0 theo       (501) staff       (20)      171 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.598456 bondzai.gateway-0.0.3/bondzai/gateway/device_connectors/
+-rw-r--r--   0 theo       (501) staff       (20)      201 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/device_connectors/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4426 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/device_connectors/serial.py
+-rw-r--r--   0 theo       (501) staff       (20)     7630 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/device_connectors/socket_server.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.599728 bondzai.gateway-0.0.3/bondzai/gateway/tests/
+-rw-r--r--   0 theo       (501) staff       (20)        0 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/tests/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2280 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/bondzai/gateway/tests/test_observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:03:27.604977 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1353 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)       57 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/entry_points.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)      117 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 16:03:27.000000 bondzai.gateway-0.0.3/bondzai.gateway.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.3/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      899 2023-06-21 16:03:27.607154 bondzai.gateway-0.0.3/setup.cfg
```

### Comparing `bondzai.gateway-0.0.2/NOTICE` & `bondzai.gateway-0.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/PKG-INFO` & `bondzai.gateway-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/__init__.py` & `bondzai.gateway-0.0.3/bondzai/gateway/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 from pathlib import Path
 
 from .core.application import Application, CONFIG_DEFAULT_PATH
 
 
 CMD_NAME = "bondzai.gateway"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 def run():
     parser = argparse.ArgumentParser(
         prog=CMD_NAME,
         description="Davinsy Gateway"
     )
```

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/application.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .websocket.client import WebsocketClient
 from .websocket.request import ACT_GET_DEVICES_LIST, ACT_SEND_TO_DEVICE, ACT_SUB_TO_DEVICE, ACT_UNSUB_FROM_DEVUCE, WebsocketRequest
 from .fsm import get_files
 
 from ..device_connectors.base import DeviceConnector
 
 
-CONFIG_DEFAULT_PATH: Path = Path(__file__).parent.parent.parent.parent / "config.yml"
+CONFIG_DEFAULT_PATH: Path = Path(__file__).parent.parent.parent / "config.yml"
 CONNECTORS_PATH: Path = Path(__file__).parent.parent / "device_connectors"
 
 
 class Application(object):
     def __init__(self, config_file_path: Path = CONFIG_DEFAULT_PATH) -> None:
         # Loading Configs
         self.config = {}
```

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/events.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/fsm.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/fsm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/logger.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/logger.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/manager.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/manager.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/message/base.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/message/base.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/message/command.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/message/command.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/message/enums.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/message/enums.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/message/event.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/message/event.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/message/process_dbm.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/message/process_dbm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/message/response.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/message/response.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/message/utils.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/message/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/observer.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/client.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/client.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/connector.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/connector.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/core/websocket/request.py` & `bondzai.gateway-0.0.3/bondzai/gateway/core/websocket/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/device_connectors/serial.py` & `bondzai.gateway-0.0.3/bondzai/gateway/device_connectors/serial.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/device_connectors/socket_server.py` & `bondzai.gateway-0.0.3/bondzai/gateway/device_connectors/socket_server.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai/gateway/tests/test_observer.py` & `bondzai.gateway-0.0.3/bondzai/gateway/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/bondzai.gateway.egg-info/PKG-INFO` & `bondzai.gateway-0.0.3/bondzai.gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.2/bondzai.gateway.egg-info/SOURCES.txt` & `bondzai.gateway-0.0.3/bondzai.gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.2/setup.cfg` & `bondzai.gateway-0.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 	pytest-mock==3.10.0
 	pytest-cov==3.0.0
 
 [options.packages.find]
 where = .
 
 [options.package_data]
-dexim = config.yml
+* = config.yml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

