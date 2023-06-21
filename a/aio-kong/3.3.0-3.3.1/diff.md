# Comparing `tmp/aio_kong-3.3.0.tar.gz` & `tmp/aio_kong-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_kong-3.3.0.tar", max compression
+gzip compressed data, was "aio_kong-3.3.1.tar", max compression
```

## Comparing `aio_kong-3.3.0.tar` & `aio_kong-3.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1461 2023-05-28 17:47:27.486255 aio_kong-3.3.0/LICENSE
--rw-r--r--   0        0        0       54 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/__init__.py
--rw-r--r--   0        0        0     2315 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/auths.py
--rw-r--r--   0        0        0      278 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/certificates.py
--rw-r--r--   0        0        0     1986 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/cli.py
--rw-r--r--   0        0        0     3783 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/client.py
--rw-r--r--   0        0        0     5342 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/components.py
--rw-r--r--   0        0        0     2720 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/consumers.py
--rw-r--r--   0        0        0     2685 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/plugins.py
--rw-r--r--   0        0        0     1526 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/routes.py
--rw-r--r--   0        0        0     2514 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/services.py
--rw-r--r--   0        0        0      665 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/snis.py
--rw-r--r--   0        0        0      931 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/utils.py
--rw-r--r--   0        0        0     1563 2023-05-28 17:47:27.486255 aio_kong-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     2192 2023-05-28 17:47:27.486255 aio_kong-3.3.0/readme.md
--rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 aio_kong-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-06-21 09:38:30.518849 aio_kong-3.3.1/LICENSE
+-rw-r--r--   0        0        0       54 2023-06-21 09:38:30.518849 aio_kong-3.3.1/kong/__init__.py
+-rw-r--r--   0        0        0     2314 2023-06-21 09:38:30.518849 aio_kong-3.3.1/kong/auths.py
+-rw-r--r--   0        0        0      278 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/certificates.py
+-rw-r--r--   0        0        0     1986 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/cli.py
+-rw-r--r--   0        0        0     3783 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/client.py
+-rw-r--r--   0        0        0     5342 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/components.py
+-rw-r--r--   0        0        0     2720 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/consumers.py
+-rw-r--r--   0        0        0     2685 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/plugins.py
+-rw-r--r--   0        0        0        0 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/py.typed
+-rw-r--r--   0        0        0     1482 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/routes.py
+-rw-r--r--   0        0        0     2514 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/services.py
+-rw-r--r--   0        0        0      665 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/snis.py
+-rw-r--r--   0        0        0      931 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/utils.py
+-rw-r--r--   0        0        0     1778 2023-06-21 09:38:30.522849 aio_kong-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2192 2023-06-21 09:38:30.522849 aio_kong-3.3.1/readme.md
+-rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 aio_kong-3.3.1/PKG-INFO
```

### Comparing `aio_kong-3.3.0/LICENSE` & `aio_kong-3.3.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Quantmind
+Copyright (c) 2023 Quantmind
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
  * Redistributions in binary form must reproduce the above copyright notice,
```

### Comparing `aio_kong-3.3.0/kong/auths.py` & `aio_kong-3.3.1/kong/auths.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 def auth_factory(consumer: Consumer, auth_type: str) -> ConsumerAuth:
     known_types = {"basic-auth": BasicAuth, "key-auth": KeyAuth}
     constructor = known_types.get(auth_type, ConsumerAuth)
     return constructor(consumer, auth_type)
 
 
 class ConsumerAuth(CrudComponent):
-
     unique_field: str = ""
 
     @property
     def url(self) -> str:
         return f"{self.root.url}/{self.name}"
 
     async def get_existing_id(self, creds_config: dict) -> str | None:
```

### Comparing `aio_kong-3.3.0/kong/cli.py` & `aio_kong-3.3.1/kong/cli.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/kong/client.py` & `aio_kong-3.3.1/kong/client.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/kong/components.py` & `aio_kong-3.3.1/kong/components.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/kong/consumers.py` & `aio_kong-3.3.1/kong/consumers.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/kong/plugins.py` & `aio_kong-3.3.1/kong/plugins.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/kong/routes.py` & `aio_kong-3.3.1/kong/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,17 @@
             name = entry.get("name")
             route = route_map.pop(name, None) if name else None
             entry = entry.copy()
             plugins = entry.pop("plugins", [])
             as_list("hosts", entry)
             as_list("paths", entry)
             as_list("methods", entry)
-            if not route:
-                entity = await self.create(**entry)
-            else:
-                entity = await self.update(route.id, **entry)
+            if route:
+                await self.delete(route.id)
+            entity = await self.create(**entry)
             route = cast(KongEntityWithPlugins, entity)
             route.data["plugins"] = await route.plugins.apply_json(plugins)
             result.append(route.data)
         if clear:
             for route in route_map.values():
                 await self.delete(route.id)
         return result
```

### Comparing `aio_kong-3.3.0/kong/services.py` & `aio_kong-3.3.1/kong/services.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/kong/snis.py` & `aio_kong-3.3.1/kong/snis.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/kong/utils.py` & `aio_kong-3.3.1/kong/utils.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/pyproject.toml` & `aio_kong-3.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-kong"
-version = "3.3.0"
+version = "3.3.1"
 description = "Asynchronous Kong Client"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD-3-Clause"
 readme = "readme.md"
 packages = [
     {include = "kong"}
 ]
@@ -33,24 +33,42 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 aiohttp = "^3.8.1"
 click = "^8.1.3"
 PyYAML = "^6.0"
 
-[tool.poetry.dev-dependencies]
-black = "^22.6.0"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
 isort = "^5.10.1"
-mypy = "^0.991"
+mypy = "^1.4.0"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
-flake8 = "^6.0.0"
-flake8-blind-except = "^0.2.0"
-codecov = "^2.1.12"
-coverage = "^6.2"
-python-dotenv = "^0.21.0"
-pytest-asyncio = "^0.20.1"
+python-dotenv = "^1.0.0"
+pytest-asyncio = "^0.21.0"
 types-PyYAML = "^6.0.11"
+ruff = "^0.0.274"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+testpaths = [
+    "tests"
+]
+
+
+[tool.isort]
+profile = "black"
+
+[tool.ruff]
+select = ["E", "F"]
+line-length = 88
+
+[tool.mypy]
+disallow_untyped_calls = true
+warn_return_any = false
+disallow_untyped_defs = true
+warn_no_return = true
```

### Comparing `aio_kong-3.3.0/readme.md` & `aio_kong-3.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.0/PKG-INFO` & `aio_kong-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-kong
-Version: 3.3.0
+Version: 3.3.1
 Summary: Asynchronous Kong Client
 License: BSD-3-Clause
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

