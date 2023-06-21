# Comparing `tmp/collective.behavior.talcondition-0.9.tar.gz` & `tmp/collective.behavior.talcondition-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.behavior.talcondition-0.9.tar", last modified: Fri Oct 12 12:38:12 2018, max compression
+gzip compressed data, was "collective.behavior.talcondition-1.0a1.tar", last modified: Wed Jun 21 11:47:04 2023, max compression
```

## Comparing `collective.behavior.talcondition-0.9.tar` & `collective.behavior.talcondition-1.0a1.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1482 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       40 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5279 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      307 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2575 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/behavior.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2812 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/extender.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      227 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/testing/types.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/testing/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1916 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/testing/types/testtype.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       67 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/default/collectivebehaviortalcondition_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      196 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2900 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      764 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/testing.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2846 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      432 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/interfaces.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1356 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2352 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_behavior.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4021 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      633 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_robot.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1320 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_extender.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/robot/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1777 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/locales/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1339 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5279 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2033 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       31 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      134 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      155 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1746 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2096 2018-10-12 12:38:12.000000 collective.behavior.talcondition-0.9/CHANGES.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3469 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       84 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      171 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6286 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1802 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/docs/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/docs/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1904 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      308 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2824 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/behavior.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2172 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2806 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/extender.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      432 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/interfaces.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/es/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1644 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/es/LC_MESSAGES/collective.behavior.talcondition.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1339 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      196 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/default/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/default/collectivebehaviortalcondition_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       67 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/default/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      181 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/testing/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/testing/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1916 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/testing/types/testtype.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      227 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/testing/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/uninstall/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      210 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      256 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2894 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      771 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/testing.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.383084 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/robot/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/robot/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2352 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_behavior.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1321 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_extender.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      633 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2483 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5289 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5031 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/utils.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-06-21 11:47:04.379084 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6286 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2202 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       53 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       31 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)       92 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-06-21 11:47:04.000000 collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.behavior.talcondition-0.9/docs/LICENSE.GPL` & `collective.behavior.talcondition-1.0a1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.behavior.talcondition-0.9/README.rst` & `collective.behavior.talcondition-1.0a1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -25,7 +25,20 @@
 For AT you have to provide the ITALConditionable on your class (see testing.zcml).
 
 For DX you just have to activate the behavior on your content type.
 
 Plone versions
 ==============
 It has been developed and tested for Plone 4 and 5.
+
+
+Translations
+============
+
+This product has been translated into
+
+- French.
+
+- Spanish.
+
+You can contribute for any message missing or other new languages, join us at `Plone Collective Team <https://www.transifex.com/plone/plone-collective/>`_ into *Transifex.net* service with all world Plone translators community.
+
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/behavior.py` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/behavior.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,89 @@
 # -*- coding: utf-8 -*-
-from zope import schema
-from zope.component import adapts
-from zope.interface import alsoProvides
-from zope.interface import implements
+
 from collective.behavior.talcondition import _
 from collective.behavior.talcondition.utils import evaluateExpressionFor
+from plone.autoform import directives as form
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.dexterity.interfaces import IDexterityContent
 from plone.supermodel import model
-from plone.autoform import directives as form
 from z3c.form.browser.checkbox import CheckBoxFieldWidget
+from zope import schema
+from zope.component import adapts
+from zope.interface import alsoProvides
+from zope.interface import implementer
 
 
 class ITALCondition(model.Schema):
 
-    form.widget('tal_condition', size=80)
+    form.widget("tal_condition", size=80)
     tal_condition = schema.TextLine(
-        title=_(u'TAL condition expression'),
-        description=_(u'Enter a TAL expression that once evaluated '
-                      'will return \'True\' if content should be '
-                      'available. Elements \'member\', \'context\' '
-                      'and \'portal\' are available for the '
-                      'expression.'),
+        title=_(u"TAL condition expression"),
+        description=_(
+            u"Enter a TAL expression that once evaluated "
+            "will return 'True' if content should be "
+            "available. Elements 'member', 'context' "
+            "and 'portal' are available for the "
+            "expression."
+        ),
         required=False,
-        default=u'',
+        default=u"",
     )
 
-    form.widget('roles_bypassing_talcondition', CheckBoxFieldWidget, multiple='multiple', size=15)
+    form.widget(
+        "roles_bypassing_talcondition",
+        CheckBoxFieldWidget,
+        multiple="multiple",
+        size=15,
+    )
     roles_bypassing_talcondition = schema.Set(
-        title=_(u'Roles that will bypass the TAL condition'),
-        description=_(u'Choose the different roles for which the TAL '
-                      'condition will not be evaluated and always '
-                      'considered \'True\'.'),
+        title=_(u"Roles that will bypass the TAL condition"),
+        description=_(
+            u"Choose the different roles for which the TAL "
+            "condition will not be evaluated and always "
+            "considered 'True'."
+        ),
         required=False,
-        value_type=schema.Choice(vocabulary='plone.app.vocabularies.Roles'),
+        value_type=schema.Choice(vocabulary="plone.app.vocabularies.Roles"),
     )
 
     def evaluate(self):
         """Evaluate the condition and returns True or False."""
 
+
 alsoProvides(ITALCondition, IFormFieldProvider)
 
 
+@implementer(ITALCondition)
 class TALCondition(object):
-    """
-    """
+    """ """
 
-    implements(ITALCondition)
     adapts(IDexterityContent)
 
     def __init__(self, context):
         self.context = context
 
     def get_tal_condition(self):
-        return getattr(self.context, 'tal_condition', '')
+        return getattr(self.context, "tal_condition", "")
 
     def set_tal_condition(self, value):
         self.context.tal_condition = value
 
     tal_condition = property(get_tal_condition, set_tal_condition)
 
     def get_roles_bypassing_talcondition(self):
-        return getattr(self.context, 'roles_bypassing_talcondition', [])
+        return getattr(self.context, "roles_bypassing_talcondition", [])
 
     def set_roles_bypassing_talcondition(self, value):
         self.context.roles_bypassing_talcondition = value
 
-    roles_bypassing_talcondition = property(get_roles_bypassing_talcondition, set_roles_bypassing_talcondition)
+    roles_bypassing_talcondition = property(
+        get_roles_bypassing_talcondition, set_roles_bypassing_talcondition
+    )
+
+    def complete_extra_expr_ctx(self, extra_expr_ctx):
+        """Complete extra_expr_ctx, this is made to be overrided."""
+        return extra_expr_ctx
 
     def evaluate(self, extra_expr_ctx={}):
+        extra_expr_ctx = self.complete_extra_expr_ctx(extra_expr_ctx)
         return evaluateExpressionFor(self, extra_expr_ctx=extra_expr_ctx)
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/extender.py` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/extender.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # -*- coding: utf-8 -*-
-from zope.component import adapts
-
-from zope.interface import implements
+from archetypes.schemaextender.field import ExtensionField
 from archetypes.schemaextender.interfaces import IBrowserLayerAwareExtender
 from archetypes.schemaextender.interfaces import ISchemaExtender
-from archetypes.schemaextender.field import ExtensionField
-
-
-from Products.Archetypes.public import MultiSelectionWidget
+from collective.behavior.talcondition.interfaces import ICollectiveBehaviorTalconditionLayer
+from collective.behavior.talcondition.interfaces import ITALConditionable
 from Products.Archetypes.public import LinesField
+from Products.Archetypes.public import MultiSelectionWidget
 from Products.Archetypes.public import StringField
 from Products.Archetypes.public import StringWidget
-
-from collective.behavior.talcondition.interfaces import ICollectiveBehaviorTalconditionLayer
-from collective.behavior.talcondition.interfaces import ITALConditionable
+from zope.component import adapts
+from zope.interface import implementer
 
 
 class TALConditionStringField(ExtensionField, StringField):
     """A string field that will contain an eventual TAL condition expression."""
 
 
 class TALConditionLinesField(ExtensionField, LinesField):
     """A Lines field that will contain all roles
        that will bypass the tal condition."""
 
 
+@implementer(ISchemaExtender, IBrowserLayerAwareExtender)
 class TALConditionExtender(object):
     """TALCondition class"""
 
-    implements(ISchemaExtender, IBrowserLayerAwareExtender)
-
     adapts(ITALConditionable)
 
     layer = ICollectiveBehaviorTalconditionLayer
 
     fields = [
         TALConditionStringField(
             'tal_condition',
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/profiles/testing/types/testtype.xml` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/profiles/testing/types/testtype.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/testing.zcml` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/testing.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:zcml="http://namespaces.zope.org/zcml"
     i18n_domain="collective.behavior.talcondition">
 
   <include file="configure.zcml" />
 
-  <class class="Products.ATContentTypes.content.document.ATDocument">
-    <implements zcml:condition="have plone-4" interface="collective.behavior.talcondition.interfaces.ITALConditionable" />
+  <class zcml:condition="not-have plone-5"
+         class="Products.ATContentTypes.content.document.ATDocument">
+    <implements interface="collective.behavior.talcondition.interfaces.ITALConditionable" />
   </class>
 
   <genericsetup:registerProfile
       name="testing"
       title="collective.behavior.talcondition tests"
       directory="profiles/testing"
       description="Steps to ease tests of collective.behavior.talcondition"
-      provides="Products.GenericSetup.interfaces.EXTENSION"
-      />
+      provides="Products.GenericSetup.interfaces.EXTENSION" />
 
 </configure>
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/testing.py` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/testing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,95 @@
 # -*- coding: utf-8 -*-
 """Base module for unittesting."""
 
+from collective.behavior.talcondition import PLONE_VERSION
 from plone import api
 from plone.app.robotframework.testing import AUTOLOGIN_LIBRARY_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import login
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
 from plone.testing import z2
 
-import unittest
-
 import collective.behavior.talcondition
+import unittest
 
 
 class CollectiveBehaviorTalconditionLayer(PloneSandboxLayer):
 
     defaultBases = (PLONE_FIXTURE,)
-    products = ('collective.behavior.talcondition', )
+    products = ("collective.behavior.talcondition",)
 
     def setUpZope(self, app, configurationContext):
         """Set up Zope."""
         # Load ZCML
-        self.loadZCML(package=collective.behavior.talcondition,
-                      name='testing.zcml')
+        self.loadZCML(package=collective.behavior.talcondition, name="testing.zcml")
         for p in self.products:
             z2.installProduct(app, p)
 
     def setUpPloneSite(self, portal):
         """Set up Plone."""
         # Set default chain for plone.app.contenttypes
-        wftool = portal['portal_workflow']
-        wftool.setDefaultChain('simple_publication_workflow')
+        wftool = portal["portal_workflow"]
+        wftool.setDefaultChain("simple_publication_workflow")
 
-        # Install into Plone site using portal_setup
-        applyProfile(portal, 'collective.behavior.talcondition:testing')
+        # Install into Plone
+        if PLONE_VERSION < 5:
+            installer = portal["portal_quickinstaller"]
+            installer.installProduct("collective.behavior.talcondition")
+        applyProfile(portal, "collective.behavior.talcondition:testing")
 
         try:
-            applyProfile(portal, 'plone.app.contenttypes:plone-content')
+            applyProfile(portal, "plone.app.contenttypes:plone-content")
         except KeyError:
             # BBB Plone 4
             pass
 
         # Login and create some test content
-        setRoles(portal, TEST_USER_ID, ['Manager'])
+        setRoles(portal, TEST_USER_ID, ["Manager"])
         login(portal, TEST_USER_NAME)
-        api.content.create(container=portal, type='Folder', id='folder')
+        api.content.create(container=portal, type="Folder", id="folder")
 
         # Commit so that the test browser sees these objects
         import transaction
+
         transaction.commit()
 
     def tearDownZope(self, app):
         """Tear down Zope."""
         for p in reversed(self.products):
             z2.uninstallProduct(app, p)
 
-FIXTURE = CollectiveBehaviorTalconditionLayer(
-    name="FIXTURE")
+
+FIXTURE = CollectiveBehaviorTalconditionLayer(name="FIXTURE")
 
 
-INTEGRATION = IntegrationTesting(
-    bases=(FIXTURE,),
-    name="INTEGRATION")
+INTEGRATION = IntegrationTesting(bases=(FIXTURE,), name="INTEGRATION")
 
 
-FUNCTIONAL = FunctionalTesting(
-    bases=(FIXTURE,),
-    name="FUNCTIONAL")
+FUNCTIONAL = FunctionalTesting(bases=(FIXTURE,), name="FUNCTIONAL")
 
 
-ACCEPTANCE = FunctionalTesting(bases=(FIXTURE,
-                                      AUTOLOGIN_LIBRARY_FIXTURE,
-                                      z2.ZSERVER_FIXTURE),
-                               name="ACCEPTANCE")
+ACCEPTANCE = FunctionalTesting(
+    bases=(FIXTURE, AUTOLOGIN_LIBRARY_FIXTURE, z2.ZSERVER_FIXTURE), name="ACCEPTANCE"
+)
 
 
 class IntegrationTestCase(unittest.TestCase):
     """Base class for integration tests."""
 
     layer = INTEGRATION
 
     def setUp(self):
         super(IntegrationTestCase, self).setUp()
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
 
 
 class FunctionalTestCase(unittest.TestCase):
     """Base class for functional tests."""
 
     layer = FUNCTIONAL
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_setup.py` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,63 @@
 # -*- coding: utf-8 -*-
 """Setup/installation tests for this package."""
-
+from collective.behavior.talcondition import PLONE_VERSION
 from collective.behavior.talcondition.testing import IntegrationTestCase
 from plone import api
 
 
+if PLONE_VERSION >= 5:
+    from Products.CMFPlone.utils import get_installer
+
+
 class TestInstall(IntegrationTestCase):
     """Test installation of collective.behavior.talcondition into Plone."""
 
     def setUp(self):
         """Custom shared utility setup for tests."""
-        self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
+        self.portal = self.layer["portal"]
+        if PLONE_VERSION < 5:
+            self.installer = api.portal.get_tool("portal_quickinstaller")
+        else:
+            self.installer = get_installer(self.portal, self.layer["request"])
 
     def test_product_installed(self):
         """Test if collective.behavior.talcondition is installed with portal_quickinstaller."""
-        self.assertTrue(self.installer.isProductInstalled('collective.behavior.talcondition'))
-
-    def test_uninstall(self):
-        """Test if collective.behavior.talcondition is cleanly uninstalled."""
-        self.installer.uninstallProducts(['collective.behavior.talcondition'])
-        self.assertFalse(self.installer.isProductInstalled('collective.behavior.talcondition'))
+        if PLONE_VERSION < 5:
+            self.assertTrue(
+                self.installer.isProductInstalled("collective.behavior.talcondition")
+            )
+        else:
+            self.assertTrue(
+                self.installer.is_product_installed("collective.behavior.talcondition")
+            )
 
     # browserlayer.xml
     def test_browserlayer(self):
         """Test that ICollectiveBehaviorTalconditionLayer is registered."""
         from collective.behavior.talcondition.interfaces import ICollectiveBehaviorTalconditionLayer
         from plone.browserlayer import utils
+
         self.assertIn(ICollectiveBehaviorTalconditionLayer, utils.registered_layers())
+
+
+class TestUninstall(IntegrationTestCase):
+    def setUp(self):
+        """Custom shared utility setup for tests."""
+        self.portal = self.layer["portal"]
+        if PLONE_VERSION < 5:
+            self.installer = api.portal.get_tool("portal_quickinstaller")
+            self.installer.uninstallProducts(["collective.behavior.talcondition"])
+        else:
+            self.installer = get_installer(self.portal, self.layer["request"])
+            self.installer.uninstall_product("collective.behavior.talcondition")
+
+    def test_uninstall(self):
+        """Test if collective.behavior.talcondition is cleanly uninstalled."""
+        if PLONE_VERSION < 5:
+            self.assertFalse(
+                self.installer.isProductInstalled("collective.behavior.talcondition")
+            )
+        else:
+            self.assertFalse(
+                self.installer.is_product_installed("collective.behavior.talcondition")
+            )
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_behavior.py` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_behavior.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
-from plone.app.testing import login
-from plone.app.testing import TEST_USER_NAME
 from collective.behavior.talcondition import PLONE_VERSION
 from collective.behavior.talcondition.behavior import ITALCondition
-from collective.behavior.talcondition.testing import IntegrationTestCase
 from collective.behavior.talcondition.interfaces import ITALConditionable
+from collective.behavior.talcondition.testing import IntegrationTestCase
+from plone.app.testing import login
+from plone.app.testing import TEST_USER_NAME
 
 
 class TestBehavior(IntegrationTestCase):
 
     def setUp(self):
         """ """
         super(TestBehavior, self).setUp()
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_robot.py` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_robot.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import os
-import unittest
-import robotsuite
+from ..testing import ACCEPTANCE
 from plone.testing import layered
 
-from ..testing import ACCEPTANCE
+import os
+import robotsuite
+import unittest
 
 
 def test_suite():
     suite = unittest.TestSuite()
     current_dir = os.path.abspath(os.path.dirname(__file__))
     robot_dir = os.path.join(current_dir, 'robot')
     robot_tests = [
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/tests/test_extender.py` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/tests/test_extender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
-import unittest
-from plone.app.testing import login
-from plone.app.testing import TEST_USER_NAME
+from collective.behavior.talcondition import PLONE_VERSION
 from collective.behavior.talcondition.interfaces import ITALConditionable
 from collective.behavior.talcondition.testing import IntegrationTestCase
 from collective.behavior.talcondition.utils import evaluateExpressionFor
-from collective.behavior.talcondition import PLONE_VERSION
+from plone.app.testing import login
+from plone.app.testing import TEST_USER_NAME
+
+import unittest
 
 
 class TestExtender(IntegrationTestCase):
 
     @unittest.skipIf(PLONE_VERSION >= 5, 'Archetypes extender test skipped in Plone 5')
     def test_extender(self):
         """The extender is enabled on ATDocument in testing.zcml.
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/configure.zcml` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/configure.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
     i18n_domain="collective.behavior.talcondition">
 
     <i18n:registerTranslations directory="locales" />
 
     <five:registerPackage package="." initialize=".initialize" />
 
     <include package="plone.behavior" file="meta.zcml" />
@@ -18,27 +19,36 @@
         description="Add a TAL condition field useable to check if content should be available."
         provides=".behavior.ITALCondition"
         for="plone.dexterity.interfaces.IDexterityContent"
         factory=".behavior.TALCondition"
         marker=".interfaces.ITALConditionable"
         />
 
-    <adapter factory=".extender.TALConditionExtender"
+    <adapter zcml:condition="not-have plone-5"
+             factory=".extender.TALConditionExtender"
              for=".interfaces.ITALConditionable"
              provides="archetypes.schemaextender.interfaces.ISchemaExtender"
              name="collective.behavior.talcondition.extender" />
 
     <genericsetup:registerProfile
         name="default"
         title="collective.behavior.talcondition"
         directory="profiles/default"
         description="Installs the collective.behavior.talcondition add-on."
         provides="Products.GenericSetup.interfaces.EXTENSION"
         />
 
+    <genericsetup:registerProfile
+        name="uninstall"
+        title="collective.behavior.talcondition"
+        directory="profiles/uninstall"
+        description="Uninstalls the collective.behavior.talcondition add-on."
+        provides="Products.GenericSetup.interfaces.EXTENSION"
+        />
+
     <genericsetup:importStep
         name="collective.behavior.talcondition-postInstall"
         title="collective.behavior.talcondition post_install import step"
         description="Post install import step from collective.behavior.talcondition"
         handler=".setuphandlers.post_install">
     </genericsetup:importStep>
```

### Comparing `collective.behavior.talcondition-0.9/src/collective/behavior/talcondition/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po` & `collective.behavior.talcondition-1.0a1/src/collective/behavior/talcondition/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po`

 * *Files identical despite different names*

### Comparing `collective.behavior.talcondition-0.9/src/collective.behavior.talcondition.egg-info/SOURCES.txt` & `collective.behavior.talcondition-1.0a1/src/collective.behavior.talcondition.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 src/collective/behavior/talcondition/configure.zcml
 src/collective/behavior/talcondition/extender.py
 src/collective/behavior/talcondition/interfaces.py
 src/collective/behavior/talcondition/setuphandlers.py
 src/collective/behavior/talcondition/testing.py
 src/collective/behavior/talcondition/testing.zcml
 src/collective/behavior/talcondition/utils.py
+src/collective/behavior/talcondition/locales/es/LC_MESSAGES/collective.behavior.talcondition.po
 src/collective/behavior/talcondition/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po
 src/collective/behavior/talcondition/profiles/default/browserlayer.xml
 src/collective/behavior/talcondition/profiles/default/collectivebehaviortalcondition_marker.txt
 src/collective/behavior/talcondition/profiles/default/metadata.xml
 src/collective/behavior/talcondition/profiles/testing/metadata.xml
 src/collective/behavior/talcondition/profiles/testing/types.xml
 src/collective/behavior/talcondition/profiles/testing/types/testtype.xml
+src/collective/behavior/talcondition/profiles/uninstall/browserlayer.xml
 src/collective/behavior/talcondition/tests/__init__.py
 src/collective/behavior/talcondition/tests/test_behavior.py
 src/collective/behavior/talcondition/tests/test_extender.py
 src/collective/behavior/talcondition/tests/test_robot.py
 src/collective/behavior/talcondition/tests/test_setup.py
 src/collective/behavior/talcondition/tests/test_utils.py
 src/collective/behavior/talcondition/tests/robot/.gitkeep
```

### Comparing `collective.behavior.talcondition-0.9/setup.py` & `collective.behavior.talcondition-1.0a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 long_description = (
     open('README.rst').read()
-    + '\n' +
-    'Contributors\n'
-    '============\n'
-    + '\n' +
-    open('CONTRIBUTORS.rst').read()
-    + '\n' +
+    + '\n\n' +
     open('CHANGES.rst').read()
-    + '\n')
+    + '\n\n')
 
 
 setup(
     name='collective.behavior.talcondition',
-    version='0.9',
+    version='1.0a1',
     description="This package contains a Dexterity behavior and AT schemaextender to add a TAL condition on a content type.",
     long_description=long_description,
-    # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
+    # Get more from https://pypi.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
+        "Framework :: Plone :: Addon",
         "Framework :: Plone :: 4.3",
         "Framework :: Plone :: 5.0",
         "Framework :: Plone :: 5.1",
+        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.10",
+        "Operating System :: OS Independent",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Zope Plone',
     author='IMIO',
     author_email='dev@imio.be',
     url='http://pypi.python.org/pypi/collective.behavior.talcondition',
     license='GPL V2',
     packages=find_packages('src', exclude=['ez_setup']),
@@ -45,16 +47,14 @@
     install_requires=[
         'plone.api',
         'setuptools',
         'plone.app.dexterity',
     ],
     extras_require={
         'test': [
-            'ecreall.helpers.testing',
-            'plone.app.imaging',
             'plone.app.testing',
             'plone.app.robotframework',
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
```

### Comparing `collective.behavior.talcondition-0.9/CHANGES.rst` & `collective.behavior.talcondition-1.0a1/CHANGES.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,69 @@
 Changelog
 =========
 
 
+1.0a1 (2023-06-21)
+------------------
+
+- Fix deprecated import AccessControl.class_init instead of App.class_init 
+  (Plone6 compatibility)
+  [boulch]
+- Set simplier setup with Makefile
+  [sgeulette]
+
+0.14 (2021-06-29)
+-----------------
+
+- Fix pypi broken package
+  [boulch]
+
+
+0.13 (2021-06-29)
+-----------------
+
+- Add uninstall profile
+  [boulch]
+- Add Plone6 compatibily
+  [boulch]
+
+
+0.12 (2021-04-20)
+-----------------
+
+- Add Transifex.net service integration to manage the translation process.
+  [macagua]
+- Add Spanish translation
+  [macagua]
+- Do not consider the `archetypes.schemaextender` on Plone5.
+  [gbastien]
+- Adapted code (except, implementer) to be Python3 compatible.
+  [gbastien]
+- Added parameter `trusted=False` to `utils._evaluateExpression`, this will use
+  a trusted expression handler instead the restricted python default.
+  [gbastien]
+
+0.11 (2019-05-16)
+-----------------
+
+- Added parameter `raise_on_error` to `utils.evaluateExpressionFor` to raise an
+  error when an exception occurs instead returning False.
+  [gbastien]
+- Added method `TALCondition.complete_extra_expr_ctx` to the behavior to
+  formalize the way to get `extra_expr_ctx` to avoid the `evaluate` method
+  to be overrided.
+  [gbastien]
+
+0.10 (2018-11-20)
+-----------------
+
+- Do not break if parameter `expression` passed to
+  `utils._evaluateExpression` is None.
+  [gbastien]
+
 0.9 (2018-10-12)
 ----------------
 
 - Added new parameter `error_pattern=WRONG_TAL_CONDITION` to
   `utils.evaluateExpressionFor` and underlying `utils._evaluateExpression` to
   be able to log a custom message in case an error occurs during
   expression evaluation.
```

