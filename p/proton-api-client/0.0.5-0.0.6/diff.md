# Comparing `tmp/proton-api-client-0.0.5.tar.gz` & `tmp/proton-api-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-api-client-0.0.5.tar", last modified: Tue Jun 20 23:41:09 2023, max compression
+gzip compressed data, was "proton-api-client-0.0.6.tar", last modified: Tue Jun 20 23:47:58 2023, max compression
```

## Comparing `proton-api-client-0.0.5.tar` & `proton-api-client-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/
--rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.5/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      922 2023-06-20 23:38:08.000000 proton-api-client-0.0.5/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:41:09.678403 proton-api-client-0.0.5/proton/
--rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.5/proton/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.5/proton/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-20 20:05:33.000000 proton-api-client-0.0.5/proton/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)     5861 2023-06-20 23:39:35.000000 proton-api-client-0.0.5/proton/client.py
--rw-r--r--   0 x         (1000) x         (1000)     2188 2023-06-20 19:43:36.000000 proton-api-client-0.0.5/proton/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     2017 2023-06-20 20:20:29.000000 proton-api-client-0.0.5/proton/helpers.py
--rw-r--r--   0 x         (1000) x         (1000)     1541 2023-06-20 23:40:32.000000 proton-api-client-0.0.5/proton/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/proton_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     1857 2023-06-20 23:38:08.000000 proton-api-client-0.0.5/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/
+-rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.6/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      922 2023-06-20 23:38:08.000000 proton-api-client-0.0.6/README.md
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/proton/
+-rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.6/proton/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.6/proton/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-20 20:05:33.000000 proton-api-client-0.0.6/proton/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     6009 2023-06-20 23:47:42.000000 proton-api-client-0.0.6/proton/client.py
+-rw-r--r--   0 x         (1000) x         (1000)     2188 2023-06-20 19:43:36.000000 proton-api-client-0.0.6/proton/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     2035 2023-06-20 23:47:42.000000 proton-api-client-0.0.6/proton/helpers.py
+-rw-r--r--   0 x         (1000) x         (1000)     1541 2023-06-20 23:40:32.000000 proton-api-client-0.0.6/proton/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/proton_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     1857 2023-06-20 23:47:42.000000 proton-api-client-0.0.6/setup.py
```

### Comparing `proton-api-client-0.0.5/LICENSE` & `proton-api-client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.5/PKG-INFO` & `proton-api-client-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `proton-api-client-0.0.5/README.md` & `proton-api-client-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.5/proton/_ctsrp.py` & `proton-api-client-0.0.6/proton/_ctsrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.5/proton/_pysrp.py` & `proton-api-client-0.0.6/proton/_pysrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.5/proton/client.py` & `proton-api-client-0.0.6/proton/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import platform
 from subprocess import Popen, PIPE
+from typing import List
 
 import gnupg
-from httpx import AsyncClient, Limits
+from httpx import AsyncClient, Limits, Response
 from tqdm.asyncio import tqdm_asyncio
 
 from .constants import PM_APP_VERSION_ACCOUNT
 from .login import login
 
 try:
     if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
@@ -32,49 +33,27 @@
         self.gpg_passphrase = gpg_passphrase
         self.client = login(username, password)
         self.api = 'https://api.protonmail.ch/api'
         self.mail_api = 'https://mail.proton.me/api'
         self.account_api = 'https://account.proton.me/api'
         self.assets = 'https://account.proton.me/assets'
 
-    def revoke_all_sessions(self):
-        return self._get(self.account_api, 'auth/v4/sessions').json()
-
-    def user_settings(self) -> dict:
-        return self._get(self.api, 'core/v4/settings').json()
-
-    def mail_settings(self) -> dict:
-        return self._get(self.api, 'mail/v4/settings').json()
-
-    def calendar_settings(self):
-        return self._get(self.api, 'settings/calendar').json()
-
-    def timezones(self):
-        return self._get(self.api, 'calendar/v1/timezones').json()
-
-    def addresses(self, params: dict = None) -> dict:
-        params = params or {
-            'Page': 0,
-            'PageSize': 150,  # max page size
-        }
-        return self._get(self.api, 'core/v4/addresses', params=params).json()
-
     def inbox(self, params: dict = None) -> dict:
         params = params or {
             'Page': 0,  # todo pagination
             'PageSize': 150,  # max page size
             'LabelID': 0,
             'Sort': 'Time',
             'Desc': 1,
             # 'Limit': 100,
             # 'Attachments': 1, # only get messages with attachments
         }
         return self._get(self.api, 'mail/v4/conversations', params=params).json()
 
-    def inbox_decrypted(self, params: dict = None):
+    def inbox_decrypted(self, params: dict = None) -> list[dict]:
         async def get(client: AsyncClient, _id: str) -> dict:
             r = await client.get(f'{self.api}/mail/v4/conversations/{_id}')
             conversation = r.json()
             messages = filter(None, (msg.get('Body') for msg in conversation.get('Messages', [])))
             decrypted = []
             for data in messages:
                 msg = await asyncio.to_thread(self.gpg_decrypt, data)
@@ -99,48 +78,70 @@
             'Sort': 'Time',
             'Desc': 1,
             # 'Attachments': 1,  ## filter attachments
         }
         inbox = self._get(self.api, 'mail/v4/conversations', params=params).json()
         return asyncio.run(process(x['ID'] for x in inbox['Conversations']))
 
+    def addresses(self, params: dict = None) -> dict:
+        params = params or {
+            'Page': 0,
+            'PageSize': 150,  # max page size
+        }
+        return self._get(self.api, 'core/v4/addresses', params=params).json()
+
     def decrypt_conversation(self, conversation_id: dict) -> dict:
         conversation = self._get(self.api, f'mail/v4/conversations/{conversation_id}').json()
         messages = filter(None, (msg.get('Body') for msg in conversation.get('Messages', [])))
         return {'id': conversation_id, 'data': [self.gpg_decrypt(data) for data in messages]}
 
-    def info(self):
+    def info(self) -> dict:
         headers = dict(self.client.headers) | {'x-pm-appversion': PM_APP_VERSION_ACCOUNT}
         return self._get(self.account_api, 'core/v4/auth/info', headers=headers).json()
 
-    def calendar_directory(self):
+    def calendar_directory(self) -> dict:
         return self._get(self.api, 'calendar/v1/directory', params={'Type': 2}).json()
 
-    def plans(self):
+    def revoke_all_sessions(self) -> dict:
+        return self._get(self.account_api, 'auth/v4/sessions').json()
+
+    def user_settings(self) -> dict:
+        return self._get(self.api, 'core/v4/settings').json()
+
+    def mail_settings(self) -> dict:
+        return self._get(self.api, 'mail/v4/settings').json()
+
+    def calendar_settings(self) -> dict:
+        return self._get(self.api, 'settings/calendar').json()
+
+    def timezones(self) -> dict:
+        return self._get(self.api, 'calendar/v1/timezones').json()
+
+    def plans(self) -> dict:
         return self._get(self.account_api, 'payments/v4/plans').json()
 
-    def salts(self):
+    def salts(self) -> dict:
         return self._get(self.account_api, 'core/v4/keys/salts').json()
 
-    def users(self):
+    def users(self) -> dict:
         return self._get(self.account_api, 'core/v4/users').json()
 
-    def sessions(self):
+    def sessions(self) -> dict:
         return self._get(self.account_api, 'auth/v4/sessions').json()
 
-    def version(self):
+    def version(self) -> dict:
         return self._get(self.assets, 'version.json').json()
 
-    def gpg_import(self, fname: str, passphrase: str = None):
+    def gpg_import(self, fname: str, passphrase: str = None) -> None:
         self.gpg.import_keys_file(fname, passphrase=passphrase or self.gpg_passphrase)
 
     def gpg_decrypt(self, data: str, passphrase: str = None) -> str:
         return self.gpg.decrypt(data, passphrase=passphrase or self.gpg_passphrase).data.decode()
 
-    def _get(self, base: str, endpoint: str, **kwargs):
+    def _get(self, base: str, endpoint: str, **kwargs) -> Response:
         self.client.cookies.delete('Session-Id', domain='.protonmail.ch')
         return self.client.get(f'{base}/{endpoint}', **kwargs)
 
     def __gpg_clear(self) -> list[dict]:
         """ Delete all GPG keys """
         fingerprints = [x['fingerprint'] for x in self.gpg.list_keys()]
         options = ['--delete-secret-keys', '--delete-keys']
```

### Comparing `proton-api-client-0.0.5/proton/constants.py` & `proton-api-client-0.0.6/proton/constants.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.5/proton/helpers.py` & `proton-api-client-0.0.6/proton/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             hashlib.sha512(self.b + b'\0').digest(),
             hashlib.sha512(self.b + b'\1').digest(),
             hashlib.sha512(self.b + b'\2').digest(),
             hashlib.sha512(self.b + b'\3').digest()
         ])
 
 
-def pm_hash(b: bytes = b''):
+def pm_hash(b: bytes = b'') -> object:
     return PMHash(b)
 
 
 def bcrypt_b64encode(s: bytes) -> bytes:
     bcrypt_base64 = b'./ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789'
     std_base64chars = b'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/'
     s = base64.b64encode(s)
@@ -65,12 +65,12 @@
 def hash_custom(hash_class: callable, *args) -> int:
     h = hash_class()
     for s in filter(None, args):
         h.update(l2b(s, SRP_LEN_BYTES) if isinstance(s, int) else s)
     return b2l(h.digest())
 
 
-def dump(path: str, **kwargs):
+def dump(path: str, **kwargs) -> None:
     fname, data = list(kwargs.items())[0]
     out = Path(path)
     out.mkdir(exist_ok=True, parents=True)
     (out / f'{fname}.json').write_bytes(orjson.dumps(data, option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS))
```

### Comparing `proton-api-client-0.0.5/proton/login.py` & `proton-api-client-0.0.6/proton/login.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.5/proton_api_client.egg-info/PKG-INFO` & `proton-api-client-0.0.6/proton_api_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `proton-api-client-0.0.5/setup.py` & `proton-api-client-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'tqdm',
     'uvloop',
     'nest_asyncio',
 ]
 
 setup(
     name='proton-api-client',
-    version='0.0.5',
+    version='0.0.6',
     python_requires='>=3.10.10',
     description='Proton Mail API',
     long_description=dedent('''
     
     ### Proton Mail API
     
     #### Examples
```

