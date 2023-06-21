# Comparing `tmp/ens_sdk-0.0.8.tar.gz` & `tmp/ens_sdk-0.0.9.tar.gz`

## Comparing `ens_sdk-0.0.8.tar` & `ens_sdk-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/src/ens_sdk/__init__.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/src/ens_sdk/ens.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/src/ens_sdk/utils/__init__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/src/ens_sdk/utils/cache.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/src/ens_sdk/utils/decouple.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/src/ens_sdk/utils/timezone.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/LICENSE
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 ens_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/src/ens_sdk/__init__.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/src/ens_sdk/ens.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/src/ens_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/src/ens_sdk/utils/cache.py
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/src/ens_sdk/utils/decouple.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/src/ens_sdk/utils/timezone.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/LICENSE
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 ens_sdk-0.0.9/PKG-INFO
```

### Comparing `ens_sdk-0.0.8/.DS_Store` & `ens_sdk-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.8/src/ens_sdk/ens.py` & `ens_sdk-0.0.9/src/ens_sdk/ens.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         credentials = "{0}:{1}".format(self._CLIENT_ID, self._CLIENT_SECRET)
         authorization = base64.b64encode(credentials.encode("utf-8"))
         headers = {"Content-Type": "application/x-www-form-urlencoded", "Cache-Control": "no-cache", "Authorization": f"Basic {authorization.decode('utf-8')}"}
         payload = dict(grant_type='client_credentials')
         response = self._send(endpoint='oauth/token/', headers=headers, payload=dict(data=payload), authenticate=False)
         self._cache.store(self._ENS_SERVER, response) if response.get('access_token', None) else print(f'Failed to authenticate:: {response}')
 
-    def send_message(self, message: str) -> dict:
+    def send_message(self, message: dict) -> dict:
         response = self.process(endpoint='notification/send/', payload=message, method='POST')
         return response
 
     def process(self, endpoint: str, payload, method: str, headers: dict = None):
         _ = self.token_expire_handler()
 
         payload = dict(params=payload) if method == 'GET' else dict(json=payload)
```

### Comparing `ens_sdk-0.0.8/src/ens_sdk/utils/cache.py` & `ens_sdk-0.0.9/src/ens_sdk/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.8/src/ens_sdk/utils/decouple.py` & `ens_sdk-0.0.9/src/ens_sdk/utils/decouple.py`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.8/LICENSE` & `ens_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.8/pyproject.toml` & `ens_sdk-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ens_sdk"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Joseph Daudi", email="joseph@encipher.dev" },
 ]
 dependencies = ['redis', 'pydantic', 'sentry_sdk', 'requests', 'esr-sdk', 'pytz']
 description = "An SDK to simplify connectivity to ENS Services"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ens_sdk-0.0.8/PKG-INFO` & `ens_sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ens_sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: An SDK to simplify connectivity to ENS Services
 Project-URL: Homepage, https://github.com/enciphertz/encipher-notificaition-service-python-sdk
 Project-URL: Bug Tracker, https://github.com/enciphertz/encipher-notificaition-service-python-sdk/issues
 Author-email: Joseph Daudi <joseph@encipher.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

