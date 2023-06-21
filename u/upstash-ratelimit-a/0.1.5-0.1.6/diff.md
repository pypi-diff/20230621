# Comparing `tmp/upstash_ratelimit_a-0.1.5.tar.gz` & `tmp/upstash_ratelimit_a-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit_a-0.1.5.tar", max compression
+gzip compressed data, was "upstash_ratelimit_a-0.1.6.tar", max compression
```

## Comparing `upstash_ratelimit_a-0.1.5.tar` & `upstash_ratelimit_a-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.5/LICENSE
--rw-r--r--   0        0        0    11073 2023-06-21 03:32:26.282431 upstash_ratelimit_a-0.1.5/README.md
--rw-r--r--   0        0        0      402 2023-06-21 04:12:46.364381 upstash_ratelimit_a-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.5/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    19009 2023-06-21 03:33:12.696738 upstash_ratelimit_a-0.1.5/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.5/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     2997 2023-06-21 03:20:53.439921 upstash_ratelimit_a-0.1.5/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.5/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-06-21 03:20:40.665118 upstash_ratelimit_a-0.1.5/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      392 2023-06-21 03:20:40.665308 upstash_ratelimit_a-0.1.5/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/LICENSE
+-rw-r--r--   0        0        0    11067 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/README.md
+-rw-r--r--   0        0        0      402 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0    18972 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/algorithm.py
+-rw-r--r--   0        0        0      167 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     2997 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0      392 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    11659 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.6/PKG-INFO
```

### Comparing `upstash_ratelimit_a-0.1.5/LICENSE` & `upstash_ratelimit_a-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.5/README.md` & `upstash_ratelimit_a-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 The constructor can take even more optional parameters, some of them being (types expanded):
 
 ```python
 url: str
 
 token: str
 
-rest_encoding: Union[Literal["base64"], Literal[False]] = "base64"
+rest_encoding: Literal["base64"] | Literal[False] = "base64"
 
 rest_retries: int = 1
 
 rest_retry_interval: int = 3 # In seconds.
 
 allow_deprecated: bool = False
```

### Comparing `upstash_ratelimit_a-0.1.5/upstash_ratelimit/algorithm.py` & `upstash_ratelimit_a-0.1.6/upstash_ratelimit/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import ClassVar, Literal, cast, Union
+from typing import ClassVar, Literal, cast
 from upstash_redis.asyncio import Redis
 from upstash_ratelimit.utils.time import to_milliseconds
 from upstash_ratelimit.config import SDK, PREFIX
 from upstash_ratelimit.schema.response import RateLimitResponse
 from asyncio import sleep
 from time import time_ns
 from math import floor
@@ -162,15 +162,15 @@
         """
         Determine the number of identifier's remaining requests.
         """
 
         key: str = f"{self.prefix}:{identifier}:{self.current_window}"
 
         async with self.redis:
-            current_requests: Union[str, None] = await self.redis.get(key)
+            current_requests: str | None = await self.redis.get(key)
 
         if (
             current_requests is None
         ):  # The identifier hasn't made any request in the current window.
             return self.max_number_of_requests
 
         return self.max_number_of_requests - int(current_requests)
@@ -311,19 +311,19 @@
         """
 
         current_key: str = f"{self.prefix}:{identifier}:{self.current_window}"
 
         previous_key: str = f"{self.prefix}:{identifier}:{self.previous_window}"
 
         async with self.redis:
-            stored_requests_in_current_window: Union[str, None] = await self.redis.get(
+            stored_requests_in_current_window: str | None = await self.redis.get(
                 current_key
             )
 
-            stored_requests_in_previous_window: Union[str, None] = await self.redis.get(
+            stored_requests_in_previous_window: str | None = await self.redis.get(
                 previous_key
             )
 
         requests_in_current_window: int
 
         # The identifier hasn't made any request in the current window.
         if stored_requests_in_current_window is None:
@@ -480,15 +480,15 @@
         """
         Determine the number of identifier's remaining requests.
         """
 
         key: str = f"{self.prefix}:{identifier}"
 
         async with self.redis:
-            bucket: list[Union[str, None]] = await self.redis.hmget(
+            bucket: list[str | None] = await self.redis.hmget(
                 key, "updated_at", "tokens"
             )
 
         if bucket[0] is None:  # The bucket does not exist yet.
             return self.max_number_of_tokens
 
         updated_at: float = float(bucket[0])
@@ -517,15 +517,15 @@
         """
 
         key: str = f"{self.prefix}:{identifier}"
 
         now: float = self.current_time_in_milliseconds
 
         async with self.redis:
-            updated_at: Union[str, None] = await self.redis.hget(key, "updated_at")
+            updated_at: str | None = await self.redis.hget(key, "updated_at")
 
         if updated_at is None:  # The bucket does not exist.
             return -1
 
         float_updated_at = int(float(updated_at))
 
         if now < float_updated_at + self.interval:
```

### Comparing `upstash_ratelimit_a-0.1.5/upstash_ratelimit/limiter.py` & `upstash_ratelimit_a-0.1.6/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.5/PKG-INFO` & `upstash_ratelimit_a-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit-a
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -94,15 +94,15 @@
 The constructor can take even more optional parameters, some of them being (types expanded):
 
 ```python
 url: str
 
 token: str
 
-rest_encoding: Union[Literal["base64"], Literal[False]] = "base64"
+rest_encoding: Literal["base64"] | Literal[False] = "base64"
 
 rest_retries: int = 1
 
 rest_retry_interval: int = 3 # In seconds.
 
 allow_deprecated: bool = False
```

