# Comparing `tmp/uid2_client-2.0.2.tar.gz` & `tmp/uid2_client-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uid2_client-2.0.2.tar", last modified: Tue Jun 13 03:30:31 2023, max compression
+gzip compressed data, was "uid2_client-2.0.3.tar", last modified: Wed Jun 21 16:25:00 2023, max compression
```

## Comparing `uid2_client-2.0.2.tar` & `uid2_client-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-13 03:30:22.000000 uid2_client-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 03:30:31.488512 uid2_client-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-13 03:30:22.000000 uid2_client-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 03:30:22.000000 uid2_client-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 03:30:31.492512 uid2_client-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 03:30:22.000000 uid2_client-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-06-13 03:30:22.000000 uid2_client-2.0.2/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-13 03:30:22.000000 uid2_client-2.0.2/tests/test_key_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-13 03:30:22.000000 uid2_client-2.0.2/tests/test_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/uid2_client/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/advertising_token_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/auto_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/identity_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/identity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/uid2_base64_url_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/uid2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.654642 uid2_client-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-21 16:24:53.000000 uid2_client-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-21 16:25:00.654642 uid2_client-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-21 16:24:53.000000 uid2_client-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-21 16:24:53.000000 uid2_client-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 16:25:00.654642 uid2_client-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 16:24:53.000000 uid2_client-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.650642 uid2_client-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-06-21 16:24:53.000000 uid2_client-2.0.3/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-21 16:24:53.000000 uid2_client-2.0.3/tests/test_key_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-21 16:24:53.000000 uid2_client-2.0.3/tests/test_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.654642 uid2_client-2.0.3/uid2_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/advertising_token_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/auto_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/identity_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/identity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/uid2_base64_url_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.654642 uid2_client-2.0.3/uid2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/zip-safe
```

### Comparing `uid2_client-2.0.2/LICENSE` & `uid2_client-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/PKG-INFO` & `uid2_client-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uid2_client
-Version: 2.0.2
+Version: 2.0.3
 Summary: UID2 SDK for Python
 Home-page: https://iabtechlab.com
 Author: UID2 team
 Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
@@ -28,27 +28,27 @@
 This SDK supports Python 3.6 and above.
 
 ## Quick Start
 
 Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
 
 ```
-from uid2_client import Uid2Client, decrypt_token
+from uid2_client import Uid2Client, decrypt
 
 client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
 keys = client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
-decrypted_token = decrypt_token(advertising_token, keys)
+decrypted_token = decrypt(advertising_token, keys)
 print(decrypted_token.uid2)
 ```
 
 Additional examples are in the [examples] directory:
 * [sample_auto_refresh.py](examples/sample_auto_refresh.py)
 * [sample_client.py](examples/sample_client.py)
-* [sample_encryption.py](examples/sample_encryption.py)
+  * Includes an example to encrypt a raw UID2 into an advertising token for UID2 sharing.
 
 ## Development
 
 First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
```

### Comparing `uid2_client-2.0.2/README.md` & `uid2_client-2.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 This SDK supports Python 3.6 and above.
 
 ## Quick Start
 
 Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
 
 ```
-from uid2_client import Uid2Client, decrypt_token
+from uid2_client import Uid2Client, decrypt
 
 client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
 keys = client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
-decrypted_token = decrypt_token(advertising_token, keys)
+decrypted_token = decrypt(advertising_token, keys)
 print(decrypted_token.uid2)
 ```
 
 Additional examples are in the [examples] directory:
 * [sample_auto_refresh.py](examples/sample_auto_refresh.py)
 * [sample_client.py](examples/sample_client.py)
-* [sample_encryption.py](examples/sample_encryption.py)
+  * Includes an example to encrypt a raw UID2 into an advertising token for UID2 sharing.
 
 ## Development
 
 First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
```

### Comparing `uid2_client-2.0.2/pyproject.toml` & `uid2_client-2.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 40.9.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uid2_client"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
     { name = "UID2 team", email = "unifiedid-admin@thetradedesk.com" }
 ]
 description = "UID2 SDK for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `uid2_client-2.0.2/setup.cfg` & `uid2_client-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/tests/test_encryption.py` & `uid2_client-2.0.3/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/tests/test_key_parse.py` & `uid2_client-2.0.3/tests/test_key_parse.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/tests/test_keys.py` & `uid2_client-2.0.3/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/uid2_client/auto_refresh.py` & `uid2_client-2.0.3/uid2_client/auto_refresh.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/uid2_client/client.py` & `uid2_client-2.0.3/uid2_client/client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/uid2_client/encryption.py` & `uid2_client-2.0.3/uid2_client/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,20 +187,20 @@
     if ad_token_version == AdvertisingTokenVersion.ADVERTISING_TOKEN_V4:
         return Uid2Base64UrlCoder.encode(root_writer)
 
     return base64.b64encode(root_writer)
 
 
 
-def encrypt(uid2, indentity_scope, keys, keyset_id=None, **kwargs):
-    """ Encrypt an uid2 into a sharing token
+def encrypt(uid2, identity_scope, keys, keyset_id=None, **kwargs):
+    """ Encrypt an UID2 into a sharing token
 
     Args:
-        uid2: the uid2 to be encrypted
-        indentity_scope (IdentityScope): If the key will be uid2 or euid2
+        uid2: the UID2 or EUID to be encrypted
+        identity_scope (IdentityScope): indicates whether the output will be for UID2 or EUID
         keys (EncryptionKeysCollection): collection of keys to choose from for encryption
         keyset_id (int) : An optional keyset id to use for the encryption. Will use default keyset if left blank
 
     Keyword Args:
         now (Datetime): the datettime to use for now. Defaults to utc now
         ad_token_version (AdvertisingTokenVersion): Defaults to v4
 
@@ -215,25 +215,25 @@
     if ad_token_version is None:
         ad_token_version = AdvertisingTokenVersion.ADVERTISING_TOKEN_V4
 
     key = keys.get_default_keyset_key(now) if keyset_id is None else keys.get_by_keyset_key(keyset_id, now)
     master_key = keys.get_by_keyset_key(keys.get_master_keyset_id(), now)
 
     token_expiry = now + dt.timedelta(days=30) if keys.get_token_expiry_seconds() is None \
-        else now + dt.timedelta(seconds=keys.get_token_expiry_seconds())
+        else now + dt.timedelta(seconds=int(keys.get_token_expiry_seconds()))
 
     site_id = keys.get_caller_site_id()
     if site_id is None:
         print("No Site ID in keys")
         return
 
     if key is None:
         raise EncryptionError("No Keyset Key Found")
 
-    return _encrypt_token(uid2, indentity_scope, master_key, key, site_id, now, token_expiry, ad_token_version)
+    return _encrypt_token(uid2, identity_scope, master_key, key, site_id, now, token_expiry, ad_token_version)
 
 
 def encrypt_data(data, identity_scope, **kwargs):
     """Encrypt arbitrary binary data.
 
     The data can be decrypted with decrypt_data() function.
```

### Comparing `uid2_client-2.0.2/uid2_client/keys.py` & `uid2_client-2.0.3/uid2_client/keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/uid2_client/uid2_base64_url_coder.py` & `uid2_client-2.0.3/uid2_client/uid2_base64_url_coder.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.2/uid2_client.egg-info/PKG-INFO` & `uid2_client-2.0.3/uid2_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uid2-client
-Version: 2.0.2
+Version: 2.0.3
 Summary: UID2 SDK for Python
 Home-page: https://iabtechlab.com
 Author: UID2 team
 Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
@@ -28,27 +28,27 @@
 This SDK supports Python 3.6 and above.
 
 ## Quick Start
 
 Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
 
 ```
-from uid2_client import Uid2Client, decrypt_token
+from uid2_client import Uid2Client, decrypt
 
 client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
 keys = client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
-decrypted_token = decrypt_token(advertising_token, keys)
+decrypted_token = decrypt(advertising_token, keys)
 print(decrypted_token.uid2)
 ```
 
 Additional examples are in the [examples] directory:
 * [sample_auto_refresh.py](examples/sample_auto_refresh.py)
 * [sample_client.py](examples/sample_client.py)
-* [sample_encryption.py](examples/sample_encryption.py)
+  * Includes an example to encrypt a raw UID2 into an advertising token for UID2 sharing.
 
 ## Development
 
 First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
```

### Comparing `uid2_client-2.0.2/uid2_client.egg-info/SOURCES.txt` & `uid2_client-2.0.3/uid2_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

