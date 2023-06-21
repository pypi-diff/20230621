# Comparing `tmp/splight-cli-3.0.0.tar.gz` & `tmp/splight-cli-3.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-cli-3.0.0.tar", last modified: Fri Jun 16 12:53:12 2023, max compression
+gzip compressed data, was "splight-cli-3.0.1.dev0.tar", last modified: Wed Jun 21 17:11:22 2023, max compression
```

## Comparing `splight-cli-3.0.0.tar` & `splight-cli-3.0.1.dev0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 12:53:12.184711 splight-cli-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-06-16 12:53:11.000000 splight-cli-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/component/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/.splightignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/Initialization
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/auto_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/spec.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/component/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/tests/test_component_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/context/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/context/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/alert/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/attribute/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/file/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/manager/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/setpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/setpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/cli/hub/component/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/component/hub_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/cli/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:53:12.184711 splight-cli-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-16 12:53:11.000000 splight-cli-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/splight_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.152864 splight-cli-3.0.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 17:11:22.152864 splight-cli-3.0.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.144865 splight-cli-3.0.1.dev0/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/component/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/templates/.splightignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/templates/Initialization
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/templates/auto_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/templates/spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/templates/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/component/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/component/tests/test_component_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/context/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/manager/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/engine/setpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/engine/setpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.148865 splight-cli-3.0.1.dev0/cli/hub/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/hub/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/hub/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/hub/component/hub_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.152864 splight-cli-3.0.1.dev0/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/utils/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.152864 splight-cli-3.0.1.dev0/cli/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/cli/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:11:22.152864 splight-cli-3.0.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 17:11:21.000000 splight-cli-3.0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:11:22.152864 splight-cli-3.0.1.dev0/splight_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 17:11:22.000000 splight-cli-3.0.1.dev0/splight_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-21 17:11:22.000000 splight-cli-3.0.1.dev0/splight_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:11:22.000000 splight-cli-3.0.1.dev0/splight_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 17:11:22.000000 splight-cli-3.0.1.dev0/splight_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 17:11:22.000000 splight-cli-3.0.1.dev0/splight_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 17:11:22.000000 splight-cli-3.0.1.dev0/splight_cli.egg-info/top_level.txt
```

### Comparing `splight-cli-3.0.0/README.md` & `splight-cli-3.0.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/cli.py` & `splight-cli-3.0.1.dev0/cli/cli.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/__init__.py` & `splight-cli-3.0.1.dev0/cli/component/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -129,7 +129,24 @@
         manager = ComponentManager()
         console.print("Testing component...", style=success_style)
         manager.test(path=path, name=name, debug=debug)
     except Exception as e:
         logger.exception(e)
         console.print(f"Error testing component: {str(e)}", style=error_style)
         typer.Exit(1)
+
+
+@component_app.command()
+def create_local_db(
+    ctx: typer.Context,
+    path: str = typer.Argument(..., help="Path to component source code"),
+) -> None:
+    try:
+        manager = ComponentManager()
+        console.print("Creating local component db...", style=success_style)
+        manager.create_local_db(path=path)
+    except Exception as e:
+        logger.exception(e)
+        console.print(
+            f"Error creating local component db: {str(e)}", style=error_style
+        )
+        typer.Exit(1)
```

### Comparing `splight-cli-3.0.0/cli/component/component.py` & `splight-cli-3.0.1.dev0/cli/component/component.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 import subprocess
 from enum import auto
 from pathlib import Path
 from typing import List, Optional
+from uuid import uuid4
 
 from caseconverter import pascalcase
 from cli.component.exceptions import (
     ComponentExecutionError,
     ComponentTestError,
     ComponentTestFileDoesNotExists,
     InvalidSplightCLIVersion,
@@ -235,7 +236,92 @@
         if debug:
             cmd = " ".join([cmd, "-s"])
         return cmd
 
     def _validate_cli_version(self, component_cli_version: str):
         if component_cli_version != __version__:
             raise InvalidSplightCLIVersion(component_cli_version, __version__)
+
+    def create_local_db(self, path: str):
+        def generate_component(json_spec, component_id):
+            return {
+                component_id: {
+                    "id": component_id,
+                    "name": json_spec.get("name"),
+                    "version": f"{json_spec['name']}-{json_spec['version']}",
+                    "custom_types": json_spec.get("custom_types", []),
+                    "component_type": json_spec.get(
+                        "component_type", "connector"
+                    ),
+                    "input": json_spec.get("input", []),
+                    "output": json_spec.get("output", []),
+                    "commands": json_spec.get("commands", []),
+                    "endpoints": json_spec.get("endpoints", []),
+                    "bindings": json_spec.get("bindings", []),
+                }
+            }
+
+        def generate_component_object(custom_type, component_id):
+            component_object_id = str(uuid4())
+            # TODO: review description and type
+            return {
+                component_object_id: {
+                    "id": component_object_id,
+                    "name": custom_type["name"],
+                    "component_id": component_id,
+                    "description": "",
+                    "type": custom_type["name"],
+                    "data": custom_type.get("fields", []),
+                }
+            }
+
+        def generate_asset(field):
+            asset_id = str(uuid4())
+            # TODO: review attributes
+            return {
+                asset_id: {
+                    "id": asset_id,
+                    "name": field["name"],
+                    "description": field.get("description"),
+                    "tags": [],
+                    "attributes": [],
+                    "verified": False,
+                    "geometry": None,
+                    "centroid": None,
+                    "external_id": None,
+                    "is_public": False,
+                }
+            }
+
+        def generate_attribute(field):
+            attribute_id = str(uuid4())
+            return {
+                attribute_id: {
+                    "id": attribute_id,
+                    "name": field["name"],
+                }
+            }
+
+        splight_db = {
+            "asset": {},
+            "attribute": {},
+            "component": {},
+            "componentobject": {},
+        }
+        spec = Spec.from_file(os.path.join(path, SPEC_FILE))
+        json_spec = json.loads(spec.json())
+
+        component_id = str(uuid4())
+        splight_db["component"] = generate_component(json_spec, component_id)
+
+        for custom_type in json_spec.get("custom_types"):
+            splight_db["componentobject"].update(
+                generate_component_object(custom_type, component_id)
+            )
+            for field in custom_type.get("fields"):
+                if field["type"] == "Asset":
+                    splight_db["asset"].update(generate_asset(field))
+                elif field["type"] == "Attribute":
+                    splight_db["attribute"].update(generate_attribute(field))
+
+        with open("splight-db.json", "w") as db_file:
+            json.dump(splight_db, db_file, indent=4)
```

### Comparing `splight-cli-3.0.0/cli/component/exceptions.py` & `splight-cli-3.0.1.dev0/cli/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/loaders.py` & `splight-cli-3.0.1.dev0/cli/component/loaders.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/templates/.splightignore` & `splight-cli-3.0.1.dev0/cli/component/templates/.splightignore`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/templates/auto_readme.md` & `splight-cli-3.0.1.dev0/cli/component/templates/auto_readme.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/templates/main.py` & `splight-cli-3.0.1.dev0/cli/component/templates/main.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/templates/spec.json` & `splight-cli-3.0.1.dev0/cli/component/templates/spec.json`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/templates/tests.py` & `splight-cli-3.0.1.dev0/cli/component/templates/tests.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/component/tests/test_component_manager.py` & `splight-cli-3.0.1.dev0/cli/component/tests/test_component_manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/config/__init__.py` & `splight-cli-3.0.1.dev0/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/constants.py` & `splight-cli-3.0.1.dev0/cli/constants.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/context/__init__.py` & `splight-cli-3.0.1.dev0/cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/context/workspace.py` & `splight-cli-3.0.1.dev0/cli/context/workspace.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/alert/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/asset/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/attribute/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/component/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/datalake/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/file/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/file/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/manager/exceptions.py` & `splight-cli-3.0.1.dev0/cli/engine/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/manager/manager.py` & `splight-cli-3.0.1.dev0/cli/engine/manager/manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/secret/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/engine/setpoint/__init__.py` & `splight-cli-3.0.1.dev0/cli/engine/setpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/hub/component/__init__.py` & `splight-cli-3.0.1.dev0/cli/hub/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/hub/component/exceptions.py` & `splight-cli-3.0.1.dev0/cli/hub/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/hub/component/hub_manager.py` & `splight-cli-3.0.1.dev0/cli/hub/component/hub_manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/settings.py` & `splight-cli-3.0.1.dev0/cli/settings.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/utils/input.py` & `splight-cli-3.0.1.dev0/cli/utils/input.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/utils/loader.py` & `splight-cli-3.0.1.dev0/cli/utils/loader.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/utils/pprint.py` & `splight-cli-3.0.1.dev0/cli/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/utils/yaml.py` & `splight-cli-3.0.1.dev0/cli/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/cli/workspace/__init__.py` & `splight-cli-3.0.1.dev0/cli/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/setup.py` & `splight-cli-3.0.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.0/splight_cli.egg-info/SOURCES.txt` & `splight-cli-3.0.1.dev0/splight_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

