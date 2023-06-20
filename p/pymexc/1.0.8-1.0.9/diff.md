# Comparing `tmp/pymexc-1.0.8.tar.gz` & `tmp/pymexc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymexc-1.0.8.tar", last modified: Tue Jun 20 19:37:43 2023, max compression
+gzip compressed data, was "dist\pymexc-1.0.9.tar", last modified: Tue Jun 20 23:42:23 2023, max compression
```

## Comparing `pymexc-1.0.8.tar` & `pymexc-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 19:37:43.415840 pymexc-1.0.8/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3321 2023-06-20 19:37:43.415840 pymexc-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 19:37:43.391836 pymexc-1.0.8/pymexc/
--rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.8/pymexc/__init__.py
--rw-rw-rw-   0        0        0     6190 2023-06-20 19:33:14.000000 pymexc-1.0.8/pymexc/base.py
--rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.8/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.8/pymexc/futures.py
--rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.8/pymexc/spot.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:37:43.414841 pymexc-1.0.8/pymexc.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 19:37:43.416841 pymexc-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-06-20 19:33:41.000000 pymexc-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:42:23.960814 pymexc-1.0.9/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3321 2023-06-20 23:42:23.960814 pymexc-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 23:42:23.934809 pymexc-1.0.9/pymexc/
+-rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.9/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     6243 2023-06-20 23:33:20.000000 pymexc-1.0.9/pymexc/base.py
+-rw-rw-rw-   0        0        0    17642 2023-06-20 23:15:54.000000 pymexc-1.0.9/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.9/pymexc/futures.py
+-rw-rw-rw-   0        0        0    68233 2023-06-20 23:22:29.000000 pymexc-1.0.9/pymexc/spot.py
+drwxrwxrwx   0        0        0        0 2023-06-20 23:42:23.959814 pymexc-1.0.9/pymexc.egg-info/
+-rw-rw-rw-   0        0        0     3321 2023-06-20 23:42:23.000000 pymexc-1.0.9/pymexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-20 23:42:23.000000 pymexc-1.0.9/pymexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 23:42:23.000000 pymexc-1.0.9/pymexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 23:42:23.000000 pymexc-1.0.9/pymexc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-20 23:42:23.000000 pymexc-1.0.9/pymexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 23:42:23.000000 pymexc-1.0.9/pymexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 23:42:23.961815 pymexc-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-06-20 23:38:08.000000 pymexc-1.0.9/setup.py
```

### Comparing `pymexc-1.0.8/LICENSE` & `pymexc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.8/PKG-INFO` & `pymexc-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.8.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.9.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.8/README.md` & `pymexc-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.8/pymexc/__init__.py` & `pymexc-1.0.9/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.8/pymexc/base.py` & `pymexc-1.0.9/pymexc/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,20 +76,23 @@
             kwargs['params'] = {k: v for k, v in kwargs['params'].items() if v is not None}
         else:
             kwargs['params'] = {}
 
         if self.api_key and self.api_secret:
             # add signature
             timestamp = str(int(time.time() * 1000))
-        kwargs['params']['recvWindow'] = self.recvWindow
-        kwargs['params']['timestamp']  = timestamp
+            kwargs['params']['recvWindow'] = self.recvWindow
+            kwargs['params']['timestamp'] = timestamp
+
         kwargs['params'] = {k: v for k, v in sorted(kwargs['params'].items())}
-        
         params = urlencode(kwargs.pop('params'), doseq=True).replace('+', '%20')
-        params += "&signature=" + self.sign(params)
+
+        if self.api_key and self.api_secret:
+            params += "&signature=" + self.sign(params)
+
 
         response = self.session.request(method, f"{self.base_url}{router}", params = params, *args, **kwargs)
 
         if not response.ok:
             raise MexcAPIError(f'(code={response.json()["code"]}): {response.json()["msg"]}')
 
         return response.json()
```

### Comparing `pymexc-1.0.8/pymexc/base_websocket.py` & `pymexc-1.0.9/pymexc/base_websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
         self.active_connections = []
         self.kwargs = kwargs
 
     def is_connected(self):
         return self._are_connections_connected(self.active_connections)
 
-    def _ws_subscribe(self, topic, callback, params: dict = {}):
+    def _ws_subscribe(self, topic, callback, params: list = []):
         if not self.ws:
             self.ws = _FuturesWebSocketManager(
                 self.ws_name, **self.kwargs)
             self.ws._connect(self.endpoint)
             self.active_connections.append(self.ws)
         self.ws.subscribe(topic, callback, params)
 
@@ -400,19 +400,20 @@
             kwargs.get("callback_function") else self._handle_incoming_message
         super().__init__(callback_function, ws_name, **kwargs)
 
         self.private_topics = ["account", "deals", "orders"]
 
         self.last_subsctiption = None
 
-    def subscribe(self, topic, callback, params: dict = {}):
+    def subscribe(self, topic: str, callback, params_list: list):
         subscription_args = {
             "method": "SUBSCRIPTION",
             "params": [
                 '@'.join([f"spot@{topic}.v3.api"] + list(map(str, params.values())))
+                for params in params_list
             ]
         }
         self._check_callback_directory(subscription_args)
 
         while not self.is_connected():
             # Wait until the connection is open before subscribing.
             time.sleep(0.1)
@@ -426,23 +427,14 @@
     def _initialise_local_data(self, topic):
         # Create self.data
         try:
             self.data[topic]
         except KeyError:
             self.data[topic] = []
 
-    #def _process_auth_message(self, message):
-    #    # If we get successful futures auth, notify user
-    #    if message.get("data") == "success":
-    #        logger.debug(f"Authorization for {self.ws_name} successful.")
-    #        self.auth = True
-    #    # If we get unsuccessful auth, notify user.
-    #    elif message.get("data") != "success": 
-    #        logger.debug(f"Authorization for {self.ws_name} failed. Please "
-    #                     f"check your API keys and restart.")
 
     def _process_subscription_message(self, message):
         sub = message["msg"].replace("spot@", "").split(".v3.api")[0]
 
         # If we get successful futures subscription, notify user
         if message.get("id") == 0 and message.get("code") == 0:
             logger.debug(f"Subscription to {sub} successful.")
```

### Comparing `pymexc-1.0.8/pymexc/futures.py` & `pymexc-1.0.9/pymexc/futures.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.8/pymexc/spot.py` & `pymexc-1.0.9/pymexc/spot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1692,17 +1692,17 @@
         :param callback: the callback function
         :type callback: Callable[..., None]
         :param symbol: the name of the contract
         :type symbol: str
 
         :return: None
         """
-        params = dict(
+        params = [dict(
             symbol = symbol
-        )
+        )]
         topic = "public.deals"
         self._ws_subscribe(topic, callback, params)
 
     def kline_stream(self, 
                      callback: Callable[..., None],
                      symbol:   str,
                      interval: int):
@@ -1717,18 +1717,18 @@
         :param symbol: the name of the contract
         :type symbol: str
         :param interval: the interval of the kline
         :type interval: int
 
         :return: None
         """
-        params = dict(
+        params = [dict(
             symbol   = symbol,
             interval = interval
-        )
+        )]
         topic = "public.kline"
         self._ws_subscribe(topic, callback, params)
 
     def increase_depth_stream(self, 
                      callback: Callable[..., None],
                      symbol:   str):
         """
@@ -1740,17 +1740,17 @@
         :param callback: the callback function
         :type callback: Callable[..., None]
         :param symbol: the name of the contract
         :type symbol: str
 
         :return: None
         """
-        params = dict(
+        params = [dict(
             symbol = symbol
-        )
+        )]
         topic = "public.increase.depth"
         self._ws_subscribe(topic, callback, params)
 
     def limit_depth_stream(self, 
                      callback: Callable[..., None],
                      symbol:   str,
                      level:    int):
@@ -1765,40 +1765,40 @@
         :param symbol: the name of the contract
         :type symbol: str
         :param level: the level of the depth. Valid are 5, 10, or 20.
         :type level: int
 
         :return: None
         """
-        params = dict(
+        params = [dict(
             symbol = symbol,
             level  = level
-        )
+        )]
         topic = "public.limit.depth"
         self._ws_subscribe(topic, callback, params)
 
-    def limit_depth_stream(self, 
+    def book_ticker(self, 
                      callback: Callable[..., None],
                      symbol:   str):
         """
         ### Individual Symbol Book Ticker Streams
         Pushes any update to the best bid or ask's price or quantity in real-time for a specified symbol.
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#partial-book-depth-streams
 
         :param callback: the callback function
         :type callback: Callable[..., None]
-        :param symbol: the name of the contract
-        :type symbol: str
+        :param symbols: the names of the contracts
+        :type symbols: str
 
         :return: None
         """
-        params = dict(
+        params = [dict(
             symbol = symbol
-        )
+        )]
         topic = "public.bookTicker"
         self._ws_subscribe(topic, callback, params)
 
     # <=================================================================>
     #
     #                                Private
     #
@@ -1812,41 +1812,41 @@
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#websocket-user-data-streams
 
         :param callback: the callback function
         :type callback: Callable[..., None]
 
         :return: None
         """
-        params = {}
+        params = [{}]
         topic = "private.account"
         self._ws_subscribe(topic, callback, params)
 
     def account_deals(self, callback: Callable[..., None]):
         """
         ### Spot Account Deals
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#spot-account-deals
 
         :param callback: the callback function
         :type callback: Callable[..., None]
 
         :return: None
         """
-        params = {}
+        params = [{}]
         topic = "private.deals"
         self._ws_subscribe(topic, callback, params)
     
     def account_orders(self, callback: Callable[..., None]):
         """
         ### Spot Account Orders
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#spot-account-orders
 
         :param callback: the callback function
         :type callback: Callable[..., None]
 
         :return: None
         """
-        params = {}
+        params = [{}]
         topic = "private.orders"
         self._ws_subscribe(topic, callback, params)
```

### Comparing `pymexc-1.0.8/pymexc.egg-info/PKG-INFO` & `pymexc-1.0.9/pymexc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.8.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.9.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.8/setup.py` & `pymexc-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.0.8'
+version = '1.0.9'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pymexc",
     version=version,
```

