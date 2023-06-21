# Comparing `tmp/ovos-phal-plugin-ipgeo-0.0.2a1.tar.gz` & `tmp/ovos-phal-plugin-ipgeo-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.2a1.tar", last modified: Tue Jun  6 04:04:55 2023, max compression
+gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.2a2.tar", last modified: Wed Jun 21 15:21:01 2023, max compression
```

## Comparing `ovos-phal-plugin-ipgeo-0.0.2a1.tar` & `ovos-phal-plugin-ipgeo-0.0.2a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-06 04:04:48.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 04:04:55.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 04:04:55.383971 ovos-phal-plugin-ipgeo-0.0.2a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-06 04:04:42.000000 ovos-phal-plugin-ipgeo-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:21:01.299032 ovos-phal-plugin-ipgeo-0.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 15:20:52.000000 ovos-phal-plugin-ipgeo-0.0.2a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-21 15:21:01.299032 ovos-phal-plugin-ipgeo-0.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 15:20:52.000000 ovos-phal-plugin-ipgeo-0.0.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:21:01.299032 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-21 15:20:52.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 15:20:55.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:21:01.299032 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-21 15:21:01.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 15:21:01.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:21:01.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 15:21:01.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 15:21:01.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 15:21:01.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:21:01.000000 ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 15:20:52.000000 ovos-phal-plugin-ipgeo-0.0.2a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:21:01.299032 ovos-phal-plugin-ipgeo-0.0.2a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-21 15:20:52.000000 ovos-phal-plugin-ipgeo-0.0.2a2/setup.py
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.2a1/PKG-INFO` & `ovos-phal-plugin-ipgeo-0.0.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-phal-plugin-ipgeo
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A PHAL plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-ipgeo
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo/__init__.py` & `ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import requests
+
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_config.config import LocalConf
 from ovos_config.locations import get_webcache_location
 from ovos_utils.messagebus import Message
+from ovos_utils import classproperty
+from ovos_utils.process_utils import RuntimeRequirements
 
 
 class IPGeoPlugin(PHALPlugin):
     def __init__(self, bus=None, config=None):
         super().__init__(bus, "ovos-phal-plugin-ipgeo", config)
         self.location = {}
         self.web_config = LocalConf(get_webcache_location())
         self.bus.on("mycroft.internet.connected", self.on_reset)
         self.bus.on("ovos.ipgeo.update", self.on_reset)
         self.on_reset()  # get initial location data
 
+    @classproperty
+    def runtime_requirements(self):
+        return RuntimeRequirements(internet_before_load=True,
+                                   network_before_load=True,
+                                   requires_internet=True,
+                                   requires_network=True,
+                                   no_internet_fallback=False,
+                                   no_network_fallback=False)
+
     def on_reset(self, message=None):
         # we update the remote config to allow
         # both backend and user config to take precedence
         # over ip geolocation
         if self.web_config.get("location") and \
                 (message is None or not message.data.get('overwrite')):
             return
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.2a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO` & `ovos-phal-plugin-ipgeo-0.0.2a2/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-phal-plugin-ipgeo
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A PHAL plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-ipgeo
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.2a1/setup.py` & `ovos-phal-plugin-ipgeo-0.0.2a2/setup.py`

 * *Files identical despite different names*

