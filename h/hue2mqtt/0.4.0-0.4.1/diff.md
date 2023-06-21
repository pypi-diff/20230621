# Comparing `tmp/hue2mqtt-0.4.0.tar.gz` & `tmp/hue2mqtt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hue2mqtt-0.4.0.tar", max compression
+gzip compressed data, was "hue2mqtt-0.4.1.tar", max compression
```

## Comparing `hue2mqtt-0.4.0.tar` & `hue2mqtt-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1071 2022-03-29 21:00:57.342048 hue2mqtt-0.4.0/LICENSE
--rw-r--r--   0        0        0     5838 2022-08-28 12:45:39.295725 hue2mqtt-0.4.0/README.md
--rw-r--r--   0        0        0      122 2022-08-28 12:45:56.176787 hue2mqtt-0.4.0/hue2mqtt/__init__.py
--rw-r--r--   0        0        0       85 2022-03-29 21:00:57.342487 hue2mqtt-0.4.0/hue2mqtt/__main__.py
--rw-r--r--   0        0        0      736 2022-03-29 21:00:57.342536 hue2mqtt-0.4.0/hue2mqtt/app.py
--rw-r--r--   0        0        0     2142 2022-08-28 12:27:24.684646 hue2mqtt-0.4.0/hue2mqtt/config.py
--rw-r--r--   0        0        0     1002 2022-03-29 21:00:57.342652 hue2mqtt-0.4.0/hue2mqtt/discovery.py
--rw-r--r--   0        0        0     8538 2022-08-28 12:45:39.296101 hue2mqtt-0.4.0/hue2mqtt/hue2mqtt.py
--rw-r--r--   0        0        0      348 2022-03-29 21:00:57.342784 hue2mqtt-0.4.0/hue2mqtt/messages.py
--rw-r--r--   0        0        0       88 2022-03-29 21:00:57.342863 hue2mqtt-0.4.0/hue2mqtt/mqtt/__init__.py
--rw-r--r--   0        0        0     2273 2022-03-29 21:00:57.342926 hue2mqtt-0.4.0/hue2mqtt/mqtt/topic.py
--rw-r--r--   0        0        0     5529 2022-03-29 21:00:57.342994 hue2mqtt-0.4.0/hue2mqtt/mqtt/wrapper.py
--rw-r--r--   0        0        0       94 2022-03-29 21:00:57.343044 hue2mqtt-0.4.0/hue2mqtt/py.typed
--rw-r--r--   0        0        0     3124 2022-08-28 12:11:43.783799 hue2mqtt-0.4.0/hue2mqtt/schema.py
--rw-r--r--   0        0        0     1112 2022-08-28 12:46:02.715206 hue2mqtt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6958 2022-08-28 12:46:28.930760 hue2mqtt-0.4.0/setup.py
--rw-r--r--   0        0        0     6875 2022-08-28 12:46:28.931114 hue2mqtt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-21 20:25:12.379481 hue2mqtt-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5894 2023-06-21 20:25:08.459253 hue2mqtt-0.4.1/README.md
+-rw-r--r--   0        0        0      122 2023-06-21 20:57:32.835040 hue2mqtt-0.4.1/hue2mqtt/__init__.py
+-rw-r--r--   0        0        0       85 2022-03-29 21:00:57.342487 hue2mqtt-0.4.1/hue2mqtt/__main__.py
+-rw-r--r--   0        0        0      736 2022-03-29 21:00:57.342536 hue2mqtt-0.4.1/hue2mqtt/app.py
+-rw-r--r--   0        0        0     2203 2023-06-21 20:33:33.229839 hue2mqtt-0.4.1/hue2mqtt/config.py
+-rw-r--r--   0        0        0     1027 2023-06-21 20:18:43.762219 hue2mqtt-0.4.1/hue2mqtt/discovery.py
+-rw-r--r--   0        0        0     8580 2023-06-21 20:26:32.586960 hue2mqtt-0.4.1/hue2mqtt/hue2mqtt.py
+-rw-r--r--   0        0        0      348 2022-03-29 21:00:57.342784 hue2mqtt-0.4.1/hue2mqtt/messages.py
+-rw-r--r--   0        0        0       88 2022-03-29 21:00:57.342863 hue2mqtt-0.4.1/hue2mqtt/mqtt/__init__.py
+-rw-r--r--   0        0        0     2271 2023-06-21 20:18:30.818836 hue2mqtt-0.4.1/hue2mqtt/mqtt/topic.py
+-rw-r--r--   0        0        0     5548 2023-06-21 19:21:22.831209 hue2mqtt-0.4.1/hue2mqtt/mqtt/wrapper.py
+-rw-r--r--   0        0        0       94 2022-03-29 21:00:57.343044 hue2mqtt-0.4.1/hue2mqtt/py.typed
+-rw-r--r--   0        0        0     3492 2023-06-21 20:18:09.732580 hue2mqtt-0.4.1/hue2mqtt/schema.py
+-rw-r--r--   0        0        0     2276 2023-06-21 20:57:24.576406 hue2mqtt-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6990 1970-01-01 00:00:00.000000 hue2mqtt-0.4.1/PKG-INFO
```

### Comparing `hue2mqtt-0.4.0/LICENSE` & `hue2mqtt-0.4.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-22 Dan Trickey
+Copyright (c) 2021-23 Dan Trickey
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hue2mqtt-0.4.0/README.md` & `hue2mqtt-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 Hue2MQTT is configured using `hue2mqtt.toml`.
 
 ```toml
 # Hue2MQTT Default Config File
 
 [mqtt]
+# use host.docker.internal to connect to mqtt broker installed on docker host
+# host = "host.docker.internal"
 host = "::1"
 port = 1883
 enable_tls = false
 force_protocol_version_3_1 = true
 
 enable_auth = false
 username = ""
@@ -122,13 +124,14 @@
 {"on": "true"}
 ```
 
 ## Docker
 
 Included is a basic Dockerfile and docker-compose example. 
 
-## Contributions
+### Connections to Docker Host
 
-This project is released under the MIT Licence. For more information, please see LICENSE.
-
-The CONTRIBUTORS file can be generated by executing CONTRIBUTORS.gen. This generated file contains a list of people who have contributed to Hue2MQTT.
+To establish a MQTT-Connection to the Docker Host (localhost is the docker instance) use host.docker.internal inside hue2mqtt.toml
 
+```toml
+host = "host.docker.internal"
+```
```

### Comparing `hue2mqtt-0.4.0/hue2mqtt/app.py` & `hue2mqtt-0.4.1/hue2mqtt/app.py`

 * *Files identical despite different names*

### Comparing `hue2mqtt-0.4.0/hue2mqtt/config.py` & `hue2mqtt-0.4.1/hue2mqtt/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 Configuration schema for Astoria.
 
 Common to all components.
 """
 from pathlib import Path
 from typing import IO, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, parse_obj_as
 
 # Backwards compatibility for TOML in stdlib from Python 3.11
 try:
-    import tomllib  # type: ignore[import]
+    import tomllib  # type: ignore[import,unused-ignore]
 except ModuleNotFoundError:
-    import tomli as tomllib  # type: ignore[no-redef]
+    import tomli as tomllib  # type: ignore[import,no-redef,unused-ignore]
 
 
 class HueBridgeInfo(BaseModel):
     """MQTT Broker Information."""
 
     ip: str
     username: str
@@ -55,32 +55,32 @@
         """Pydantic config."""
 
         extra = "forbid"
 
     @classmethod
     def _get_config_path(cls, config_str: Optional[str] = None) -> Path:
         """Check for a config file or search the filesystem for one."""
-        CONFIG_SEARCH_PATHS = [
+        config_search_paths = [
             Path("hue2mqtt.toml"),
             Path("/etc/hue2mqtt.toml"),
         ]
         if config_str is None:
-            for path in CONFIG_SEARCH_PATHS:
+            for path in config_search_paths:
                 if path.exists() and path.is_file():
                     return path
         else:
             path = Path(config_str)
             if path.exists() and path.is_file():
                 return path
         raise FileNotFoundError("Unable to find config file.")
 
     @classmethod
-    def load(cls, config_str: Optional[str] = None) -> 'Hue2MQTTConfig':
+    def load(cls, config_str: Optional[str] = None) -> "Hue2MQTTConfig":
         """Load the config."""
         config_path = cls._get_config_path(config_str)
         with config_path.open("rb") as fh:
             return cls.load_from_file(fh)
 
     @classmethod
-    def load_from_file(cls, fh: IO[bytes]) -> 'Hue2MQTTConfig':
+    def load_from_file(cls, fh: IO[bytes]) -> "Hue2MQTTConfig":
         """Load the config from a file."""
-        return cls(**tomllib.load(fh))
+        return parse_obj_as(cls, tomllib.load(fh))
```

### Comparing `hue2mqtt-0.4.0/hue2mqtt/discovery.py` & `hue2mqtt-0.4.1/hue2mqtt/discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,9 +21,11 @@
             bridge = bridges[0]
             print("Found bridge at", bridge.host)
             try:
                 await bridge.create_user("hue2mqtt")
                 print("Your username is", bridge.username)
                 print("Please add these details to hue2mqtt.toml")
             except LinkButtonNotPressed:
-                print("Error: Press the link button on the bridge before running discovery")  # noqa: E501
+                print(
+                    "Error: Press the link button on the bridge before running discovery",
+                )
                 sys.exit(1)
```

### Comparing `hue2mqtt-0.4.0/hue2mqtt/hue2mqtt.py` & `hue2mqtt-0.4.1/hue2mqtt/hue2mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import sys
 from signal import SIGHUP, SIGINT, SIGTERM
 from types import FrameType
 from typing import Match, Optional
 
 import aiohue
 from aiohttp.client import ClientSession
-from pydantic import ValidationError
+from pydantic import ValidationError, parse_obj_as
 
 from hue2mqtt import __version__
 from hue2mqtt.messages import BridgeInfo, Hue2MQTTStatus
 from hue2mqtt.schema import (
     GroupInfo,
     GroupSetState,
     LightInfo,
@@ -32,15 +32,15 @@
 from .mqtt.wrapper import MQTTWrapper
 
 LOGGER = logging.getLogger(__name__)
 
 loop = asyncio.get_event_loop()
 
 
-class Hue2MQTT():
+class Hue2MQTT:
     """Hue to MQTT Bridge."""
 
     config: Hue2MQTTConfig
 
     def __init__(
         self,
         verbose: bool,
@@ -161,15 +161,15 @@
         uniqueid = match.group(1)
 
         # Find the light with that uniqueid
         for light_id in self._bridge.lights:
             light = self._bridge.lights[light_id]
             if light.uniqueid == uniqueid:
                 try:
-                    state = LightSetState(**json.loads(payload))
+                    state = parse_obj_as(LightSetState, json.loads(payload))
                     LOGGER.info(f"Updating {light.name}")
                     await light.set_state(**state.dict())
                 except json.JSONDecodeError:
                     LOGGER.warning(f"Bad JSON on light request: {payload}")
                 except TypeError:
                     LOGGER.warning(f"Expected dictionary, got: {payload}")
                 except ValidationError as e:
@@ -179,42 +179,42 @@
 
     async def handle_set_group(self, match: Match[str], payload: str) -> None:
         """Handle an update to a group."""
         groupid = match.group(1)
 
         try:
             group = self._bridge.groups[groupid]
-            state = GroupSetState(**json.loads(payload))
+            state = parse_obj_as(GroupSetState, json.loads(payload))
             LOGGER.info(f"Updating group {group.name}")
             await group.set_action(**state.dict())
         except IndexError:
             LOGGER.warning(f"Unknown group id: {groupid}")
         except json.JSONDecodeError:
             LOGGER.warning(f"Bad JSON on light request: {payload}")
         except TypeError:
             LOGGER.warning(f"Expected dictionary, got: {payload}")
         except ValidationError as e:
             LOGGER.warning(f"Invalid light state: {e}")
 
     async def main(self, websession: ClientSession) -> None:
         """Main method of the data component."""
         # Publish initial info about lights
-        for id, light_raw in self._bridge.lights._items.items():
-            light = LightInfo(id=id, **light_raw.raw)
+        for idx, light_raw in self._bridge.lights._items.items():
+            light = LightInfo(id=idx, **light_raw.raw)
             self.publish_light(light)
 
         # Publish initial info about groups
-        for id, group_raw in self._bridge.groups._items.items():
-            group = GroupInfo(id=id, **group_raw.raw)
+        for idx, group_raw in self._bridge.groups._items.items():
+            group = GroupInfo(id=idx, **group_raw.raw)
             self.publish_group(group)
 
         # Publish initial info about sensors
-        for id, sensor_raw in self._bridge.sensors._items.items():
+        for idx, sensor_raw in self._bridge.sensors._items.items():
             if "uniqueid" in sensor_raw.raw and "productname" in sensor_raw.raw:
-                sensor = SensorInfo(id=id, **sensor_raw.raw)
+                sensor = SensorInfo(id=idx, **sensor_raw.raw)
                 self.publish_sensor(sensor)
             else:
                 LOGGER.debug(f"Ignoring virtual sensor: {sensor_raw.name}")
 
         # Publish updates
         try:
             async for updated_object in self._bridge.listen_events():
```

### Comparing `hue2mqtt-0.4.0/hue2mqtt/mqtt/topic.py` & `hue2mqtt-0.4.1/hue2mqtt/mqtt/topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.parts = parts
 
     def match(self, topic: str) -> Optional[Match[str]]:
         """Perform a regex match on a topic."""
         return self.regex.match(topic)
 
     @classmethod
-    def parse(cls, topic: str) -> 'Topic':
+    def parse(cls, topic: str) -> "Topic":
         """
         Parse a string topic into a Topic instance.
 
         It is assumed that the supplied topic complies with the MQTT spec.
         If not, then behaviour is undefined.
         """
         if len(topic) > 1:
@@ -44,15 +44,15 @@
 
         return cls(topic.split("/"))
 
     def __str__(self) -> str:
         return "/".join(str(p) for p in self.parts)
 
     def __repr__(self) -> str:
-        return f"Topic(\"{self}\")"
+        return f'Topic("{self}")'
 
     def __hash__(self) -> int:
         return hash(repr(self))
 
     def __eq__(self, other: object) -> bool:
         try:
             return self.parts == other.parts  # type: ignore
```

### Comparing `hue2mqtt-0.4.0/hue2mqtt/mqtt/wrapper.py` & `hue2mqtt-0.4.1/hue2mqtt/mqtt/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             topic_complete = Topic.parse(topic)
 
         if not topic_complete.is_publishable:
             raise ValueError(f"Cannot publish to MQTT topic: {topic_complete}")
 
         self._client.publish(
             str(topic_complete),
-            payload.json(by_alias=True),
+            payload.json(by_alias=True, exclude_none=True),
             qos=1,
             retain=retain,
         )
 
     def subscribe(
         self,
         topic: str,
```

### Comparing `hue2mqtt-0.4.0/hue2mqtt/schema.py` & `hue2mqtt-0.4.1/hue2mqtt/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Schemas for data about lights."""
-from datetime import datetime
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, create_model
 
 
 class LightBaseState(BaseModel):
     """The base attributes of a light state."""
 
     on: Optional[bool]
 
@@ -43,120 +42,123 @@
     color_mode: Optional[str]
     mode: Optional[str]
 
 
 class LightInfo(BaseModel):
     """Information about a light."""
 
-    id: int
+    id: int  # noqa: A003
     name: str
     uniqueid: str
     state: Optional[LightState]
 
     manufacturername: str
     modelid: str
     productname: str
-    type: str
+    type: str  # noqa: A003
 
     swversion: str
 
 
 class GroupState(BaseModel):
     """The state of lights in a group."""
 
     all_on: bool
     any_on: bool
 
 
 class GroupInfo(BaseModel):
     """Information about a light group."""
 
-    id: int
+    id: int  # noqa: A003
     name: str
     lights: List[int]
     sensors: List[int]
-    type: str
+    type: str  # noqa: A003
     state: GroupState
 
     group_class: Optional[str] = Field(default=None, alias="class")
 
     action: LightState
 
 
 class GenericSensorState(BaseModel):
     """Information about the state of a sensor."""
 
-    lastupdated: datetime
+    lastupdated: Optional[str] = None
 
 
 class PresenceSensorState(GenericSensorState):
     """Information about the state of a sensor."""
 
-    presence: bool
+    presence: Optional[bool] = None
 
 
 class RotarySensorState(GenericSensorState):
     """Information about the state of a sensor."""
 
-    rotaryevent: str
-    expectedrotation: str
-    expectedeventduration: str
+    rotaryevent: Optional[str] = None
+    expectedrotation: Optional[str] = None
+    expectedeventduration: Optional[str] = None
 
 
 class SwitchSensorState(GenericSensorState):
     """Information about the state of a sensor."""
 
-    buttonevent: Optional[int]
+    buttonevent: Optional[int] = None
 
 
 class LightLevelSensorState(GenericSensorState):
     """Information about the state of a sensor."""
 
-    dark: bool
-    daylight: bool
-    lightlevel: int
+    dark: Optional[bool] = None
+    daylight: Optional[bool] = None
+    lightlevel: Optional[int] = None
 
 
 class TemperatureSensorState(GenericSensorState):
     """Information about the state of a sensor."""
 
-    temperature: int
+    temperature: Optional[int] = None
 
 
 class HumiditySensorState(GenericSensorState):
     """Information about the state of a sensor."""
 
-    humidity: int
+    humidity: Optional[int] = None
 
 
 class OpenCloseSensorState(GenericSensorState):
     """Information about the state of a sensor."""
 
-    open: str
+    open: Optional[str] = None  # noqa: A003
 
 
-SensorState = Union[
-    PresenceSensorState,
-    RotarySensorState,
-    SwitchSensorState,
-    LightLevelSensorState,
-    TemperatureSensorState,
-    HumiditySensorState,
-    OpenCloseSensorState,
-]
+SensorState = create_model(
+    "SensorState",
+    __base__=(
+        LightLevelSensorState,
+        PresenceSensorState,
+        RotarySensorState,
+        SwitchSensorState,
+        TemperatureSensorState,
+        HumiditySensorState,
+        OpenCloseSensorState,
+    ),
+)
 
 
 class SensorInfo(BaseModel):
     """Information about a sensor."""
 
-    id: int
+    id: int  # noqa: A003
     name: str
-    type: str
+    type: str  # noqa: A003
     modelid: str
     manufacturername: str
 
     productname: str
     uniqueid: str
     swversion: Optional[str]
 
-    state: SensorState
+    state: SensorState  # type: ignore[valid-type]
     capabilities: Any
```

### Comparing `hue2mqtt-0.4.0/setup.py` & `hue2mqtt-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,165 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hue2mqtt
+Version: 0.4.1
+Summary: Python Hue to MQTT Bridge
+Home-page: https://github.com/trickeydan/hue2mqtt-python
+License: MIT
+Author: Dan Trickey
+Author-email: contact@trickey.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: aiohue (>=2.5.1,<3.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: gmqtt (>=0.6.10,<0.7.0)
+Requires-Dist: pydantic (>=1.9.2,<2.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_full_version <= "3.10.0"
+Project-URL: Documentation, https://github.com/trickeydan/hue2mqtt-python
+Project-URL: Repository, https://github.com/trickeydan/hue2mqtt-python
+Description-Content-Type: text/markdown
 
-packages = \
-['hue2mqtt', 'hue2mqtt.mqtt']
+# Hue2MQTT
 
-package_data = \
-{'': ['*']}
+Python Hue to MQTT Bridge
 
-install_requires = \
-['aiohttp>=3.8.1,<4.0.0',
- 'aiohue>=2.5.1,<3.0.0',
- 'click>=8.1.3,<9.0.0',
- 'gmqtt>=0.6.10,<0.7.0',
- 'pydantic>=1.9.2,<2.0.0']
-
-extras_require = \
-{':python_version <= "3.10"': ['tomli>=2.0.1,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['hue2mqtt = hue2mqtt.app:app']}
-
-setup_kwargs = {
-    'name': 'hue2mqtt',
-    'version': '0.4.0',
-    'description': 'Python Hue to MQTT Bridge',
-    'long_description': '# Hue2MQTT\n\nPython Hue to MQTT Bridge\n\n## What and Why?\n\nHue2MQTT lets you control your Hue setup using MQTT and publishes the current state in real-time.\n\n- Python 3.8+ with type hints and asyncio\n- Uses the excellent [aiohue](https://github.com/home-assistant-libs/aiohue) library to communicate with Hue.\n- Control your lights using MQTT\n- Receive live events (i.e button pushes, motion sensors) in real-time.\n- No polling your Hue Bridge for changes\n- IPv6 Support\n\n## Configuration\n\nHue2MQTT is configured using `hue2mqtt.toml`.\n\n```toml\n# Hue2MQTT Default Config File\n\n[mqtt]\nhost = "::1"\nport = 1883\nenable_tls = false\nforce_protocol_version_3_1 = true\n\nenable_auth = false\nusername = ""\npassword = ""\n\ntopic_prefix = "hue2mqtt"\n\n[hue]\nip = "192.0.2.2"  # or IPv6: "[2001:db0::1]"\nusername = "some secret here"\n```\n\nIf you do not know the username for your bridge, find it using `hue2mqtt --discover`.\n\n## Running Hue2MQTT\n\nUsually, it is as simple as running `hue2mqtt`.\n\n```\nUsage: hue2mqtt [OPTIONS]\n\n  Main function for Hue2MQTT.\n\nOptions:\n  -v, --verbose\n  -c, --config-file PATH\n  --discover\n  --help                  Show this message and exit.\n```\n\n## Bridge Status\n\nThe status of Hue2MQTT is published to `hue2mqtt/status` as a JSON object:\n\n```json\n{"online": true, "bridge": {"name": "Philips Hue", "mac_address": "ec:b5:fa:ab:cd:ef", "api_version": "1.45.0"}}\n```\n\nIf `online` is `false`, then all other information published by the bridge should be assumed to be inaccurate.\n\nThe `bridge` object contains information about the Hue Bridge, if available.\n\n## Getting information about Hue\n\nInformation about the state of Hue is published to MQTT as retained messages. Messages are re-published when the state changes.\n\n### Lights\n\nInformation about lights is published to `hue2mqtt/light/{{UNIQUEID}}` where `UNIQUEID` is the Zigbee MAC of the light.\n\ne.g `hue2mqtt/light/00:17:88:01:ab:cd:ef:01-02`\n\n```json\n{"id": 1, "name": "Lounge Lamp", "uniqueid": "00:17:88:01:ab:cd:ef:01-02", "state": {"on": false, "alert": "none", "bri": 153, "ct": 497, "effect": "none", "hue": 7170, "sat": 225, "xy": [0, 0], "transitiontime": null, "reachable": true, "color_mode": null, "mode": "homeautomation"}, "manufacturername": "Signify Netherlands B.V.", "modelid": "LCT012", "productname": "Hue color candle", "type": "Extended color light", "swversion": "1.50.2_r30933"}\n\n```\n\n### Groups\n\nA group represents a group of lights, referred to as Rooms and Zones in the Hue app.\n\nInformation about lights is published to `hue2mqtt/group/{{GROUPID}}` where `GROUPID` is an integer.\n\n```json\nhue2mqtt/group/3 {"id": 3, "name": "Lounge", "lights": [24, 21, 20, 3, 5], "sensors": [], "type": "Room", "state": {"all_on": false, "any_on": false}, "group_class": "Living room", "action": {"on": false, "alert": "none", "bri": 153, "ct": 497, "effect": "none", "hue": 7170, "sat": 225, "xy": [0, 0], "transitiontime": null, "reachable": null, "color_mode": null, "mode": null}}\n```\n\n### Sensors\n\nSensors represent other objects in the Hue ecosystem, such as switches and motion sensors. There are also a number of "virtual" sensors that the Hue Hub uses to represent calculated values (e.g `daylight`), but these are ignored by Hue2MQTT.\n\nInformation about sensors is published to `hue2mqtt/sensor/{{UNIQUEID}}` where `UNIQUEID` is the Zigbee MAC of the device.\n\ne.g `hue2mqtt/sensor/00:17:88:01:ab:cd:ef:01-02`\n\n**Switch**\n\n```json\n{"id": 10, "name": "Lounge switch", "type": "ZLLSwitch", "modelid": "RWL021", "manufacturername": "Signify Netherlands B.V.", "productname": "Hue dimmer switch", "uniqueid": "00:17:88:01:ab:cd:ef:01-02", "swversion": "6.1.1.28573", "state": {"lastupdated": "2021-07-10T11:37:58", "buttonevent": 4002}, "capabilities": {"certified": true, "primary": true, "inputs": [{"repeatintervals": [800], "events": [{"buttonevent": 1000, "eventtype": "initial_press"}, {"buttonevent": 1001, "eventtype": "repeat"}, {"buttonevent": 1002, "eventtype": "short_release"}, {"buttonevent": 1003, "eventtype": "long_release"}]}, {"repeatintervals": [800], "events": [{"buttonevent": 2000, "eventtype": "initial_press"}, {"buttonevent": 2001, "eventtype": "repeat"}, {"buttonevent": 2002, "eventtype": "short_release"}, {"buttonevent": 2003, "eventtype": "long_release"}]}, {"repeatintervals": [800], "events": [{"buttonevent": 3000, "eventtype": "initial_press"}, {"buttonevent": 3001, "eventtype": "repeat"}, {"buttonevent": 3002, "eventtype": "short_release"}, {"buttonevent": 3003, "eventtype": "long_release"}]}, {"repeatintervals": [800], "events": [{"buttonevent": 4000, "eventtype": "initial_press"}, {"buttonevent": 4001, "eventtype": "repeat"}, {"buttonevent": 4002, "eventtype": "short_release"}, {"buttonevent": 4003, "eventtype": "long_release"}]}]}}\n```\n\n**Light Sensor**\n\n```json\n{"id": 5, "name": "Hue ambient light sensor 1", "type": "ZLLLightLevel", "modelid": "SML001", "manufacturername": "Signify Netherlands B.V.", "productname": "Hue ambient light sensor", "uniqueid": "00:17:88:01:04:b7:b5:20-02-0400", "swversion": "6.1.1.27575", "state": {"lastupdated": "2021-07-10T12:28:17", "dark": true, "daylight": false, "lightlevel": 14606}, "capabilities": {"certified": true, "primary": false}}\n```\n\n## Controlling Hue\n\nLights and Groups can be controlled by publishing objects to the `hue2mqtt/light/{{UNIQUEID}}/set` or `hue2mqtt/group/{{GROUPID}}/set` topics.\n\nThe object should be a JSON object containing the state values that you wish to change.\n\n```json\n{"on": "true"}\n```\n\n## Docker\n\nIncluded is a basic Dockerfile and docker-compose example. \n\n## Contributions\n\nThis project is released under the MIT Licence. For more information, please see LICENSE.\n\nThe CONTRIBUTORS file can be generated by executing CONTRIBUTORS.gen. This generated file contains a list of people who have contributed to Hue2MQTT.\n\n',
-    'author': 'Dan Trickey',
-    'author_email': 'contact@trickey.io',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/trickeydan/hue2mqtt-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## What and Why?
 
+Hue2MQTT lets you control your Hue setup using MQTT and publishes the current state in real-time.
+
+- Python 3.8+ with type hints and asyncio
+- Uses the excellent [aiohue](https://github.com/home-assistant-libs/aiohue) library to communicate with Hue.
+- Control your lights using MQTT
+- Receive live events (i.e button pushes, motion sensors) in real-time.
+- No polling your Hue Bridge for changes
+- IPv6 Support
+
+## Configuration
+
+Hue2MQTT is configured using `hue2mqtt.toml`.
+
+```toml
+# Hue2MQTT Default Config File
+
+[mqtt]
+# use host.docker.internal to connect to mqtt broker installed on docker host
+# host = "host.docker.internal"
+host = "::1"
+port = 1883
+enable_tls = false
+force_protocol_version_3_1 = true
+
+enable_auth = false
+username = ""
+password = ""
+
+topic_prefix = "hue2mqtt"
+
+[hue]
+ip = "192.0.2.2"  # or IPv6: "[2001:db0::1]"
+username = "some secret here"
+```
+
+If you do not know the username for your bridge, find it using `hue2mqtt --discover`.
+
+## Running Hue2MQTT
+
+Usually, it is as simple as running `hue2mqtt`.
+
+```
+Usage: hue2mqtt [OPTIONS]
+
+  Main function for Hue2MQTT.
+
+Options:
+  -v, --verbose
+  -c, --config-file PATH
+  --discover
+  --help                  Show this message and exit.
+```
+
+## Bridge Status
+
+The status of Hue2MQTT is published to `hue2mqtt/status` as a JSON object:
+
+```json
+{"online": true, "bridge": {"name": "Philips Hue", "mac_address": "ec:b5:fa:ab:cd:ef", "api_version": "1.45.0"}}
+```
+
+If `online` is `false`, then all other information published by the bridge should be assumed to be inaccurate.
+
+The `bridge` object contains information about the Hue Bridge, if available.
+
+## Getting information about Hue
+
+Information about the state of Hue is published to MQTT as retained messages. Messages are re-published when the state changes.
+
+### Lights
+
+Information about lights is published to `hue2mqtt/light/{{UNIQUEID}}` where `UNIQUEID` is the Zigbee MAC of the light.
+
+e.g `hue2mqtt/light/00:17:88:01:ab:cd:ef:01-02`
+
+```json
+{"id": 1, "name": "Lounge Lamp", "uniqueid": "00:17:88:01:ab:cd:ef:01-02", "state": {"on": false, "alert": "none", "bri": 153, "ct": 497, "effect": "none", "hue": 7170, "sat": 225, "xy": [0, 0], "transitiontime": null, "reachable": true, "color_mode": null, "mode": "homeautomation"}, "manufacturername": "Signify Netherlands B.V.", "modelid": "LCT012", "productname": "Hue color candle", "type": "Extended color light", "swversion": "1.50.2_r30933"}
+
+```
+
+### Groups
+
+A group represents a group of lights, referred to as Rooms and Zones in the Hue app.
+
+Information about lights is published to `hue2mqtt/group/{{GROUPID}}` where `GROUPID` is an integer.
+
+```json
+hue2mqtt/group/3 {"id": 3, "name": "Lounge", "lights": [24, 21, 20, 3, 5], "sensors": [], "type": "Room", "state": {"all_on": false, "any_on": false}, "group_class": "Living room", "action": {"on": false, "alert": "none", "bri": 153, "ct": 497, "effect": "none", "hue": 7170, "sat": 225, "xy": [0, 0], "transitiontime": null, "reachable": null, "color_mode": null, "mode": null}}
+```
+
+### Sensors
+
+Sensors represent other objects in the Hue ecosystem, such as switches and motion sensors. There are also a number of "virtual" sensors that the Hue Hub uses to represent calculated values (e.g `daylight`), but these are ignored by Hue2MQTT.
+
+Information about sensors is published to `hue2mqtt/sensor/{{UNIQUEID}}` where `UNIQUEID` is the Zigbee MAC of the device.
+
+e.g `hue2mqtt/sensor/00:17:88:01:ab:cd:ef:01-02`
+
+**Switch**
+
+```json
+{"id": 10, "name": "Lounge switch", "type": "ZLLSwitch", "modelid": "RWL021", "manufacturername": "Signify Netherlands B.V.", "productname": "Hue dimmer switch", "uniqueid": "00:17:88:01:ab:cd:ef:01-02", "swversion": "6.1.1.28573", "state": {"lastupdated": "2021-07-10T11:37:58", "buttonevent": 4002}, "capabilities": {"certified": true, "primary": true, "inputs": [{"repeatintervals": [800], "events": [{"buttonevent": 1000, "eventtype": "initial_press"}, {"buttonevent": 1001, "eventtype": "repeat"}, {"buttonevent": 1002, "eventtype": "short_release"}, {"buttonevent": 1003, "eventtype": "long_release"}]}, {"repeatintervals": [800], "events": [{"buttonevent": 2000, "eventtype": "initial_press"}, {"buttonevent": 2001, "eventtype": "repeat"}, {"buttonevent": 2002, "eventtype": "short_release"}, {"buttonevent": 2003, "eventtype": "long_release"}]}, {"repeatintervals": [800], "events": [{"buttonevent": 3000, "eventtype": "initial_press"}, {"buttonevent": 3001, "eventtype": "repeat"}, {"buttonevent": 3002, "eventtype": "short_release"}, {"buttonevent": 3003, "eventtype": "long_release"}]}, {"repeatintervals": [800], "events": [{"buttonevent": 4000, "eventtype": "initial_press"}, {"buttonevent": 4001, "eventtype": "repeat"}, {"buttonevent": 4002, "eventtype": "short_release"}, {"buttonevent": 4003, "eventtype": "long_release"}]}]}}
+```
+
+**Light Sensor**
+
+```json
+{"id": 5, "name": "Hue ambient light sensor 1", "type": "ZLLLightLevel", "modelid": "SML001", "manufacturername": "Signify Netherlands B.V.", "productname": "Hue ambient light sensor", "uniqueid": "00:17:88:01:04:b7:b5:20-02-0400", "swversion": "6.1.1.27575", "state": {"lastupdated": "2021-07-10T12:28:17", "dark": true, "daylight": false, "lightlevel": 14606}, "capabilities": {"certified": true, "primary": false}}
+```
+
+## Controlling Hue
+
+Lights and Groups can be controlled by publishing objects to the `hue2mqtt/light/{{UNIQUEID}}/set` or `hue2mqtt/group/{{GROUPID}}/set` topics.
+
+The object should be a JSON object containing the state values that you wish to change.
+
+```json
+{"on": "true"}
+```
+
+## Docker
+
+Included is a basic Dockerfile and docker-compose example. 
+
+### Connections to Docker Host
+
+To establish a MQTT-Connection to the Docker Host (localhost is the docker instance) use host.docker.internal inside hue2mqtt.toml
+
+```toml
+host = "host.docker.internal"
+```
 
-setup(**setup_kwargs)
```

