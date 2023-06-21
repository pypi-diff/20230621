# Comparing `tmp/rubi-2.0.3.tar.gz` & `tmp/rubi-2.0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.3.tar", max compression
+gzip compressed data, was "rubi-2.0.4b1.tar", max compression
```

## Comparing `rubi-2.0.3.tar` & `rubi-2.0.4b1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.3/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.3/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.3/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.3/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.3/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.3/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      645 2023-06-01 18:59:40.465341 rubi-2.0.3/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.3/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.3/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      664 2023-06-01 18:59:40.468200 rubi-2.0.3/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.3/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.3/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      518 2023-06-01 18:59:40.468648 rubi-2.0.3/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.3/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.3/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      631 2023-06-01 18:59:40.469759 rubi-2.0.3/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0      748 2023-06-08 02:20:45.126846 rubi-2.0.3/pyproject.toml
--rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.3/rubi/__init__.py
--rw-r--r--   0        0        0    26809 2023-06-07 23:47:41.357240 rubi-2.0.3/rubi/client.py
--rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.3/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.3/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11394 2023-06-07 23:47:41.357521 rubi-2.0.3/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0    16600 2023-06-07 23:47:41.358043 rubi-2.0.3/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24654 2023-06-07 23:47:41.358440 rubi-2.0.3/rubi/contracts/market.py
--rw-r--r--   0        0        0    14838 2023-06-07 23:47:41.358885 rubi-2.0.3/rubi/contracts/router.py
--rw-r--r--   0        0        0       74 2023-06-07 23:47:41.359211 rubi-2.0.3/rubi/contracts/types/__init__.py
--rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.3/rubi/contracts/types/events.py
--rw-r--r--   0        0        0     2674 2023-06-07 23:47:41.359354 rubi-2.0.3/rubi/contracts/types/transaction_reciept.py
--rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.3/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.3/rubi/data/__init__.py
--rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.3/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.3/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.3/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.3/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.3/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.3/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.3/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.3/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.3/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.3/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.3/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.3/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.3/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.3/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.3/rubi/data/sources/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.3/rubi/network/__init__.py
--rw-r--r--   0        0        0     7589 2023-06-01 23:03:08.489079 rubi-2.0.3/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.3/rubi/types/__init__.py
--rw-r--r--   0        0        0    12516 2023-06-07 23:47:41.359563 rubi-2.0.3/rubi/types/order.py
--rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.3/rubi/types/orderbook.py
--rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.3/rubi/types/pair.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.4b1/LICENSE
+-rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.4b1/README.md
+-rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.4b1/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.4b1/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.4b1/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.4b1/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      633 2023-06-13 17:59:13.620185 rubi-2.0.4b1/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.4b1/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.4b1/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      651 2023-06-13 17:59:13.620375 rubi-2.0.4b1/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.4b1/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.4b1/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      508 2023-06-13 17:59:13.620539 rubi-2.0.4b1/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.4b1/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.4b1/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      619 2023-06-13 17:59:13.620686 rubi-2.0.4b1/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0      750 2023-06-21 19:17:01.151438 rubi-2.0.4b1/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-06-21 19:17:01.151640 rubi-2.0.4b1/rubi/__init__.py
+-rw-r--r--   0        0        0    25763 2023-06-21 19:17:01.151931 rubi-2.0.4b1/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-06-21 19:17:01.152075 rubi-2.0.4b1/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.4b1/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11403 2023-06-21 19:17:01.152239 rubi-2.0.4b1/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       73 2023-06-21 19:17:01.152321 rubi-2.0.4b1/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15968 2023-06-21 19:17:01.152942 rubi-2.0.4b1/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2674 2023-06-21 19:17:01.153096 rubi-2.0.4b1/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    16609 2023-06-21 19:17:01.153278 rubi-2.0.4b1/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24669 2023-06-21 19:17:01.153743 rubi-2.0.4b1/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14847 2023-06-21 19:17:01.153923 rubi-2.0.4b1/rubi/contracts/router.py
+-rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.4b1/rubi/data/README.md
+-rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.4b1/rubi/data/__init__.py
+-rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.4b1/rubi/data/data.py
+-rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.4b1/rubi/data/processing/README.md
+-rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.4b1/rubi/data/processing/__init__.py
+-rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.4b1/rubi/data/processing/aid.py
+-rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.4b1/rubi/data/processing/helper/__init__.py
+-rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.4b1/rubi/data/processing/helper/processing.py
+-rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.4b1/rubi/data/processing/user.py
+-rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.4b1/rubi/data/sources/__init__.py
+-rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.4b1/rubi/data/sources/aid.py
+-rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.4b1/rubi/data/sources/helper/README.md
+-rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.4b1/rubi/data/sources/helper/__init__.py
+-rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.4b1/rubi/data/sources/helper/gas.py
+-rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.4b1/rubi/data/sources/helper/price.py
+-rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.4b1/rubi/data/sources/helper/rolodex.py
+-rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.4b1/rubi/data/sources/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.4b1/rubi/network/__init__.py
+-rw-r--r--   0        0        0     7596 2023-06-21 19:17:01.154084 rubi-2.0.4b1/rubi/network/network.py
+-rw-r--r--   0        0        0       66 2023-06-21 19:17:01.154162 rubi-2.0.4b1/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15552 2023-06-21 19:17:01.154405 rubi-2.0.4b1/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0     5727 2023-06-21 19:17:01.154503 rubi-2.0.4b1/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2776 2023-06-21 19:17:01.154577 rubi-2.0.4b1/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 rubi-2.0.4b1/PKG-INFO
```

### Comparing `rubi-2.0.3/LICENSE` & `rubi-2.0.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/README.md` & `rubi-2.0.4b1/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/ERC20.json` & `rubi-2.0.4b1/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/README.md` & `rubi-2.0.4b1/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/abitrum_goerli/abis/market.json` & `rubi-2.0.4b1/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/abitrum_goerli/abis/router.json` & `rubi-2.0.4b1/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/abitrum_goerli/network.yaml` & `rubi-2.0.4b1/network_config/abitrum_goerli/network.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 name: "Arbitrum Goerli"
 chain_id: 421613
 currency: "ETH"
 rpc_url: "https://goerli-rollup.arbitrum.io/rpc"
 explorer_url: "https://goerli-rollup-explorer.arbitrum.io"
 
 rubicon:
-  market:
-    address: "0x506407f25B746C39807c03A96DD595a6BE223211"
-  router:
-    address: "0x3AbA34a8C9616eA927225C045EEa5d5b51a7a6FC"
+ market:
+  address: "0x506407f25B746C39807c03A96DD595a6BE223211"
+ router:
+  address: "0x3AbA34a8C9616eA927225C045EEa5d5b51a7a6FC"
 
 token_addresses:
-  WETH: "0x175A6D830579CAcf1086ECC718fAB2A86b12e0D3"
-  USDC: "0x34cB584d2E4f3Cd37e93A46A4C754044085439b4"
-  TEST:	"0x83250b2783554D4D401c45c39fF8A161dE44BC15"
-  USDT:	"0x6ABc1231d85D422c9Fe25b5974B4C0D4AB85d9b5"
-  DAI:	"0xb37b4399880AfEF7025755d65C193363966b8b89"
-  WBTC:	"0x710c1A969cbC8ab5644571697824c655ffBDE926"
+ WETH: "0x175A6D830579CAcf1086ECC718fAB2A86b12e0D3"
+ USDC: "0x34cB584d2E4f3Cd37e93A46A4C754044085439b4"
+ TEST:	"0x83250b2783554D4D401c45c39fF8A161dE44BC15"
+ USDT:	"0x6ABc1231d85D422c9Fe25b5974B4C0D4AB85d9b5"
+ DAI:	"0xb37b4399880AfEF7025755d65C193363966b8b89"
+ WBTC:	"0x710c1A969cbC8ab5644571697824c655ffBDE926"
```

### Comparing `rubi-2.0.3/network_config/optimism/abis/market.json` & `rubi-2.0.4b1/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/optimism/abis/router.json` & `rubi-2.0.4b1/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/optimism/network.yaml` & `rubi-2.0.4b1/network_config/optimism/network.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 name: "Optimism"
 chain_id: 10
 currency: "ETH"
 rpc_url: "https://mainnet.optimism.io"
 explorer_url: "https://optimistic.etherscan.io/"
 
 rubicon:
-  market:
-    address: "0x7a512d3609211e719737e82c7bb7271ec05da70d"
-  router:
-    address: "0x7Af14ADc8Aea70f063c7eA3B2C1AD0D7A59C4bFf"
+ market:
+  address: "0x7a512d3609211e719737e82c7bb7271ec05da70d"
+ router:
+  address: "0x7Af14ADc8Aea70f063c7eA3B2C1AD0D7A59C4bFf"
 
 token_addresses:
-  ETH: "0xDeadDeAddeAddEAddeadDEaDDEAdDeaDDeAD0000"
-  WETH: "0x4200000000000000000000000000000000000006"
-  WBTC: "0x68f180fcCe6836688e9084f035309E29Bf0A2095"
-  OP: "0x4200000000000000000000000000000000000042"
-  USDC: "0x7F5c764cBc14f9669B88837ca1490cCa17c31607"
-  DAI: "0xDA10009cBd5D07dd0CeCc66161FC93D7c9000da1"
-  USDT: "0x94b008aA00579c1307B0EF2c499aD98a8ce58e58"
+ ETH: "0xDeadDeAddeAddEAddeadDEaDDEAdDeaDDeAD0000"
+ WETH: "0x4200000000000000000000000000000000000006"
+ WBTC: "0x68f180fcCe6836688e9084f035309E29Bf0A2095"
+ OP: "0x4200000000000000000000000000000000000042"
+ USDC: "0x7F5c764cBc14f9669B88837ca1490cCa17c31607"
+ DAI: "0xDA10009cBd5D07dd0CeCc66161FC93D7c9000da1"
+ USDT: "0x94b008aA00579c1307B0EF2c499aD98a8ce58e58"
```

### Comparing `rubi-2.0.3/network_config/optimism_goerli/abis/market.json` & `rubi-2.0.4b1/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/optimism_goerli/abis/router.json` & `rubi-2.0.4b1/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/polygon_mumbai/abis/market.json` & `rubi-2.0.4b1/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/polygon_mumbai/abis/router.json` & `rubi-2.0.4b1/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/network_config/polygon_mumbai/network.yaml` & `rubi-2.0.4b1/network_config/polygon_mumbai/network.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 name: "Polygon Mumbai"
 chain_id: 80001
 currency: "MATIC"
 rpc_url: "https://rpc-mumbai.maticvigil.com/"
 explorer_url: "https://mumbai.polygonscan.com/"
 
 rubicon:
-  market:
-    address: "0x10418D9e730fa659b0Baf0b640ee41FcF4EA2aaE"
-  router:
-    address: "0xbA81dF0251A017C2fB687e5469a897529442f008"
+ market:
+  address: "0x10418D9e730fa659b0Baf0b640ee41FcF4EA2aaE"
+ router:
+  address: "0xbA81dF0251A017C2fB687e5469a897529442f008"
 
 token_addresses:
-  WETH: "0xE412a307764cCBE02E055e926516ebD74230cfE0"
-  USDC: "0xcC5f8571D858DAD7fA2238FB9df4Ad384493013C"
-  TEST:	"0x6aeda41c98ab5399044fc36162B57d39c13b658a"
-  USDT:	"0x97fcdaA045F4a3Bc8Fc7ad721EFf38d66B234C7F"
-  DAI:	"0xAb647DF8262580c1caB61Eb165B22616365d3C67"
-  WBTC:	"0x639C6472C45037F7aA868729dFfF69eB3843f1A0"
+ WETH: "0xE412a307764cCBE02E055e926516ebD74230cfE0"
+ USDC: "0xcC5f8571D858DAD7fA2238FB9df4Ad384493013C"
+ TEST: "0x6aeda41c98ab5399044fc36162B57d39c13b658a"
+ USDT: "0x97fcdaA045F4a3Bc8Fc7ad721EFf38d66B234C7F"
+ DAI: "0xAb647DF8262580c1caB61Eb165B22616365d3C67"
+ WBTC: "0x639C6472C45037F7aA868729dFfF69eB3843f1A0"
```

### Comparing `rubi-2.0.3/pyproject.toml` & `rubi-2.0.4b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.0.3"
+version = "2.0.4b1"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.0.3/rubi/client.py` & `rubi-2.0.4b1/rubi/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 from eth_typing import ChecksumAddress
 from web3.types import EventData
 
 from rubi.contracts import (
     RubiconMarket,
     RubiconRouter,
     ERC20,
-    TransactionReceipt
+    TransactionReceipt,
+    EmitFeeEvent
 )
 from rubi.network import (
     Network,
 )
-from rubi.types import (
+from rubi.rubicon_types import (
     OrderSide,
     NewMarketOrder,
     NewLimitOrder,
     Pair,
     OrderBook,
     PairDoesNotExistException,
     BaseEvent,
+    FeeEvent,
     OrderEvent,
     Transaction,
     BaseNewOrder,
     NewCancelOrder,
     UpdateLimitOrder
 )
 
@@ -126,23 +128,27 @@
         """
 
         base, quote = pair_name.split("/")
 
         base_asset = ERC20.from_network(name=base, network=self.network, wallet=self.wallet, key=self.key)
         quote_asset = ERC20.from_network(name=quote, network=self.network, wallet=self.wallet, key=self.key)
 
-        current_base_asset_allowance = base_asset.to_decimal(
-            number=base_asset.allowance(owner=self.wallet, spender=self.market.address)
-        )
-        current_quote_asset_allowance = quote_asset.to_decimal(
-            number=quote_asset.allowance(owner=self.wallet, spender=self.market.address)
-        )
+        current_base_asset_allowance = None
+        current_quote_asset_allowance = None
+
+        if self.wallet is not None and self.key is not None:
+            current_base_asset_allowance = base_asset.to_decimal(
+                number=base_asset.allowance(owner=self.wallet, spender=self.market.address)
+            )
+            current_quote_asset_allowance = quote_asset.to_decimal(
+                number=quote_asset.allowance(owner=self.wallet, spender=self.market.address)
+            )
 
-        if current_base_asset_allowance == Decimal("0") or current_quote_asset_allowance == Decimal("0"):
-            log.warning("allowance for base or quote asset is zero. this may cause issues when placing orders")
+            if current_base_asset_allowance == Decimal("0") or current_quote_asset_allowance == Decimal("0"):
+                log.warning("allowance for base or quote asset is zero. this may cause issues when placing orders")
 
         self._pairs[f"{base}/{quote}"] = Pair(
             name=pair_name,
             base_asset=base_asset,
             quote_asset=quote_asset,
             current_base_asset_allowance=current_base_asset_allowance,
             current_quote_asset_allowance=current_quote_asset_allowance
@@ -376,17 +382,20 @@
         :type event_data: EventData
         """
         raw_event = event_type(block_number=event_data["blockNumber"], **event_data["args"])
 
         if raw_event.client_filter(wallet=self.wallet):
             pair = self._pairs.get(pair_name)
 
-            order_event = OrderEvent.from_event(pair=pair, event=raw_event, wallet=self.wallet)
+            if isinstance(raw_event, EmitFeeEvent):
+                event = FeeEvent.from_event(pair=pair, event=raw_event)
+            else:
+                event = OrderEvent.from_event(pair=pair, event=raw_event, wallet=self.wallet)
 
-            self.message_queue.put(order_event)
+            self.message_queue.put(event)
 
     ######################################################################
     # order methods
     ######################################################################
 
     def place_market_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a market order transaction by executing the specified transaction object. The transaction
@@ -409,29 +418,23 @@
         match order.order_side:
             case OrderSide.BUY:
                 return self.market.buy_all_amount(
                     buy_gem=pair.base_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.quote_asset.address,
                     max_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price),
-                    nonce=transaction.nonce,
-                    gas=transaction.gas,
-                    max_fee_per_gas=transaction.max_fee_per_gas,
-                    max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+                    **transaction.args(),
                 )
             case OrderSide.SELL:
                 return self.market.sell_all_amount(
                     pay_gem=pair.base_asset.address,
                     pay_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.quote_asset.address,
                     min_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price),
-                    nonce=transaction.nonce,
-                    gas=transaction.gas,
-                    max_fee_per_gas=transaction.max_fee_per_gas,
-                    max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+                    **transaction.args(),
                 )
 
     def place_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order transaction by executing the specified transaction object. The transaction object should
         contain a single order of type NewLimitOrder.
 
         :param transaction: Transaction object containing the limit order.
@@ -450,29 +453,23 @@
         match order.order_side:
             case OrderSide.BUY:
                 return self.market.offer(
                     pay_amt=pair.quote_asset.to_integer(order.price * order.size),
                     pay_gem=pair.quote_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.base_asset.address,
-                    nonce=transaction.nonce,
-                    gas=transaction.gas,
-                    max_fee_per_gas=transaction.max_fee_per_gas,
-                    max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+                    **transaction.args(),
                 )
             case OrderSide.SELL:
                 return self.market.offer(
                     pay_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.base_asset.address,
                     buy_amt=pair.quote_asset.to_integer(order.price * order.size),
                     buy_gem=pair.quote_asset.address,
-                    nonce=transaction.nonce,
-                    gas=transaction.gas,
-                    max_fee_per_gas=transaction.max_fee_per_gas,
-                    max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+                    **transaction.args(),
                 )
 
     def cancel_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order cancel transaction by executing the specified transaction object. The transaction object
         should contain a single order of type NewCancelOrder.
 
         :param transaction: Transaction object containing the cancel order.
@@ -484,18 +481,15 @@
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewCancelOrder = transaction.orders[0]  # noqa
 
         return self.market.cancel(
             id=order.order_id,
-            nonce=transaction.nonce,
-            gas=transaction.gas,
-            max_fee_per_gas=transaction.max_fee_per_gas,
-            max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+            **transaction.args(),
         )
 
     def batch_place_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Place multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit orders.
         :type transaction: Transaction
@@ -524,18 +518,15 @@
                     buy_gems.append(pair.quote_asset.address)
 
         return self.market.batch_offer(
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
-            nonce=transaction.nonce,
-            gas=transaction.gas,
-            max_fee_per_gas=transaction.max_fee_per_gas,
-            max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+            **transaction.args(),
         )
 
     def batch_update_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Update multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order updates.
         :type transaction: Transaction
@@ -562,23 +553,21 @@
                     buy_gems.append(pair.base_asset.address)
                 case OrderSide.SELL:
                     pay_amts.append(pair.base_asset.to_integer(order.size))
                     pay_gems.append(pair.base_asset.address)
                     buy_amts.append(pair.quote_asset.to_integer(order.price * order.size))
                     buy_gems.append(pair.quote_asset.address)
 
-        return self.market.batch_offer(
+        return self.market.batch_requote(
+            ids=order_ids,
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
-            nonce=transaction.nonce,
-            gas=transaction.gas,
-            max_fee_per_gas=transaction.max_fee_per_gas,
-            max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+            **transaction.args(),
         )
 
     def batch_cancel_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Cancel multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order cancellations.
         :type transaction: Transaction
@@ -590,18 +579,15 @@
         for order in transaction.orders:
             order: NewCancelOrder
 
             order_ids.append(order.order_id)
 
         return self.market.batch_cancel(
             ids=order_ids,
-            nonce=transaction.nonce,
-            gas=transaction.gas,
-            max_fee_per_gas=transaction.max_fee_per_gas,
-            max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
+            **transaction.args(),
         )
 
     ######################################################################
     # helper methods
     ######################################################################
 
     # TODO: revisit as the safer thing is to set approval to 0 and then set approval to new_allowance
```

### Comparing `rubi-2.0.3/rubi/contracts/aid.py` & `rubi-2.0.4b1/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/contracts/base_contract.py` & `rubi-2.0.4b1/rubi/contracts/base_contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3._utils.filters import LogFilter  # noqa
 from web3.contract import Contract
 from web3.contract.contract import ContractFunction
 from web3.types import ABI, Nonce
 
-from rubi.contracts.types import BaseEvent, TransactionReceipt
+from rubi.contracts.contract_types import BaseEvent, TransactionReceipt
 
 
 class BaseContract:
     """Base class representation of a contract which defines the structure of a contract and provides several helpful
     methods that can be used by subclass contracts that extend this contract.
 
     :param w3: Web3 instance
```

### Comparing `rubi-2.0.3/rubi/contracts/erc20.py` & `rubi-2.0.4b1/rubi/contracts/erc20.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 from web3.types import ABI
 
 from rubi.contracts.base_contract import BaseContract
-from rubi.contracts.types import TransactionReceipt
+from rubi.contracts.contract_types import TransactionReceipt
 from rubi.network import Network
 
 
 class ERC20(BaseContract):
     """this class represents a contract that implements the ERC20 standard. it is used to read the contract instance.
     if a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
```

### Comparing `rubi-2.0.3/rubi/contracts/market.py` & `rubi-2.0.4b1/rubi/contracts/market.py`

 * *Files identical despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Tuple, List
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 
 from rubi.contracts.base_contract import BaseContract
-from rubi.contracts.types import TransactionReceipt
+from rubi.contracts.contract_types import TransactionReceipt
 from rubi.network import Network
 
 
 class RubiconMarket(BaseContract):
     """This class represents the RubiconMarket.sol contract and by default has read functionality.
     If a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
 
@@ -326,15 +326,15 @@
     def batch_offer(
         self,
         pay_amts: List[int],
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: int = 3500000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Batch the placement of a set of offers in one transaction
 
         :param pay_amts: the amounts of the token being sold
         :type pay_amts: List[int]
@@ -372,15 +372,15 @@
         )
 
     # batchCancel (ids (uint256[])) -> bool[]
     def batch_cancel(
         self,
         ids: List[int],
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: int = 3500000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Cancel a set offer by offer id in a single transaction
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
@@ -394,15 +394,15 @@
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
-        cancels = self.contract.functions.cancel(ids)
+        cancels = self.contract.functions.batchCancel(ids)
 
         return self._default_transaction_handler(
             instantiated_contract_function=cancels,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
             max_priority_fee_per_gas=max_priority_fee_per_gas
@@ -414,15 +414,15 @@
         self,
         ids: List[int],
         pay_amts: List[int],
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: int = 3500000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Batch update a set of offers in a single transaction and return a list of new offer ids
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
@@ -539,16 +539,16 @@
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
-        buy_all_amount = self.contract.functions.sellAllAmount(buy_gem, buy_amt, pay_gem, max_fill_amount)
+        buy_all_amount = self.contract.functions.buyAllAmount(buy_gem, buy_amt, pay_gem, max_fill_amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=buy_all_amount,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
             max_priority_fee_per_gas=max_priority_fee_per_gas
-        )
+        )
```

### Comparing `rubi-2.0.3/rubi/contracts/router.py` & `rubi-2.0.4b1/rubi/contracts/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Tuple, List
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 
 from rubi.contracts.base_contract import BaseContract
-from rubi.contracts.types import TransactionReceipt
+from rubi.contracts.contract_types import TransactionReceipt
 from rubi.network import Network
 
 
 class RubiconRouter(BaseContract):
     """This class represents the RubiconRouter.sol contract and by default has read functionality.
     If a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
```

### Comparing `rubi-2.0.3/rubi/contracts/types/events.py` & `rubi-2.0.4b1/rubi/contracts/contract_types/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
         """implementation of BaseEvent create_event_filter"""
         return contract.events.emitFee.create_filter(argument_filters=argument_filters, fromBlock="latest")
 
     @staticmethod
     def default_filters(bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress) -> dict:
         """implementation of BaseEvent default_filters"""
-        filters = {"pair": [bid_identifier, ask_identifier], "fee_to": wallet}
+        filters = {"feeTo": wallet}
 
         return {key: value for key, value in filters.items() if value is not None}
 
 
 class EmitDeleteEvent(BaseMarketEvent):
     """Event emitted whenever an offer is fully taken by a market order on the RubiconMarket resulting in the offer
     being closed
```

### Comparing `rubi-2.0.3/rubi/contracts/types/transaction_reciept.py` & `rubi-2.0.4b1/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/data.py` & `rubi-2.0.4b1/rubi/data/data.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/processing/README.md` & `rubi-2.0.4b1/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/processing/aid.py` & `rubi-2.0.4b1/rubi/data/processing/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/processing/helper/processing.py` & `rubi-2.0.4b1/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/processing/user.py` & `rubi-2.0.4b1/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/sources/aid.py` & `rubi-2.0.4b1/rubi/data/sources/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/sources/helper/README.md` & `rubi-2.0.4b1/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/sources/helper/gas.py` & `rubi-2.0.4b1/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/sources/helper/price.py` & `rubi-2.0.4b1/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/sources/helper/rolodex.py` & `rubi-2.0.4b1/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/data/sources/market.py` & `rubi-2.0.4b1/rubi/data/sources/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.3/rubi/network/network.py` & `rubi-2.0.4b1/rubi/network/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         rubicon: dict,
         token_addresses: dict,
         # optional custom token config file from the user
         custom_token_addresses_file: Optional[str] = None
     ):
         """Initializes a Network instance.
 
-        :param path: The path to the network configuration.
+        :param path: The path to the network configuration folder.
         :type path: str
         :param w3: The Web3 instance connected to the network.
         :type w3: Web3
         :param name: The name of the network.
         :type name: str
         :param chain_id: The chain ID of the network.
         :type chain_id: int
```

### Comparing `rubi-2.0.3/rubi/types/order.py` & `rubi-2.0.4b1/rubi/rubicon_types/order.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 from _decimal import Decimal
 from enum import Enum
-from typing import Optional, Union, List
+from typing import Optional, Union, List, Dict
 
 from eth_typing import ChecksumAddress
 
-from rubi.contracts.types.events import BaseEvent, EmitOfferEvent, EmitCancelEvent, EmitTakeEvent
-from rubi.types.pair import Pair
+from rubi.contracts.contract_types.events import BaseEvent, EmitOfferEvent, EmitCancelEvent, EmitTakeEvent, \
+    EmitDeleteEvent, EmitFeeEvent
+from rubi.rubicon_types.pair import Pair
 
 
 class OrderSide(Enum):
     """Enumeration representing the order side."""
     BUY = "BUY"
     SELL = "SELL"
+    NEUTRAL = "NEUTRAL"
+
+    def sign(self) -> int:
+        """
+        :return: Numerical value of the side.
+        :rtype: int
+        """
+        match self:
+            case OrderSide.NEUTRAL:
+                return 0
+
+            case OrderSide.BUY:
+                return 1
+
+            case OrderSide.SELL:
+                return -1
 
 
 class OrderType(Enum):
     """Enumeration representing the order type."""
     MARKET = "MARKET"
     LIMIT = "LIMIT"
 
     # Only used for events coming from the RubiconMarket
     LIMIT_TAKEN = "LIMIT_TAKEN"
+    LIMIT_DELETED = "LIMIT_DELETED"
     CANCEL = "CANCEL"
 
 
 class BaseNewOrder:
     """Base class for representing a new order.
 
     :param pair_name: The name of the trading pair.
@@ -151,102 +169,113 @@
 
 
 class NewCancelOrder(BaseNewOrder):
     """Class representing a limit order cancellation
 
     :param pair_name: The name of the trading pair.
     :type pair_name: str
-    :param order_side: The side of the order (buy or sell).
-    :type order_side: OrderSide
     :param order_id: The ID of the order to cancel.
     :type order_id: int
     """
 
     def __init__(
         self,
         pair_name: str,
-        order_side: OrderSide,
         order_id: int
     ):
         """constructor method"""
         super().__init__(
             pair_name=pair_name,
             order_type=OrderType.LIMIT,
-            order_side=order_side,
+            order_side=OrderSide.NEUTRAL,
         )
 
         self.order_id = order_id
 
 
 class Transaction:
     """
     Class representing a transaction to be executed on chain
 
     :param orders: The list of orders to include in the transaction.
     :type orders: List[BaseNewOrder]
     :param nonce: The nonce for the transaction (optional).
     :type nonce: int
-    :param gas: The gas limit for the transaction.
+    :param gas: The gas limit for the transaction (optional)
     :type gas: int
     :param max_fee_per_gas: The maximum fee per gas for the transaction (optional).
     :type max_fee_per_gas: int
     :param max_priority_fee_per_gas: The maximum priority fee per gas for the transaction (optional).
     :type max_priority_fee_per_gas: int
     """
 
     def __init__(
         self,
         orders: List[BaseNewOrder],
         nonce: Optional[int] = None,
-        gas: int = 3500000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ):
         """constructor method"""
         if len(orders) < 1:
             raise Exception("Transaction cannot be instantiated with an empty order list")
 
         self.orders = orders
         self.nonce = nonce
         self.gas = gas
         self.max_fee_per_gas = max_fee_per_gas
         self.max_priority_fee_per_gas = max_priority_fee_per_gas
 
+    def args(self) -> Dict:
+        """Creates a dictionary of not None arguments to pass to contract functions.
+        :return: dictionary of arguments used to send transactions.
+        :rtype: Dict
+        """
+        args = {
+            "nonce": self.nonce,
+            "gas": self.gas,
+            "max_fee_per_gas": self.max_fee_per_gas,
+            "max_priority_fee_per_gas": self.max_priority_fee_per_gas
+        }
+
+        return {key: value for key, value in args.items() if value is not None}
+
 
 class OrderEvent:
     """Class to represent Rubicon Market events as an order
 
     :param limit_order_id: The ID of the limit order.
     :type limit_order_id: int
     :param limit_order_owner: The owner of the limit order.
     :type limit_order_owner: ChecksumAddress
     :param market_order_owner: The owner of the market order (optional). Only has a value if event is an emitTakeEvent.
     :type market_order_owner: Optional[ChecksumAddress]
     :param pair_name: The name of the pair being traded e.g. WETH/USDC.
     :type pair_name: str
     :param order_side: The side of the order (BUY or SELL).
     :type order_side: OrderSide
-    :param order_type: The type of the order (MARKET, LIMIT, LIMIT_TAKEN, or CANCEL).
+    :param order_type: The type of the order (MARKET, LIMIT, LIMIT_TAKEN, LIMIT_DELETED, or CANCEL).
     :type order_type: OrderType
     :param price: The price of the order.
     :type price: Decimal
     :param size: The size of the order.
     :type size: Decimal
     """
 
     def __init__(
         self,
         limit_order_id: int,
         limit_order_owner: ChecksumAddress,
         market_order_owner: Optional[ChecksumAddress],
         pair_name: str,
-        order_side: OrderSide,
+        order_side: Optional[OrderSide],
         order_type: OrderType,
-        price: Decimal,
-        size: Decimal,
+        price: Optional[Decimal],
+        size: Optional[Decimal],
     ):
         self.limit_order_id = limit_order_id
         self.limit_order_owner = limit_order_owner
         self.market_order_owner: Optional[ChecksumAddress] = market_order_owner
         self.pair_name = pair_name
         self.order_side = order_side
         self.order_type = order_type
@@ -262,15 +291,15 @@
         :param event: The event to convert.
         :type event: BaseEvent
         :param wallet: The wallet address associated with the event.
         :type wallet: ChecksumAddress
         :return: The created OrderEvent.
         :rtype: OrderEvent
         :raises Exception: If the event cannot be converted into an OrderEvent. This occurs if the Base event has a type
-            other than EmitOfferEvent, EmitCancelEvent or EmitTakeEvent
+            other than EmitOfferEvent, EmitCancelEvent, EmitTakeEvent or EmitDeleteEvent
         """
         if isinstance(event, EmitOfferEvent):
             if pair.bid_identifier == event.pair:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=OrderSide.BUY,
@@ -324,46 +353,66 @@
                     event=event,
                     pair=pair,
                     side=OrderSide.SELL if wallet == event.maker else OrderSide.BUY,
                     order_type=OrderType.LIMIT_TAKEN if wallet == event.maker else OrderType.MARKET,
                     base_amt=event.take_amt,
                     quote_amt=event.give_amt
                 )
+        elif isinstance(event, EmitDeleteEvent):
+            if pair.bid_identifier == event.pair:
+                return cls._build_order(
+                    event=event,
+                    pair=pair,
+                    side=None,
+                    order_type=OrderType.LIMIT_DELETED,
+                    base_amt=None,
+                    quote_amt=None
+                )
+            else:
+                return cls._build_order(
+                    event=event,
+                    pair=pair,
+                    side=None,
+                    order_type=OrderType.LIMIT_DELETED,
+                    base_amt=None,
+                    quote_amt=None
+                )
+
         else:
             Exception(f"{event.__class__} cannot be converted into an OrderEvent")
 
     @classmethod
     def _build_order(
         cls,
-        event: Union[EmitOfferEvent, EmitCancelEvent, EmitTakeEvent],
+        event: Union[EmitOfferEvent, EmitCancelEvent, EmitTakeEvent, EmitDeleteEvent],
         pair: Pair,
-        side: OrderSide,
+        side: Optional[OrderSide],
         order_type: OrderType,
-        base_amt: int,
-        quote_amt: int
+        base_amt: Optional[int],
+        quote_amt: Optional[int]
     ) -> "OrderEvent":
         """Build an OrderEvent from event data.
 
         :param event: The event data.
         :type event: Union[EmitOfferEvent, EmitCancelEvent, EmitTakeEvent]
         :param pair: The asset pair associated with the event.
         :type pair: Pair
         :param side: The order side.
-        :type side: OrderSide
+        :type side: Optional[OrderSide]
         :param order_type: The order type.
         :type order_type: OrderType
         :param base_amt: The base amount of the order.
-        :type base_amt: int
+        :type base_amt: Optional[int]
         :param quote_amt: The quote amount of the order.
-        :type quote_amt: int
+        :type quote_amt: Optional[int]
         :return: The constructed OrderEvent.
         :rtype: OrderEvent
         """
-        size = pair.base_asset.to_decimal(base_amt)
-        price = pair.quote_asset.to_decimal(quote_amt) / size
+        size = pair.base_asset.to_decimal(base_amt) if base_amt else None
+        price = pair.quote_asset.to_decimal(quote_amt) / size if quote_amt else None
 
         return cls(
             limit_order_id=event.id,
             limit_order_owner=event.maker,
             market_order_owner=event.taker if isinstance(event, EmitTakeEvent) else None,
             pair_name=pair.name,
             order_side=side,
@@ -371,7 +420,53 @@
             size=size,
             price=price
         )
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
+
+
+class FeeEvent:
+    def __init__(
+        self,
+        id: int,
+        pair_name: str,
+        fee_to: ChecksumAddress,
+        market_order_owner: ChecksumAddress,
+        fee: Decimal,
+        fee_asset: str,
+    ):
+        self.id = id
+        self.pair_name = pair_name
+        self.fee_to = fee_to
+        self.market_order_owner = market_order_owner
+        self.fee = fee
+        self.fee_asset = fee_asset
+
+    @classmethod
+    def from_event(
+        cls,
+        pair: Pair,
+        event: EmitFeeEvent,
+    ) -> "FeeEvent":
+        if event.asset == pair.base_asset.address:
+            fee = pair.base_asset.to_decimal(event.fee_amt)
+            asset_symbol = pair.base_asset.symbol
+        elif event.asset == pair.quote_asset.address:
+            fee = pair.quote_asset.to_decimal(event.fee_amt)
+            asset_symbol = pair.quote_asset.symbol
+        else:
+            raise Exception("Unexpected fee asset")
+
+        return cls(
+            id=event.id,
+            pair_name=pair.name,
+            fee_to=event.fee_to,
+            market_order_owner=event.taker,
+            fee=fee,
+            fee_asset=asset_symbol
+        )
+
+    def __repr__(self):
+        items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
+        return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.0.3/rubi/types/orderbook.py` & `rubi-2.0.4b1/rubi/rubicon_types/orderbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from _decimal import Decimal
 from typing import List, Tuple
 
 from rubi import ERC20
-from rubi.types.order import OrderSide
+from rubi.rubicon_types.order import OrderSide
 
 
 class BookLevel:
     """Class representing a level in the order book.
 
     :param price: The price of the level.
     :type price: Decimal
```

### Comparing `rubi-2.0.3/rubi/types/pair.py` & `rubi-2.0.4b1/rubi/rubicon_types/pair.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from _decimal import Decimal
+from typing import Optional
 
 from rubi import ERC20
 
 
 class Pair:
     """Class representing a trading asset pair, e.g. WETH/USDC would have WETH as the base asset and USDC as the quote
     asset.
 
     :param name: The name of the pair, e.g. WETH/USDC.
     :type name: str
     :param base_asset: Base asset of the pair.
     :type base_asset: ERC20
     :param quote_asset: Quote asset of the pair.
     :type quote_asset: ERC20
-    :param current_base_asset_allowance: The base asset spending allowance of the RubiconMarket contract.
+    :param current_base_asset_allowance: The base asset spending allowance of the RubiconMarket contract, Optional.
     :type current_base_asset_allowance: Decimal
-    :param current_quote_asset_allowance: The quote asset spending allowance of the RubiconMarket contract.
+    :param current_quote_asset_allowance: The quote asset spending allowance of the RubiconMarket contract, Optional.
     :type current_quote_asset_allowance: Decimal
     """
 
     def __init__(
         self,
         name: str,
         base_asset: ERC20,
         quote_asset: ERC20,
-        current_base_asset_allowance: Decimal,
-        current_quote_asset_allowance: Decimal
+        current_base_asset_allowance: Optional[Decimal],
+        current_quote_asset_allowance: Optional[Decimal]
     ):
         self.name = name
 
         self.base_asset: ERC20 = base_asset
         self.quote_asset: ERC20 = quote_asset
 
         self.bid_identifier: str = base_asset.w3.solidity_keccak(
@@ -37,15 +38,15 @@
             values=[self.quote_asset.address, self.base_asset.address]
         ).hex()
         self.ask_identifier: str = base_asset.w3.solidity_keccak(
             abi_types=["address", "address"],
             values=[self.base_asset.address, self.quote_asset.address]
         ).hex()
 
-        # TODO: think about structure of allowances on this class. Currently this only caters for the RubiconMarket
+        # TODO: think about structure of allowances on this class. Currently, this only caters for the RubiconMarket
         #  contract.
         self.current_base_asset_allowance = current_base_asset_allowance
         self.current_quote_asset_allowance = current_quote_asset_allowance
 
     def update_base_asset_allowance(self, new_base_asset_allowance: Decimal) -> None:
         """Update the current base asset allowance.
```

### Comparing `rubi-2.0.3/PKG-INFO` & `rubi-2.0.4b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.3
+Version: 2.0.4b1
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

