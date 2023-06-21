# Comparing `tmp/nqgreenapi-1.0.0a3.tar.gz` & `tmp/nqgreenapi-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nqgreenapi-1.0.0a3.tar", max compression
+gzip compressed data, was "nqgreenapi-1.0.0a4.tar", max compression
```

## Comparing `nqgreenapi-1.0.0a3.tar` & `nqgreenapi-1.0.0a4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      557 2023-05-15 11:41:54.752522 nqgreenapi-1.0.0a3/LICENSE
--rw-r--r--   0        0        0      358 2023-06-19 11:01:49.933710 nqgreenapi-1.0.0a3/README.md
--rw-r--r--   0        0        0      661 2023-05-20 13:59:37.932301 nqgreenapi-1.0.0a3/nqgreenapi/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-18 17:50:08.352808 nqgreenapi-1.0.0a3/nqgreenapi/callback.py
--rw-r--r--   0        0        0     1715 2023-05-18 09:21:41.441545 nqgreenapi-1.0.0a3/nqgreenapi/message.py
--rw-r--r--   0        0        0     5093 2023-06-19 11:01:49.945710 nqgreenapi-1.0.0a3/nqgreenapi/provider.py
--rw-r--r--   0        0        0      580 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a3/nqgreenapi/quotas.py
--rw-r--r--   0        0        0      331 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a3/nqgreenapi/resources/config_schema.json
--rw-r--r--   0        0        0     1380 2023-06-19 11:01:49.945710 nqgreenapi-1.0.0a3/nqgreenapi/serializers.py
--rw-r--r--   0        0        0      854 2023-05-18 14:20:08.482922 nqgreenapi-1.0.0a3/nqgreenapi/utils.py
--rw-r--r--   0        0        0     1759 2023-06-19 11:38:45.950126 nqgreenapi-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 nqgreenapi-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-05-15 11:41:54.752522 nqgreenapi-1.0.0a4/LICENSE
+-rw-r--r--   0        0        0      358 2023-06-19 11:01:49.933710 nqgreenapi-1.0.0a4/README.md
+-rw-r--r--   0        0        0      661 2023-05-20 13:59:37.932301 nqgreenapi-1.0.0a4/nqgreenapi/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-18 17:50:08.352808 nqgreenapi-1.0.0a4/nqgreenapi/callback.py
+-rw-r--r--   0        0        0      626 2023-06-21 14:08:51.001483 nqgreenapi-1.0.0a4/nqgreenapi/exceptions.py
+-rw-r--r--   0        0        0     1715 2023-05-18 09:21:41.441545 nqgreenapi-1.0.0a4/nqgreenapi/message.py
+-rw-r--r--   0        0        0     5636 2023-06-21 14:08:51.001483 nqgreenapi-1.0.0a4/nqgreenapi/provider.py
+-rw-r--r--   0        0        0      580 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a4/nqgreenapi/quotas.py
+-rw-r--r--   0        0        0      331 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a4/nqgreenapi/resources/config_schema.json
+-rw-r--r--   0        0        0     1380 2023-06-19 11:01:49.945710 nqgreenapi-1.0.0a4/nqgreenapi/serializers.py
+-rw-r--r--   0        0        0      854 2023-05-18 14:20:08.482922 nqgreenapi-1.0.0a4/nqgreenapi/utils.py
+-rw-r--r--   0        0        0     1759 2023-06-21 19:29:54.365922 nqgreenapi-1.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 nqgreenapi-1.0.0a4/PKG-INFO
```

### Comparing `nqgreenapi-1.0.0a3/LICENSE` & `nqgreenapi-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a3/nqgreenapi/__init__.py` & `nqgreenapi-1.0.0a4/nqgreenapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a3/nqgreenapi/callback.py` & `nqgreenapi-1.0.0a4/nqgreenapi/callback.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a3/nqgreenapi/message.py` & `nqgreenapi-1.0.0a4/nqgreenapi/message.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a3/nqgreenapi/provider.py` & `nqgreenapi-1.0.0a4/nqgreenapi/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from nqsdk.exceptions import (
     CallbackHandlingException,
     SentException,
     UnsupportedCallbackEventException,
 )
 
 from .callback import GreenApiCallbackResponse
+from .exceptions import CheckHealthError
 from .message import GreenApiExtIdCallbackMeta, GreenApiSentMeta
 from .serializers import (
     InstanceState,
     InstanceStateModel,
     InstanceStatus,
     InstanceStatusModel,
     MessageStatus,
@@ -74,21 +75,40 @@
     @classmethod
     def get_channels(cls) -> list[type[Channel]]:
         return [Channel.create(label="whatsapp", is_ack_supported=True, is_delivery_supported=True)]
 
     def check_health(self) -> bool:
         """Checks provider health."""
 
-        state_model = InstanceStateModel(**self._green_api.account.getStateInstance().data)
-        status_model = InstanceStatusModel(**self._green_api.account.getStatusInstance().data)
+        state_response = self._green_api.account.getStateInstance()
+        status_response = self._green_api.account.getStatusInstance()
 
-        return (
+        errors = []
+
+        if state_response.error:
+            errors.append(state_response.error)
+
+        if status_response.error:
+            errors.append(status_response.error)
+
+        if errors:
+            raise Exception("; ".join(errors))
+
+        state_model = InstanceStateModel(**state_response.data)
+        status_model = InstanceStatusModel(**status_response.data)
+
+        if not (
             state_model.stateInstance == InstanceState.authorized
             and status_model.statusInstance == InstanceStatus.online
-        )
+        ):
+            raise CheckHealthError(
+                f"State: {state_model.stateInstance}; Status: {status_model.statusInstance}"
+            )
+
+        return True
 
     def send(self, *, message: Message) -> GreenApiSentMeta:
         result = self._green_api.sending.sendMessage(
             chatId=f"{message.get_recipient_id()}@c.us",
             message=message.get_content(),
             linkPreview=False,
         )
```

### Comparing `nqgreenapi-1.0.0a3/nqgreenapi/quotas.py` & `nqgreenapi-1.0.0a4/nqgreenapi/quotas.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a3/nqgreenapi/serializers.py` & `nqgreenapi-1.0.0a4/nqgreenapi/serializers.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a3/nqgreenapi/utils.py` & `nqgreenapi-1.0.0a4/nqgreenapi/utils.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a3/pyproject.toml` & `nqgreenapi-1.0.0a4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry_core >= 1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nqgreenapi"
-version = "1.0.0-alpha-3"
+version = "1.0.0-alpha-4"
 description = "NQ GreenApi Provider"
 authors = [ "Inqana Ltd. <develop@inqana.com>",]
 readme = "README.md"
 classifiers = [ "Development Status :: 3 - Alpha", "Intended Audience :: Developers", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 
 [tool.setuptools]
 zip-safe = true
```

### Comparing `nqgreenapi-1.0.0a3/PKG-INFO` & `nqgreenapi-1.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nqgreenapi
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: NQ GreenApi Provider
 Author: Inqana Ltd.
 Author-email: develop@inqana.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

