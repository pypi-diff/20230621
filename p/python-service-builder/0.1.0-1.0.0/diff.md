# Comparing `tmp/python-service-builder-0.1.0.tar.gz` & `tmp/python-service-builder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-service-builder-0.1.0.tar", last modified: Tue Sep 20 21:26:16 2022, max compression
+gzip compressed data, was "python-service-builder-1.0.0.tar", last modified: Wed Jun 21 15:43:50 2023, max compression
```

## Comparing `python-service-builder-0.1.0.tar` & `python-service-builder-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2022-09-20 21:26:16.957530 python-service-builder-0.1.0/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      651 2022-09-20 21:26:16.957530 python-service-builder-0.1.0/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       73 2022-09-20 14:03:24.000000 python-service-builder-0.1.0/README.md
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       98 2022-09-20 13:49:05.000000 python-service-builder-0.1.0/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2022-09-20 21:26:16.953529 python-service-builder-0.1.0/python_service_builder.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      651 2022-09-20 21:26:16.000000 python-service-builder-0.1.0/python_service_builder.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      507 2022-09-20 21:26:16.000000 python-service-builder-0.1.0/python_service_builder.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-09-20 21:26:16.000000 python-service-builder-0.1.0/python_service_builder.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-09-20 21:26:16.000000 python-service-builder-0.1.0/python_service_builder.egg-info/not-zip-safe
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      328 2022-09-20 21:26:16.000000 python-service-builder-0.1.0/python_service_builder.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       18 2022-09-20 21:26:16.000000 python-service-builder-0.1.0/python_service_builder.egg-info/top_level.txt
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2022-09-20 21:26:16.957530 python-service-builder-0.1.0/service_framework/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1946 2022-09-20 21:20:44.000000 python-service-builder-0.1.0/service_framework/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      979 2022-09-20 21:20:44.000000 python-service-builder-0.1.0/service_framework/__init_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1670 2022-09-20 21:20:44.000000 python-service-builder-0.1.0/service_framework/list_services.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3910 2022-09-20 21:20:00.000000 python-service-builder-0.1.0/service_framework/service_builder.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    13959 2022-09-20 21:20:44.000000 python-service-builder-0.1.0/service_framework/services.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1330 2022-09-20 21:20:44.000000 python-service-builder-0.1.0/service_framework/services_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2022-09-20 21:26:16.957530 python-service-builder-0.1.0/setup.cfg
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1995 2022-09-20 21:00:15.000000 python-service-builder-0.1.0/setup.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3278 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2758 2023-06-20 19:07:05.000000 python-service-builder-1.0.0/README.md
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1180 2023-06-07 19:47:23.000000 python-service-builder-1.0.0/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/python_service_builder.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3278 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      453 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      328 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       18 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/top_level.txt
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/service_framework/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3630 2023-06-20 15:29:24.000000 python-service-builder-1.0.0/service_framework/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3743 2023-06-15 20:04:02.000000 python-service-builder-1.0.0/service_framework/__init_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1687 2023-06-20 15:06:26.000000 python-service-builder-1.0.0/service_framework/list_services.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3941 2023-06-20 16:02:27.000000 python-service-builder-1.0.0/service_framework/service_builder.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    14358 2023-06-20 15:33:57.000000 python-service-builder-1.0.0/service_framework/services.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1270 2023-06-20 15:45:57.000000 python-service-builder-1.0.0/service_framework/services_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/setup.cfg
```

### Comparing `python-service-builder-0.1.0/service_framework/list_services.py` & `python-service-builder-1.0.0/service_framework/list_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from absl import app
 import urllib.request
 from contextlib import closing, suppress
 from urllib.request import urlopen
 import urllib.parse
 import json
 
-
+""" _summary_
+"""
 def main(unused):
   del unused
 
   Components = namedtuple(
       typename='Components',
       field_names=['scheme', 'netloc', 'url', 'path', 'query', 'fragment']
   )
```

### Comparing `python-service-builder-0.1.0/service_framework/service_builder.py` & `python-service-builder-1.0.0/service_framework/service_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,29 +25,30 @@
 import google_auth_httplib2
 from apiclient import discovery
 from google.auth import exceptions
 from google.oauth2 import credentials as oauth
 from httplib2 import Http
 from oauth2client import service_account
 
-from .services import Service
-from . import field
+from service_framework.services import Service
+from service_framework import snake_field
 
-@dataclasses_json.dataclass_json(letter_case=dataclasses_json.LetterCase.CAMEL)
+
+@dataclasses_json.dataclass_json
 @dataclasses.dataclass
 class OAuthKey(object):
   """Dataclass from the json key.
 
   NOTE: This is by no means the entire key; just the fields neccessary for OAuth.
   """
-  access_token: Optional[str] = field(field_name='token')
-  refresh_token: Optional[str] = field()
-  token_uri: Optional[str] = field()
-  client_id: Optional[str] = field()
-  client_secret: Optional[str] = field()
+  access_token: Optional[str] = snake_field(field_name='token')
+  refresh_token: Optional[str] = snake_field()
+  token_uri: Optional[str] = snake_field()
+  client_id: Optional[str] = snake_field()
+  client_secret: Optional[str] = snake_field()
 
 
 def build_service(service: Service,
                   key: Union[OAuthKey, oauth.Credentials,
                              str, Mapping[str, str]],
                   api_key: Optional[str] = None,
                   extra_scopes: Optional[List[str]] = None) -> discovery.Resource:
@@ -116,14 +117,14 @@
             key, scopes=extra_scopes)
     https = credentials.authorize(Http())
 
   else:
     raise Exception('No valid credentials provided.')
 
   discovery_args = {
-    'http': https,
-    'developerKey': api_key,
-    'cache_discovery': False,
-    **definition.to_dict()
+      'http': https,
+      'developerKey': api_key,
+      'cache_discovery': False,
+      **definition.to_dict()
   }
 
   return discovery.build(**discovery_args)
```

### Comparing `python-service-builder-0.1.0/service_framework/services.py` & `python-service-builder-1.0.0/service_framework/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,32 @@
 import dataclasses
 import enum
 from typing import Any, Optional
 
 import dataclasses_json
 import immutabledict
 
-from . import field, lazy_property
+from . import camel_field, lazy_property
 
 
 @dataclasses_json.dataclass_json
 @dataclasses.dataclass
 class ServiceDefinition(object):
-  service_name: Optional[str] = field()
-  version: Optional[str] = field()
-  discovery_service_url: Optional[str] = field()
+  """Defines a Google Service for the builder."""
+  service_name: Optional[str] = camel_field()
+  version: Optional[str] = camel_field()
+  discovery_service_url: Optional[str] = camel_field()
 
 
 class S(enum.Enum):
+  """Defines the generic Enum for any service.
+
+  Raises:
+      ValueError: if no enum is defined.
+  """
   @lazy_property
   def definition(self) -> ServiceDefinition:
     """Fetch the ServiceDefinition.
 
     Lazily returns the dataclass containing the service definition
     details. It has to be lazy, as it can't be defined at
     initialization time.
@@ -48,15 +54,26 @@
         service_name=service_name,
         version=version,
         discovery_service_url=(
             f'https://{service_name}.googleapis.com/$discovery/rest'
             f'?version={version}'))
 
   @classmethod
-  def from_value(cls, value) -> S:
+  def from_value(cls, value: str) -> S:
+    """Creates a service enum from the name of the service.
+
+    Args:
+        value (str): the service name
+
+    Raises:
+        ValueError: no service found
+
+    Returns:
+        S: the service definition
+    """
     for k, v in cls.__members__.items():
       if k == value.upper():
         return v
     else:
       raise ValueError(f"'{cls.__name__}' enum not found for '{value}'")
```

### Comparing `python-service-builder-0.1.0/service_framework/services_test.py` & `python-service-builder-1.0.0/service_framework/services_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,26 +13,23 @@
 # limitations under the License.
 import unittest
 
 from service_framework import services
 
 SA360_DEFINITION = \
     services.ServiceDefinition(
-        name='doubleclicksearch',
-        uri='https://doubleclicksearch.googleapis.com/$discovery/rest?version=v2',
+        service_name='doubleclicksearch',
+        discovery_service_url='https://doubleclicksearch.googleapis.com/$discovery/rest?version=v2',
         version='v2')
 GMAIL_ARGS = {
     'serviceName': 'gmail',
     'discoveryServiceUrl': 'https://gmail.googleapis.com/$discovery/rest?version=v1',
     'version': 'v1',
 }
 
 
 class ServicesTest(unittest.TestCase):
   def test_valid_service(self):
-    self.assertGreater(services.Service.SA360.value, 0)
+    self.assertGreater(services.Service.DOUBLECLICKSEARCH.value, 0)
 
   def test_single_definition(self):
-    self.assertEqual(SA360_DEFINITION, services.Service.SA360.definition)
-
-  def test_single_to_args(self):
-    self.assertEqual(GMAIL_ARGS, services.Service.GMAIL.definition.to_args)
+    self.assertEqual(SA360_DEFINITION, services.Service.DOUBLECLICKSEARCH.definition)
```

