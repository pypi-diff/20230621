# Comparing `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.1a2.tar.gz` & `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.1a2.tar", last modified: Wed Jun 14 16:39:51 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.1a3.tar", last modified: Wed Jun 21 19:41:38 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2.tar` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:51.227169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 16:39:44.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-14 16:39:51.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:41:38.596827 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3237 2023-06-21 19:41:32.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/setup.py
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/LICENSE` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/README.md` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/__init__.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/setup.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 import os
 from setuptools import setup
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
+
 def get_version():
     """ Find the version of the package"""
     version = None
     version_file = os.path.join(BASEDIR, 'ovos_PHAL_plugin_wallpaper_manager', 'version.py')
     major, minor, build, alpha = (None, None, None, None)
     with open(version_file) as f:
         for line in f:
@@ -24,36 +25,47 @@
                     '# END_VERSION_BLOCK' in line):
                 break
     version = f"{major}.{minor}.{build}"
     if alpha and int(alpha) > 0:
         version += f"a{alpha}"
     return version
 
+
 def required(requirements_file):
     """ Read requirements file and remove comments and empty lines. """
     with open(os.path.join(BASEDIR, requirements_file), 'r') as f:
         requirements = f.read().splitlines()
         if 'MYCROFT_LOOSE_REQUIREMENTS' in os.environ:
             print('USING LOOSE REQUIREMENTS!')
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
+
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
+
+def get_description():
+    with open(os.path.join(BASEDIR, "README.md"), "r") as f:
+        long_description = f.read()
+    return long_description
+
+
 PLUGIN_ENTRY_POINT = 'ovos-PHAL-plugin-wallpaper-manager=ovos_PHAL_plugin_wallpaper_manager:WallpaperManager'
 setup(
     name='ovos-PHAL-plugin-wallpaper-manager',
     version=get_version(),
     description='A plugin for OpenVoiceOS hardware abstraction layer',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wallpaper-manager',
     author='Aiix',
     author_email='aix.m@outlook.com',
     license='Apache-2.0',
     packages=['ovos_PHAL_plugin_wallpaper_manager'],
     package_data={'': package_files('ovos_PHAL_plugin_wallpaper_manager')},
     install_requires=required("requirements.txt"),
```

