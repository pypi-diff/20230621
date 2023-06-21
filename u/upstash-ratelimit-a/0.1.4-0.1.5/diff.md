# Comparing `tmp/upstash_ratelimit_a-0.1.4.tar.gz` & `tmp/upstash_ratelimit_a-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit_a-0.1.4.tar", max compression
+gzip compressed data, was "upstash_ratelimit_a-0.1.5.tar", max compression
```

## Comparing `upstash_ratelimit_a-0.1.4.tar` & `upstash_ratelimit_a-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.4/LICENSE
--rw-r--r--   0        0        0    11073 2023-06-21 03:32:26.282431 upstash_ratelimit_a-0.1.4/README.md
--rw-r--r--   0        0        0      402 2023-06-21 03:34:34.876458 upstash_ratelimit_a-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.4/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    19009 2023-06-21 03:33:12.696738 upstash_ratelimit_a-0.1.4/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.4/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     2997 2023-06-21 03:20:53.439921 upstash_ratelimit_a-0.1.4/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.4/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-06-21 03:20:40.665118 upstash_ratelimit_a-0.1.4/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      392 2023-06-21 03:20:40.665308 upstash_ratelimit_a-0.1.4/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.5/LICENSE
+-rw-r--r--   0        0        0    11073 2023-06-21 03:32:26.282431 upstash_ratelimit_a-0.1.5/README.md
+-rw-r--r--   0        0        0      402 2023-06-21 04:12:46.364381 upstash_ratelimit_a-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.5/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0    19009 2023-06-21 03:33:12.696738 upstash_ratelimit_a-0.1.5/upstash_ratelimit/algorithm.py
+-rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.5/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     2997 2023-06-21 03:20:53.439921 upstash_ratelimit_a-0.1.5/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.5/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-06-21 03:20:40.665118 upstash_ratelimit_a-0.1.5/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0      392 2023-06-21 03:20:40.665308 upstash_ratelimit_a-0.1.5/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.5/PKG-INFO
```

### Comparing `upstash_ratelimit_a-0.1.4/LICENSE` & `upstash_ratelimit_a-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.4/README.md` & `upstash_ratelimit_a-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.4/upstash_ratelimit/algorithm.py` & `upstash_ratelimit_a-0.1.5/upstash_ratelimit/algorithm.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.4/upstash_ratelimit/limiter.py` & `upstash_ratelimit_a-0.1.5/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.4/PKG-INFO` & `upstash_ratelimit_a-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit-a
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

