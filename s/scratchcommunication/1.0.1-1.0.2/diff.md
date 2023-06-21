# Comparing `tmp/scratchcommunication-1.0.1.tar.gz` & `tmp/scratchcommunication-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "scratchcommunication-1.0.2.tar", last modified: Wed Jun 21 15:42:08 2023, max compression
```

## Comparing `scratchcommunication-1.0.1.tar` & `scratchcommunication-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,17 @@
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/Pipfile
--rw-r--r--   0        0        0    29429 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/Pipfile.lock
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/__init__.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/cloud.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/exceptions.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/headers.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/session.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/LICENSE
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/setup.py
```

### Comparing `scratchcommunication-1.0.1/scratchcommunication/cloud.py` & `scratchcommunication-1.0.2/scratchcommunication/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from types import NoneType
 from typing import Any, Iterable, Literal, Mapping, Union
 from .exceptions import QuickAccessDisabledError
 from websocket import WebSocket
 from threading import Thread
 import json, math, time, requests
 
+NoneType = type(None)
+
 class Event:
     def __init__(self, type : Literal["set", "delete", "connect", "create"], **entries):
         entries["type"] = type
         self.__dict__.update(entries)
 
     @property
     def data(self):
@@ -117,16 +118,16 @@
     def verify_value(value : Union[float, int, bool, NoneType]):
         '''
         Use for detecting if a  value can be used for cloud variables.
         '''
         try:
             assert not isinstance(value, Union[str, list, dict, tuple]) or isinstance(float(value), float)
             assert len(json.dumps(value)) <= 256
-        except:
-            raise ValueError("Bad value for cloud variables.")
+        except Exception as e:
+            raise ValueError("Bad value for cloud variables.") from e
 
     def _set_variable(self, *, name : str, value : Union[float, int, bool, NoneType], retry : int):
         '''
         Don't use this.
         '''
         try:
             self.send_packet(
```

### Comparing `scratchcommunication-1.0.1/scratchcommunication/session.py` & `scratchcommunication-1.0.2/scratchcommunication/session.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,8 @@
             raise InvalidValueError("Your login was wrong")
         except Exception as e:
             raise Exception("An error occurred while trying to log in.") from e
     def create_cloudconnection(self, project_id : int, **kwargs) -> cloud.CloudConnection:
         '''
         Create a cloud connection to a project.
         '''
-        return cloud.CloudConnection(project_id=project_id, session=self, **kwargs)
+        return cloud.CloudConnection(project_id=project_id, session=self, **kwargs)
```

