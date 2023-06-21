# Comparing `tmp/upstash_ratelimit_a-0.1.6.tar.gz` & `tmp/upstash_ratelimit_a-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit_a-0.1.6.tar", max compression
+gzip compressed data, was "upstash_ratelimit_a-0.1.7.tar", max compression
```

## Comparing `upstash_ratelimit_a-0.1.6.tar` & `upstash_ratelimit_a-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/LICENSE
--rw-r--r--   0        0        0    11067 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/README.md
--rw-r--r--   0        0        0      402 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 06:33:30.373891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    18972 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     2997 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      392 2023-06-21 06:33:30.377891 upstash_ratelimit_a-0.1.6/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    11659 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-21 06:38:41.533745 upstash_ratelimit_a-0.1.7/LICENSE
+-rw-r--r--   0        0        0    11067 2023-06-21 06:38:41.533745 upstash_ratelimit_a-0.1.7/README.md
+-rw-r--r--   0        0        0      402 2023-06-21 06:38:41.533745 upstash_ratelimit_a-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 06:38:41.533745 upstash_ratelimit_a-0.1.7/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0    18972 2023-06-21 06:38:41.533745 upstash_ratelimit_a-0.1.7/upstash_ratelimit/algorithm.py
+-rw-r--r--   0        0        0      167 2023-06-21 06:38:41.537745 upstash_ratelimit_a-0.1.7/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     2997 2023-06-21 06:38:41.537745 upstash_ratelimit_a-0.1.7/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:38:41.537745 upstash_ratelimit_a-0.1.7/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-06-21 06:38:41.537745 upstash_ratelimit_a-0.1.7/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0      392 2023-06-21 06:38:41.537745 upstash_ratelimit_a-0.1.7/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    11659 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.7/PKG-INFO
```

### Comparing `upstash_ratelimit_a-0.1.6/LICENSE` & `upstash_ratelimit_a-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.6/README.md` & `upstash_ratelimit_a-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.6/upstash_ratelimit/algorithm.py` & `upstash_ratelimit_a-0.1.7/upstash_ratelimit/algorithm.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.6/upstash_ratelimit/limiter.py` & `upstash_ratelimit_a-0.1.7/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.6/PKG-INFO` & `upstash_ratelimit_a-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit-a
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

