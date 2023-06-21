# Comparing `tmp/gestalt-cfg-3.2.0.tar.gz` & `tmp/gestalt-cfg-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gestalt-cfg-3.2.0.tar", last modified: Fri Jun  2 00:26:43 2023, max compression
+gzip compressed data, was "gestalt-cfg-3.3.0.tar", last modified: Wed Jun 21 17:34:37 2023, max compression
```

## Comparing `gestalt-cfg-3.2.0.tar` & `gestalt-cfg-3.3.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/gestalt/
--rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/gestalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/gestalt/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/gestalt/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-02 00:26:43.462014 gestalt-cfg-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/tests/test_gestalt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.277049 gestalt-cfg-3.3.0/gestalt/
+-rw-r--r--   0 runner    (1001) docker     (123)    25398 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/test_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/test_vault.py
```

### Comparing `gestalt-cfg-3.2.0/LICENSE` & `gestalt-cfg-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.2.0/PKG-INFO` & `gestalt-cfg-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.2.0
+Version: 3.3.0
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.2.0/README.md` & `gestalt-cfg-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.2.0/gestalt/__init__.py` & `gestalt-cfg-3.3.0/gestalt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from gestalt.vault import Vault
+from gestalt.vault import Vault  # noqa: E999
 from gestalt.provider import Provider
 import os
 import glob
-import collections.abc as collections
+
 from typing import Dict, List, Type, Union, Optional, MutableMapping, Text, Any
 import yaml
 import re
 import json
 
+from .utils import flatten
+
 
 def merge_into(
         a: Dict[Text, Union[List[Any], Text, int, bool, float]],
         b: Dict[Text, Union[List[Any], Text, int, bool, float]]) -> None:
     """ merge_into merges a into b"""
     for k, v in a.items():
         if isinstance(v, dict):
@@ -45,29 +47,14 @@
         self.__conf_defaults: Dict[Text, Union[List[Any], Text, int, bool,
                                                float]] = dict()
         self.providers: Dict[str, Provider] = dict()
         self.__secret_map: Dict[str, List[str]] = {}
         self.regex_pattern = re.compile(
             r"^ref\+([^\+]*)://([^(\+)]+)\#([^\+]+)?$")
 
-    def __flatten(
-        self,
-        d: MutableMapping[Text, Any],
-        parent_key: str = '',
-        sep: str = '.'
-    ) -> Dict[Text, Union[List[Any], Text, int, bool, float]]:
-        items: List[Any] = []
-        for k, v in d.items():
-            new_key = parent_key + sep + k if parent_key else k
-            if isinstance(v, collections.MutableMapping):
-                items.extend(self.__flatten(v, new_key, sep=sep).items())
-            else:
-                items.append((new_key, v))
-        return dict(items)
-
     def add_config_path(self, path: str) -> None:
         """Adds a path to read configs from.
 
         Configurations are read in the order they are added in, and overlapping keys are
         overwritten in that same order, so the last config path added has the highest
         priority.
 
@@ -158,21 +145,18 @@
                         yaml_dict = yaml.load(yf, Loader=yaml.FullLoader)
                         merge_into(yaml_dict, self.__conf_data)
                 except yaml.YAMLError as e:
                     raise ValueError(
                         f'File {f} is marked as ".yaml" but cannot be read as such: {e}'
                     )
 
-        self.__conf_data = self.__flatten(self.__conf_data,
-                                          sep=self.__delim_char)
+        self.__conf_data = flatten(self.__conf_data, sep=self.__delim_char)
 
         self.__parse_dictionary_keys(self.__conf_data)
-        self.__conf_data = self.__interpolate_keys(self.__conf_data)
         self.__parse_dictionary_keys(self.__conf_sets)
-        self.__conf_sets = self.__interpolate_keys(self.__conf_sets)
 
     def __parse_dictionary_keys(
         self, dictionary: Dict[str, Union[List[Any], str, int, bool, float]]
     ) -> None:
         """Parses the keys in the configuration data.
 
         Raises:
@@ -204,32 +188,14 @@
             TypeError: If the provider is not an instance of the Provider class
         """
         if provider_name == "vault" and isinstance(provider, Vault):
             self.providers.update({"vault": provider})
         else:
             raise TypeError("Provider provider is not supported")
 
-    def __interpolate_keys(
-        self, dictionary: Dict[str, Union[List[Any], str, int, bool, float]]
-    ) -> Dict[str, Union[List[Any], str, int, bool, float]]:
-        """Interpolates the keys in the configuration data.
-        """
-        for path, v in self.__secret_map.items():
-            m = self.regex_pattern.search(path)
-            if m is not None:
-                provider = self.providers[m.group(1)]
-                for config_key in v:
-                    secret = provider.get(key=config_key,
-                                          path=m.group(2),
-                                          filter=m.group(3))
-                    dictionary.update({config_key: secret})
-
-        dictionary = self.__flatten(dictionary, sep=self.__delim_char)
-        return dictionary
-
     def auto_env(self) -> None:
         """Auto env provides sane defaults for using environment variables
 
         Specifically, auto_env will enable the use of environment variables and
         will also clear the prefix for environment variables.
         """
         self.__use_env = True
@@ -423,45 +389,26 @@
     ) -> Union[str, int, float, bool, List[Any]]:
         if not isinstance(key, str):
             raise TypeError(f'Given key is not of string type')
         if default and not isinstance(default, t):
             raise TypeError(
                 f'Provided default is of incorrect type {type(default)}, it should be of type {t}'
             )
-        if key in self.__conf_sets:
-            val = self.__conf_sets[key]
-            if not isinstance(val, t):
-                raise TypeError(
-                    f'Given set key is not of type {t}, but of type {type(val)}'
-                )
-            return val
-        if self.__use_env:
-            e_key = key.upper().replace(self.__delim_char, '_')
-            if e_key in os.environ:
-                try:
-                    return t(os.environ[e_key])
-                except ValueError as e:
-                    raise TypeError(
-                        f'The environment variable {e_key} could not be converted to type {t}: {e}'
-                    )
-        if key in self.__conf_data:
-            if not isinstance(self.__conf_data[key], t):
-                raise TypeError(
-                    f'The requested key of {key} is not of type {t} (it is {type(self.__conf_data[key])})'
-                )
-            return self.__conf_data[key]
-        if default:
-            return default
-        if key in self.__conf_defaults:
-            val = self.__conf_defaults[key]
-            if not isinstance(val, t):
-                raise TypeError(
-                    f'Given default set key is not of type {t}, but of type {type(val)}'
-                )
-            return val
+        split_keys = key.split(self.__delim_char)
+        consider_keys = list()
+        for split_key in split_keys:
+            consider_keys.append(split_key)
+            joined_key = self.__delim_char.join(consider_keys)
+            config_val = self._get_config_for_key(key=key,
+                                                  key_to_search=joined_key,
+                                                  default=default,
+                                                  object_type=t)
+            if config_val is not None:
+                return config_val
+
         raise ValueError(
             f'Given key {key} is not in any configuration and no default is provided'
         )
 
     def get_string(self, key: str, default: Optional[Text] = None) -> str:
         """Gets the configuration string for a given key
 
@@ -593,7 +540,68 @@
         Returns:
             str: JSON string representation
         """
         ret: Dict[str, Any] = self.__conf_defaults
         ret.update(self.__conf_data)
         ret.update(self.__conf_sets)
         return str(json.dumps(ret, indent=4))
+
+    def _get_config_for_key(
+        self, key: str, key_to_search: str,
+        default: Optional[Union[str, int, float, bool, List[Any]]],
+        object_type: Type[Union[str, int, float, bool, List[Any]]]
+    ) -> Optional[Union[str, int, float, bool, List[Any]]]:
+        if key_to_search in self.__conf_sets:
+            val = self.__conf_sets[key_to_search]
+            if not isinstance(val, object_type):
+                raise TypeError(
+                    f'Given set key is not of type {object_type}, but of type {type(val)}'
+                )
+            return val
+        if self.__use_env:
+            e_key = key_to_search.upper().replace(self.__delim_char, '_')
+            if e_key in os.environ:
+                try:
+                    return object_type(os.environ[e_key])
+                except ValueError as e:
+                    raise TypeError(
+                        f'The environment variable {e_key} could not be converted to type {object_type}: {e}'
+                    )
+
+        if key_to_search in self.__conf_data:
+            val = self.__conf_data[key_to_search]
+            for provider in self.providers.values():
+                if isinstance(val, str) and val.startswith(provider.scheme):
+                    regex_search = self.regex_pattern.search(val)
+                    if regex_search is not None:
+                        path = regex_search.group(2)
+                        filter_ = regex_search.group(3)
+                        remainder_filter = key[len(key_to_search):]
+                        if len(remainder_filter) > 1:
+                            if filter_ is not None:
+                                filter_ = f".{filter_}{remainder_filter}"
+
+                            else:
+                                filter_ = remainder_filter
+
+                        interpolated_val = provider.get(key=val,
+                                                        path=path,
+                                                        filter=filter_,
+                                                        sep=self.__delim_char)
+                        break
+            else:
+                interpolated_val = val
+            if not isinstance(interpolated_val, object_type):
+                raise TypeError(
+                    f'Given set key is not of type {object_type}, but of type {type(interpolated_val)}'
+                )
+            return interpolated_val
+        if default:
+            return default
+        if key_to_search in self.__conf_defaults:
+            val = self.__conf_defaults[key_to_search]
+            if not isinstance(val, object_type):
+                raise TypeError(
+                    f'Given default set key is not of type {object_type}, but of type {type(val)}'
+                )
+            return val
+        return None
```

### Comparing `gestalt-cfg-3.2.0/gestalt/vault.py` & `gestalt-cfg-3.3.0/gestalt/vault.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from datetime import datetime, timedelta
 from time import sleep
 from gestalt.provider import Provider
 import requests
 from jsonpath_ng import parse  # type: ignore
-from typing import Optional, Tuple, Any
+from typing import Optional, Tuple, Any, Dict, Union, List
 import hvac  # type: ignore
 import asyncio
 import os
 from threading import Thread
 from retry import retry
 
 
@@ -14,31 +15,36 @@
     @retry(exceptions=RuntimeError, delay=2, tries=5)  # type: ignore
     def __init__(self,
                  cert: Optional[Tuple[str, str]] = None,
                  role: Optional[str] = None,
                  jwt: Optional[str] = None,
                  url: Optional[str] = os.environ.get("VAULT_ADDR"),
                  token: Optional[str] = os.environ.get("VAULT_TOKEN"),
-                 verify: Optional[bool] = True) -> None:
+                 verify: Optional[bool] = True,
+                 scheme: str = "ref+vault://") -> None:
         """Initialized vault client and authenticates vault
 
         Args:
             client_config (HVAC_ClientConfig): initializes vault. URL can be set in VAULT_ADDR
                 environment variable, token can be set to VAULT_TOKEN environment variable.
                 These will be picked by default if not set to empty string
             auth_config (HVAC_ClientAuthentication): authenticates the initialized vault client
                 with role and jwt string from kubernetes
         """
+        self._scheme: str = scheme
         self.dynamic_token_queue: asyncio.Queue[Any] = asyncio.Queue(maxsize=0)
         self.kubes_token_queue: asyncio.Queue[Any] = asyncio.Queue(maxsize=0)
 
         self.vault_client = hvac.Client(url=url,
                                         token=token,
                                         cert=cert,
                                         verify=verify)
+        self._secret_expiry_times: Dict[str, datetime] = dict()
+        self._secret_values: Dict[str, Union[str, int, float, bool,
+                                             List[Any]]] = dict()
 
         try:
             self.vault_client.is_authenticated()
         except requests.exceptions.MissingSchema:
             raise RuntimeError(
                 "Gestalt Error: Unable to connect to vault with the given configuration"
             )
@@ -69,23 +75,39 @@
                                           target=asyncio.run,
                                           daemon=True,
                                           args=(self.worker(
                                               self.kubes_token_queue), ))
             kubernetes_ttl_renew.start()
 
     @retry(RuntimeError, delay=3, tries=3)  # type: ignore
-    def get(self, key: str, path: str, filter: str) -> Any:
+    def get(
+        self,
+        key: str,
+        path: str,
+        filter: str,
+        sep: Optional[str] = "."
+    ) -> Union[str, int, float, bool, List[Any]]:
         """Gets secret from vault
         Args:
             key (str): key to get secret from
             path (str): path to secret
             filter (str): filter to apply to secret
+            sep (str): delimiter used for flattening
         Returns:
             secret (str): secret
         """
+        # if the key has been read before and is not a TTL secret
+        if key in self._secret_values and key not in self._secret_expiry_times:
+            return self._secret_values[key]
+
+        # if the secret can expire but hasn't expired yet
+        if key in self._secret_expiry_times and not self._is_secret_expired(
+                key):
+            return self._secret_values[key]
+
         try:
             response = self.vault_client.read(path)
             if response is None:
                 raise RuntimeError("Gestalt Error: No secrets found")
             if response['lease_id']:
                 dynamic_token = ("dynamic", response['lease_id'],
                                  response['lease_duration'])
@@ -105,15 +127,36 @@
         jsonpath_expression = parse(f"${filter}")
         match = jsonpath_expression.find(secret)
         if len(match) == 0:
             print("Path returned not matches for your secret")
         returned_value_from_secret = match[0].value
         if returned_value_from_secret == "":
             raise RuntimeError("Gestalt Error: Empty secret!")
-        return returned_value_from_secret
+
+        self._secret_values[key] = returned_value_from_secret
+        if "ttl" in requested_data:
+            self._set_secrets_ttl(requested_data, key)
+
+        return returned_value_from_secret  # type: ignore
+
+    def _is_secret_expired(self, key: str) -> bool:
+        now = datetime.now()
+        secret_expires_dt = self._secret_expiry_times[key]
+        is_expired = now >= secret_expires_dt
+        return is_expired
+
+    def _set_secrets_ttl(self, requested_data: Dict[str, Any],
+                         key: str) -> None:
+        last_vault_rotation_str = requested_data["last_vault_rotation"].split(
+            ".")[0]  # to the nearest second
+        last_vault_rotation_dt = datetime.strptime(last_vault_rotation_str,
+                                                   '%Y-%m-%dT%H:%M:%S')
+        ttl = requested_data["ttl"]
+        secret_expires_dt = last_vault_rotation_dt + timedelta(seconds=ttl)
+        self._secret_expiry_times[key] = secret_expires_dt
 
     async def worker(self, token_queue: Any) -> None:
         """
         Worker function to renew lease on expiry
         """
 
         try:
@@ -134,7 +177,11 @@
             raise RuntimeError(
                 "Gestalt Error: The lease path or mount is set incorrectly")
         except requests.exceptions.ConnectionError:
             raise RuntimeError(
                 "Gestalt Error: Gestalt couldn't connect to Vault")
         except Exception as err:
             raise RuntimeError(f"Gestalt Error: {err}")
+
+    @property
+    def scheme(self) -> str:
+        return self._scheme
```

### Comparing `gestalt-cfg-3.2.0/gestalt_cfg.egg-info/PKG-INFO` & `gestalt-cfg-3.3.0/gestalt_cfg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.2.0
+Version: 3.3.0
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.2.0/setup.py` & `gestalt-cfg-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("requirements.txt") as reqs_file:
     reqs = filter(lambda x: not x.startswith("-"), reqs_file.readlines())
     reqs_list = list(map(lambda x: x.rstrip(), reqs))
 
 setup(name='gestalt-cfg',
-      version='3.2.0',
+      version='3.3.0',
       description='A sensible configuration library for Python',
       long_description=readme(),
       long_description_content_type="text/markdown",
       url='https://github.com/clear-street/gestalt',
       author='Clear Street',
       author_email='engineering@clearstreet.io',
       license='MIT',
```

### Comparing `gestalt-cfg-3.2.0/tests/test_gestalt.py` & `gestalt-cfg-3.3.0/tests/test_gestalt.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,51 +5,14 @@
 from gestalt.vault import Vault
 from gestalt import merge_into
 import asyncio
 import pytest
 import os
 import gestalt
 import hvac
-import requests
-
-
-class MockSession(requests.Session):
-    def request(self, *_, **__):
-        resp = {
-            'request_id': '230f5e67-e55d-bdae-bd24-c7bc13c1a3e9',
-            'lease_id': '',
-            'renewable': False,
-            'lease_duration': 0,
-            'data': {
-                'last_vault_rotation': '2023-05-31T14:24:41.724285249Z',
-                'password': 'foo',
-                'rotation_period': 60,
-                'ttl': 0,
-                'username': 'foo'
-            },
-            'wrap_info': None,
-            'warnings': None,
-            'auth': None
-        }
-        return MockResponse(resp, 200)
-
-
-class MockResponse:
-    def __init__(self, json_data, status_code):
-        self.json_data = json_data
-        self.status_code = status_code
-        self.ok = True
-
-    def json(self):
-        return self.json_data
-
-
-@pytest.fixture
-def mock_db_role_request(mocker):
-    mocker.patch("requests.Session", MockSession)
 
 
 # Testing member function
 def test_merge_into():
     combine1 = {}
     combine2 = {}
     combine3 = {"local": 1234, "pg": {"host": "dict1_pg", "pass": "dict1_pg"}}
@@ -511,142 +474,75 @@
     g = gestalt.Gestalt()
     g.set_string('mykey', 'mystring')
     with pytest.raises(TypeError) as terr:
         g.set_default_int('mykey', 123)
         assert 'Set config has' in terr
 
 
-# Vault testing
-@pytest.fixture(scope="function")
-def env_setup():
-    os.environ['VAULT_ADDR'] = "http://localhost:8200"
-    os.environ['VAULT_TOKEN'] = "myroot"
-
-
-def test_vault_setup(env_setup):
+def test_vault_setup():
     vault = Vault(role=None, jwt=None)
     assert vault.vault_client.is_authenticated() is True
 
 
-@pytest.fixture(scope="function")
-def incorrect_env_setup():
-    os.environ['VAULT_ADDR'] = ""
-
-
-@pytest.fixture(scope="function")
-def secret_setup(env_setup):
-    client = hvac.Client()
-    client.secrets.kv.v2.create_or_update_secret(
-        path="test", secret=dict(test_secret="test_secret_password"))
-
-
 def test_vault_interpolation(secret_setup):
     g = gestalt.Gestalt()
     g.add_config_file("./tests/testvault/testcorrect.json")
     vault = Vault(role=None, jwt=None)
     g.configure_provider("vault", vault)
     g.build_config()
     secret = g.get_string("test_secret.test_secret")
     assert secret == "test_secret_password"
 
 
-@pytest.fixture(scope="function")
-def mount_setup(env_setup):
-    client = hvac.Client()
-    secret_engines_list = client.sys.list_mounted_secrets_engines(
-    )['data'].keys()
-    if "test-mount/" in secret_engines_list:
-        client.sys.disable_secrets_engine(path="test-mount")
-    client.sys.enable_secrets_engine(backend_type="kv", path="test-mount")
-    client.secrets.kv.v2.create_or_update_secret(
-        mount_point="test-mount",
-        path="test",
-        secret=dict(test_mount="test_mount_password"))
-
-
-def test_vault_mount_path(env_setup, mount_setup):
+def test_vault_mount_path(mount_setup):
     g = gestalt.Gestalt()
     g.add_config_file("./tests/testvault/testmount.json")
     g.configure_provider("vault", Vault(role=None, jwt=None))
     g.build_config()
     secret = g.get_string("test_mount.test_mount")
     assert secret == "test_mount_password"
 
 
-def test_vault_incorrect_path(env_setup, mount_setup):
+def test_vault_incorrect_path(mount_setup):
     g = gestalt.Gestalt()
     g.add_config_file("./tests/testvault/testincorrectmount.json")
     g.configure_provider("vault", Vault(role=None, jwt=None))
     with pytest.raises(RuntimeError):
         g.build_config()
+        g.get_string("test_mount")
 
 
-@pytest.fixture(scope="function")
-def mount_setup(env_setup):
-    client = hvac.Client()
-    secret_engines_list = client.sys.list_mounted_secrets_engines(
-    )['data'].keys()
-    if "test-mount/" in secret_engines_list:
-        client.sys.disable_secrets_engine(path="test-mount")
-    client.sys.enable_secrets_engine(backend_type="kv", path="test-mount")
-    client.secrets.kv.v2.create_or_update_secret(
-        mount_point="test-mount",
-        path="test",
-        secret=dict(test_mount="test_mount_password"))
-
-
-@pytest.fixture(scope="function")
-def nested_setup(env_setup):
-    client = hvac.Client()
-    client.secrets.kv.v2.create_or_update_secret(
-        path="testnested", secret=dict(slack={"token": "random-token"}))
-
-
-def test_nest_key_for_vault(env_setup, nested_setup):
+def test_nest_key_for_vault(nested_setup, secret_setup):
     g = gestalt.Gestalt()
     g.add_config_file("./tests/testvault/testnested.json")
     g.configure_provider("vault", Vault(role=None, jwt=None))
     g.build_config()
     secret_db = g.get_string("remoteAPI.database.test_secret")
     secret_slack = g.get_string("remoteAPI.slack.token")
     assert secret_db == "test_secret_password"
     assert secret_slack == "random-token"
 
 
-def test_read_no_nest_db_role(env_setup, mock_db_role_request):
+def test_read_no_nest_db_role(mock_db_role_request):
     g = gestalt.Gestalt()
     g.add_config_file("./tests/testvault/testsfdynamic.json")
     g.configure_provider("vault", Vault(role=None, jwt=None))
     g.build_config()
-    secret_username = g.get_string("snowflake.username")
+    secret_username = g.get_string("username")
     assert secret_username == "foo"
 
 
-def test_set_vault_key(env_setup, nested_setup):
+def test_set_vault_key(nested_setup):
     g = gestalt.Gestalt()
     g.configure_provider("vault", Vault(role=None, jwt=None))
     g.set_string(key="test",
                  value="ref+vault://secret/data/testnested#.slack.token")
     g.build_config()
     secret = g.get_string("test")
-    assert secret == "random-token"
-
-
-@pytest.fixture
-def mock_vault_workers():
-    mock_dynamic_renew = Mock()
-    mock_k8s_renew = Mock()
-    patch("gestalt.vault.Thread",
-          side_effect=[mock_dynamic_renew, mock_k8s_renew]).start()
-    return (mock_dynamic_renew, mock_k8s_renew)
-
-
-@pytest.fixture
-def mock_vault_k8s_auth():
-    return patch("gestalt.vault.hvac.api.auth_methods.Kubernetes").start()
+    assert secret == "ref+vault://secret/data/testnested#.slack.token"
 
 
 @pytest.mark.asyncio
 async def test_vault_worker_dynamic(mock_vault_workers, mock_vault_k8s_auth):
     mock_dynamic_renew, mock_k8s_renew = mock_vault_workers
 
     mock_sleep = None
@@ -670,15 +566,14 @@
             with pytest.raises(RuntimeError):
                 await v.worker(test_token_queue)
 
             mock_sleep.assert_called()
             mock_client().sys.renew_lease.assert_called()
             mock_k8s_renew.start.assert_called_once()
 
-            mock_vault_k8s_auth.stop()
             mock_dynamic_renew.stop()
             mock_k8s_renew.stop()
 
 
 @pytest.mark.asyncio
 async def test_vault_worker_k8s(mock_vault_workers):
     mock_dynamic_renew, mock_k8s_renew = mock_vault_workers
@@ -716,30 +611,33 @@
     mock_response = {
         "lease_id": "1",
         "lease_duration": 5,
         "data": {
             "data": "mock_data"
         }
     }
-    mock_vault_client_read = patch("gestalt.vault.hvac.Client.read",
-                                   return_value=mock_response).start()
-
-    mock_dynamic_token_queue = Mock()
-    mock_kube_token_queue = Mock()
-    mock_queues = patch(
-        "gestalt.vault.asyncio.Queue",
-        side_effect=[mock_dynamic_token_queue, mock_kube_token_queue]).start()
-
-    v = Vault(role=None, jwt=None)
-    g = gestalt.Gestalt()
-    g.add_config_file("./tests/testvault/testmount.json")
-    g.configure_provider("vault", v)
-    g.build_config()
-
-    mock_vault_client_read.assert_called()
-    mock_dynamic_token_queue.put_nowait.assert_called()
 
-    mock_vault_client_read.stop()
-    mock_dynamic_token_queue.stop()
-    mock_kube_token_queue.stop()
-    mock_queues.stop()
-    mock_vault_client_read.stop()
+    mock_vault_client_patch = patch("gestalt.vault.hvac.Client.read",
+                                    return_value=mock_response)
+    with mock_vault_client_patch as mock_vault_client_read:
+        mock_dynamic_token_queue = Mock()
+        mock_kube_token_queue = Mock()
+        with patch(
+                "gestalt.vault.asyncio.Queue",
+                side_effect=[mock_dynamic_token_queue,
+                             mock_kube_token_queue]) as mock_queues:
+
+            v = Vault(role=None, jwt=None)
+            g = gestalt.Gestalt()
+            g.add_config_file("./tests/testvault/testmount.json")
+            g.configure_provider("vault", v)
+            g.build_config()
+            g.get_string("test_mount")
+
+            mock_vault_client_read.assert_called()
+            mock_dynamic_token_queue.put_nowait.assert_called()
+
+            mock_vault_client_read.stop()
+            mock_dynamic_token_queue.stop()
+            mock_kube_token_queue.stop()
+            mock_queues.stop()
+            mock_vault_client_read.stop()
```

