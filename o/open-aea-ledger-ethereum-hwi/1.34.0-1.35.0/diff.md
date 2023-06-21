# Comparing `tmp/open-aea-ledger-ethereum-hwi-1.34.0.tar.gz` & `tmp/open-aea-ledger-ethereum-hwi-1.35.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-hwi-1.34.0.tar", last modified: Tue May 16 04:26:18 2023, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-hwi-1.35.0.tar", last modified: Wed Jun 21 10:08:54 2023, max compression
```

## Comparing `open-aea-ledger-ethereum-hwi-1.34.0.tar` & `open-aea-ledger-ethereum-hwi-1.35.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:18.545127 open-aea-ledger-ethereum-hwi-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-05-16 04:26:18.541127 open-aea-ledger-ethereum-hwi-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:18.541127 open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13964 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7390 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/hwi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:18.541127 open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-05-16 04:26:18.000000 open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-16 04:26:18.000000 open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 04:26:18.000000 open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-16 04:26:18.000000 open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-16 04:26:18.000000 open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-16 04:26:18.000000 open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 04:26:18.545127 open-aea-ledger-ethereum-hwi-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:18.541127 open-aea-ledger-ethereum-hwi-1.34.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6054 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-hwi-1.34.0/tests/test_account.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:54.915210 open-aea-ledger-ethereum-hwi-1.35.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-21 10:08:54.915210 open-aea-ledger-ethereum-hwi-1.35.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:54.911210 open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13912 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7390 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/hwi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:54.911210 open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-21 10:08:54.000000 open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-06-21 10:08:54.000000 open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 10:08:54.000000 open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-21 10:08:54.000000 open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-06-21 10:08:54.000000 open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-21 10:08:54.000000 open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 10:08:54.915210 open-aea-ledger-ethereum-hwi-1.35.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:54.915210 open-aea-ledger-ethereum-hwi-1.35.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6054 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-hwi-1.35.0/tests/test_account.py
```

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/LICENSE` & `open-aea-ledger-ethereum-hwi-1.35.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/PKG-INFO` & `open-aea-ledger-ethereum-hwi-1.35.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-hwi
-Version: 1.34.0
+Version: 1.35.0
 Summary: Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/__init__.py` & `open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/account.py` & `open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 from eth_account.messages import SignableMessage
 from eth_keys.main import PublicKey
 from eth_rlp import HashableRLP
 from eth_typing.evm import ChecksumAddress
 from eth_utils.curried import keccak
 from ledgerwallet.client import CommException, LedgerClient
 from ledgerwallet.transport import enumerate_devices
-from ledgerwallet.transport.device import Device
 
 from aea.common import JSONLike
 
 
 address = rlp.sedes.Binary.fixed_length(20, allow_empty=True)
 access_list_sede_type = rlp.sedes.CountableList(
     rlp.sedes.List(
@@ -191,15 +190,15 @@
         self._default_device_index = default_device_index
         self._default_key_index = default_key_index
         self._default_account_index = default_account_index
 
         self.default_account = None
 
     @property
-    def devices(self) -> List[Device]:
+    def devices(self) -> List[Any]:
         """Returns the list of available devices."""
         devices = enumerate_devices()
         if len(devices) == 0:
             raise HWIError(message="Cannot find any ledger device", sw=0)
         return devices
 
     def get_client(
```

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/exceptions.py` & `open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/aea_ledger_ethereum_hwi/hwi.py` & `open-aea-ledger-ethereum-hwi-1.35.0/aea_ledger_ethereum_hwi/hwi.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-hwi
-Version: 1.34.0
+Version: 1.35.0
 Summary: Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-hwi-1.35.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/setup.py` & `open-aea-ledger-ethereum-hwi-1.35.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,35 @@
 """Setup script for "aea_ledger_ethereum_hwi" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-hwi",
-    version="1.34.0",
+    version="1.35.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and support for hardware wallet interactions.",
     long_description="Python package wrapping the public and private key cryptography and support for hardware wallet interactions.",
     long_description_content_type="text/markdown",
     packages=find_packages(include=["aea_ledger_ethereum_hwi*"]),
     package_data={
         "aea_ledger_ethereum_hwi": [
             "py.typed",
         ]
     },
     install_requires=[
         "open-aea>=1.0.0, <2.0.0",
-        "web3==5.25.0",
+        "web3==5.31.4",
         "ipfshttpclient==0.8.0a2",
-        "eth-account==0.5.6",
-        "open-aea-ledger-ethereum~=1.34.0",
+        "eth-account>=0.5.9,<0.6.0",
+        "open-aea-ledger-ethereum~=1.35.0",
         "apduboy>=0.5.0",
-        "protobuf>=3.20,<4",
+        "protobuf==3.19.5",
+        "construct<=2.10.61",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": ["ethereum_hwi = aea_ledger_ethereum_hwi:EthereumHWICrypto"],
         "aea.ledger_apis": ["ethereum_hwi = aea_ledger_ethereum_hwi:EthereumHWIApi"],
         "aea.faucet_apis": [
             "ethereum_hwi = aea_ledger_ethereum_hwi:EthereumHWIFaucetApi"
```

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/tests/__init__.py` & `open-aea-ledger-ethereum-hwi-1.35.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.34.0/tests/test_account.py` & `open-aea-ledger-ethereum-hwi-1.35.0/tests/test_account.py`

 * *Files identical despite different names*

