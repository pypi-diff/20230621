# Comparing `tmp/ovos-phal-plugin-connectivity-events-0.0.3a2.tar.gz` & `tmp/ovos-phal-plugin-connectivity-events-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.3a2.tar", last modified: Tue Jun 20 15:54:44 2023, max compression
+gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.3a3.tar", last modified: Wed Jun 21 15:46:16 2023, max compression
```

## Comparing `ovos-phal-plugin-connectivity-events-0.0.3a2.tar` & `ovos-phal-plugin-connectivity-events-0.0.3a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-20 15:54:35.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 15:54:39.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-20 15:54:35.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-20 15:54:35.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/test/test_connectivity_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-21 15:46:07.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 15:46:10.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 15:46:16.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-21 15:46:07.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-21 15:46:07.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/test/test_connectivity_events.py
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a2/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: # ovos-PHAL-plugin - Connectivity Events
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/__init__.py` & `ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from enum import IntEnum
 from threading import Event
 
 from ovos_bus_client.message import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.log import LOG
 from ovos_utils.network_utils import is_connected_dns, is_connected_http
+from ovos_utils import classproperty
+from ovos_utils.process_utils import RuntimeRequirements
 
 
 class ConnectivityState(IntEnum):
     """ State of network/internet connectivity.
 
     See also:
     https://developer-old.gnome.org/NetworkManager/stable/nm-dbus-types.html
@@ -38,14 +40,23 @@
         super().__init__(bus=bus, name="ovos-PHAL-plugin-connectivity-events",
                          config=config)
         self.sleep_time = self.config.get("check_interval") or 60
         self.stopping = Event()
         self.state = ConnectivityState.UNKNOWN
         self.bus.on("ovos.PHAL.internet_check", self.handle_check)
 
+    @classproperty
+    def runtime_requirements(self):
+        return RuntimeRequirements(internet_before_load=False,
+                                   network_before_load=False,
+                                   requires_internet=False,
+                                   requires_network=False,
+                                   no_internet_fallback=True,
+                                   no_network_fallback=True)
+
     def run(self):
         if self.config.get("disable_scheduled_checks"):
             LOG.info("Scheduled Checks are disabled")
             return
         message = Message("ovos.PHAL.internet_check")
         self.handle_check(message)
         while not self.stopping.wait(self.sleep_time):
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: # ovos-PHAL-plugin - Connectivity Events
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt` & `ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a2/setup.py` & `ovos-phal-plugin-connectivity-events-0.0.3a3/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a2/test/test_connectivity_events.py` & `ovos-phal-plugin-connectivity-events-0.0.3a3/test/test_connectivity_events.py`

 * *Files identical despite different names*

