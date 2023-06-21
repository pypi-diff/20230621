# Comparing `tmp/ovos-PHAL-plugin-alsa-0.0.3a3.tar.gz` & `tmp/ovos-PHAL-plugin-alsa-0.0.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.3a3.tar", last modified: Wed Jun 21 18:32:17 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.3a4.tar", last modified: Wed Jun 21 18:38:46 2023, max compression
```

## Comparing `ovos-PHAL-plugin-alsa-0.0.3a3.tar` & `ovos-PHAL-plugin-alsa-0.0.3a4.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87676 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2990 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.930738 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87676 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2990 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/test/test_alsa.py
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a3/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.3a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.3a3
+Version: 0.0.3a4
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ovos-PHAL-plugin - alsa volume control
 
 controls system volume with alsa
 
 ```python
 self.bus.on("mycroft.volume.get", self.handle_volume_request)
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/__init__.py` & `ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,47 @@
 
 from ovos_plugin_manager.phal import PHALPlugin
 from os.path import join, dirname
 from ovos_utils.sound import play_audio
 from ovos_utils.log import LOG
 from ovos_bus_client import Message
 from json_database import JsonConfigXDG
+from ovos_utils.system import find_executable, is_process_running
+from ovos_plugin_manager.phal import find_phal_plugins
+
+
+class AlsaValidator:
+    @staticmethod
+    def validate(config=None):
+        """ this method is called before loading the plugin.
+        If it returns False the plugin is not loaded.
+        This allows a plugin to run platform checks"""
+        # any aliases we need here ?
+        execs = ["pulseaudio"]
+        is_pulse = any((find_executable(e) or is_process_running(e)
+                    for e in execs))
+
+        # check if pulseaudio is installed in system
+        # if missing load alsa
+        if not is_pulse:
+            return True
+
+        # check if pulse plugin is installed
+        # if missing load alsa
+        plugs = list(find_phal_plugins().keys())
+        if "ovos-PHAL-plugin-pulseaudio" not in plugs:
+            return True
+
+        # pulseaudio installed + companion plugin, do not load alsa
+        return False
 
 
 class AlsaVolumeControlPlugin(PHALPlugin):
+    validator = AlsaValidator
+
     def __init__(self, bus=None, config=None):
         super().__init__(bus=bus, name="ovos-PHAL-plugin-alsa", config=config)
         self.settings = JsonConfigXDG(self.name, subfolder="OpenVoiceOS")
         self.alsa = AlsaControl()
         self.volume_sound = join(dirname(__file__), "blop-mark-diangelo.wav")
         self.bus.on("mycroft.volume.get", self.handle_volume_request)
         self.bus.on("mycroft.volume.set", self.handle_volume_change)
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav` & `ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.3a3
+Version: 0.0.3a4
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ovos-PHAL-plugin - alsa volume control
 
 controls system volume with alsa
 
 ```python
 self.bus.on("mycroft.volume.get", self.handle_volume_request)
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a3/setup.py` & `ovos-PHAL-plugin-alsa-0.0.3a4/setup.py`

 * *Files identical despite different names*

