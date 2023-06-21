# Comparing `tmp/tastytrade-5.4.tar.gz` & `tmp/tastytrade-5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.4.tar", last modified: Wed May 31 19:22:00 2023, max compression
+gzip compressed data, was "tastytrade-5.5.tar", last modified: Wed Jun 21 15:20:51 2023, max compression
```

## Comparing `tastytrade-5.4.tar` & `tastytrade-5.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.627303 tastytrade-5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-31 19:21:46.000000 tastytrade-5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-31 19:22:00.627303 tastytrade-5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-05-31 19:21:46.000000 tastytrade-5.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:22:00.627303 tastytrade-5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 19:21:46.000000 tastytrade-5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.623303 tastytrade-5.4/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34366 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.627303 tastytrade-5.4/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-31 19:21:46.000000 tastytrade-5.4/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:22:00.623303 tastytrade-5.4/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 19:22:00.000000 tastytrade-5.4/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.173865 tastytrade-5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 15:20:41.000000 tastytrade-5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-21 15:20:51.173865 tastytrade-5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-21 15:20:41.000000 tastytrade-5.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:20:51.173865 tastytrade-5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-21 15:20:41.000000 tastytrade-5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.165865 tastytrade-5.5/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.169865 tastytrade-5.5/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22045 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.169865 tastytrade-5.5/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.4/LICENSE` & `tastytrade-5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/PKG-INFO` & `tastytrade-5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.4
+Version: 5.5
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-5.4/README.rst` & `tastytrade-5.5/README.rst`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/setup.py` & `tastytrade-5.5/setup.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/account.py` & `tastytrade-5.5/tastytrade/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,25 +94,25 @@
     day_trading_call_value: Decimal
     day_equity_call_value: Decimal
     net_liquidating_value: Decimal
     cash_available_to_withdraw: Decimal
     day_trade_excess: Decimal
     pending_cash: Decimal
     pending_cash_effect: PriceEffect
-    long_cryptocurrency_value: Decimal
-    short_cryptocurrency_value: Decimal
-    cryptocurrency_margin_requirement: Decimal
-    unsettled_cryptocurrency_fiat_amount: Decimal
-    unsettled_cryptocurrency_fiat_effect: PriceEffect
-    closed_loop_available_balance: Decimal
-    equity_offering_margin_requirement: Decimal
-    long_bond_value: Decimal
-    bond_margin_requirement: Decimal
     snapshot_date: date
     time_of_day: Optional[str] = None
+    long_cryptocurrency_value: Optional[Decimal] = None
+    short_cryptocurrency_value: Optional[Decimal] = None
+    cryptocurrency_margin_requirement: Optional[Decimal] = None
+    unsettled_cryptocurrency_fiat_amount: Optional[Decimal] = None
+    unsettled_cryptocurrency_fiat_effect: Optional[PriceEffect] = None
+    closed_loop_available_balance: Optional[Decimal] = None
+    equity_offering_margin_requirement: Optional[Decimal] = None
+    long_bond_value: Optional[Decimal] = None
+    bond_margin_requirement: Optional[Decimal] = None
 
 
 class CurrentPosition(TastytradeJsonDataclass):
     """
     Dataclass containing imformation about an individual position in a portfolio.
     """
     account_number: str
```

### Comparing `tastytrade-5.4/tastytrade/dxfeed/candle.py` & `tastytrade-5.5/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/event.py` & `tastytrade-5.5/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/greeks.py` & `tastytrade-5.5/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/profile.py` & `tastytrade-5.5/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/quote.py` & `tastytrade-5.5/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/summary.py` & `tastytrade-5.5/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.5/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/timeandsale.py` & `tastytrade-5.5/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/dxfeed/trade.py` & `tastytrade-5.5/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/instruments.py` & `tastytrade-5.5/tastytrade/instruments.py`

 * *Files 4% similar despite different names*

```diff
@@ -997,14 +997,18 @@
 
 
 def get_option_chain(session: Session, symbol: str) -> dict[date, list[Option]]:
     """
     Returns a mapping of expiration date to a list of :class:`Option` objects
     representing the options chain for the given symbol.
 
+    In the case that there are two expiries on the same day (e.g. SPXW and SPX AM
+    options), both will be returned in the same list. If you just want one expiry,
+    you'll need to filter the list yourself, or use ~:class:`NestedOptionChain` instead.
+
     :param session: the session to use for the request.
     :param symbol: the symbol to get the option chain for.
 
     :return: a dict mapping expiration date to a list of :class:`Option` objects.
     """
     symbol = symbol.replace('/', '%2F')
     response = requests.get(
@@ -1026,14 +1030,18 @@
 
 
 def get_future_option_chain(session: Session, symbol: str) -> dict[date, list[FutureOption]]:
     """
     Returns a mapping of expiration date to a list of :class:`FutureOption` objects
     representing the options chain for the given symbol.
 
+    In the case that there are two expiries on the same day (e.g. EW and ES options),
+    both will be returned in the same list. If you just want one expiry, you'll need
+    to filter the list yourself, or use ~:class:`NestedFutureOptionChain` instead.
+
     :param session: the session to use for the request.
     :param symbol: the symbol to get the option chain for.
 
     :return: a dict mapping expiration date to a list of :class:`FutureOption` objects.
     """
     symbol = symbol.replace('/', '')
     response = requests.get(
```

### Comparing `tastytrade-5.4/tastytrade/metrics.py` & `tastytrade-5.5/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/order.py` & `tastytrade-5.5/tastytrade/order.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/search.py` & `tastytrade-5.5/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/session.py` & `tastytrade-5.5/tastytrade/session.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/streamer.py` & `tastytrade-5.5/tastytrade/streamer.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,17 @@
         # see Github issue #45:
         # once the handshake completes, although setup is completed locally, remotely there
         # is still some kind of setup process that hasn't happened that takes about 8-9
         # seconds, and afterwards you're good to go. Unfortunately, there's no way to know
         # when that process concludes remotely, as there's no kind of confirmation message
         # sent. This is a hacky solution to ensure streamer setup completes.
         await self.oneshot(EventType.QUOTE, ['SPY'])
+        # clear queue if there's any lingering data
+        while not self._queue.empty():
+            self._queue.get_nowait()
 
         return self
 
     async def _next_id(self):
         async with self._lock:
             self._counter += 1
         return self._counter
```

### Comparing `tastytrade-5.4/tastytrade/utils.py` & `tastytrade-5.5/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade/watchlists.py` & `tastytrade-5.5/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.4/tastytrade.egg-info/PKG-INFO` & `tastytrade-5.5/tastytrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.4
+Version: 5.5
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-5.4/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.5/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

