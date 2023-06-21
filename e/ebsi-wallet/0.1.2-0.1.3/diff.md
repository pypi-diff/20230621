# Comparing `tmp/ebsi_wallet-0.1.2.tar.gz` & `tmp/ebsi_wallet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebsi_wallet-0.1.2.tar", max compression
+gzip compressed data, was "ebsi_wallet-0.1.3.tar", max compression
```

## Comparing `ebsi_wallet-0.1.2.tar` & `ebsi_wallet-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11368 2023-01-10 08:28:57.766492 ebsi_wallet-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/__init__.py
--rw-r--r--   0        0        0     4192 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/__init__.py
--rw-r--r--   0        0        0     2515 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/signer_algorithm.py
--rw-r--r--   0        0        0      805 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/__init__.py
--rw-r--r--   0        0        0    18274 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py
--rw-r--r--   0        0        0     3954 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py
--rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/__init__.py
--rw-r--r--   0        0        0     5363 2023-06-20 16:50:47.088113 ebsi_wallet-0.1.2/ebsi_wallet/did_key/__init__.py
--rw-r--r--   0        0        0     1346 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_client/__init__.py
--rw-r--r--   0        0        0     1118 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did/__init__.py
--rw-r--r--   0        0        0      319 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/__init__.py
--rw-r--r--   0        0        0      280 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/constants/__init__.py
--rw-r--r--   0        0        0     1155 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/validators/__init__.py
--rw-r--r--   0        0        0     3709 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ethereum/__init__.py
--rw-r--r--   0        0        0      436 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ethereum/util.py
--rw-r--r--   0        0        0    27001 2023-05-01 07:34:47.063782 ebsi_wallet-0.1.2/ebsi_wallet/main.py
--rw-r--r--   0        0        0     2764 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/siop_auth/__init__.py
--rw-r--r--   0        0        0    15771 2023-06-20 09:52:09.193345 ebsi_wallet-0.1.2/ebsi_wallet/siop_auth/util.py
--rw-r--r--   0        0        0     4861 2023-06-20 17:08:15.296537 ebsi_wallet-0.1.2/ebsi_wallet/util/__init__.py
--rw-r--r--   0        0        0     3363 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/util/verifiable_presentation.py
--rw-r--r--   0        0        0     2499 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/validators/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_credential/__init__.py
--rw-r--r--   0        0        0      148 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_credential/validators/__init__.py
--rw-r--r--   0        0        0      536 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/__init__.py
--rw-r--r--   0        0        0     1431 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/v2/__init__.py
--rw-r--r--   0        0        0      645 2023-06-20 17:24:29.488089 ebsi_wallet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 ebsi_wallet-0.1.2/setup.py
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 ebsi_wallet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11368 2023-01-10 08:28:57.766492 ebsi_wallet-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/__init__.py
+-rw-r--r--   0        0        0     4192 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/__init__.py
+-rw-r--r--   0        0        0     2515 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/signer_algorithm.py
+-rw-r--r--   0        0        0      805 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/util/__init__.py
+-rw-r--r--   0        0        0    18274 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py
+-rw-r--r--   0        0        0     3954 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/util/json_canonicalize/__init__.py
+-rw-r--r--   0        0        0     5363 2023-06-21 16:05:07.212026 ebsi_wallet-0.1.3/ebsi_wallet/did_key/__init__.py
+-rw-r--r--   0        0        0     1346 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/ebsi_client/__init__.py
+-rw-r--r--   0        0        0     1118 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/ebsi_did/__init__.py
+-rw-r--r--   0        0        0      319 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/ebsi_did_resolver/__init__.py
+-rw-r--r--   0        0        0      280 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/ebsi_did_resolver/constants/__init__.py
+-rw-r--r--   0        0        0     1155 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/ebsi_did_resolver/validators/__init__.py
+-rw-r--r--   0        0        0     3709 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/ethereum/__init__.py
+-rw-r--r--   0        0        0      436 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/ethereum/util.py
+-rw-r--r--   0        0        0    27001 2023-05-01 07:34:47.063782 ebsi_wallet-0.1.3/ebsi_wallet/main.py
+-rw-r--r--   0        0        0     2764 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/siop_auth/__init__.py
+-rw-r--r--   0        0        0    15771 2023-06-20 09:52:09.193345 ebsi_wallet-0.1.3/ebsi_wallet/siop_auth/util.py
+-rw-r--r--   0        0        0     4866 2023-06-21 16:05:57.668640 ebsi_wallet-0.1.3/ebsi_wallet/util/__init__.py
+-rw-r--r--   0        0        0     3363 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/util/verifiable_presentation.py
+-rw-r--r--   0        0        0     2499 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/validators/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/verifiable_credential/__init__.py
+-rw-r--r--   0        0        0      148 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/verifiable_credential/validators/__init__.py
+-rw-r--r--   0        0        0      536 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/verifiable_presentation/__init__.py
+-rw-r--r--   0        0        0     1431 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.3/ebsi_wallet/verifiable_presentation/v2/__init__.py
+-rw-r--r--   0        0        0      645 2023-06-21 16:05:15.384126 ebsi_wallet-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 ebsi_wallet-0.1.3/setup.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 ebsi_wallet-0.1.3/PKG-INFO
```

### Comparing `ebsi_wallet-0.1.2/LICENSE` & `ebsi_wallet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/signer_algorithm.py` & `ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/signer_algorithm.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py` & `ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py` & `ebsi_wallet-0.1.3/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/did_key/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/did_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/ebsi_client/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/ebsi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/ebsi_did/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/validators/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/ebsi_did_resolver/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/ethereum/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/main.py` & `ebsi_wallet-0.1.3/ebsi_wallet/main.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/siop_auth/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/siop_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/siop_auth/util.py` & `ebsi_wallet-0.1.3/ebsi_wallet/siop_auth/util.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/util/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,12 +163,12 @@
     salt = os.urandom(16)
 
     # Convert the salt to hexadecimal representation
     salt_hex = salt.hex()
 
     return salt_hex
 
-def generate_disclosure_content_and_base64(claim_key: str, claims: dict) -> typing.Tuple[str, str]:
+def generate_disclosure_content_and_base64(claim_key: str, claim_value: typing.Any) -> typing.Tuple[str, str]:
     claim_salt = generate_random_salt()
-    claim_disclosure = [claim_salt, claim_key, claims[claim_key]]
+    claim_disclosure = [claim_salt, claim_key, claim_value]
     claim_disclosure_base64 = base64.urlsafe_b64encode(json.dumps(claim_disclosure).encode('utf-8')).decode('utf-8').rstrip("=")
     return claim_disclosure, claim_disclosure_base64
```

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/util/verifiable_presentation.py` & `ebsi_wallet-0.1.3/ebsi_wallet/util/verifiable_presentation.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/validators/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/verifiable_presentation/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/v2/__init__.py` & `ebsi_wallet-0.1.3/ebsi_wallet/verifiable_presentation/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi_wallet-0.1.2/pyproject.toml` & `ebsi_wallet-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebsi-wallet"
-version = "0.1.2"
+version = "0.1.3"
 description = "EBSI Python SDK"
 authors = ["George J Padayatti <george.padayatti@igrant.io>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 jwcrypto = "^1.3.1"
```

### Comparing `ebsi_wallet-0.1.2/setup.py` & `ebsi_wallet-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
  'py-multibase>=1.0.3,<2.0.0',
  'pysha3>=1.0.2,<2.0.0',
  'rich>=12.5.1,<13.0.0',
  'sslcrypto>=5.3,<6.0']
 
 setup_kwargs = {
     'name': 'ebsi-wallet',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'EBSI Python SDK',
     'long_description': 'None',
     'author': 'George J Padayatti',
     'author_email': 'george.padayatti@igrant.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ebsi_wallet-0.1.2/PKG-INFO` & `ebsi_wallet-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebsi-wallet
-Version: 0.1.2
+Version: 0.1.3
 Summary: EBSI Python SDK
 License: MIT
 Author: George J Padayatti
 Author-email: george.padayatti@igrant.io
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

