# Comparing `tmp/ovos-PHAL-plugin-alsa-0.0.3a2.tar.gz` & `tmp/ovos-PHAL-plugin-alsa-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.3a2.tar", last modified: Fri Jun 16 16:57:31 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.3a3.tar", last modified: Wed Jun 21 18:32:17 2023, max compression
```

## Comparing `ovos-PHAL-plugin-alsa-0.0.3a2.tar` & `ovos-PHAL-plugin-alsa-0.0.3a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87676 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2990 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87676 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:32:17.000000 ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:32:17.064495 ovos-PHAL-plugin-alsa-0.0.3a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2990 2023-06-21 18:32:13.000000 ovos-PHAL-plugin-alsa-0.0.3a3/setup.py
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a2/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.3a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/__init__.py` & `ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import alsaaudio
 
 from ovos_plugin_manager.phal import PHALPlugin
 from os.path import join, dirname
 from ovos_utils.sound import play_audio
 from ovos_utils.log import LOG
-from mycroft_bus_client import Message
+from ovos_bus_client import Message
 from json_database import JsonConfigXDG
 
 
 class AlsaVolumeControlPlugin(PHALPlugin):
     def __init__(self, bus=None, config=None):
         super().__init__(bus=bus, name="ovos-PHAL-plugin-alsa", config=config)
         self.settings = JsonConfigXDG(self.name, subfolder="OpenVoiceOS")
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav` & `ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.3a3/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a2/setup.py` & `ovos-PHAL-plugin-alsa-0.0.3a3/setup.py`

 * *Files identical despite different names*

