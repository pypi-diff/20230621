# Comparing `tmp/upstash_ratelimit_a-0.1.3.tar.gz` & `tmp/upstash_ratelimit_a-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit_a-0.1.3.tar", max compression
+gzip compressed data, was "upstash_ratelimit_a-0.1.4.tar", max compression
```

## Comparing `upstash_ratelimit_a-0.1.3.tar` & `upstash_ratelimit_a-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.3/LICENSE
--rw-r--r--   0        0        0     9798 2023-05-24 13:49:29.502103 upstash_ratelimit_a-0.1.3/README.md
--rw-r--r--   0        0        0      402 2023-06-19 04:13:19.287224 upstash_ratelimit_a-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.3/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    12115 2023-06-19 03:20:03.856569 upstash_ratelimit_a-0.1.3/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.3/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3066 2023-06-19 03:11:10.807977 upstash_ratelimit_a-0.1.3/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.3/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      474 2023-05-24 13:49:29.504424 upstash_ratelimit_a-0.1.3/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      392 2023-06-19 04:13:07.829439 upstash_ratelimit_a-0.1.3/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    10390 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.4/LICENSE
+-rw-r--r--   0        0        0    11073 2023-06-21 03:32:26.282431 upstash_ratelimit_a-0.1.4/README.md
+-rw-r--r--   0        0        0      402 2023-06-21 03:34:34.876458 upstash_ratelimit_a-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.4/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0    19009 2023-06-21 03:33:12.696738 upstash_ratelimit_a-0.1.4/upstash_ratelimit/algorithm.py
+-rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.4/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     2997 2023-06-21 03:20:53.439921 upstash_ratelimit_a-0.1.4/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.4/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-06-21 03:20:40.665118 upstash_ratelimit_a-0.1.4/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0      392 2023-06-21 03:20:40.665308 upstash_ratelimit_a-0.1.4/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.4/PKG-INFO
```

### Comparing `upstash_ratelimit_a-0.1.3/LICENSE` & `upstash_ratelimit_a-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.3/README.md` & `upstash_ratelimit_a-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   - [Install](#install)
     - [PyPi](#pypi)
   - [Setup database client](#setup-database-client)
   - [Usage](#usage)
   - [Telemetry](#telemetry)
   - [Block until ready](#block-until-ready)
   - [Timeout](#timeout)
+  - [Rate-limiting outbound requests](#rate-limiting-outbound-requests)
 - [Ratelimiting algorithms](#ratelimiting-algorithms)
   - [Fixed Window](#fixed-window)
     - [Pros:](#pros)
     - [Cons:](#cons)
     - [Usage:](#usage)
   - [Sliding Window](#sliding-window)
     - [Pros:](#pros-1)
@@ -76,15 +77,15 @@
 The constructor can take even more optional parameters, some of them being (types expanded):
 
 ```python
 url: str
 
 token: str
 
-rest_encoding: Literal["base64"] | Literal[False] = "base64"
+rest_encoding: Union[Literal["base64"], Literal[False]] = "base64"
 
 rest_retries: int = 1
 
 rest_retry_interval: int = 3 # In seconds.
 
 allow_deprecated: bool = False
 
@@ -114,20 +115,22 @@
 
 """
 Use a constant to limit all the requests together.
 For enforcing individual limits, use some kind of identifying variable (IP address, API key, etc.).
 """
 identifier: str = "constant"
 
-request_result: RateLimitResponse = await fixed_window.limit(identifier)
 
-if not request_result["is_allowed"]:
-    print(f"{identifier} is rate-limited!")
-else:
-    print("Request passed!")
+async def main() -> str:
+    request_result: RateLimitResponse = await fixed_window.limit(identifier)
+
+    if not request_result["is_allowed"]:
+        return f"{identifier} is rate-limited!"
+    else:
+        return "Request passed!"
 ```
 
 You can also pass a `prefix` to the `RateLimit` constructor to distinguish between the keys used for rate limiting and others.
 It defaults to `"ratelimit"`.
 
 The `limit` method also returns some metadata that might be useful :
 
@@ -178,20 +181,22 @@
     max_number_of_requests=1,
     window=3,
     unit="s"
 )
 
 identifier: str = "constant"
 
-request_result: RateLimitResponse = await fixed_window.block_until_ready(identifier, timeout=2000)
 
-if not request_result["is_allowed"]:
-    print(f"The {identifier}'s request cannot be processed, even after 2 seconds.")
-else:
-    print("Request passed!")
+async def main() -> str:
+    request_result: RateLimitResponse = await fixed_window.block_until_ready(identifier, timeout=2000)
+
+    if not request_result["is_allowed"]:
+        return f"The {identifier}'s request cannot be processed, even after 2 seconds."
+    else:
+        return "Request passed!"
 ```
 
 
 ## Timeout
 If you worry that network issues can cause your application to reject requests, you can use python's `wait_for` to 
 allow the requests which exceed a given timeout to pass regardless of what the current limit is.
 
@@ -224,19 +229,50 @@
         return "Request passed!"
 
     except TimeoutError:
         return "Request passed"
 ```
 
 
+## Rate-limiting outbound requests
+It's also possible to limit the number of requests you're making to an external API.
+
+```python
+from upstash_ratelimit.limiter import RateLimit
+from upstash_ratelimit.schema.response import RateLimitResponse
+
+from upstash_redis.client import Redis
+
+rate_limit = RateLimit(Redis.from_env())
+
+fixed_window = rate_limit.fixed_window(
+    max_number_of_requests=1,
+    window=3,
+    unit="s"
+)
+
+identifier: str = "constant"  # Or, use an identifier to limit your requests to a certain endpoint.
+
+
+async def main() -> str:
+    request_result: RateLimitResponse = await fixed_window.limit(identifier)
+
+    if not request_result["is_allowed"]:
+        return f"{identifier} is rate-limited!"
+    else:
+        # Call the API
+        # ...
+        return "Request passed!"
+```
+
+
 # Ratelimiting algorithms
 
 ## Fixed Window
-This algorithm divides time into windows of fixed duration. The first request after a window has elapsed triggers the creation of a new one. 
-For each subsequent request, the algorithm checks whether the number of requests has exceeded the limit.
+The time is divided into windows of fixed length and each window has a maximum number of allowed requests.
 
 ### Pros
 - Very cheap in terms of data size and computation
 - Newer requests are not starved due to a high burst in the past
 
 ### Cons
 - Can cause high bursts at the window boundaries to leak through
@@ -330,23 +366,30 @@
 
 They are also grouped in the [RateLimit](upstash_ratelimit/limiter.py) class for ease of use.
 
 
 ## Running tests
 All tests live in the [test](./tests) folder.
 
-Only the limiting logic of 100%-accuracy algorithms and other utility functions are unit-tested.
+Only the logic of 100%-accuracy algorithms and other utility functions are unit-tested.
 
 To run all the tests, make sure you are in the `tests` folder and have the poetry virtual environment activated with all 
 the necessary dependencies. Set the `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` environment variables and run:
 
 ```bash
-poetry run pytest
+poetry run pytest --import-mode importlib
 ```
 
+The reason we need to use the `importlib` mode is because there are multiple test files with the same name. See the 
+[pytest docs](https://docs.pytest.org/en/stable/explanation/pythonpath.html#import-modes) for more info.
+
+**Warning**: The current evaluation speed of the tests does not take the HTTP requests duration into account. 
+Because of that, if a request takes more than 2 seconds to complete, a test might fail.
+
+
 ## Releasing
 To create a new release, first use Poetry's [version](https://python-poetry.org/docs/cli/#version) command.
 
 You will then need to connect your PyPi API token to Poetry. 
 A simple tutorial showcasing how to do it was posted by Tony Tran
 [on DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
```

### Comparing `upstash_ratelimit_a-0.1.3/upstash_ratelimit/algorithm.py` & `upstash_ratelimit_a-0.1.4/upstash_ratelimit/algorithm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
-from typing import ClassVar, Literal
+from typing import ClassVar, Literal, cast, Union
 from upstash_redis.asyncio import Redis
 from upstash_ratelimit.utils.time import to_milliseconds
 from upstash_ratelimit.config import SDK, PREFIX
 from upstash_ratelimit.schema.response import RateLimitResponse
-from time import time_ns, sleep
+from asyncio import sleep
+from time import time_ns
 from math import floor
 
 
 class RateLimitAlgorithm(ABC):
     @abstractmethod
     def __init__(self, redis: Redis, prefix: str = PREFIX):
         """
@@ -16,33 +17,35 @@
         :param prefix: a prefix to distinguish between the keys used for rate limiting and others
         """
 
         self.redis = redis
         self.prefix = prefix
 
         if redis.allow_telemetry:
-            self.redis.telemetry_data = {
-                "sdk": SDK
-            }
+            self.redis.telemetry_data = {"sdk": SDK}
 
     @property
     @abstractmethod
     def script(self) -> str:
         """
         Setting this as read-only property enforces the subclasses to implement it without using a setter.
         However, replacing it with a class attribute has the same effect.
         """
 
+    # Limiting methods
     @abstractmethod
     async def limit(self, identifier: str) -> RateLimitResponse:
         """
-        Determine whether the identifier's request should pass and return additional metadata.
+        Increment identifier's request counter, determine whether it should pass
+        and return additional metadata.
         """
 
-    async def block_until_ready(self, identifier: str, timeout: int) -> RateLimitResponse:
+    async def block_until_ready(
+        self, identifier: str, timeout: int
+    ) -> RateLimitResponse:
         """
         If a request is denied, wait for it to pass in the given timeout in milliseconds
         and if it doesn't, return the last response.
         """
 
         if timeout <= 0:
             raise Exception("Timeout must be greater than 0.")
@@ -52,28 +55,51 @@
         if response["is_allowed"]:
             return response
 
         deadline: int = time_ns() + timeout * 1000000  # Transform in nanoseconds.
 
         while response["is_allowed"] is False and time_ns() < deadline:
             # Transform the reset time from milliseconds to seconds and the sleep time in seconds.
-            sleep((min(response["reset"] * 1000000, deadline) - time_ns()) / 1000000000)
+            await sleep(
+                (min(response["reset"] * 1000000, deadline) - time_ns()) / 1000000000
+            )
 
             response = await self.limit(identifier)
 
         return response
 
+    # Metadata methods
+    @abstractmethod
+    async def remaining(self, identifier: str) -> int:
+        """
+        Determine the number of identifier's remaining requests.
+        """
+
+    @abstractmethod
+    async def reset(self, identifier: str) -> int:
+        """
+        Determine the unix time in milliseconds when the next window begins.
+
+        If the identifier is not rate-limited, the returned value will be -1.
+        """
+
+    # Helpers & utils.
+    @property
+    def current_time_in_milliseconds(self) -> float:
+        return time_ns() / 1000000
+
 
 class FixedWindow(RateLimitAlgorithm):
     """
-    The first request after a window has elapsed triggers the creation of a new one with the specified duration.
-    For each subsequent request, the algorithm checks whether the number of requests has exceeded the limit.
+    The time is divided into windows of fixed length and each window has a maximum number of allowed requests.
     """
 
-    script: ClassVar[str] = """
+    script: ClassVar[
+        str
+    ] = """
     -- "key" will store the number of requests made within the window and will expire once the window elapsed.
     local key     = KEYS[1]
     local window  = ARGV[1]
 
     local current_requests = redis.call("INCR", key)
     if current_requests == 1 then
         -- Set the expiry time to the window duration once the first request has been made.
@@ -101,58 +127,104 @@
         """
 
         super().__init__(redis, prefix)
 
         self.max_number_of_requests = max_number_of_requests
         self.window = window if unit == "ms" else to_milliseconds(window, unit)
 
+    @property
+    def current_window(self) -> int:
+        return floor(self.current_time_in_milliseconds / self.window)
+
     async def limit(self, identifier: str) -> RateLimitResponse:
         """
-        Determine whether the identifier's request should pass and return additional metadata.
+        Increment identifier's request counter, determine whether it should pass
+        and return additional metadata.
         """
 
-        key: str = f'{self.prefix}:{identifier}'
+        key: str = f"{self.prefix}:{identifier}:{self.current_window}"
 
         async with self.redis:
-            current_requests: int = await self.redis.eval(
-                script=FixedWindow.script,
-                keys=[key],
-                args=[self.window]
+            current_requests: int
+
+            current_requests = await self.redis.eval(
+                script=FixedWindow.script, keys=[key], args=[self.window]
             )
 
         return {
             "is_allowed": current_requests <= self.max_number_of_requests,
             "limit": self.max_number_of_requests,
             "remaining": self.max_number_of_requests - current_requests,
-            "reset": floor((time_ns() / 1000000) / self.window) * self.window + self.window,
+            "reset": floor((time_ns() / 1000000) / self.window) * self.window
+            + self.window,
         }
 
+    async def remaining(self, identifier: str) -> int:
+        """
+        Determine the number of identifier's remaining requests.
+        """
+
+        key: str = f"{self.prefix}:{identifier}:{self.current_window}"
+
+        async with self.redis:
+            current_requests: Union[str, None] = await self.redis.get(key)
+
+        if (
+            current_requests is None
+        ):  # The identifier hasn't made any request in the current window.
+            return self.max_number_of_requests
+
+        return self.max_number_of_requests - int(current_requests)
+
+    async def reset(self, identifier: str) -> int:
+        """
+        Determine the unix time in milliseconds when the next window begins.
+
+        If the identifier is not rate-limited, the returned value will be -1.
+        """
+
+        key: str = f"{self.prefix}:{identifier}:{self.current_window}"
+
+        async with self.redis:
+            if (
+                await self.redis.exists(key) != 1
+            ):  # The identifier hasn't made any request in the current window.
+                return -1
+
+        return floor((time_ns() / 1000000) / self.window) * self.window + self.window
+
 
 class SlidingWindow(RateLimitAlgorithm):
     """
     Combined approach of sliding logs and fixed window with lower storage
     costs than sliding logs and improved boundary behavior by calculating a
     weighted score between two windows.
     """
 
-    script: ClassVar[str] = """
+    script: ClassVar[
+        str
+    ] = """
       local current_key             = KEYS[1]                      -- identifier including prefixes
       local previous_key            = KEYS[2]                      -- key of the previous bucket
       local max_number_of_requests  = tonumber(ARGV[1])            -- max number of requests per window
-      local now                     = ARGV[2]                      -- current timestamp in milliseconds
-      local window                  = ARGV[3]                      -- interval in milliseconds
+      local now                     = tonumber(ARGV[2])            -- current timestamp in milliseconds
+      local window                  = tonumber(ARGV[3])            -- interval in milliseconds
 
       local requests_in_current_window = redis.call("GET", current_key)
       if requests_in_current_window == false then
         requests_in_current_window = -1
+      else
+        requests_in_current_window = tonumber(requests_in_current_window)
       end
 
       local requests_in_previous_window = redis.call("GET", previous_key)
       if requests_in_previous_window == false then
         requests_in_previous_window = 0
+      else
+        requests_in_previous_window = tonumber(requests_in_previous_window)
       end
       
       local percentage_in_current_window = ( now % window) / window
       
       local estimated = requests_in_previous_window * ( 1 - percentage_in_current_window ) + requests_in_current_window
       if estimated >= max_number_of_requests then
         return -1
@@ -184,88 +256,167 @@
         """
 
         super().__init__(redis, prefix)
 
         self.max_number_of_requests = max_number_of_requests
         self.window = window if unit == "ms" else to_milliseconds(window, unit)
 
+    """
+    Divide the current time by the window duration and round down 
+    to get possible sliding-after-window values for the intervals.
+    """
+
+    @property
+    def current_window(self) -> int:
+        return floor(self.current_time_in_milliseconds / self.window)
+
+    @property
+    def previous_window(self) -> int:
+        return self.current_window - self.window
+
     async def limit(self, identifier: str) -> RateLimitResponse:
         """
-        Determine whether the identifier's request should pass and return additional metadata.
+        Increment identifier's request counter, determine whether it should pass
+        and return additional metadata.
 
         Although we return the unix time when the next window begins (via "reset"), the limit is still enforced
         between the two intervals.
         """
 
-        now: float = time_ns() / 1000000  # Convert to milliseconds.
+        current_key: str = f"{self.prefix}:{identifier}:{self.current_window}"
 
-        """
-        Divide the current time by the window duration and round down 
-        to get possible sliding-after-window values for the intervals.
-        """
-        current_window: int = floor(now / self.window)
-
-        previous_window: int = current_window - self.window
-
-        current_key: str = f'{self.prefix}:{identifier}:{current_window}'
-
-        previous_key: str = f'{self.prefix}:{identifier}:{previous_window}'
+        previous_key: str = f"{self.prefix}:{identifier}:{self.previous_window}"
 
         async with self.redis:
             remaining_requests: int = await self.redis.eval(
                 script=SlidingWindow.script,
                 keys=[current_key, previous_key],
-                args=[self.max_number_of_requests, now, self.window]
+                args=[
+                    self.max_number_of_requests,
+                    self.current_time_in_milliseconds,
+                    self.window,
+                ],
             )
 
         return {
             "is_allowed": remaining_requests >= 0,
             "limit": self.max_number_of_requests,
             "remaining": remaining_requests,
-            "reset": floor((time_ns() / 1000000) / self.window) * self.window + self.window,
+            "reset": floor((time_ns() / 1000000) / self.window) * self.window
+            + self.window,
         }
 
+    async def remaining(self, identifier: str) -> int:
+        """
+        Determine the number of identifier's remaining requests.
+        """
+
+        current_key: str = f"{self.prefix}:{identifier}:{self.current_window}"
+
+        previous_key: str = f"{self.prefix}:{identifier}:{self.previous_window}"
+
+        async with self.redis:
+            stored_requests_in_current_window: Union[str, None] = await self.redis.get(
+                current_key
+            )
+
+            stored_requests_in_previous_window: Union[str, None] = await self.redis.get(
+                previous_key
+            )
+
+        requests_in_current_window: int
+
+        # The identifier hasn't made any request in the current window.
+        if stored_requests_in_current_window is None:
+            requests_in_current_window = 0
+        else:
+            requests_in_current_window = int(stored_requests_in_current_window)
+
+        requests_in_previous_window: int
+
+        if stored_requests_in_previous_window is None:
+            requests_in_previous_window = 0
+        else:
+            requests_in_previous_window = int(stored_requests_in_previous_window)
+
+        percentage_in_current_window = (
+            self.current_time_in_milliseconds % self.window
+        ) / self.window
+
+        estimated = (
+            requests_in_previous_window * (1 - percentage_in_current_window)
+            + requests_in_current_window
+        )
+
+        if estimated >= self.max_number_of_requests:  # The limit has been exceeded.
+            return 0
+
+        return self.max_number_of_requests - requests_in_current_window
+
+    async def reset(self, identifier: str) -> int:
+        """
+        Determine the unix time in milliseconds when the next window begins.
+
+        If the identifier is not rate-limited, the returned value will be -1.
+        """
+
+        current_key: str = f"{self.prefix}:{identifier}:{self.current_window}"
+
+        previous_key: str = f"{self.prefix}:{identifier}:{self.previous_window}"
+
+        async with self.redis:
+            # The identifier hasn't made any requests in either the previous or the current window.
+            if await self.redis.exists(previous_key, current_key) == 0:
+                return -1
+
+        return floor((time_ns() / 1000000) / self.window) * self.window + self.window
+
 
 class TokenBucket(RateLimitAlgorithm):
     """
     A bucket is filled with "max_number_of_tokens" that refill at "refill_rate" per "interval".
     Each request tries to consume one token and if the bucket is empty, the request is rejected.
     """
 
-    script: ClassVar[str] = """
+    script: ClassVar[
+        str
+    ] = """
     local key                       = KEYS[1]               -- identifier including prefixes
     local max_number_of_tokens      = tonumber(ARGV[1])     -- max number of tokens
     local interval                  = tonumber(ARGV[2])     -- size of the window in milliseconds
     local refill_rate               = tonumber(ARGV[3])     -- how many tokens are refilled after each interval
     local now                       = tonumber(ARGV[4])     -- current timestamp in milliseconds
     local remaining                 = 0
 
     local bucket = redis.call("HMGET", key, "updated_at", "tokens")
 
-    if bucket[1] == false then
-      -- The bucket does not exist yet, create it and set its ttl to "interval".
+    if bucket[1] == false then -- The bucket does not exist
       remaining = max_number_of_tokens - 1
 
       redis.call("HMSET", key, "updated_at", now, "tokens", remaining)
 
       return {remaining, now + interval}
     end
 
     local updated_at = tonumber(bucket[1])
     local tokens = tonumber(bucket[2])
 
     if now >= updated_at + interval then
+      local number_of_refills = math.floor((now - updated_at)/interval)
+    
       if tokens <= 0 then -- No more tokens were left before the refill.
-        remaining = math.min(max_number_of_tokens, refill_rate) - 1
+        remaining = math.min(max_number_of_tokens, number_of_refills * refill_rate) - 1
       else
-        remaining = math.min(max_number_of_tokens, tokens + refill_rate) - 1
+        remaining = math.min(max_number_of_tokens, tokens + number_of_refills * refill_rate) - 1
       end
+      
+      local last_refill = updated_at + number_of_refills * interval
 
-      redis.call("HMSET", key, "updated_at", now, "tokens", remaining)
-      return {remaining, now + interval}
+      redis.call("HMSET", key, "updated_at", last_refill, "tokens", remaining)
+      return {remaining, last_refill + interval}
     end
     
     remaining = tokens - 1
     redis.call("HSET", key, "tokens", remaining)
 
     return {remaining, updated_at + interval}
     """
@@ -293,27 +444,95 @@
 
         self.max_number_of_tokens = max_number_of_tokens
         self.refill_rate = refill_rate
         self.interval = interval if unit == "ms" else to_milliseconds(interval, unit)
 
     async def limit(self, identifier: str) -> RateLimitResponse:
         """
-        Determine whether the identifier's request should pass and return additional metadata.
+        Increment identifier's request counter, determine whether it should pass
+        and return additional metadata.
         """
 
-        now: float = time_ns() / 1000000
-
-        key: str = f'{self.prefix}:{identifier}'
+        key: str = f"{self.prefix}:{identifier}"
 
         async with self.redis:
+            remaining_tokens: int
+            next_refill_at: int
+
             remaining_tokens, next_refill_at = await self.redis.eval(
                 script=TokenBucket.script,
                 keys=[key],
-                args=[self.max_number_of_tokens, self.interval, self.refill_rate, now]
+                args=[
+                    self.max_number_of_tokens,
+                    self.interval,
+                    self.refill_rate,
+                    self.current_time_in_milliseconds,
+                ],
             )
 
         return {
             "is_allowed": remaining_tokens >= 0,
             "limit": self.max_number_of_tokens,
             "remaining": remaining_tokens,
-            "reset": next_refill_at
+            "reset": next_refill_at,
         }
+
+    async def remaining(self, identifier: str) -> int:
+        """
+        Determine the number of identifier's remaining requests.
+        """
+
+        key: str = f"{self.prefix}:{identifier}"
+
+        async with self.redis:
+            bucket: list[Union[str, None]] = await self.redis.hmget(
+                key, "updated_at", "tokens"
+            )
+
+        if bucket[0] is None:  # The bucket does not exist yet.
+            return self.max_number_of_tokens
+
+        updated_at: float = float(bucket[0])
+
+        tokens: int = int(cast(str, bucket[1]))  # Signal that it can't be None.
+
+        if self.current_time_in_milliseconds < updated_at + self.interval:
+            return tokens
+
+        remaining_requests: int
+
+        if tokens <= 0:  # No more tokens were left before the refill.
+            remaining_requests = min(self.max_number_of_tokens, self.refill_rate)
+        else:
+            remaining_requests = min(
+                self.max_number_of_tokens, tokens + self.refill_rate
+            )
+
+        return remaining_requests
+
+    async def reset(self, identifier: str) -> int:
+        """
+        Determine the unix time in milliseconds when the next window begins.
+
+        If the identifier is not rate-limited, the returned value will be -1.
+        """
+
+        key: str = f"{self.prefix}:{identifier}"
+
+        now: float = self.current_time_in_milliseconds
+
+        async with self.redis:
+            updated_at: Union[str, None] = await self.redis.hget(key, "updated_at")
+
+        if updated_at is None:  # The bucket does not exist.
+            return -1
+
+        float_updated_at = int(float(updated_at))
+
+        if now < float_updated_at + self.interval:
+            return float_updated_at + self.interval
+
+        number_of_refills: int = floor((now - float_updated_at) / self.interval)
+
+        last_refill: int = float_updated_at + number_of_refills * self.interval
+
+        return last_refill + self.interval
```

### Comparing `upstash_ratelimit_a-0.1.3/upstash_ratelimit/limiter.py` & `upstash_ratelimit_a-0.1.4/upstash_ratelimit/limiter.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,48 +21,51 @@
     def fixed_window(
         self,
         max_number_of_requests: int,
         window: int,
         unit: Literal["ms", "s", "m", "h", "d"] = "ms",
     ) -> FixedWindow:
         """
-        The first request after a window has elapsed triggers the creation of a new one with the specified duration.
-        For each subsequent request, the algorithm checks whether the number of requests has exceeded the limit.
+        The time is divided into windows of fixed length and each window has a maximum number of allowed requests.
 
         :param max_number_of_requests: the number of requests allowed within the window
         :param window: the number of time units in which requests are limited
         :param unit: the shorthand version of the time measuring unit
         """
 
-        return FixedWindow(self.redis, max_number_of_requests, window, unit, self.prefix)
+        return FixedWindow(
+            self.redis, max_number_of_requests, window, unit, self.prefix
+        )
 
     def sliding_window(
         self,
         max_number_of_requests: int,
         window: int,
-        unit: Literal["ms", "s", "m", "h", "d"] = "ms"
+        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
     ) -> SlidingWindow:
         """
         Combined approach of sliding logs and fixed window with lower storage
         costs than sliding logs and improved boundary behavior by calculating a
         weighted score between two windows.
 
         :param max_number_of_requests: the number of requests allowed within the window
         :param window: the number of time units in which requests are limited
         :param unit: the shorthand version of the time measuring unit
         """
 
-        return SlidingWindow(self.redis, max_number_of_requests, window, unit, self.prefix)
+        return SlidingWindow(
+            self.redis, max_number_of_requests, window, unit, self.prefix
+        )
 
     def token_bucket(
         self,
         max_number_of_tokens: int,
         refill_rate: int,
         interval: int,
-        unit: Literal["ms", "s", "m", "h", "d"] = "ms"
+        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
     ) -> TokenBucket:
         """
         A bucket is filled with "max_number_of_tokens" that refill at "refill_rate" per "interval".
         Each request tries to consume one token and if the bucket is empty, the request is rejected.
 
         :param max_number_of_tokens: the maximum number of tokens that the bucket can hold
         :param refill_rate: the number of tokens that are refilled per interval
```

### Comparing `upstash_ratelimit_a-0.1.3/PKG-INFO` & `upstash_ratelimit_a-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit-a
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,14 +30,15 @@
   - [Install](#install)
     - [PyPi](#pypi)
   - [Setup database client](#setup-database-client)
   - [Usage](#usage)
   - [Telemetry](#telemetry)
   - [Block until ready](#block-until-ready)
   - [Timeout](#timeout)
+  - [Rate-limiting outbound requests](#rate-limiting-outbound-requests)
 - [Ratelimiting algorithms](#ratelimiting-algorithms)
   - [Fixed Window](#fixed-window)
     - [Pros:](#pros)
     - [Cons:](#cons)
     - [Usage:](#usage)
   - [Sliding Window](#sliding-window)
     - [Pros:](#pros-1)
@@ -93,15 +94,15 @@
 The constructor can take even more optional parameters, some of them being (types expanded):
 
 ```python
 url: str
 
 token: str
 
-rest_encoding: Literal["base64"] | Literal[False] = "base64"
+rest_encoding: Union[Literal["base64"], Literal[False]] = "base64"
 
 rest_retries: int = 1
 
 rest_retry_interval: int = 3 # In seconds.
 
 allow_deprecated: bool = False
 
@@ -131,20 +132,22 @@
 
 """
 Use a constant to limit all the requests together.
 For enforcing individual limits, use some kind of identifying variable (IP address, API key, etc.).
 """
 identifier: str = "constant"
 
-request_result: RateLimitResponse = await fixed_window.limit(identifier)
 
-if not request_result["is_allowed"]:
-    print(f"{identifier} is rate-limited!")
-else:
-    print("Request passed!")
+async def main() -> str:
+    request_result: RateLimitResponse = await fixed_window.limit(identifier)
+
+    if not request_result["is_allowed"]:
+        return f"{identifier} is rate-limited!"
+    else:
+        return "Request passed!"
 ```
 
 You can also pass a `prefix` to the `RateLimit` constructor to distinguish between the keys used for rate limiting and others.
 It defaults to `"ratelimit"`.
 
 The `limit` method also returns some metadata that might be useful :
 
@@ -195,20 +198,22 @@
     max_number_of_requests=1,
     window=3,
     unit="s"
 )
 
 identifier: str = "constant"
 
-request_result: RateLimitResponse = await fixed_window.block_until_ready(identifier, timeout=2000)
 
-if not request_result["is_allowed"]:
-    print(f"The {identifier}'s request cannot be processed, even after 2 seconds.")
-else:
-    print("Request passed!")
+async def main() -> str:
+    request_result: RateLimitResponse = await fixed_window.block_until_ready(identifier, timeout=2000)
+
+    if not request_result["is_allowed"]:
+        return f"The {identifier}'s request cannot be processed, even after 2 seconds."
+    else:
+        return "Request passed!"
 ```
 
 
 ## Timeout
 If you worry that network issues can cause your application to reject requests, you can use python's `wait_for` to 
 allow the requests which exceed a given timeout to pass regardless of what the current limit is.
 
@@ -241,19 +246,50 @@
         return "Request passed!"
 
     except TimeoutError:
         return "Request passed"
 ```
 
 
+## Rate-limiting outbound requests
+It's also possible to limit the number of requests you're making to an external API.
+
+```python
+from upstash_ratelimit.limiter import RateLimit
+from upstash_ratelimit.schema.response import RateLimitResponse
+
+from upstash_redis.client import Redis
+
+rate_limit = RateLimit(Redis.from_env())
+
+fixed_window = rate_limit.fixed_window(
+    max_number_of_requests=1,
+    window=3,
+    unit="s"
+)
+
+identifier: str = "constant"  # Or, use an identifier to limit your requests to a certain endpoint.
+
+
+async def main() -> str:
+    request_result: RateLimitResponse = await fixed_window.limit(identifier)
+
+    if not request_result["is_allowed"]:
+        return f"{identifier} is rate-limited!"
+    else:
+        # Call the API
+        # ...
+        return "Request passed!"
+```
+
+
 # Ratelimiting algorithms
 
 ## Fixed Window
-This algorithm divides time into windows of fixed duration. The first request after a window has elapsed triggers the creation of a new one. 
-For each subsequent request, the algorithm checks whether the number of requests has exceeded the limit.
+The time is divided into windows of fixed length and each window has a maximum number of allowed requests.
 
 ### Pros
 - Very cheap in terms of data size and computation
 - Newer requests are not starved due to a high burst in the past
 
 ### Cons
 - Can cause high bursts at the window boundaries to leak through
@@ -347,23 +383,30 @@
 
 They are also grouped in the [RateLimit](upstash_ratelimit/limiter.py) class for ease of use.
 
 
 ## Running tests
 All tests live in the [test](./tests) folder.
 
-Only the limiting logic of 100%-accuracy algorithms and other utility functions are unit-tested.
+Only the logic of 100%-accuracy algorithms and other utility functions are unit-tested.
 
 To run all the tests, make sure you are in the `tests` folder and have the poetry virtual environment activated with all 
 the necessary dependencies. Set the `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` environment variables and run:
 
 ```bash
-poetry run pytest
+poetry run pytest --import-mode importlib
 ```
 
+The reason we need to use the `importlib` mode is because there are multiple test files with the same name. See the 
+[pytest docs](https://docs.pytest.org/en/stable/explanation/pythonpath.html#import-modes) for more info.
+
+**Warning**: The current evaluation speed of the tests does not take the HTTP requests duration into account. 
+Because of that, if a request takes more than 2 seconds to complete, a test might fail.
+
+
 ## Releasing
 To create a new release, first use Poetry's [version](https://python-poetry.org/docs/cli/#version) command.
 
 You will then need to connect your PyPi API token to Poetry. 
 A simple tutorial showcasing how to do it was posted by Tony Tran
 [on DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
```

