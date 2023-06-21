# Comparing `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.1a3.tar.gz` & `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.1a3.tar", last modified: Wed Jun 21 19:41:38 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.1a4.tar", last modified: Wed Jun 21 21:05:07 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3.tar` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3237 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:05:07.054426 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 21:05:02.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-21 21:05:07.054426 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-21 21:05:02.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:05:07.054426 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-06-21 21:05:02.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-21 21:05:02.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 21:05:02.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:05:07.054426 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-21 21:05:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-21 21:05:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:05:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 21:05:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 21:05:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 21:05:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:05:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:05:07.054426 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3237 2023-06-21 21:05:02.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/setup.py
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/LICENSE` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/PKG-INFO` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-wallpaper-manager
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wallpaper-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/README.md` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/__init__.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,23 @@
         super().__init__(bus=bus, name=name, config=config)
 
         # this is a XDG compliant json storage object similar to self.settings in MycroftSkill
         # it can be used to keep state
         core_config = Configuration()
         enclosure_config = core_config.get("gui") or {}
         self.active_extension = enclosure_config.get("extension", "generic")
-        self.event_scheduler_interface = EventSchedulerInterface(name=name, bus=self.bus)
+        self.event_scheduler_interface = EventSchedulerInterface(skill_id=name,
+                                                                 bus=self.bus)
 
         self.settings = PrivateSettings(name)
         self.registered_providers = []
         self.setup_default_provider_running = False
         self.threading_event = threading.Event()
-        self.local_wallpaper_storage = os.path.join(xdg_data_home(), "wallpapers")
+        self.local_wallpaper_storage = os.path.join(xdg_data_home(),
+                                                    "wallpapers")
     
         if not os.path.exists(self.local_wallpaper_storage):
             os.makedirs(self.local_wallpaper_storage)
         self.d_provider = DownloadedProvider(self.bus,
                                              self.local_wallpaper_storage)
 
         # Manage provider registration, activation and deactivation
@@ -72,15 +74,16 @@
         # both simply call the same method
         self.bus.on("ovos.wallpaper.manager.set.wallpaper",
                     self.handle_set_wallpaper)
         self.bus.on("ovos.wallpaper.manager.get.wallpaper",
                     self.handle_get_wallpaper)
         
         # Handle swipe and voice intents to change wallpaper, also auto rotation
-        self.bus.on("ovos.wallpaper.manager.change.wallpaper", self.handle_change_wallpaper)
+        self.bus.on("ovos.wallpaper.manager.change.wallpaper",
+                    self.handle_change_wallpaper)
 
         # Auto wallpaper rotation and setting up time for change
         self.bus.on("ovos.wallpaper.manager.enable.auto.rotation", self.handle_enable_auto_rotation)
         self.bus.on("ovos.wallpaper.manager.disable.auto.rotation", self.handle_disable_auto_rotation)
         self.bus.on("ovos.wallpaper.manager.get.auto.rotation", self.handle_get_auto_rotation)
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-wallpaper-manager
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wallpaper-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/setup.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a4/setup.py`

 * *Files identical despite different names*

