# Comparing `tmp/ovos-PHAL-plugin-system-0.0.4a5.tar.gz` & `tmp/ovos-PHAL-plugin-system-0.0.4a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a5.tar", last modified: Wed Jun 21 16:16:05 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a6.tar", last modified: Wed Jun 21 19:41:45 2023, max compression
```

## Comparing `ovos-PHAL-plugin-system-0.0.4a5.tar` & `ovos-PHAL-plugin-system-0.0.4a6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.855097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Reboot.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Restart.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Shutdown.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Status.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/loading.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-fail.json
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-success.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:15:59.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:16:05.000000 ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:16:05.859097 ovos-PHAL-plugin-system-0.0.4a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-06-21 16:15:56.000000 ovos-PHAL-plugin-system-0.0.4a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.810620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Reboot.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Restart.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Shutdown.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Status.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/loading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-fail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/setup.py
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/__init__.py` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Reboot.qml` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Reboot.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Restart.qml` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Restart.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Shutdown.qml` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Shutdown.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/Status.qml` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/loading.json` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/loading.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-fail.json` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system/ui/animations/status-success.json` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-success.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/ovos_PHAL_plugin_system.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a5/setup.py` & `ovos-PHAL-plugin-system-0.0.4a6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,19 +45,28 @@
         requirements = f.read().splitlines()
         if 'MYCROFT_LOOSE_REQUIREMENTS' in os.environ:
             print('USING LOOSE REQUIREMENTS!')
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
+
+def get_description():
+    with open(os.path.join(BASEDIR, "readme.md"), "r") as f:
+        long_description = f.read()
+    return long_description
+
+
 PLUGIN_ENTRY_POINT = 'ovos-PHAL-plugin-system=ovos_PHAL_plugin_system:SystemEvents'
 setup(
     name='ovos-PHAL-plugin-system',
     version=get_version(),
     description='A plugin for OpenVoiceOS hardware abstraction layer',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system',
     author='JarbasAi',
     author_email='jarbasai@mailfence.com',
     license='Apache-2.0',
     packages=['ovos_PHAL_plugin_system'],
     package_data={'': package_files('ovos_PHAL_plugin_system')},
     install_requires=required("requirements.txt"),
```

