# Comparing `tmp/splight-lib-3.0.0.tar.gz` & `tmp/splight-lib-3.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.0.0.tar", last modified: Fri Jun 16 12:30:43 2023, max compression
+gzip compressed data, was "splight-lib-3.1.0.dev0.tar", last modified: Wed Jun 21 13:10:10 2023, max compression
```

## Comparing `splight-lib-3.0.0.tar` & `splight-lib-3.1.0.dev0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.192204 splight-lib-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:42.000000 splight-lib-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 12:30:43.192204 splight-lib-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-16 12:30:42.000000 splight-lib-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:30:43.192204 splight-lib-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-16 12:30:42.000000 splight-lib-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.184204 splight-lib-3.0.0/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.184204 splight-lib-3.0.0/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.184204 splight-lib-3.0.0/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.188204 splight-lib-3.0.0/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.192204 splight-lib-3.0.0/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.192204 splight-lib-3.0.0/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.192204 splight-lib-3.0.0/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.192204 splight-lib-3.0.0/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-16 12:30:42.000000 splight-lib-3.0.0/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:43.184204 splight-lib-3.0.0/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 12:30:43.000000 splight-lib-3.0.0/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-16 12:30:43.000000 splight-lib-3.0.0/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:30:43.000000 splight-lib-3.0.0/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:30:43.000000 splight-lib-3.0.0/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 12:30:43.000000 splight-lib-3.0.0/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 12:30:43.000000 splight-lib-3.0.0/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.0.0/setup.py` & `splight-lib-3.1.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.0.0",
+    version="3.1.0.dev0",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.0.0/splight_lib/abstract/client.py` & `splight-lib-3.1.0.dev0/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/auth/mac_auth.py` & `splight-lib-3.1.0.dev0/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/communication/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/communication/remote_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/database/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/database/builder.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/database/classmap.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/database/local_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/database/remote_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/datalake/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/datalake/builder.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/datalake/local_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/exceptions.py` & `splight-lib-3.1.0.dev0/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/file_handler.py` & `splight-lib-3.1.0.dev0/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/filter.py` & `splight-lib-3.1.0.dev0/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/hub/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/client/hub/client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/communication/event_handler.py` & `splight-lib-3.1.0.dev0/splight_lib/communication/event_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/component/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/component/exceptions.py` & `splight-lib-3.1.0.dev0/splight_lib/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/component/spec.py` & `splight-lib-3.1.0.dev0/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/encryption.py` & `splight-lib-3.1.0.dev0/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/execution.py` & `splight-lib-3.1.0.dev0/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/logging/_internal.py` & `splight-lib-3.1.0.dev0/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/logging/component.py` & `splight-lib-3.1.0.dev0/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/logging/logging.py` & `splight-lib-3.1.0.dev0/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/__init__.py` & `splight-lib-3.1.0.dev0/splight_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/alert.py` & `splight-lib-3.1.0.dev0/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/asset.py` & `splight-lib-3.1.0.dev0/splight_lib/models/asset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from typing import Any, List, Optional, Tuple
+from typing import Any, List, Optional
 
-from geojson_pydantic import GeometryCollection
+from geojson_pydantic import GeometryCollection, Point
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.base import SplightDatabaseBaseModel
 
 
+class Tag:
+    name: str
+    description: Optional[str] = None
+
+
 class Asset(SplightDatabaseBaseModel):
     id: Optional[str]
     name: str
     description: Optional[str] = None
-    latitude: Optional[float]
-    longitude: Optional[float]
-    tags: List[str] = []
+    tags: List[Tag] = []
     attributes: List[Attribute] = []
     verified: bool = False
     geometry: Optional[GeometryCollection]
-    centroid_coordinates: Optional[Tuple[float, float]]
+    centroid: Optional[Point]
+    external_id: Optional[str] = None
+    is_public: bool = False
 
     def set_attribute(self, attribute: Attribute, value: Any, value_type: str):
         new_value = self._db_client.operate(
             resource_name="set-asset-attribute",
             instance={
                 "asset": self.id,
                 "attribute": attribute.id,
```

### Comparing `splight-lib-3.0.0/splight_lib/models/base.py` & `splight-lib-3.1.0.dev0/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/communication.py` & `splight-lib-3.1.0.dev0/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/component.py` & `splight-lib-3.1.0.dev0/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/event.py` & `splight-lib-3.1.0.dev0/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/file.py` & `splight-lib-3.1.0.dev0/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/hub.py` & `splight-lib-3.1.0.dev0/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/native.py` & `splight-lib-3.1.0.dev0/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/query.py` & `splight-lib-3.1.0.dev0/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/models/setpoint.py` & `splight-lib-3.1.0.dev0/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/restclient/client.py` & `splight-lib-3.1.0.dev0/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/restclient/exceptions.py` & `splight-lib-3.1.0.dev0/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/restclient/types.py` & `splight-lib-3.1.0.dev0/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/settings.py` & `splight-lib-3.1.0.dev0/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/testing/__init__.py` & `splight-lib-3.1.0.dev0/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/utils/custom_model.py` & `splight-lib-3.1.0.dev0/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/utils/hub.py` & `splight-lib-3.1.0.dev0/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib/webhook.py` & `splight-lib-3.1.0.dev0/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.1.0.dev0/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0/splight_lib.egg-info/requires.txt` & `splight-lib-3.1.0.dev0/splight_lib.egg-info/requires.txt`

 * *Files identical despite different names*

