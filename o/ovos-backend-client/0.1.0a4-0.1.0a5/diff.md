# Comparing `tmp/ovos-backend-client-0.1.0a4.tar.gz` & `tmp/ovos-backend-client-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.1.0a4.tar", last modified: Thu Jun  8 22:58:07 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.1.0a5.tar", last modified: Wed Jun 21 18:03:26 2023, max compression
```

## Comparing `ovos-backend-client-0.1.0a4.tar` & `ovos-backend-client-0.1.0a5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:58:07.284795 ovos-backend-client-0.1.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 22:58:07.280795 ovos-backend-client-0.1.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:58:07.280795 ovos-backend-client-0.1.0a4/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:58:07.280795 ovos-backend-client-0.1.0a4/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    40915 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38679 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:58:07.280795 ovos-backend-client-0.1.0a4/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 22:58:07.000000 ovos-backend-client-0.1.0a4/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 22:58:07.000000 ovos-backend-client-0.1.0a4/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:58:07.000000 ovos-backend-client-0.1.0a4/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 22:58:07.000000 ovos-backend-client-0.1.0a4/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 22:58:07.000000 ovos-backend-client-0.1.0a4/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:58:07.284795 ovos-backend-client-0.1.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-08 22:58:03.000000 ovos-backend-client-0.1.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40915 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38679 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/setup.py
```

### Comparing `ovos-backend-client-0.1.0a4/CHANGELOG.md` & `ovos-backend-client-0.1.0a5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
-## [0.1.0a4](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.0a4) (2023-06-08)
+## [0.1.0a5](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.0a5) (2023-06-21)
 
-[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.0a3...0.1.0a4)
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.0a4...0.1.0a5)
+
+**Merged pull requests:**
+
+- Import xdg functions from ovos\_config rather than ovos\_utils [\#43](https://github.com/OpenVoiceOS/ovos-backend-client/pull/43) ([PureTryOut](https://github.com/PureTryOut))
+
+## [V0.1.0a4](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.1.0a4) (2023-06-08)
+
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.0a3...V0.1.0a4)
 
 **Implemented enhancements:**
 
 - feat/admin\_update\_backend\_config [\#42](https://github.com/OpenVoiceOS/ovos-backend-client/pull/42) ([JarbasAl](https://github.com/JarbasAl))
 
 ## [V0.1.0a3](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.1.0a3) (2023-06-08)
```

### Comparing `ovos-backend-client-0.1.0a4/README.md` & `ovos-backend-client-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/api.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/api.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/offline.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/personal.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/cloud.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/config.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/database.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/identity.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
 import shutil
 import time
 from os.path import isfile, dirname, expanduser
 
 from combo_lock import ComboLock
-from ovos_utils.configuration import get_xdg_config_save_path, get_xdg_base
+from ovos_config.config import get_xdg_config_save_path
+from ovos_config.meta import get_xdg_base
 from ovos_utils.log import LOG
 
 identity_lock = ComboLock('/tmp/identity-lock')
 
 
 def find_identity():
     locations = [
```

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/pairing.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client/settings.py` & `ovos-backend-client-0.1.0a5/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a4/setup.py` & `ovos-backend-client-0.1.0a5/setup.py`

 * *Files identical despite different names*

