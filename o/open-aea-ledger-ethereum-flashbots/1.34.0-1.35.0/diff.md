# Comparing `tmp/open-aea-ledger-ethereum-flashbots-1.34.0.tar.gz` & `tmp/open-aea-ledger-ethereum-flashbots-1.35.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.34.0.tar", last modified: Tue May 16 04:26:19 2023, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.35.0.tar", last modified: Wed Jun 21 10:08:55 2023, max compression
```

## Comparing `open-aea-ledger-ethereum-flashbots-1.34.0.tar` & `open-aea-ledger-ethereum-flashbots-1.35.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:19.429140 open-aea-ledger-ethereum-flashbots-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-16 04:26:19.429140 open-aea-ledger-ethereum-flashbots-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:19.429140 open-aea-ledger-ethereum-flashbots-1.34.0/aea_ledger_ethereum_flashbots/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/aea_ledger_ethereum_flashbots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:19.429140 open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-16 04:26:19.000000 open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-05-16 04:26:19.000000 open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 04:26:19.000000 open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-16 04:26:19.000000 open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-16 04:26:19.000000 open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-16 04:26:19.000000 open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 04:26:19.429140 open-aea-ledger-ethereum-flashbots-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 04:26:19.429140 open-aea-ledger-ethereum-flashbots-1.34.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10646 2023-05-16 04:25:37.000000 open-aea-ledger-ethereum-flashbots-1.34.0/tests/test_ethereum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:55.907220 open-aea-ledger-ethereum-flashbots-1.35.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-21 10:08:55.903221 open-aea-ledger-ethereum-flashbots-1.35.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:55.903221 open-aea-ledger-ethereum-flashbots-1.35.0/aea_ledger_ethereum_flashbots/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/aea_ledger_ethereum_flashbots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13945 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:55.903221 open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-21 10:08:55.000000 open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-06-21 10:08:55.000000 open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 10:08:55.000000 open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-21 10:08:55.000000 open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-21 10:08:55.000000 open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-21 10:08:55.000000 open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 10:08:55.907220 open-aea-ledger-ethereum-flashbots-1.35.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 10:08:55.903221 open-aea-ledger-ethereum-flashbots-1.35.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11057 2023-06-21 10:08:09.000000 open-aea-ledger-ethereum-flashbots-1.35.0/tests/test_ethereum.py
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/LICENSE` & `open-aea-ledger-ethereum-flashbots-1.35.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.35.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.34.0
+Version: 1.35.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/aea_ledger_ethereum_flashbots/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.35.0/aea_ledger_ethereum_flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py` & `open-aea-ledger-ethereum-flashbots-1.35.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,22 +18,26 @@
 # ------------------------------------------------------------------------------
 
 # pylint: disable=no-member
 
 """Python package extending the default open-aea ethereum ledger plugin to add support for flashbots."""
 
 import logging
-from typing import Any, List, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 from uuid import uuid4
 
-from aea_ledger_ethereum import EthereumApi, EthereumCrypto
+from aea_ledger_ethereum import DEFAULT_ADDRESS, EthereumApi, EthereumCrypto
 from eth_account import Account
-from flashbots import Flashbots, flashbot
+from eth_account.signers.local import LocalAccount
+from flashbots import FlashbotProvider, Flashbots, construct_flashbots_middleware
+from flashbots.flashbots import FlashbotsBundleResponse
 from flashbots.types import FlashbotsBundleRawTx, FlashbotsBundleTx
 from hexbytes import HexBytes
+from web3 import HTTPProvider, Web3
+from web3._utils.module import attach_modules
 from web3.exceptions import TransactionNotFound
 
 from aea.common import JSONLike
 from aea.helpers.base import try_decorator
 
 
 _default_logger = logging.getLogger("aea.ledger_apis.ethereum_flashbots")
@@ -42,48 +46,108 @@
 
 _TARGET_BLOCKS = "target_blocks"
 
 _DEFAULT_TARGET_BLOCKS = 25
 
 _RAISE_ON_FAILED_SIMULATION = "raise_on_failed_simulation"
 
+_USE_ALL_BUILDERS = "use_all_builders"
+
+
+def multiple_flashbots_builders(
+    signature_account: LocalAccount,
+    builders: List[Tuple[str, str]],
+    rpc_endpoint: str = DEFAULT_ADDRESS,
+) -> Dict[str, Web3]:
+    """Setup multiple flashbots providers."""
+    builder_to_instance = {}
+    for builder_name, endpoint_uri in builders:
+        flashbots_provider = FlashbotProvider(signature_account, endpoint_uri)
+        w3 = Web3(HTTPProvider(endpoint_uri=rpc_endpoint))
+        flash_middleware = construct_flashbots_middleware(flashbots_provider)
+        w3.middleware_onion.add(flash_middleware)
+        # attach modules to add the new namespace commands
+        attach_modules(w3, {"flashbots": (Flashbots,)})
+        builder_to_instance[builder_name] = w3
+    return builder_to_instance
+
 
 class EthereumFlashbotApi(EthereumApi):
     """Class to interact with the Ethereum Web3 APIs."""
 
     identifier = _ETHEREUM_FLASHBOTS
 
     def __init__(self, **kwargs: Any):
         """
         Initialize the Ethereum API.
 
         :param kwargs: the keyword arguments.
         """
+        rpc_endpoint = kwargs.get("address", DEFAULT_ADDRESS)
         super().__init__(**kwargs)
         authentication_private_key = kwargs.pop("authentication_private_key", None)
         authentication_account = (
             Account.create()  # pylint: disable=no-value-for-parameter
             if authentication_private_key is None
             else Account.from_key(  # pylint: disable=no-value-for-parameter
                 private_key=authentication_private_key
             )
         )
-        flashbot_relayer_uri = kwargs.pop("flashbot_relayer_uri", None)
-
-        # if flashbot_relayer_uri is None, the default URI is used
-        flashbot(self.api, authentication_account, flashbot_relayer_uri)
+        flashbots_builders = kwargs.pop("flashbots_builders", None)
+        if (
+            flashbots_builders is None
+            or not isinstance(flashbots_builders, list)
+            or len(flashbots_builders) == 0
+        ):
+            raise ValueError(
+                "flashbots_builders: List[Tuple[str, str]] must be provided."
+            )
+        # use the first builder as default
+        self._default_flashbots_builder_name = flashbots_builders[0][0]
+        self._builder_to_web3 = multiple_flashbots_builders(
+            authentication_account,
+            flashbots_builders,
+            rpc_endpoint,
+        )
 
     @property
     def flashbots(self) -> Flashbots:
         """Get the flashbots Web3 module."""
-        flashbots_module = getattr(self.api, "flashbots", None)
+        # use the first builder as default
+        builder_name = self._default_flashbots_builder_name
+        flashbots_module = getattr(
+            self._builder_to_web3[builder_name], "flashbots", None
+        )
         if flashbots_module is None:  # pragma: nocover
-            raise ValueError("Flashbots have not been registered as a Web3 module.")
+            raise ValueError(
+                f"Flashbots-{builder_name} have not been registered as a Web3 module."
+            )
         return cast(Flashbots, flashbots_module)
 
+    def send_to_all_builders(
+        self,
+        bundle: List[FlashbotsBundleRawTx],
+        target_block: int,
+        opts: Dict[str, Any],
+    ) -> Dict[str, FlashbotsBundleResponse]:
+        """Send the transaction to multiple builders."""
+        builder_to_response = {}
+        for builder_name, web3 in self._builder_to_web3.items():
+            flashbots_module = getattr(web3, "flashbots", None)
+            if flashbots_module is None:  # pragma: nocover
+                raise ValueError(
+                    f"Flashbots {builder_name} have not been registered as a Web3 module."
+                )
+            response = flashbots_module.send_bundle(bundle, target_block, opts=opts)
+            _default_logger.info(
+                f"Flashbots-{builder_name} send_bundle response: {response}"
+            )
+            builder_to_response[builder_name] = response
+        return builder_to_response
+
     @staticmethod
     def bundle_transactions(
         signed_transactions: List[JSONLike],
     ) -> List[FlashbotsBundleRawTx]:
         """Bundle transactions."""
         return [
             FlashbotsBundleRawTx(
@@ -120,27 +184,29 @@
         return False
 
     def send_bundle(
         self,
         bundle: List[Union[FlashbotsBundleTx, FlashbotsBundleRawTx]],
         target_blocks: List[int],
         raise_on_failed_simulation: bool = False,
+        use_all_builders: bool = False,
     ) -> Optional[List[str]]:
         """
         Send a bundle.
 
         1. Simulate the bundle.
         2. Send the bundle in a try catch block.
         3. Wait for the response. If successful, go to step 4.
          If current block number is less than the maximum target block number, go to step 1.
         4. Return the transaction digests if the transactions went through, or None if something went wrong.
 
         :param bundle: the signed transactions to bundle together and send.
         :param target_blocks: the target blocks for the transactions.
         :param raise_on_failed_simulation: whether to raise an exception if the simulation fails.
+        :param use_all_builders: whether to send the bundle to all builders.
         :return: the transaction digest if the transaction went through, None otherwise.
         """
         for target_block in target_blocks:
             current_block = self.api.eth.blockNumber
             if current_block >= target_block:
                 # we can only target future blocks
                 _default_logger.debug(
@@ -156,33 +222,45 @@
                 continue
 
             replacement_uuid = str(uuid4())
             _default_logger.debug(
                 f"Sending bundle {bundle} with replacement_uuid {replacement_uuid} targeting block {target_block}"
             )
             # we try to send the bundle on the target block, which MUST be greater than the current block
-            response = self.flashbots.send_bundle(
-                bundle, target_block, opts={"replacementUuid": replacement_uuid}
-            )
+            builder_to_response = {}
+            if use_all_builders:
+                builder_to_response = self.send_to_all_builders(
+                    bundle, target_block, opts={"replacementUuid": replacement_uuid}
+                )
+            else:
+                response = self.flashbots.send_bundle(
+                    bundle, target_block, opts={"replacementUuid": replacement_uuid}
+                )
+                builder_to_response[self._default_flashbots_builder_name] = response
             _default_logger.debug(
-                f"Response from bundle with replacement uuid {replacement_uuid}: {response}"
+                f"Response from bundle with replacement uuid {replacement_uuid}: {builder_to_response}"
             )
-            response.wait()
+
+            default_builder_response = builder_to_response[
+                self._default_flashbots_builder_name
+            ]
+            # all builders target the same block, so we can just wait for the default builder
+            default_builder_response.wait()
             try:
-                receipts = response.receipts()
-                tx_hashes = [tx["hash"].hex() for tx in response.bundle]
+                receipts = default_builder_response.receipts()
+                tx_hashes = [tx["hash"].hex() for tx in default_builder_response.bundle]
                 _default_logger.debug(
                     f"Bundle with replacement uuid {replacement_uuid} was mined in block {receipts[0]['blockNumber']}"
                     f"Tx hashes: {tx_hashes}"
                 )
                 return tx_hashes
             except TransactionNotFound:
                 # get & log the bundle stats in case it was not included in the block
                 stats = self.flashbots.get_bundle_stats_v2(
-                    self.api.toHex(response.bundle_hash()), target_block
+                    self.api.toHex(default_builder_response.bundle_hash()), target_block
                 )
                 _default_logger.info(
                     f"Bundle with replacement uuid {replacement_uuid} not found in block {target_block}. "
                     f"bundle stats: {stats}"
                 )
                 # essentially a no-op but it shows that the function works
                 cancel_res = self.flashbots.cancel_bundles(replacement_uuid)
@@ -208,20 +286,25 @@
         """
         Try sending a bundle of transactions.
 
         :param signed_transactions: the raw signed transactions to bundle together and send.
         :param _kwargs: the keyword arguments. Possible kwargs are:
             `raise_on_try`: bool flag specifying whether the method will raise or log on error (used by `try_decorator`)
             `target_blocks`: the target blocks for the transactions.
+            `raise_on_failed_simulation`: whether to raise an exception if the simulation fails.
+            `use_all_builders`: whether to send the bundle to all builders.
         :return: the transaction digest if the transactions went through, None otherwise.
         """
         bundle = self.bundle_transactions(signed_transactions)
         target_blocks = _kwargs.get(_TARGET_BLOCKS, self._get_next_blocks())
         raise_on_failed_simulation = _kwargs.get(_RAISE_ON_FAILED_SIMULATION, False)
-        tx_hashes = self.send_bundle(bundle, target_blocks, raise_on_failed_simulation)
+        use_all_builders = _kwargs.get(_USE_ALL_BUILDERS, False)
+        tx_hashes = self.send_bundle(
+            bundle, target_blocks, raise_on_failed_simulation, use_all_builders
+        )
         return tx_hashes
 
     def send_signed_transactions(
         self,
         signed_transactions: List[JSONLike],
         raise_on_try: bool = False,
         **kwargs: Any,
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.34.0
+Version: 1.35.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-flashbots-1.35.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/setup.py` & `open-aea-ledger-ethereum-flashbots-1.35.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_ethereum_flashbots" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-flashbots",
-    version="1.34.0",
+    version="1.35.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.",
     long_description=(
         "Python package extending the default open-aea ethereum ledger plugin to add support for flashbots."
     ),
     long_description_content_type="text/markdown",
@@ -37,15 +37,15 @@
     package_data={
         "aea_ledger_ethereum_flashbots": [
             "py.typed",
         ]
     },
     python_requires=">=3.9,<4.0",
     install_requires=[
-        "open-aea-ledger-ethereum~=1.34.0",
+        "open-aea-ledger-ethereum~=1.35.0",
         "flashbots==1.1.1",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": [
             "ethereum_flashbots = aea_ledger_ethereum_flashbots:EthereumFlashbotCrypto"
         ],
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/tests/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.35.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.34.0/tests/test_ethereum.py` & `open-aea-ledger-ethereum-flashbots-1.35.0/tests/test_ethereum.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,50 +13,61 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 # pylint: disable=redefined-outer-name,import-error,protected-access
+# flake8: noqa: B009
 
 """Tests for the aea_ledger_ethereum_flashbots package."""
 from typing import Tuple
 from unittest.mock import ANY, MagicMock, patch
 
 import pytest
 from aea_ledger_ethereum_flashbots.ethereum_flashbots import EthereumFlashbotApi
 from eth_account import Account
 from flashbots.types import FlashbotsBundleRawTx
 from hexbytes import HexBytes
 from web3.exceptions import TransactionNotFound
 from web3.types import TxReceipt
 
 
+_DUMMY_FLASHBOTS_BUILDERS = [
+    ["dummy", "dummy_uri1"],
+    ["builder0x69", "dummy_uri2"],
+]
+
+
 @pytest.fixture
 def ethereum_flashbot_api() -> EthereumFlashbotApi:
     """Get the ethereum flashbot API."""
-    return EthereumFlashbotApi()
+
+    return EthereumFlashbotApi(flashbots_builders=_DUMMY_FLASHBOTS_BUILDERS)
 
 
 def test_init_with_signature_private_key() -> None:
     """Test init with signature private key."""
     signature_private_key = "my private key"
     with patch.object(
         Account, "from_key", side_effect=lambda private_key: MagicMock()
     ) as account_from_key_mock:
-        EthereumFlashbotApi(signature_private_key=signature_private_key)
+        EthereumFlashbotApi(
+            signature_private_key=signature_private_key,
+            flashbots_builders=_DUMMY_FLASHBOTS_BUILDERS,
+        )
         assert account_from_key_mock.called_once_with(signature_private_key)
 
 
 def test_init_without_signature_private_key() -> None:
     """Test init without signature private key."""
     with patch.object(
         Account, "create", side_effect=MagicMock()
     ) as account_create_mock:
-        EthereumFlashbotApi()
+        EthereumFlashbotApi(flashbots_builders=_DUMMY_FLASHBOTS_BUILDERS)
         assert account_create_mock.called_once_with()
 
 
 @pytest.mark.parametrize("signed_txs", (("0x1234", "0x0000", "0x5232"), ("0x1234",)))
 def test_bundle_transactions(ethereum_flashbot_api, signed_txs: Tuple[str]) -> None:
     """Test bundle transactions."""
     dummy_signed_transactions = [
@@ -66,28 +77,32 @@
     actual_bundle = [tx.get("signed_transaction", None) for tx in bundle]
     expected_bundle = [
         HexBytes(tx.get("raw_transaction", None)) for tx in dummy_signed_transactions
     ]
     assert expected_bundle == actual_bundle
 
 
-def test_simulate_with_successful_simulation(ethereum_flashbot_api) -> None:
+def test_simulate_with_successful_simulation(
+    ethereum_flashbot_api,
+) -> None:
     """Test simulate with successful simulation."""
     # mock
     response_mock = MagicMock()
-    ethereum_flashbot_api._api.flashbots.simulate = MagicMock(
-        return_value=response_mock
+    default_builder = _DUMMY_FLASHBOTS_BUILDERS[0][0]
+    flashbots_module = getattr(
+        ethereum_flashbot_api._builder_to_web3[default_builder], "flashbots"
     )
+    flashbots_module.simulate = MagicMock(return_value=response_mock)
 
     # run
     bundle = [FlashbotsBundleRawTx(signed_transaction=HexBytes("0x1234"))]
     success = ethereum_flashbot_api.simulate(bundle, 123)
 
     # check
-    ethereum_flashbot_api._api.flashbots.simulate.assert_called_once_with(bundle, 123)
+    flashbots_module.simulate.assert_called_once_with(bundle, 123)
     assert success
 
 
 def test_simulate_with_failed_simulation(ethereum_flashbot_api) -> None:
     """Test simulate with failed simulation."""
     # mock
     response_mock = MagicMock(side_effect=Exception)
```

