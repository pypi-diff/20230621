# Comparing `tmp/rubi-2.0.4.tar.gz` & `tmp/rubi-2.0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.4.tar", max compression
+gzip compressed data, was "rubi-2.0.4b1.tar", max compression
```

## Comparing `rubi-2.0.4.tar` & `rubi-2.0.4b1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.4/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.4/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.4/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.4/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.4/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.4/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      633 2023-06-13 17:59:13.620185 rubi-2.0.4/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.4/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.4/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      651 2023-06-13 17:59:13.620375 rubi-2.0.4/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.4/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.4/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      508 2023-06-13 17:59:13.620539 rubi-2.0.4/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.4/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.4/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      619 2023-06-13 17:59:13.620686 rubi-2.0.4/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0      748 2023-06-21 19:23:51.928609 rubi-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-21 19:17:01.151640 rubi-2.0.4/rubi/__init__.py
--rw-r--r--   0        0        0    25763 2023-06-21 19:17:01.151931 rubi-2.0.4/rubi/client.py
--rw-r--r--   0        0        0      163 2023-06-21 19:17:01.152075 rubi-2.0.4/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.4/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11403 2023-06-21 19:17:01.152239 rubi-2.0.4/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       73 2023-06-21 19:17:01.152321 rubi-2.0.4/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15968 2023-06-21 19:17:01.152942 rubi-2.0.4/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2674 2023-06-21 19:17:01.153096 rubi-2.0.4/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    16609 2023-06-21 19:17:01.153278 rubi-2.0.4/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24669 2023-06-21 19:17:01.153743 rubi-2.0.4/rubi/contracts/market.py
--rw-r--r--   0        0        0    14847 2023-06-21 19:17:01.153923 rubi-2.0.4/rubi/contracts/router.py
--rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.4/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.4/rubi/data/__init__.py
--rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.4/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.4/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.4/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.4/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.4/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.4/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.4/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.4/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.4/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.4/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.4/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.4/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.4/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.4/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.4/rubi/data/sources/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.4/rubi/network/__init__.py
--rw-r--r--   0        0        0     7596 2023-06-21 19:17:01.154084 rubi-2.0.4/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-21 19:17:01.154162 rubi-2.0.4/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15552 2023-06-21 19:17:01.154405 rubi-2.0.4/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0     5727 2023-06-21 19:17:01.154503 rubi-2.0.4/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2776 2023-06-21 19:17:01.154577 rubi-2.0.4/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.4/PKG-INFO
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

### Comparing `rubi-2.0.4/LICENSE` & `rubi-2.0.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/README.md` & `rubi-2.0.4b1/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/ERC20.json` & `rubi-2.0.4b1/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/README.md` & `rubi-2.0.4b1/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/abitrum_goerli/abis/market.json` & `rubi-2.0.4b1/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/abitrum_goerli/abis/router.json` & `rubi-2.0.4b1/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/abitrum_goerli/network.yaml` & `rubi-2.0.4b1/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/optimism/abis/market.json` & `rubi-2.0.4b1/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/optimism/abis/router.json` & `rubi-2.0.4b1/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/optimism/network.yaml` & `rubi-2.0.4b1/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/optimism_goerli/abis/market.json` & `rubi-2.0.4b1/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/optimism_goerli/abis/router.json` & `rubi-2.0.4b1/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/polygon_mumbai/abis/market.json` & `rubi-2.0.4b1/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/polygon_mumbai/abis/router.json` & `rubi-2.0.4b1/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/network_config/polygon_mumbai/network.yaml` & `rubi-2.0.4b1/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/pyproject.toml` & `rubi-2.0.4b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.0.4"
+version = "2.0.4b1"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.0.4/rubi/client.py` & `rubi-2.0.4b1/rubi/client.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/contracts/aid.py` & `rubi-2.0.4b1/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/contracts/base_contract.py` & `rubi-2.0.4b1/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/contracts/contract_types/events.py` & `rubi-2.0.4b1/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.0.4b1/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/contracts/erc20.py` & `rubi-2.0.4b1/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/contracts/market.py` & `rubi-2.0.4b1/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/contracts/router.py` & `rubi-2.0.4b1/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/data.py` & `rubi-2.0.4b1/rubi/data/data.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/processing/README.md` & `rubi-2.0.4b1/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/processing/aid.py` & `rubi-2.0.4b1/rubi/data/processing/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/processing/helper/processing.py` & `rubi-2.0.4b1/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/processing/user.py` & `rubi-2.0.4b1/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/sources/aid.py` & `rubi-2.0.4b1/rubi/data/sources/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/sources/helper/README.md` & `rubi-2.0.4b1/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/sources/helper/gas.py` & `rubi-2.0.4b1/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/sources/helper/price.py` & `rubi-2.0.4b1/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/sources/helper/rolodex.py` & `rubi-2.0.4b1/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/data/sources/market.py` & `rubi-2.0.4b1/rubi/data/sources/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/network/network.py` & `rubi-2.0.4b1/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/rubicon_types/order.py` & `rubi-2.0.4b1/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/rubicon_types/orderbook.py` & `rubi-2.0.4b1/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/rubi/rubicon_types/pair.py` & `rubi-2.0.4b1/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.4/PKG-INFO` & `rubi-2.0.4b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.4
+Version: 2.0.4b1
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

