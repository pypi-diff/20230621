# Comparing `tmp/ovos-PHAL-plugin-system-0.0.4a4.tar.gz` & `tmp/ovos-PHAL-plugin-system-0.0.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a4.tar", last modified: Wed Jun 14 01:44:11 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a5.tar", last modified: Wed Jun 21 16:16:05 2023, max compression
```

## Comparing `ovos-PHAL-plugin-system-0.0.4a4.tar` & `ovos-PHAL-plugin-system-0.0.4a5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:11.991934 ovos-PHAL-plugin-system-0.0.4a4/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 01:44:11.991934 ovos-PHAL-plugin-system-0.0.4a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:11.991934 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:11.991934 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Reboot.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Restart.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Shutdown.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Status.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:11.991934 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/animations/loading.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/animations/status-fail.json
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/animations/status-success.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:44:05.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:11.991934 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 01:44:11.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 01:44:11.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:44:11.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-14 01:44:11.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 01:44:11.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 01:44:11.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:44:11.000000 ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:44:11.991934 ovos-PHAL-plugin-system-0.0.4a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-06-14 01:44:02.000000 ovos-PHAL-plugin-system-0.0.4a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.855097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Reboot.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Restart.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Shutdown.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Status.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/loading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-fail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:15:59.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/setup.py
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a4
+Version: 0.0.4a5
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/__init__.py` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 from json_database import JsonStorageXDG, JsonDatabaseXDG
 from ovos_bus_client.message import Message
 from ovos_backend_client.identity import IdentityManager
 from ovos_config.config import update_mycroft_config
 from ovos_config.locale import set_default_lang
 from ovos_config.locations import OLD_USER_CONFIG, USER_CONFIG, WEB_CONFIG_CACHE
 from ovos_config.meta import get_xdg_base
+
 from ovos_plugin_manager.phal import PHALPlugin
+from ovos_utils import classproperty
 from ovos_utils.gui import GUIInterface
-from ovos_utils.system import system_shutdown, system_reboot, ssh_enable,\
+from ovos_utils.process_utils import RuntimeRequirements
+from ovos_utils.system import system_reboot, ssh_enable,\
     ssh_disable, ntp_sync, restart_service, is_process_running, \
     check_service_active
 from ovos_utils.xdg_utils import xdg_state_home, xdg_cache_home, xdg_data_home
 from ovos_utils.log import LOG
 
 
 class SystemEventsValidator:
@@ -54,14 +57,23 @@
         self.use_root = config.get("sudo", True)
 
         self.factory_reset_plugs = []
 
         # trigger register events from phal plugins
         self.bus.emit(Message("system.factory.reset.ping"))
 
+    @classproperty
+    def runtime_requirements(self):
+        return RuntimeRequirements(internet_before_load=False,
+                                   network_before_load=False,
+                                   requires_internet=False,
+                                   requires_network=False,
+                                   no_internet_fallback=True,
+                                   no_network_fallback=True)
+
     @property
     def use_external_factory_reset(self):
         # see if PHAL service / mycroft.conf requested external handling
         external_requested = self.config.get("use_external_factory_reset")
         # auto detect ovos-shell if no explicit preference
         if external_requested is None and is_process_running("ovos-shell"):
             return True
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Reboot.qml` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Reboot.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Restart.qml` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Restart.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Shutdown.qml` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Shutdown.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/Status.qml` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/animations/loading.json` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/loading.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/animations/status-fail.json` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system/ui/animations/status-success.json` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-success.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a4
+Version: 0.0.4a5
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/ovos_PHAL_plugin_system.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a4/setup.py` & `ovos-PHAL-plugin-system-0.0.4a5/setup.py`

 * *Files identical despite different names*

