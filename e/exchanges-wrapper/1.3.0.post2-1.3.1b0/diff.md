# Comparing `tmp/exchanges-wrapper-1.3.0.post2.tar.gz` & `tmp/exchanges_wrapper-1.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges-wrapper-1.3.0.post2.tar", last modified: Mon Jun 19 18:52:52 2023, max compression
+gzip compressed data, was "exchanges_wrapper-1.3.1b0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exchanges-wrapper-1.3.0.post2.tar` & `exchanges_wrapper-1.3.1b0.tar`

### file list

```diff
@@ -1,29 +1,20 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.0.post2/.deepsource.toml
--rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.0.post2/.dockerignore
--rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.0.post2/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.0.post2/.github/dependabot.yml
--rwxr-xr-x   0        0        0     6058 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/CHANGELOG.md
--rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.0.post2/Dockerfile
--rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.0.post2/LICENSE.md
--rw-r--r--   0        0        0     6698 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post2/README.md
--rw-r--r--   0        0        0    15398 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/example/exch_client.py
--rwxr-xr-x   0        0        0      159 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post2/example/ms_cfg.toml
--rw-r--r--   0        0        0     1289 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45215 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19618 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6048 2023-06-13 17:51:56.390756 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    61936 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2601 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12494 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    43798 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4189 2023-02-22 15:25:52.464921 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10270 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16098 2023-03-02 12:37:56.947270 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22384 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0      986 2023-06-19 18:46:17.291107 exchanges-wrapper-1.3.0.post2/pyproject.toml
--rw-r--r--   0        0        0      105 2023-06-19 18:46:17.291107 exchanges-wrapper-1.3.0.post2/requirements.txt
--rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.0.post2/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-06-21 11:42:27.744918 exchanges_wrapper-1.3.1b0/LICENSE.md
+-rw-r--r--   0        0        0     6941 2023-06-21 11:42:27.744918 exchanges_wrapper-1.3.1b0/README.md
+-rw-r--r--   0        0        0     1319 2023-06-21 11:42:27.744918 exchanges_wrapper-1.3.1b0/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    45215 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19618 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6048 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    61936 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2601 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12494 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    43819 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4189 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10270 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15723 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16098 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22384 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1121 2023-06-21 11:42:27.748919 exchanges_wrapper-1.3.1b0/pyproject.toml
+-rw-r--r--   0        0        0     7822 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.1b0/PKG-INFO
```

### Comparing `exchanges-wrapper-1.3.0.post2/LICENSE.md` & `exchanges_wrapper-1.3.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/README.md` & `exchanges_wrapper-1.3.1b0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,32 +39,61 @@
 - Auto reconnect after exchanges API or network failure
 - Completely free and without limitations
 
 ### Added Features
 - Multi exchanges support
 - Adaptive algorithm to ensure maximum performance and avoid exceeding the rates limits
 - Passthrough logging
+- WSS keepalive
+- Reuse session for new client sessions
 
 ## Extra exchanges implementation features
 - Binance REST API and WSS are accepted as basic, connection of other exchanges wrapped their API to Binance compatible
 - For other, some data cannot be obtained by directly calling one method, it is generated by a synthetic or calculation
 method
 - Some exchanges have not any testing or "paper trading" features, therefore, application development and testing is possible only
-at real bidding. First, run applications on the [Binance Spot Test Network](https://testnet.binance.vision/) or Bitfinex test account.
+at real bidding. First, run applications on the [Binance Spot Test Network](https://testnet.binance.vision/) or (Bitfinex, OKX) test account.
 
 ## Get started
 ### Prepare exchange account
 * Create account on [Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10% discount on all trading fee
 * Create account on [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6% rebate fee
 * Create account on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/?invite_code=9uaw3223) and get 10% cashback
 on all trading fee
 * Create account on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes worth up to $10,000
 * For test purpose log in at [Binance Spot Test Network](https://testnet.binance.vision/)
 * Create API Key
-* After install and first run specify api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/exch_srv_cfg.toml```
+* After install and create environment specify api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/exch_srv_cfg.toml```
+
+### Install use PIP
+To install just run the following command:
+```console
+pip install exchanges-wrapper
+```
+After first install create environment by run ```exchanges-wrapper-init``` in terminal window.
+
+The structure of the working directory will be created and the necessary files will be copied:
+For Ubuntu it will be here: ```home/user/.MartinBinance/```
+
+For upgrade to latest versions use:
+```console
+pip install -U exchanges-wrapper
+```
+
+#### Start server
+* Run in terminal window
+  ```
+  exchanges-wrapper-srv
+  ``` 
+  
+* Use an example to study
+  + Copy [example/ms_cfg.toml](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/example/ms_cfg.toml)
+  to ```/home/ubuntu/.MartinBinance/config/``` and select (uncomment) desired exchange. Don't change exchange name.
+  + Run [example/exch_client.py](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/example/exch_client.py)
+  in other terminal window
 
 ### Use Docker image
 ```console
 docker pull ghcr.io/dogstailfarmer/exchanges-wrapper:latest
 ```
 #### First run
 The structure of the working directory will be created and the necessary files will be copied:
@@ -80,35 +109,14 @@
  --mount type=bind,source=/home/ubuntu/.MartinBinance,target=/home/appuser/.MartinBinance \
  --network=host \
  --restart=always \
  --name=exchanges-wrapper \
  exchanges-wrapper
 ```
 
-### Install use PIP
-To install the library, you can just run the following command:
-```console
-pip install exchanges-wrapper
-```
-After first install run ```exchanges_wrapper/exch_srv.py```
-You can find this where pip installs packages, often it's ```/home/ubuntu/.local/lib/python3.10/site-packages```
-
-The structure of the working directory will be created and the necessary files will be copied:
-For Ubuntu it will be here: ```home/user/.MartinBinance/```
-
-For upgrade to latest versions use:
-```console
-pip install -U martin-binance
-```
-
-### Start server
-* Run ```exchanges_wrapper/exch_srv.py``` in terminal window
-* In ```example/ms_cfg.toml``` select desired exchange. Don't change exchange name.
-* Run ```example/exch_client.py``` in other terminal window
-
 ### Documentations
 * For [binance.py](https://th0rgal.gitbook.io/binance-py/) use original
 * Served methods and examples of their use are described at ```example/exch_client.py```
 * For [Protocol Buffers](https://developers.google.com/protocol-buffers/docs/overview) serializing structured data
 see ```proto/exchanges_wrapper/api.proto```
 
 ## Donate
```

#### html2text {}

```diff
@@ -18,59 +18,61 @@
 capabilities (inherited from binance.py) - Covers general endpoints (test
 connectivity and get exchange information's) - Covers market data endpoints -
 Covers Account endpoints (create and manage orders) - Covers user data stream
 (receive real time user updates) - Covers web socket streams (receive real time
 market updates) - Async support - Auto reconnect after exchanges API or network
 failure - Completely free and without limitations ### Added Features - Multi
 exchanges support - Adaptive algorithm to ensure maximum performance and avoid
-exceeding the rates limits - Passthrough logging ## Extra exchanges
-implementation features - Binance REST API and WSS are accepted as basic,
-connection of other exchanges wrapped their API to Binance compatible - For
-other, some data cannot be obtained by directly calling one method, it is
-generated by a synthetic or calculation method - Some exchanges have not any
-testing or "paper trading" features, therefore, application development and
-testing is possible only at real bidding. First, run applications on the
-[Binance Spot Test Network](https://testnet.binance.vision/) or Bitfinex test
-account. ## Get started ### Prepare exchange account * Create account on
-[Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10%
-discount on all trading fee * Create account on [Bitfinex](https://
-www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6% rebate fee * Create
-account on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
-?invite_code=9uaw3223) and get 10% cashback on all trading fee * Create account
-on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes worth up to
-$10,000 * For test purpose log in at [Binance Spot Test Network](https://
-testnet.binance.vision/) * Create API Key * After install and first run specify
-api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/
-exch_srv_cfg.toml``` ### Use Docker image ```console docker pull ghcr.io/
-dogstailfarmer/exchanges-wrapper:latest ``` #### First run The structure of the
-working directory will be created and the necessary files will be copied: For
-Ubuntu it will be here: ```home/user/.MartinBinance/``` ```console docker run -
--rm --entrypoint /bin/sh exchanges-wrapper -c "cat ./exchanges_wrapper/
-__init__.py" > init.py && \ docker run --rm --entrypoint /bin/sh exchanges-
-wrapper -c "cat ./exchanges_wrapper/exch_srv_cfg.toml.template" >
-exch_srv_cfg.toml.template &&\ python3 init.py && rm init.py && rm
-exch_srv_cfg.toml.template ``` #### Start server ```console docker run -itP \ -
--mount type=bind,source=/home/ubuntu/.MartinBinance,target=/home/
-appuser/.MartinBinance \ --network=host \ --restart=always \ --name=exchanges-
-wrapper \ exchanges-wrapper ``` ### Install use PIP To install the library, you
-can just run the following command: ```console pip install exchanges-wrapper
-``` After first install run ```exchanges_wrapper/exch_srv.py``` You can find
-this where pip installs packages, often it's ```/home/ubuntu/.local/lib/
-python3.10/site-packages``` The structure of the working directory will be
+exceeding the rates limits - Passthrough logging - WSS keepalive - Reuse
+session for new client sessions ## Extra exchanges implementation features -
+Binance REST API and WSS are accepted as basic, connection of other exchanges
+wrapped their API to Binance compatible - For other, some data cannot be
+obtained by directly calling one method, it is generated by a synthetic or
+calculation method - Some exchanges have not any testing or "paper trading"
+features, therefore, application development and testing is possible only at
+real bidding. First, run applications on the [Binance Spot Test Network](https:
+//testnet.binance.vision/) or (Bitfinex, OKX) test account. ## Get started ###
+Prepare exchange account * Create account on [Binance](https://
+accounts.binance.com/en/register?ref=QCS4OGWR) and get 10% discount on all
+trading fee * Create account on [Bitfinex](https://www.bitfinex.com/sign-
+up?refcode=v_4az2nCP) and get 6% rebate fee * Create account on [HUOBI](https:/
+/www.huobi.com/en-us/topic/double-reward/?invite_code=9uaw3223) and get 10%
+cashback on all trading fee * Create account on [OKX](https://www.okx.com/join/
+2607649) and get Mystery Boxes worth up to $10,000 * For test purpose log in at
+[Binance Spot Test Network](https://testnet.binance.vision/) * Create API Key *
+After install and create environment specify api_key and api_secret in ```/
+home/ubuntu/.MartinBinance/config/exch_srv_cfg.toml``` ### Install use PIP To
+install just run the following command: ```console pip install exchanges-
+wrapper ``` After first install create environment by run ```exchanges-wrapper-
+init``` in terminal window. The structure of the working directory will be
 created and the necessary files will be copied: For Ubuntu it will be here:
 ```home/user/.MartinBinance/``` For upgrade to latest versions use: ```console
-pip install -U martin-binance ``` ### Start server * Run ```exchanges_wrapper/
-exch_srv.py``` in terminal window * In ```example/ms_cfg.toml``` select desired
-exchange. Don't change exchange name. * Run ```example/exch_client.py``` in
-other terminal window ### Documentations * For [binance.py](https://
-th0rgal.gitbook.io/binance-py/) use original * Served methods and examples of
-their use are described at ```example/exch_client.py``` * For [Protocol
-Buffers](https://developers.google.com/protocol-buffers/docs/overview)
-serializing structured data see ```proto/exchanges_wrapper/api.proto``` ##
-Donate *BNB*, *BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92
-*USDT* (TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-
-wrapper
+pip install -U exchanges-wrapper ``` #### Start server * Run in terminal window
+``` exchanges-wrapper-srv ``` * Use an example to study + Copy [example/
+ms_cfg.toml](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/
+example/ms_cfg.toml) to ```/home/ubuntu/.MartinBinance/config/``` and select
+(uncomment) desired exchange. Don't change exchange name. + Run [example/
+exch_client.py](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/
+master/example/exch_client.py) in other terminal window ### Use Docker image
+```console docker pull ghcr.io/dogstailfarmer/exchanges-wrapper:latest ``` ####
+First run The structure of the working directory will be created and the
+necessary files will be copied: For Ubuntu it will be here: ```home/
+user/.MartinBinance/``` ```console docker run --rm --entrypoint /bin/sh
+exchanges-wrapper -c "cat ./exchanges_wrapper/__init__.py" > init.py && \
+docker run --rm --entrypoint /bin/sh exchanges-wrapper -c "cat ./
+exchanges_wrapper/exch_srv_cfg.toml.template" > exch_srv_cfg.toml.template &&\
+python3 init.py && rm init.py && rm exch_srv_cfg.toml.template ``` #### Start
+server ```console docker run -itP \ --mount type=bind,source=/home/
+ubuntu/.MartinBinance,target=/home/appuser/.MartinBinance \ --network=host \ --
+restart=always \ --name=exchanges-wrapper \ exchanges-wrapper ``` ###
+Documentations * For [binance.py](https://th0rgal.gitbook.io/binance-py/) use
+original * Served methods and examples of their use are described at
+```example/exch_client.py``` * For [Protocol Buffers](https://
+developers.google.com/protocol-buffers/docs/overview) serializing structured
+data see ```proto/exchanges_wrapper/api.proto``` ## Donate *BNB*, *BUSD*,
+*USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT* (TRC20)
+TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-wrapper
 [https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/
 Modified%20martingale.svg]
 [martin-binance](https://github.com/DogsTailFarmer/martin-binance) Free trading
 system for crypto exchanges SPOT markets. Adaptive customizable reverse grid
 strategy based on martingale.
```

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/__init__.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.0-2"
+__version__ = "1.3.1b0"
 
 from pathlib import Path
 import shutil
-#
-import platform
-print(f"Python {platform.python_version()}")
-#
+
 WORK_PATH = Path(Path.home(), ".MartinBinance")
 CONFIG_PATH = Path(WORK_PATH, "config")
 CONFIG_FILE = Path(CONFIG_PATH, "exch_srv_cfg.toml")
 LOG_PATH = Path(WORK_PATH, "exch_srv_log")
 LOG_FILE = Path(LOG_PATH, "exch_srv.log")
 
-if CONFIG_FILE.exists():
-    print(f"Config found at {CONFIG_FILE}")
-else:
-    print("Can't find config file! Creating it...")
-    CONFIG_PATH.mkdir(parents=True, exist_ok=True)
-    LOG_PATH.mkdir(parents=True, exist_ok=True)
-    shutil.copy(Path(Path(__file__).parent.absolute(), "exch_srv_cfg.toml.template"), CONFIG_FILE)
-    print(f"Before first run place account(s) API key into {CONFIG_FILE}")
-    raise SystemExit(1)
+def init():
+    if CONFIG_FILE.exists():
+        print(f"Server config found at {CONFIG_FILE}")
+    else:
+        print("Can't find config file! Creating it...")
+        CONFIG_PATH.mkdir(parents=True, exist_ok=True)
+        LOG_PATH.mkdir(parents=True, exist_ok=True)
+        shutil.copy(Path(Path(__file__).parent.absolute(), "exch_srv_cfg.toml.template"), CONFIG_FILE)
+        print(f"Before first run place account(s) API key into {CONFIG_FILE}")
+        raise SystemExit(1)
+
+if __name__ == '__main__':
+    init()
```

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2_grpc.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/bitfinex_parser.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/c_structures.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/c_structures.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/client.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/definitions.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/errors.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/events.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from exchanges_wrapper.client import Client
 from exchanges_wrapper.definitions import Side, OrderType, TimeInForce, ResponseType
 from exchanges_wrapper.c_structures import OrderUpdateEvent, OrderTradesEvent
 from exchanges_wrapper import WORK_PATH, CONFIG_FILE, LOG_FILE
 #
 HEARTBEAT = 1  # Sec
 MAX_QUEUE_SIZE = 50
+logger = logging.getLogger('exch_srv_logger')
 
 
 def get_account(_account_name: str) -> ():
     config = toml.load(str(CONFIG_FILE))
     accounts = config.get('accounts')
     res = ()
     for account in accounts:
@@ -832,16 +833,15 @@
     api_pb2_grpc.add_MartinServicer_to_server(Martin(), server)
     server.add_insecure_port(listen_addr)
     logger.info(f"Starting server on {listen_addr}")
     await server.start()
     await server.wait_for_termination()
 
 
-if __name__ == '__main__':
-    logger = logging.getLogger('exch_srv_logger')
+def main():
     logger.setLevel(logging.DEBUG)
     formatter = logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s")
     #
     file_handler = logging.handlers.RotatingFileHandler(LOG_FILE, maxBytes=1000000, backupCount=10)
     file_handler.setFormatter(formatter)
     file_handler.setLevel(logging.DEBUG)
     logger.addHandler(file_handler)
@@ -857,7 +857,11 @@
     try:
         loop.run_forever()
     except KeyboardInterrupt:
         pass
     finally:
         loop.run_until_complete(asyncio.sleep(0.250))
         loop.close()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/http_client.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/huobi_parser.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/okx_parser.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/web_sockets.py` & `exchanges_wrapper-1.3.1b0/exchanges_wrapper/web_sockets.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post2/pyproject.toml` & `exchanges_wrapper-1.3.1b0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 ]
 
 [tool.flit.module]
 name = "exchanges_wrapper"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/exchanges-wrapper"
+
+[project.scripts]
+exchanges-wrapper-init = "exchanges_wrapper.__init__:init"
+exchanges-wrapper-srv = "exchanges_wrapper.exch_srv:main"
```

### Comparing `exchanges-wrapper-1.3.0.post2/PKG-INFO` & `exchanges_wrapper-1.3.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.0.post2
+Version: 1.3.1b0
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -61,32 +61,61 @@
 - Auto reconnect after exchanges API or network failure
 - Completely free and without limitations
 
 ### Added Features
 - Multi exchanges support
 - Adaptive algorithm to ensure maximum performance and avoid exceeding the rates limits
 - Passthrough logging
+- WSS keepalive
+- Reuse session for new client sessions
 
 ## Extra exchanges implementation features
 - Binance REST API and WSS are accepted as basic, connection of other exchanges wrapped their API to Binance compatible
 - For other, some data cannot be obtained by directly calling one method, it is generated by a synthetic or calculation
 method
 - Some exchanges have not any testing or "paper trading" features, therefore, application development and testing is possible only
-at real bidding. First, run applications on the [Binance Spot Test Network](https://testnet.binance.vision/) or Bitfinex test account.
+at real bidding. First, run applications on the [Binance Spot Test Network](https://testnet.binance.vision/) or (Bitfinex, OKX) test account.
 
 ## Get started
 ### Prepare exchange account
 * Create account on [Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10% discount on all trading fee
 * Create account on [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6% rebate fee
 * Create account on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/?invite_code=9uaw3223) and get 10% cashback
 on all trading fee
 * Create account on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes worth up to $10,000
 * For test purpose log in at [Binance Spot Test Network](https://testnet.binance.vision/)
 * Create API Key
-* After install and first run specify api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/exch_srv_cfg.toml```
+* After install and create environment specify api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/exch_srv_cfg.toml```
+
+### Install use PIP
+To install just run the following command:
+```console
+pip install exchanges-wrapper
+```
+After first install create environment by run ```exchanges-wrapper-init``` in terminal window.
+
+The structure of the working directory will be created and the necessary files will be copied:
+For Ubuntu it will be here: ```home/user/.MartinBinance/```
+
+For upgrade to latest versions use:
+```console
+pip install -U exchanges-wrapper
+```
+
+#### Start server
+* Run in terminal window
+  ```
+  exchanges-wrapper-srv
+  ``` 
+  
+* Use an example to study
+  + Copy [example/ms_cfg.toml](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/example/ms_cfg.toml)
+  to ```/home/ubuntu/.MartinBinance/config/``` and select (uncomment) desired exchange. Don't change exchange name.
+  + Run [example/exch_client.py](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/example/exch_client.py)
+  in other terminal window
 
 ### Use Docker image
 ```console
 docker pull ghcr.io/dogstailfarmer/exchanges-wrapper:latest
 ```
 #### First run
 The structure of the working directory will be created and the necessary files will be copied:
@@ -102,35 +131,14 @@
  --mount type=bind,source=/home/ubuntu/.MartinBinance,target=/home/appuser/.MartinBinance \
  --network=host \
  --restart=always \
  --name=exchanges-wrapper \
  exchanges-wrapper
 ```
 
-### Install use PIP
-To install the library, you can just run the following command:
-```console
-pip install exchanges-wrapper
-```
-After first install run ```exchanges_wrapper/exch_srv.py```
-You can find this where pip installs packages, often it's ```/home/ubuntu/.local/lib/python3.10/site-packages```
-
-The structure of the working directory will be created and the necessary files will be copied:
-For Ubuntu it will be here: ```home/user/.MartinBinance/```
-
-For upgrade to latest versions use:
-```console
-pip install -U martin-binance
-```
-
-### Start server
-* Run ```exchanges_wrapper/exch_srv.py``` in terminal window
-* In ```example/ms_cfg.toml``` select desired exchange. Don't change exchange name.
-* Run ```example/exch_client.py``` in other terminal window
-
 ### Documentations
 * For [binance.py](https://th0rgal.gitbook.io/binance-py/) use original
 * Served methods and examples of their use are described at ```example/exch_client.py```
 * For [Protocol Buffers](https://developers.google.com/protocol-buffers/docs/overview) serializing structured data
 see ```proto/exchanges_wrapper/api.proto```
 
 ## Donate
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.0.post2 Summary:
-REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
-Author-email: Thomas Marchand
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.1b0 Summary: REST
+API and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
+email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist: grpcio-
@@ -31,59 +31,61 @@
 capabilities (inherited from binance.py) - Covers general endpoints (test
 connectivity and get exchange information's) - Covers market data endpoints -
 Covers Account endpoints (create and manage orders) - Covers user data stream
 (receive real time user updates) - Covers web socket streams (receive real time
 market updates) - Async support - Auto reconnect after exchanges API or network
 failure - Completely free and without limitations ### Added Features - Multi
 exchanges support - Adaptive algorithm to ensure maximum performance and avoid
-exceeding the rates limits - Passthrough logging ## Extra exchanges
-implementation features - Binance REST API and WSS are accepted as basic,
-connection of other exchanges wrapped their API to Binance compatible - For
-other, some data cannot be obtained by directly calling one method, it is
-generated by a synthetic or calculation method - Some exchanges have not any
-testing or "paper trading" features, therefore, application development and
-testing is possible only at real bidding. First, run applications on the
-[Binance Spot Test Network](https://testnet.binance.vision/) or Bitfinex test
-account. ## Get started ### Prepare exchange account * Create account on
-[Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10%
-discount on all trading fee * Create account on [Bitfinex](https://
-www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6% rebate fee * Create
-account on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
-?invite_code=9uaw3223) and get 10% cashback on all trading fee * Create account
-on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes worth up to
-$10,000 * For test purpose log in at [Binance Spot Test Network](https://
-testnet.binance.vision/) * Create API Key * After install and first run specify
-api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/
-exch_srv_cfg.toml``` ### Use Docker image ```console docker pull ghcr.io/
-dogstailfarmer/exchanges-wrapper:latest ``` #### First run The structure of the
-working directory will be created and the necessary files will be copied: For
-Ubuntu it will be here: ```home/user/.MartinBinance/``` ```console docker run -
--rm --entrypoint /bin/sh exchanges-wrapper -c "cat ./exchanges_wrapper/
-__init__.py" > init.py && \ docker run --rm --entrypoint /bin/sh exchanges-
-wrapper -c "cat ./exchanges_wrapper/exch_srv_cfg.toml.template" >
-exch_srv_cfg.toml.template &&\ python3 init.py && rm init.py && rm
-exch_srv_cfg.toml.template ``` #### Start server ```console docker run -itP \ -
--mount type=bind,source=/home/ubuntu/.MartinBinance,target=/home/
-appuser/.MartinBinance \ --network=host \ --restart=always \ --name=exchanges-
-wrapper \ exchanges-wrapper ``` ### Install use PIP To install the library, you
-can just run the following command: ```console pip install exchanges-wrapper
-``` After first install run ```exchanges_wrapper/exch_srv.py``` You can find
-this where pip installs packages, often it's ```/home/ubuntu/.local/lib/
-python3.10/site-packages``` The structure of the working directory will be
+exceeding the rates limits - Passthrough logging - WSS keepalive - Reuse
+session for new client sessions ## Extra exchanges implementation features -
+Binance REST API and WSS are accepted as basic, connection of other exchanges
+wrapped their API to Binance compatible - For other, some data cannot be
+obtained by directly calling one method, it is generated by a synthetic or
+calculation method - Some exchanges have not any testing or "paper trading"
+features, therefore, application development and testing is possible only at
+real bidding. First, run applications on the [Binance Spot Test Network](https:
+//testnet.binance.vision/) or (Bitfinex, OKX) test account. ## Get started ###
+Prepare exchange account * Create account on [Binance](https://
+accounts.binance.com/en/register?ref=QCS4OGWR) and get 10% discount on all
+trading fee * Create account on [Bitfinex](https://www.bitfinex.com/sign-
+up?refcode=v_4az2nCP) and get 6% rebate fee * Create account on [HUOBI](https:/
+/www.huobi.com/en-us/topic/double-reward/?invite_code=9uaw3223) and get 10%
+cashback on all trading fee * Create account on [OKX](https://www.okx.com/join/
+2607649) and get Mystery Boxes worth up to $10,000 * For test purpose log in at
+[Binance Spot Test Network](https://testnet.binance.vision/) * Create API Key *
+After install and create environment specify api_key and api_secret in ```/
+home/ubuntu/.MartinBinance/config/exch_srv_cfg.toml``` ### Install use PIP To
+install just run the following command: ```console pip install exchanges-
+wrapper ``` After first install create environment by run ```exchanges-wrapper-
+init``` in terminal window. The structure of the working directory will be
 created and the necessary files will be copied: For Ubuntu it will be here:
 ```home/user/.MartinBinance/``` For upgrade to latest versions use: ```console
-pip install -U martin-binance ``` ### Start server * Run ```exchanges_wrapper/
-exch_srv.py``` in terminal window * In ```example/ms_cfg.toml``` select desired
-exchange. Don't change exchange name. * Run ```example/exch_client.py``` in
-other terminal window ### Documentations * For [binance.py](https://
-th0rgal.gitbook.io/binance-py/) use original * Served methods and examples of
-their use are described at ```example/exch_client.py``` * For [Protocol
-Buffers](https://developers.google.com/protocol-buffers/docs/overview)
-serializing structured data see ```proto/exchanges_wrapper/api.proto``` ##
-Donate *BNB*, *BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92
-*USDT* (TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-
-wrapper
+pip install -U exchanges-wrapper ``` #### Start server * Run in terminal window
+``` exchanges-wrapper-srv ``` * Use an example to study + Copy [example/
+ms_cfg.toml](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/master/
+example/ms_cfg.toml) to ```/home/ubuntu/.MartinBinance/config/``` and select
+(uncomment) desired exchange. Don't change exchange name. + Run [example/
+exch_client.py](https://github.com/DogsTailFarmer/exchanges-wrapper/blob/
+master/example/exch_client.py) in other terminal window ### Use Docker image
+```console docker pull ghcr.io/dogstailfarmer/exchanges-wrapper:latest ``` ####
+First run The structure of the working directory will be created and the
+necessary files will be copied: For Ubuntu it will be here: ```home/
+user/.MartinBinance/``` ```console docker run --rm --entrypoint /bin/sh
+exchanges-wrapper -c "cat ./exchanges_wrapper/__init__.py" > init.py && \
+docker run --rm --entrypoint /bin/sh exchanges-wrapper -c "cat ./
+exchanges_wrapper/exch_srv_cfg.toml.template" > exch_srv_cfg.toml.template &&\
+python3 init.py && rm init.py && rm exch_srv_cfg.toml.template ``` #### Start
+server ```console docker run -itP \ --mount type=bind,source=/home/
+ubuntu/.MartinBinance,target=/home/appuser/.MartinBinance \ --network=host \ --
+restart=always \ --name=exchanges-wrapper \ exchanges-wrapper ``` ###
+Documentations * For [binance.py](https://th0rgal.gitbook.io/binance-py/) use
+original * Served methods and examples of their use are described at
+```example/exch_client.py``` * For [Protocol Buffers](https://
+developers.google.com/protocol-buffers/docs/overview) serializing structured
+data see ```proto/exchanges_wrapper/api.proto``` ## Donate *BNB*, *BUSD*,
+*USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT* (TRC20)
+TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC ## Powered by exchanges-wrapper
 [https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/
 Modified%20martingale.svg]
 [martin-binance](https://github.com/DogsTailFarmer/martin-binance) Free trading
 system for crypto exchanges SPOT markets. Adaptive customizable reverse grid
 strategy based on martingale.
```

