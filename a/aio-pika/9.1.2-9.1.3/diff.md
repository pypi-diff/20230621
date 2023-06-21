# Comparing `tmp/aio_pika-9.1.2.tar.gz` & `tmp/aio_pika-9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.1.2.tar", max compression
+gzip compressed data, was "aio_pika-9.1.3.tar", max compression
```

## Comparing `aio_pika-9.1.2.tar` & `aio_pika-9.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.1.2/README.rst
--rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.2/aio_pika/__init__.py
--rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.2/aio_pika/abc.py
--rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.2/aio_pika/channel.py
--rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.2/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.2/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.2/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.2/aio_pika/log.py
--rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.2/aio_pika/message.py
--rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.2/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.2/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.2/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14343 2023-06-01 15:55:44.129787 aio_pika-9.1.2/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.2/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.2/aio_pika/py.typed
--rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.2/aio_pika/queue.py
--rw-r--r--   0        0        0     8219 2023-06-01 15:55:44.133275 aio_pika-9.1.2/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.2/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.2/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4883 2023-06-01 15:55:44.136895 aio_pika-9.1.2/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.2/aio_pika/tools.py
--rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.2/aio_pika/transaction.py
--rw-r--r--   0        0        0     3269 2023-06-01 16:15:08.448713 aio_pika-9.1.2/pyproject.toml
--rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.1.3/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.3/aio_pika/__init__.py
+-rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.3/aio_pika/abc.py
+-rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.3/aio_pika/channel.py
+-rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.3/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.3/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.3/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.3/aio_pika/log.py
+-rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.3/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.3/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.3/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.3/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.1.3/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.3/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.3/aio_pika/py.typed
+-rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.3/aio_pika/queue.py
+-rw-r--r--   0        0        0     8219 2023-06-01 15:55:44.133275 aio_pika-9.1.3/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.3/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.3/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4883 2023-06-01 15:55:44.136895 aio_pika-9.1.3/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.3/aio_pika/tools.py
+-rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.3/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3269 2023-06-21 09:55:41.970816 aio_pika-9.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.1.3/PKG-INFO
```

### Comparing `aio_pika-9.1.2/README.rst` & `aio_pika-9.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/__init__.py` & `aio_pika-9.1.3/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/abc.py` & `aio_pika-9.1.3/aio_pika/abc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/channel.py` & `aio_pika-9.1.3/aio_pika/channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/connection.py` & `aio_pika-9.1.3/aio_pika/connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/exceptions.py` & `aio_pika-9.1.3/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/exchange.py` & `aio_pika-9.1.3/aio_pika/exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/message.py` & `aio_pika-9.1.3/aio_pika/message.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/patterns/base.py` & `aio_pika-9.1.3/aio_pika/patterns/base.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/patterns/master.py` & `aio_pika-9.1.3/aio_pika/patterns/master.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/patterns/rpc.py` & `aio_pika-9.1.3/aio_pika/patterns/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,20 +270,30 @@
                 'RPC message without "reply_to" header %r call result '
                 "will be lost",
                 message,
             )
             await message.ack()
             return
 
-        result_message = await self.serialize_message(
-            payload=result,
-            message_type=message_type,
-            correlation_id=message.correlation_id,
-            delivery_mode=message.delivery_mode,
-        )
+        try:
+            result_message = await self.serialize_message(
+                payload=result,
+                message_type=message_type,
+                correlation_id=message.correlation_id,
+                delivery_mode=message.delivery_mode,
+            )
+        except asyncio.CancelledError:
+            raise
+        except Exception as e:
+            result_message = await self.serialize_message(
+                payload=e,
+                message_type=RPCMessageType.ERROR,
+                correlation_id=message.correlation_id,
+                delivery_mode=message.delivery_mode,
+            )
 
         try:
             await self.channel.default_exchange.publish(
                 result_message, message.reply_to, mandatory=False,
             )
         except Exception:
             log.exception("Failed to send reply %r", result_message)
```

### Comparing `aio_pika-9.1.2/aio_pika/pool.py` & `aio_pika-9.1.3/aio_pika/pool.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/queue.py` & `aio_pika-9.1.3/aio_pika/queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/robust_channel.py` & `aio_pika-9.1.3/aio_pika/robust_channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/robust_connection.py` & `aio_pika-9.1.3/aio_pika/robust_connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/robust_exchange.py` & `aio_pika-9.1.3/aio_pika/robust_exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/robust_queue.py` & `aio_pika-9.1.3/aio_pika/robust_queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/tools.py` & `aio_pika-9.1.3/aio_pika/tools.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/aio_pika/transaction.py` & `aio_pika-9.1.3/aio_pika/transaction.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.2/pyproject.toml` & `aio_pika-9.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.1.2"
+version = "9.1.3"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
```

### Comparing `aio_pika-9.1.2/PKG-INFO` & `aio_pika-9.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pika
-Version: 9.1.2
+Version: 9.1.3
 Summary: Wrapper around the aiormq for asyncio and humans
 Home-page: https://github.com/mosquito/aio-pika
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,aiormq
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
```

