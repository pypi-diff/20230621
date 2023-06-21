# Comparing `tmp/xju-1.2.9.tar.gz` & `tmp/xju-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xju-1.2.9.tar", last modified: Sun Apr 30 10:52:37 2023, max compression
+gzip compressed data, was "xju-1.3.0.tar", last modified: Wed Jun 21 10:31:40 2023, max compression
```

## Comparing `xju-1.2.9.tar` & `xju-1.3.0.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/
--rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-04-30 10:52:36.000000 xju-1.2.9/MIT-LICENCE
--rw-r--r--   0 xju       (1001) xju       (1001)     6560 2023-04-30 10:52:37.663515 xju-1.2.9/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     5024 2023-04-30 10:52:36.000000 xju-1.2.9/README.rst
--rw-r--r--   0 xju       (1001) xju       (1001)     1597 2023-04-30 10:52:36.000000 xju-1.2.9/pyproject.toml
--rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-04-30 10:52:37.663515 xju-1.2.9/setup.cfg
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.659515 xju-1.2.9/src/
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.659515 xju-1.2.9/src/xju/
--rw-r--r--   0 xju       (1001) xju       (1001)     5803 2023-02-25 06:28:28.000000 xju-1.2.9/src/xju/assert_.py
--rw-r--r--   0 xju       (1001) xju       (1001)     5837 2023-03-18 10:37:15.000000 xju-1.2.9/src/xju/assert_.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/src/xju/cmc/
--rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.2.9/src/xju/cmc/AsyncServiceQueue.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.2.9/src/xju/cmc/Dict.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.2.9/src/xju/cmc/ThreadMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    17022 2023-03-18 11:11:14.000000 xju-1.2.9/src/xju/cmc/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2238 2023-03-18 10:40:23.000000 xju-1.2.9/src/xju/cmc/cmc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    14656 2023-03-18 10:40:28.000000 xju-1.2.9/src/xju/cmc/cmclass.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/src/xju/cmc/io/
--rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.2.9/src/xju/cmc/io/FileLock.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.2.9/src/xju/cmc/io/FileMode.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.2.9/src/xju/cmc/io/FilePosition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.2.9/src/xju/cmc/io/FileReader.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.2.9/src/xju/cmc/io/FileWriter.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.2.9/src/xju/cmc/io/Pipe.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.2.9/src/xju/cmc/io/UnixStreamSocket.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.2.9/src/xju/cmc/io/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.2.9/src/xju/cmc/perflog.py
--rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.2.9/src/xju/cmc/perflog.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.2.9/src/xju/cmc/signal.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.2.9/src/xju/cmc/signal.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.2.9/src/xju/cmc/tstore.py
--rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.2.9/src/xju/cmc/tstore.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.2.9/src/xju/cmd.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.2.9/src/xju/cmd.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    49437 2023-04-30 10:42:18.000000 xju-1.2.9/src/xju/json_codec.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)    28466 2023-04-30 10:35:38.000000 xju-1.2.9/src/xju/json_codec.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.2.9/src/xju/jsonschema.py
--rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.2.9/src/xju/jsonschema.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.2.9/src/xju/misc.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.2.9/src/xju/misc.py.test
--r--r--r--   0 xju       (1001) xju       (1001)    21254 2023-04-16 02:25:56.000000 xju-1.2.9/src/xju/newtype.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11849 2023-03-18 10:39:25.000000 xju-1.2.9/src/xju/newtype.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.2.9/src/xju/patch.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.2.9/src/xju/patch.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-1.2.9/src/xju/pq.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.2.9/src/xju/pq.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:36.000000 xju-1.2.9/src/xju/py.typed
--rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.2.9/src/xju/rfc2616.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.2.9/src/xju/rfc2616.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3280 2023-04-30 10:35:38.000000 xju-1.2.9/src/xju/time.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.2.9/src/xju/time.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7226 2023-01-22 04:53:39.000000 xju-1.2.9/src/xju/xn.py
--rw-r--r--   0 xju       (1001) xju       (1001)     5869 2023-03-18 10:41:39.000000 xju-1.2.9/src/xju/xn.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/src/xju.egg-info/
--rw-r--r--   0 xju       (1001) xju       (1001)     6560 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     1215 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/SOURCES.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/dependency_links.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/top_level.txt
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.132263 xju-1.3.0/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-06-21 10:31:39.000000 xju-1.3.0/MIT-LICENCE
+-rw-r--r--   0 xju       (1001) xju       (1001)     9044 2023-06-21 10:31:40.132263 xju-1.3.0/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     7508 2023-06-21 10:31:39.000000 xju-1.3.0/README.rst
+-rw-r--r--   0 xju       (1001) xju       (1001)     1742 2023-06-21 10:31:39.000000 xju-1.3.0/pyproject.toml
+-rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-06-21 10:31:40.132263 xju-1.3.0/setup.cfg
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.124263 xju-1.3.0/src/
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.128263 xju-1.3.0/src/xju/
+-rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-1.3.0/src/xju/assert_.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-1.3.0/src/xju/assert_.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.128263 xju-1.3.0/src/xju/cmc/
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     9781 2023-06-20 09:48:20.000000 xju-1.3.0/src/xju/cmc/AsyncDict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-1.3.0/src/xju/cmc/AsyncOpt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.3.0/src/xju/cmc/AsyncServiceQueue.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-06-11 03:07:27.000000 xju-1.3.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.3.0/src/xju/cmc/Dict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-1.3.0/src/xju/cmc/Opt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.3.0/src/xju/cmc/ThreadMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    41771 2023-06-21 01:30:26.000000 xju-1.3.0/src/xju/cmc/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6803 2023-06-19 11:23:59.000000 xju-1.3.0/src/xju/cmc/async_cmclass.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-1.3.0/src/xju/cmc/cmc.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    14657 2023-06-17 10:59:19.000000 xju-1.3.0/src/xju/cmc/cmclass.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.132263 xju-1.3.0/src/xju/cmc/io/
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.3.0/src/xju/cmc/io/FileLock.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.3.0/src/xju/cmc/io/FileMode.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.3.0/src/xju/cmc/io/FilePosition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.3.0/src/xju/cmc/io/FileReader.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.3.0/src/xju/cmc/io/FileWriter.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.3.0/src/xju/cmc/io/Pipe.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.3.0/src/xju/cmc/io/UnixStreamSocket.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.3.0/src/xju/cmc/io/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.3.0/src/xju/cmc/perflog.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.3.0/src/xju/cmc/perflog.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.3.0/src/xju/cmc/signal.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.3.0/src/xju/cmc/signal.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.3.0/src/xju/cmc/tstore.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.3.0/src/xju/cmc/tstore.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.3.0/src/xju/cmd.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.3.0/src/xju/cmd.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    63268 2023-06-21 10:25:57.000000 xju-1.3.0/src/xju/json_codec.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)    42007 2023-06-11 10:43:01.000000 xju-1.3.0/src/xju/json_codec.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.3.0/src/xju/jsonschema.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.3.0/src/xju/jsonschema.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.3.0/src/xju/misc.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.3.0/src/xju/misc.py.test
+-r--r--r--   0 xju       (1001) xju       (1001)    22865 2023-06-11 07:25:02.000000 xju-1.3.0/src/xju/newtype.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11796 2023-06-11 09:21:50.000000 xju-1.3.0/src/xju/newtype.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.3.0/src/xju/patch.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.3.0/src/xju/patch.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-1.3.0/src/xju/pq.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.3.0/src/xju/pq.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:39.000000 xju-1.3.0/src/xju/py.typed
+-rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.3.0/src/xju/rfc2616.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.3.0/src/xju/rfc2616.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3280 2023-04-30 10:35:38.000000 xju-1.3.0/src/xju/time.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.3.0/src/xju/time.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7236 2023-06-21 01:02:08.000000 xju-1.3.0/src/xju/xn.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     5202 2023-06-21 01:07:25.000000 xju-1.3.0/src/xju/xn.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.128263 xju-1.3.0/src/xju.egg-info/
+-rw-r--r--   0 xju       (1001) xju       (1001)     9044 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     1380 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/SOURCES.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/dependency_links.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/top_level.txt
```

### Comparing `xju-1.2.9/MIT-LICENCE` & `xju-1.3.0/MIT-LICENCE`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/PKG-INFO` & `xju-1.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.2.9
+Version: 1.3.0
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -53,14 +53,34 @@
 * see `xju/cmc/cmclass.py.test <xju/cmc/cmclass.py.test>`_ for sample code
 
 
 `xju.cmc.Dict <xju/cmc/__init__.py>`_ - dictionary that is a context manager for its (context manager) values
 
 * see `xju/cmc/Dict.py.test <xju/cmc/Dict.py.test>`_ for sample code
 
+`xju.cmc.Opt <xju/cmc/__init__.py>`_ - context manager for its optional (context manager) value
+
+* see `xju/cmc/Opt.py.test <xju/cmc/Opt.py.test>`_ for sample code
+
+`xju.cmc.async_cmclass <xju/cmc/__init__.py>`_  - provides async context management for class attributes that are async / sync context managers
+
+* managing multiple resource attributes is clumsy with AsyncExitStack, this module implements
+  \__aenter__ and \__aexit__ automatically to ensure correct ordering and cleanup on exceptions
+
+* see `xju/cmc/async_cmclass.py.test <xju/cmc/async_cmclass.py.test>`_ for sample code
+
+
+`xju.cmc.AsyncDict <xju/cmc/__init__.py>`_ - dictionary that is a async context manager for its (async context manager) values
+
+* see `xju/cmc/AsyncDict.py.test <xju/cmc/AsyncDict.py.test>`_ for sample code
+
+`xju.cmc.AsyncOpt <xju/cmc/__init__.py>`_ - async context manager for its optional (async context manager) value
+
+* see `xju/cmc/AsyncOpt.py.test <xju/cmc/AsyncOpt.py.test>`_ for sample code
+
 
 `xju.cmc.io <xju/cmc/io/__init__.py>`_ - pure context management for e.g. file reading and writing, non-blocking io
 
 * see unit tests for sample code:
   *  `FileLock.py.test <xju/cmc/io/FileLock.py.test>`_
   *  `FileMode.py.test <xju/cmc/io/FileMode.py.test>`_
   *  `FilePosition.py.test <xju/cmc/io/FilePosition.py.test>`_
@@ -86,19 +106,19 @@
 `xju.cmc.Thread/Mutex/Lock/Condition <xju/cmc/__init__.py>`_
 
 * threading primitives that encourage correct design
 
 * see `xju/cmc/ThreadMutexLockCondition.py.test <xju/cmc/ThreadMutexLockCondition.py.test>`_ for sample code
 
 
-`xju.cmc.Task <xju/cmc/__init__.py>`_
+`xju.cmc.AsyncTask/Mutex/Lock/Condition <xju/cmc/__init__.py>`_
 
-* asyncio Task context manager
+* asyncio Task/Mutex/Lock/Condition context managers
 
-* see `xju/cmc/Task.py.test <xju/cmc/Task.py.test>`_ for sample code
+* see `xju/cmc/Task.py.test <xju/cmc/AsyncTaskMutexLockCondition.py.test>`_ for sample code
 
 
 `xju.cmc.AsyncServiceQueue <xju/cmc/__init__.py>`_
 
 * asyncio thread-safe service queue, allows any thread to queue a coroutine on an event loop
   so it is executed by a task in that event loop
 
@@ -134,14 +154,16 @@
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
 * generates typescript code (types, type-guards and dynamic casts) equivalents
 
+* extensible with custom encodings
+
 * see `xju/json_codec.py.test <xju/json_codec.py.test>`_ for full sample code
 
 
 `xju.jsonschema <xju/jsonschema.py>`_
 
 * represents JSON schemas as straight-foward, easy-to-read python data structures, because life's too short for jsonschema.org
 
@@ -166,14 +188,31 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
+- 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
+- 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
+- 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
+- 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
+- 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
+- 1.2.13 xju.newtype eq/neq now follows python "you can compare apples to oranges", rely on mypy --strict-equality (which for what it's worth is broken at mypy 1.3.0)
+- 1.2.13 now compatible with mypy --strict-equality
+- 1.2.13 add xju.cmc.AsyncTask/Mutex/Condition/Lock (thread equivalents for asyncio); note Task deprecated, use AsyncTask
+- 1.2.13 add custom encoding facility to xju.json_codec
+- 1.2.13 add typescript aliases to json_codec generated code for xju.newtype Str/Int/Float
+- 1.2.12 fixes typescript null v object handling
+- 1.2.12 adds typescript aliases for NewStr, NewInt, NewFloat
+- 1.2.11 adds typescript --strict support and fixes typescript code generation bugs
+- 1.2.11 xju.json_codec supports Literal[int] and Literal[bool]
+- 1.2.11 xju.json_codec supports generic classes
+- 1.2.10 xju.json_codec supports typing.NewType str/int/bool/float
 - 1.2.9 xju.json_codec generates typescript equivalents
 - 1.2.9 xju.json_codec adds codec() convenience method
 - 1.2.9 xju.json_codec uses kw_args to construct classes
 
 - 1.2.8 xju.json_codec supports string type-hints (for foward definitions)
 - 1.2.8 xju.json_codec adds typing.Self support (for recursive types)
 - 1.2.8 xju.json_codec requires python 3.11, tested with mypy 1.1.1
```

### Comparing `xju-1.2.9/pyproject.toml` & `xju-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xju"
-version = "1.2.9"
+version = "1.3.0"
 description = "xju library"
 readme = "README.rst"
 authors = [{ name = "Trevor Taylor"}]
 license = { file = "MIT-LICENCE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -19,8 +19,8 @@
 Homepage = "https://github.com/urnest/urnest"
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["xju","xju.*","xju.cmc.*"]  # package names should match these glob patterns (["*"] by default)
 exclude = []  # exclude packages matching these glob patterns (empty by default)
 namespaces = true  # to disable scanning PEP 420 namespaces (true by default)
 [tool.setuptools.package-data]
-xju = [ "./cmd.py.test","./xn.py.test","./newtype.py.test","./time.py.test","./json_codec.py.test","./pq.py.test","./jsonschema.py.test","./misc.py.test","./assert_.py.test","./rfc2616.py.test","./cmc/tstore.py.test","./cmc/Dict.py.test","./cmc/io/FileWriter.py.test","./cmc/io/UnixStreamSocket.py.test","./cmc/io/Pipe.py.test","./cmc/io/FilePosition.py.test","./cmc/io/FileLock.py.test","./cmc/io/FileReader.py.test","./cmc/io/FileMode.py.test","./cmc/ThreadMutexLockCondition.py.test","./cmc/signal.py.test","./cmc/cmc.py.test","./cmc/AsyncServiceQueue.py.test","./cmc/perflog.py.test","./cmc/cmclass.py.test","./patch.py.test", "py.typed"]
+xju = [ "./cmd.py.test","./xn.py.test","./newtype.py.test","./time.py.test","./json_codec.py.test","./pq.py.test","./jsonschema.py.test","./misc.py.test","./assert_.py.test","./rfc2616.py.test","./cmc/tstore.py.test","./cmc/Dict.py.test","./cmc/AsyncDict.py.test","./cmc/io/FileWriter.py.test","./cmc/io/UnixStreamSocket.py.test","./cmc/io/Pipe.py.test","./cmc/io/FilePosition.py.test","./cmc/io/FileLock.py.test","./cmc/io/FileReader.py.test","./cmc/io/FileMode.py.test","./cmc/ThreadMutexLockCondition.py.test","./cmc/async_cmclass.py.test","./cmc/AsyncOpt.py.test","./cmc/Opt.py.test","./cmc/signal.py.test","./cmc/cmc.py.test","./cmc/AsyncServiceQueue.py.test","./cmc/perflog.py.test","./cmc/cmclass.py.test","./cmc/AsyncTaskMutexLockCondition.py.test","./patch.py.test", "py.typed"]
```

### Comparing `xju-1.2.9/src/xju/assert_.py` & `xju-1.3.0/src/xju/assert_.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,24 @@
         return self.x
     def isNotInstanceOf(self,y):
         if isinstance(self.x,y):
             xc=self.x.__class__.__name__
             yc=y.__name__
             raise Exception(f'{self.x!r} is unexpectedly an instance of class {yc} (it is of class {xc})')
         return self.x
+    def isSubclassOf(self,y):
+        if not issubclass(self.x,y):
+            yc=y.__name__
+            raise Exception(f'{self.x!r} is not an subclass of class {yc}')
+        return self.x
+    def isNotSubclassOf(self,y):
+        if issubclass(self.x,y):
+            yc=y.__name__
+            raise Exception(f'{self.x!r} is unexpectedly an subclass of class {yc}')
+        return self.x
     def hasAttr(self,y:str):
         if not hasattr(self.x,y):
             raise Exception(f'{self.x!r} has no {y!r} attribute')
     def doesNotHaveAttr(self,y:str):
         if hasattr(self.x,y):
             raise Exception(f'{self.x!r} unexpectedly has {y!r} attribute')
     def startsWith(self,y):
```

### Comparing `xju-1.2.9/src/xju/assert_.py.test` & `xju-1.3.0/src/xju/assert_.py.test`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 Assert('fred').starts_with('f')
 Assert('fred').endswith('d')
 Assert('fred').endsWith('d')
 Assert('fred').ends_with('d')
 Assert('fred').contains('d')
 Assert(7).isInstanceOf(int)
 Assert(7).isNotInstanceOf(str)
+Assert(int).isSubclassOf(int)
+Assert(int).isNotSubclassOf(str)
 Assert(7)==7
 Assert(7)!=8
 Assert(7)>6
 Assert(7)>=6
 Assert(7)<=8
 Assert(7)<8
 Assert(7).isIn([7,8,9])
@@ -81,14 +83,30 @@
 except Exception as e:
     assert "7 is unexpectedly an instance of class int (it is of class int)" in str(e), str(e)
 else:
     assert False
     pass
 
 try:
+    Assert(int).isSubclassOf(str)
+except Exception as e:
+    assert "<class 'int'> is not an subclass of class str" in str(e), str(e)
+else:
+    assert False
+    pass
+
+try:
+    Assert(int).isNotSubclassOf(int)
+except Exception as e:
+    assert "<class 'int'> is unexpectedly an subclass of class int" in str(e), str(e)
+else:
+    assert False
+    pass
+
+try:
     Assert(7)>10
 except Exception as e:
     assert "7 is not greater than 10" in str(e), str(e)
 else:
     assert False
     pass
```

### Comparing `xju-1.2.9/src/xju/cmc/AsyncServiceQueue.py.test` & `xju-1.3.0/src/xju/cmc/AsyncServiceQueue.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/Dict.py.test` & `xju-1.3.0/src/xju/cmc/Dict.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/ThreadMutexLockCondition.py.test` & `xju-1.3.0/src/xju/cmc/ThreadMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/cmc.py.test` & `xju-1.3.0/src/xju/cmc/cmc.py.test`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from xju import cmc
 
 import asyncio
 from xju.assert_ import Assert
 from typing import cast, Awaitable
 
 try:
-    cmc.is_subclass('fred', 7, cast(type, 'jock'))
+    cmc._is_subclass('fred', 7, cast(type, 'jock'))
 except Exception as e:
     Assert("'jock' is not an instance of class type (it is of class str)").isIn(str(e))
     pass
 
 
 async def async_main() -> None:
     async def task_that_succeeds() -> int:
```

### Comparing `xju-1.2.9/src/xju/cmc/cmclass.py.test` & `xju-1.3.0/src/xju/cmc/cmclass.py.test`

 * *Files 0% similar despite different names*

```diff
@@ -600,8 +600,8 @@
     Assert(r.y.entered_at) == 1
     Assert(r.y.exited_at) == None
     pass
 
 Assert(r.y.entered_at) == 1
 Assert(r.y.exited_at) == 2
 
-Assert(cmc.is_subclass('a',7,int))==False
+Assert(cmc._is_subclass('a',7,int))==False
```

### Comparing `xju-1.2.9/src/xju/cmc/io/FileLock.py.test` & `xju-1.3.0/src/xju/cmc/io/FileLock.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/io/FileMode.py.test` & `xju-1.3.0/src/xju/cmc/io/FileMode.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/io/FilePosition.py.test` & `xju-1.3.0/src/xju/cmc/io/FilePosition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/io/FileReader.py.test` & `xju-1.3.0/src/xju/cmc/io/FileReader.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/io/FileWriter.py.test` & `xju-1.3.0/src/xju/cmc/io/FileWriter.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/io/Pipe.py.test` & `xju-1.3.0/src/xju/cmc/io/Pipe.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/io/UnixStreamSocket.py.test` & `xju-1.3.0/src/xju/cmc/io/UnixStreamSocket.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/io/__init__.py` & `xju-1.3.0/src/xju/cmc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/perflog.py` & `xju-1.3.0/src/xju/cmc/perflog.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/perflog.py.test` & `xju-1.3.0/src/xju/cmc/perflog.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/signal.py` & `xju-1.3.0/src/xju/cmc/signal.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/signal.py.test` & `xju-1.3.0/src/xju/cmc/signal.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/tstore.py` & `xju-1.3.0/src/xju/cmc/tstore.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmc/tstore.py.test` & `xju-1.3.0/src/xju/cmc/tstore.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmd.py` & `xju-1.3.0/src/xju/cmd.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/cmd.py.test` & `xju-1.3.0/src/xju/cmd.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/json_codec.py` & `xju-1.3.0/src/xju/json_codec.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,17 +26,19 @@
 #   codec(Address).encode(Address(32,'asler'))=={'number':32, 'street': 'asler'}
 #
 # For examples see json_codec.py.test
 #
 from dataclasses import dataclass
 from xju.xn import Xn,in_context,in_function_context,readable_repr
 from typing import TypeVar, Generic, Type, cast, Any, Protocol, Self, Callable, get_type_hints
-from typing import Sequence, Literal
+from typing import Sequence, Literal, NewType
 from typing import _LiteralGenericAlias  # type: ignore  # mypy 1.1.1
 from typing import _UnionGenericAlias  # type: ignore  # mypy 1.1.1
+from typing import _GenericAlias  # type: ignore  # mypy 1.2.0
+from typing import get_origin,get_args, runtime_checkable
 from types import GenericAlias, UnionType, NoneType
 import xju.newtype
 
 T=TypeVar('T')
 
 JsonType = None|bool|dict|list|float|str
 
@@ -89,15 +91,15 @@
     return Codec[T](t)
 
 class Codec(Generic[T]):
     t:Type[T]
     def __init__(self, t: Type[T]):
         'initialse json decoder for type %(t)r'
         self.t=t
-        self.codec:CodecProto=_explodeSchema(self.t)
+        self.codec:CodecProto=_explodeSchema(self.t, {})
         pass
 
     def __repr__(self):
         return f'{self.t!r} json codec'
 
     def encode(self,x:T) -> JsonType:
         'encode {self.t} {x} to json'
@@ -120,16 +122,34 @@
         result.update({
             'definitions':definitions
         })
         return result
     def typescript_type(self) -> TypeScriptUQN:
         '''return typescript unqualified equivalent type for T'''
         return self.codec.typescript_type(None)
-    def ensure_typescript_defs(self, namespace) -> None:
+    def ensure_typescript_defs(self, namespace:TypeScriptNamespace) -> None:
         return self.codec.ensure_typescript_defs(namespace)
+    def add_typescript_alias(self, namespace:TypeScriptNamespace, fqn:Sequence[TypeScriptUQN]) -> None:
+        '''add {fqn} as typescript alias for {self.t}'''
+        assert len(fqn)>0
+        try:
+            target_namespace=namespace.get_namespace_of(fqn)
+            if fqn[-1] in target_namespace.defs:
+                m='.'.join([str(_) for _ in fqn])
+                raise Exception(
+                    f'{m} is already defined as {target_namespace.defs[fqn[-1]]}')
+            target_namespace.defs[fqn[-1]]=TypeScriptSourceCode(
+                f'type {fqn[-1]} = {self.typescript_type()};')
+            target_namespace.defs[TypeScriptUQN(f"asInstanceOf{fqn[-1]}")] = TypeScriptSourceCode(
+                f"function asInstanceOf{fqn[-1]}(v:any):{fqn[-1]} {{ return {self.codec.get_typescript_asa(TypeScriptSourceCode('v'),namespace,None)}; }}")
+            target_namespace.defs[TypeScriptUQN(f"isInstanceOf{fqn[-1]}")] = TypeScriptSourceCode(
+                f"function isInstanceOf{fqn[-1]}(v:any):v is {fqn[-1]} {{ return {self.codec.get_typescript_isa(TypeScriptSourceCode('v'),namespace,None)}; }}")
+        except:
+            raise in_function_context(Codec.add_typescript_alias,vars())
+        pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace) -> TypeScriptSourceCode:
         '''get typescript "{expression} is a T" code, adding any necessary definitions to {namespace}
            result is a type-guard expression, examples of some possible results:
              parameter       possible code                  note
              "x.y"           "(typeof (x.y) == 'number')"   (uses built-in type guard pattern)
@@ -291,15 +311,15 @@
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         tt=self.typescript_type(back_refs)
         return TypeScriptSourceCode(
             f"((v: any): {tt} => {{try{{\n"
             f"    if (!Array.isArray(v)) throw new Error(`${{v}} is not an array it is a ${{typeof v}}`);\n"
             f"    v.forEach((x)=>{indent(4,self.value_codec.get_typescript_asa(TypeScriptSourceCode('x'),namespace,back_refs))});\n"
             f"    return v as {tt};\n"
-            f"}}catch(e){{throw new Error(`${{v}} is not a {tt} because ${{e}}`);}}}})({expression})")
+            f"}}catch(e:any){{throw new Error(`${{v}} is not a {tt} because ${{e}}`);}}}})({expression})")
     pass
 
 class AnyListCodec:
     def __init__(self):
         self.value_codec=AnyJsonCodec()
         pass
     def encode(self,x,back_ref:None|Callable[[Any],JsonType]):
@@ -400,21 +420,21 @@
         tt=self.typescript_type(back_refs)
         return TypeScriptSourceCode(
             f"((v: any): {tt} => {{try{{\n" +
             f"    if (!Array.isArray(v)) throw new Error(`${{v}} is not an array it is a ${{typeof v}}`);\n" +
             f"    if (v.length != {self.number_of_codecs}) throw new Error(`${{v}} does not have {self.number_of_codecs} elements (it has ${{v.length}} elements)`);\n" +
             ''.join(asas)+
             f"    return v as {tt};\n"+
-            f"}}catch(e){{ throw new Error(`${{v}} is not a {tt} because ${{e}}`);}}}})({expression})")
+            f"}}catch(e:any){{ throw new Error(`${{v}} is not a {tt} because ${{e}}`);}}}})({expression})")
     pass
 
 class UnionCodec:
-    def __init__(self,allowed_types):
+    def __init__(self,allowed_types, value_codecs):
         self.allowed_types=allowed_types
-        self.value_codecs={t:_explodeSchema(t) for t in allowed_types}
+        self.value_codecs=value_codecs
         pass
     def encode(self,x,back_ref:None|Callable[[Any],JsonType]) -> JsonType:
         'encode {x!r} as one of {self.allowed_types}'
         try:
             exceptions=[]
             for t, c in self.value_codecs.items():
                 try:
@@ -425,24 +445,25 @@
                 pass
             raise Exception(' and '.join([f'failed to encode as {t} because {e}' for t,e in exceptions]))
                 
         except Exception:
             raise in_function_context(UnionCodec.encode,vars()) from None
         pass
     def decode(self,x,back_ref:None|Callable[[JsonType],Any]) -> tuple:
+        '''decode {x!r} as one of {self.allowed_types}'''
         try:
             exceptions=[]
             for t, c in self.value_codecs.items():
                 try:
                     return c.decode(x,back_ref)
                 except Exception as e:
                     exceptions.append( (t, e) )
                     pass
                 pass
-            raise Exception(' and '.join([f'failed to decode as {t} because {e}' for t,e in exceptions]))
+            raise Exception(' and '.join([f'failed to decode as {t!r} because {e}' for t,e in exceptions]))
         except Exception:
             raise in_function_context(UnionCodec.decode,vars()) from None
         pass
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             "oneOf": [ codec.get_json_schema(definitions, self_ref) for codec in self.value_codecs.values() ]
         }
@@ -466,24 +487,24 @@
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         tt=self.typescript_type(back_refs)
         asas=[f"    try{{\n"+
               f"        {indent(8,value_codec.get_typescript_asa('v',namespace,back_refs))};\n"+
               f"        return v as {tt};\n"+
               f"    }}\n"+
-              f"    catch(e){{\n"+
+              f"    catch(e:any){{\n"+
               f"        es.push(e.message);\n"+
               f"    }};\n"
               for value_codec in self.value_codecs.values()]
         return TypeScriptSourceCode(
             f"((v: any): {tt} => {{try{{\n" +
             f"    var es = new Array<string>();\n"+
             "".join(asas)+
             f"    throw new Error(es.join(' and '));\n"+
-            f"}}catch(e)\n"+
+            f"}}catch(e:any)\n"+
             f"{{\n"+
             f"    throw new Error(`${{v}} is not a {tt} because ${{e}}`);\n"+
             f"}}}})({expression})")
     pass
 
 class DictCodec:
     def __init__(self, key_codec, value_codec):
@@ -516,14 +537,15 @@
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         return TypeScriptSourceCode(
             f"(((x:any):x is {self.typescript_type(back_refs)}=>(\n"
+            f"    x !== null &&\n"
             f"    typeof (x) === 'object' &&\n"
             f"    !Array.isArray(x) &&\n"
             f"    (():boolean=>{{for (const k in x){{\n"
             f"        if (!x.hasOwnProperty(k)) continue;\n"
             f"        if (!({indent(8,self.key_codec.get_typescript_isa(TypeScriptSourceCode('k'),namespace,back_refs))} )||\n"
             f"            !({indent(8,self.value_codec.get_typescript_isa(TypeScriptSourceCode('x[k]'),namespace,back_refs))})) return false;}}\n"
             f"    return true;\n"
@@ -531,26 +553,27 @@
     def get_typescript_asa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         tt=self.typescript_type(back_refs)
         return TypeScriptSourceCode(
             f"((x: any): {tt} => {{try{{\n"
+            f"    if (x === null) throw new Error(`${{x}} is not an object it is null`);\n"
             f"    if (typeof x !== 'object') throw new Error(`${{x}} is not an object it is a ${{typeof x}}`);\n"
             f"    if (Array.isArray(x)) throw new Error(`${{x}} is not an object it is an array`);\n"
             f"    for(const k in x){{\ntry{{\n"+
             f"        if (!x.hasOwnProperty(k)) continue;\n"+
             f"        const v=x[k];\n"
             f"        {indent(8,self.key_codec.get_typescript_asa(TypeScriptSourceCode('k'),namespace,back_refs))};\n"
             f"        {indent(8,self.value_codec.get_typescript_asa(TypeScriptSourceCode('v'),namespace,back_refs))};\n"
-            f"    }}catch(e){{\n"
+            f"    }}catch(e:any){{\n"
             f"        throw new Error(`element ${{k}} is invalid because ${{e}}`);\n"
             f"    }}}};\n"
             f"    return x as {tt};\n"
-            f"}}catch(e){{throw new Error(`${{x}} is not a {tt} because ${{e}}`);}}}})({expression})")
+            f"}}catch(e:any){{throw new Error(`${{x}} is not a {tt} because ${{e}}`);}}}})({expression})")
     pass
 
 class AnyDictCodec:
     def __init__(self):
         self.key_codec=NoopCodec[str](str)
         self.value_codec=AnyJsonCodec()
     def encode(self,x:dict,back_ref:None|Callable[[Any],JsonType])->dict:
@@ -576,41 +599,43 @@
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         return TypeScriptSourceCode(
             f"(((x:any):x is {self.typescript_type(back_refs)}=>(\n"
-            f"    (typeof (x) === 'object' &&\n"
+            f"    (x !== null &&\n"
+            f"    typeof (x) === 'object' &&\n"
             f"    !Array.isArray(x) &&\n"
             f"    (():boolean=>{{for (const k in x){{\n"
             f"        if (!x.hasOwnProperty(k)) continue;\n"
             f"        if (!({indent(12,self.key_codec.get_typescript_isa(TypeScriptSourceCode('k'),namespace,back_refs))} )||\n"
             f"            !({indent(12,self.value_codec.get_typescript_isa(TypeScriptSourceCode('x[k]'),namespace,back_refs))})) return false;}}\n"
             f"        return true;\n"
             f"    }})())))({expression}))")
     def get_typescript_asa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         tt=self.typescript_type(back_refs)
         return TypeScriptSourceCode(
             f"((x: any): {tt} => {{try{{\n"
+            f"    if (x === null) throw new Error(`${{x}} is not an object it is null`);\n"
             f"    if (typeof x !== 'object') throw new Error(`${{x}} is not an object it is a ${{typeof x}}`);\n"
             f"    if (Array.isArray(x)) throw new Error(`${{x}} is not an object it is an array`);\n"
             f"    for(const k in x){{\ntry{{\n"+
             f"        if (!x.hasOwnProperty(k)) continue;\n"+
             f"        const v=x[k];\n"
             f"        {indent(8,self.key_codec.get_typescript_asa(TypeScriptSourceCode('k'),namespace,back_refs))};\n"
             f"        {indent(8,self.value_codec.get_typescript_asa(TypeScriptSourceCode('v'),namespace,back_refs))};\n"
-            f"    }}catch(e){{\n"
+            f"    }}catch(e:any){{\n"
             f"        throw new Error(`element ${{k}} is invalid because ${{e}}`);\n"
             f"    }}}};\n"
             f"    return x as {tt};\n"
-            f"}}catch(e){{throw new Error(`${{x}} is not a {tt} because ${{e}}`);}}}})({expression})")
+            f"}}catch(e:any){{throw new Error(`${{x}} is not a {tt} because ${{e}}`);}}}})({expression})")
     pass
 
 class AnyJsonCodec:
     def encode(self,x,_:None|Callable[[Any],JsonType]):
         # we assume x will be subsequently json.dumps()ed so defer validation to that
         return x
     def decode(self,x,_:None|Callable[[JsonType],Any]):
@@ -652,23 +677,45 @@
             t=type(x)
             raise Exception(f'{x!r} (of type {t}) is not an int')
         return self.t(self.base_codec.decode(x,back_ref))
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
         if self.t.__module__=='__main__':
             return self.t.__name__
-        return f"{self.t.__module__}.f{self.t.__name__}"
+        return f"{self.t.__module__}.{self.t.__name__}"
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             'description': self.get_type_fqn(),
             'type': 'integer'
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         return 'number'
     def ensure_typescript_defs(self, namespace) -> None:
+        typescript_fqn=[TypeScriptUQN(_) for _ in self.get_type_fqn().split('.')]
+        target_namespace=namespace.get_namespace_of(typescript_fqn)
+        typescript_type_name=typescript_fqn[-1]
+        if typescript_type_name not in target_namespace.defs:
+            target_namespace.defs[typescript_type_name]=TypeScriptSourceCode(
+                f"type {typescript_type_name} = number;")
+            target_namespace.defs[TypeScriptUQN(f"asInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
+                f"function asInstanceOf{typescript_type_name}(v: any): {typescript_type_name}\n"
+                f"{{\n"
+                f"    try{{\n"
+                f"        if (typeof v !== 'number') throw new Error(`${{v}} is a ${{typeof v}}`);\n"
+                f"        return v;\n"
+                f"    }}\n"
+                f"    catch(e:any){{\n"
+                f"        throw new Error(`${{v}} is not a {typescript_type_name} because ${{e}}`);\n"
+                f"    }}\n"
+                f"}}")
+            target_namespace.defs[TypeScriptUQN(f'isInstanceOf{typescript_type_name}')]=TypeScriptSourceCode(
+                f"function isInstanceOf{typescript_type_name}(v:any): v is number\n"
+                f"{{\n"
+                f"    return typeof v === 'number';\n"
+                f"}}")
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         return TypeScriptSourceCode(
             f"(typeof ({expression}) == '{self.typescript_type(back_refs)}')")
@@ -698,23 +745,45 @@
             t=type(x)
             raise Exception(f'{x!r} (of type {t}) is not a float (or an int)')
         return self.t(self.base_codec.decode(x,back_ref))
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
         if self.t.__module__=='__main__':
             return self.t.__name__
-        return f"{self.t.__module__}.f{self.t.__name__}"
+        return f"{self.t.__module__}.{self.t.__name__}"
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             'description': self.get_type_fqn(),
             'type': 'number'
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         return 'number'
     def ensure_typescript_defs(self, namespace) -> None:
+        typescript_fqn=[TypeScriptUQN(_) for _ in self.get_type_fqn().split('.')]
+        target_namespace=namespace.get_namespace_of(typescript_fqn)
+        typescript_type_name=typescript_fqn[-1]
+        if typescript_type_name not in target_namespace.defs:
+            target_namespace.defs[typescript_type_name]=TypeScriptSourceCode(
+                f"type {typescript_type_name} = number;")
+            target_namespace.defs[TypeScriptUQN(f"asInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
+                f"function asInstanceOf{typescript_type_name}(v: any): {typescript_type_name}\n"
+                f"{{\n"
+                f"    try{{\n"
+                f"        if (typeof v !== 'number') throw new Error(`${{v}} is a ${{typeof v}}`);\n"
+                f"        return v;\n"
+                f"    }}\n"
+                f"    catch(e:any){{\n"
+                f"        throw new Error(`${{v}} is not a {typescript_type_name} because ${{e}}`);\n"
+                f"    }}\n"
+                f"}}")
+            target_namespace.defs[TypeScriptUQN(f'isInstanceOf{typescript_type_name}')]=TypeScriptSourceCode(
+                f"function isInstanceOf{typescript_type_name}(v:any): v is number\n"
+                f"{{\n"
+                f"    return typeof v === 'number';\n"
+                f"}}")
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         return TypeScriptSourceCode(
             f"(typeof ({expression}) == '{self.typescript_type(back_refs)}')")
@@ -744,23 +813,45 @@
             t=type(x)
             raise Exception(f'{x!r} (of type {t}) is not an str')
         return self.t(self.base_codec.decode(x,back_ref))
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
         if self.t.__module__=='__main__':
             return self.t.__name__
-        return f"{self.t.__module__}.f{self.t.__name__}"
+        return f"{self.t.__module__}.{self.t.__name__}"
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             'description': self.get_type_fqn(),
             'type': 'string'
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         return 'string'
     def ensure_typescript_defs(self, namespace) -> None:
+        typescript_fqn=[TypeScriptUQN(_) for _ in self.get_type_fqn().split('.')]
+        target_namespace=namespace.get_namespace_of(typescript_fqn)
+        typescript_type_name=typescript_fqn[-1]
+        if typescript_type_name not in target_namespace.defs:
+            target_namespace.defs[typescript_type_name]=TypeScriptSourceCode(
+                f"type {typescript_type_name} = string;")
+            target_namespace.defs[TypeScriptUQN(f"asInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
+                f"function asInstanceOf{typescript_type_name}(v: any): {typescript_type_name}\n"
+                f"{{\n"
+                f"    try{{\n"
+                f"        if (typeof v !== 'string') throw new Error(`${{v}} is a ${{typeof v}}`);\n"
+                f"        return v;\n"
+                f"    }}\n"
+                f"    catch(e:any){{\n"
+                f"        throw new Error(`${{v}} is not a {typescript_type_name} because ${{e}}`);\n"
+                f"    }}\n"
+                f"}}")
+            target_namespace.defs[TypeScriptUQN(f'isInstanceOf{typescript_type_name}')]=TypeScriptSourceCode(
+                f"function isInstanceOf{typescript_type_name}(v:any): v is string\n"
+                f"{{\n"
+                f"    return typeof v === 'string';\n"
+                f"}}")
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         return TypeScriptSourceCode(
             f"(typeof ({expression}) == '{self.typescript_type(back_refs)}')")
@@ -814,27 +905,154 @@
         return TypeScriptSourceCode(
             f"((v: any): {tt} => {{\n"
             f"    if (v !== {tt}) throw new Error(`the ${{typeof v}} ${{v}} is not the string {self.value}`);\n"
             f"    return v as {tt};\n"
             f"}})({expression})")
     pass
 
+class LiteralIntCodec:
+    value:int
+    def __init__(self,value:int):
+        self.value=value
+    def encode(self, x:int, _:None|Callable[[Any],JsonType])->int:
+        if type(x) is not int or x != self.value:
+            raise Exception(f'{x!r} is not {self.value!r}')
+        return x
+    def decode(self, x:JsonType,_:None|Callable[[JsonType],Any])->int:
+        if type(x) is not int:
+            raise Exception(f'{x!r} is not a int')
+        if x != self.value:
+            raise Exception(f'{x!r} is not {self.value!r}')
+        return x
+    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
+        return {
+            'type': 'number',
+            'enum': [ self.value ]
+        }
+    def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
+        return f'{self.value}'
+    def ensure_typescript_defs(self, namespace) -> None:
+        pass
+    def get_typescript_isa(self,
+                           expression:TypeScriptSourceCode,
+                           namespace: TypeScriptNamespace,
+                           back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        tt=self.typescript_type(back_refs)
+        return TypeScriptSourceCode(
+            f"((v:any): v is {tt}=>(v==={tt}))({expression})")
+    def get_typescript_asa(self,
+                           expression:TypeScriptSourceCode,
+                           namespace: TypeScriptNamespace,
+                           back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        tt=self.typescript_type(back_refs)
+        return TypeScriptSourceCode(
+            f"((v: any): {tt} => {{\n"
+            f"    if (v !== {tt}) throw new Error(`the ${{typeof v}} ${{v}} is not the number {self.value}`);\n"
+            f"    return v as {tt};\n"
+            f"}})({expression})")
+    pass
+
+class LiteralBoolCodec:
+    value:bool
+    def __init__(self,value:bool):
+        self.value=value
+    def encode(self, x:bool, _:None|Callable[[Any],JsonType])->bool:
+        if type(x) is not bool or x != self.value:
+            raise Exception(f'{x!r} is not {self.value!r}')
+        return x
+    def decode(self, x:JsonType,_:None|Callable[[JsonType],Any])->bool:
+        if type(x) is not bool:
+            raise Exception(f'{x!r} is not a boolean')
+        if x != self.value:
+            raise Exception(f'{x!r} is not {self.value!r}')
+        return x
+    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
+        return {
+            'type': 'boolean',
+            'enum': [ self.value ]
+        }
+    def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
+        return 'true' if self.value else 'false'
+    def ensure_typescript_defs(self, namespace) -> None:
+        pass
+    def get_typescript_isa(self,
+                           expression:TypeScriptSourceCode,
+                           namespace: TypeScriptNamespace,
+                           back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        tt=self.typescript_type(back_refs)
+        return TypeScriptSourceCode(
+            f"((v:any): v is {tt}=>(v==={tt}))({expression})")
+    def get_typescript_asa(self,
+                           expression:TypeScriptSourceCode,
+                           namespace: TypeScriptNamespace,
+                           back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        tt=self.typescript_type(back_refs)
+        typescript_value='true' if self.value else 'false'
+        return TypeScriptSourceCode(
+            f"((v: any): {tt} => {{\n"
+            f"    if (v !== {tt}) throw new Error(`the ${{typeof v}} ${{v}} is not {self.typescript_type(None)}`);\n"
+            f"    return v as {tt};\n"
+            f"}})({expression})")
+    pass
+
+@runtime_checkable
+class CustomClassCodec(Protocol):
+    '''implement these methods on class T to use custom encoding of instances of T'''
+    @staticmethod
+    def xju_json_codec_encode(
+            x:object  # x is a T
+    ) -> JsonType:
+        assert False  #pragma NO COVER
+        pass
+    @staticmethod
+    def xju_json_codec_decode(x:JsonType) -> object:  # must return a T
+        assert False  #pragma NO COVER
+        pass
+    @staticmethod
+    def xju_json_codec_get_json_schema(definitions:dict[str,dict]) -> dict:
+        '''return json schema for T
+           - may add any supporting definitions to definitions'''
+        assert False  #pragma NO COVER
+        return {}
+    @staticmethod
+    def xju_json_codec_get_typescript_isa(
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace) -> TypeScriptSourceCode:
+        '''return typescript source code that turns {expression} into a bool indicating whether the expression is a T
+           - may add any supporting definitions to namespace, e.g. type for T itself'''
+        assert False  #pragma NO COVER
+        return TypeScriptSourceCode('')
+    @staticmethod
+    def xju_json_codec_get_typescript_asa(
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace) -> TypeScriptSourceCode:
+        '''return typescript source code that safely casts {expression} to a T, throwing an Error if {expression} is not valid as a T
+           - may add any supporting definitions to namespace, e.g. type for T itself'''
+        assert False  #pragma NO COVER
+        return TypeScriptSourceCode('')
+    pass
+
 class ClassCodec:
     t:type
     attr_codecs:dict[str,Any]  # codec
+    custom_codec:CustomClassCodec|None = None
     def __init__(self, t:type, attr_codecs:dict[str,Any]):
         self.t=t
         self.attr_codecs=attr_codecs
+        if issubclass(t,CustomClassCodec):
+            self.custom_codec=t
         pass
-    def encode(self,x,_:None|Callable[[Any],JsonType]) -> dict:
+    def encode(self,x,_:None|Callable[[Any],JsonType]) -> JsonType:
         'encode {x} as a {self.t}'
         try:
             if type(x) is not self.t:
                 xt=type(x)
                 raise Exception(f'{x!r} (of type {xt}) is not a {self.t}')
+            if self.custom_codec is not None:
+                return self.custom_codec.xju_json_codec_encode(x)
             def back_ref(x:Any) -> JsonType:
                 return self.encode(x,None)
             result={}
             for n, attr_codec in self.attr_codecs.items():
                 try:
                     result[n]=attr_codec.encode(getattr(x,n),back_ref)
                 except Exception:
@@ -843,14 +1061,18 @@
             return result
         except Exception:
             raise in_function_context(ClassCodec.encode,vars()) from None
         pass
     def decode(self,x,_:None|Callable[[JsonType],Any]) -> object:
         'deocde {x} as a {self.t}'
         try:
+            if self.custom_codec is not None:
+                result=self.custom_codec.xju_json_codec_decode(x)
+                assert isinstance(result,self.t), (repr(result),self.t)
+                return result
             def back_ref(x:JsonType) -> object:
                 return self.decode(x,None)
             attr_values={}
             for n, attr_codec in self.attr_codecs.items():
                 if n in x:
                     try:
                         value=attr_codec.decode(x[n],back_ref)
@@ -869,14 +1091,16 @@
         pass
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
         if self.t.__module__ == "__main__":
             return self.t.__name__
         return f'{self.t.__module__}.{self.t.__name__}'
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
+        if self.custom_codec is not None:
+            return self.custom_codec.xju_json_codec_get_json_schema(definitions)
         fqn=self.get_type_fqn()
         self_ref=f'#/definitions/{fqn}'
         if not fqn in definitions:
             definitions[fqn]={
                 'description': self.t.__name__,
                 'type': 'object',
                 'properties': {
@@ -910,54 +1134,60 @@
                          for attr_name, attr_codec in self.attr_codecs.items()])+
                 f"}};")
             target_namespace.defs[TypeScriptUQN(f"asInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
                 f"function asInstanceOf{typescript_type_name}(v: any): {tt}\n"
                 f"{{\n"
                 f"    try{{\n"
                 f"        if (Array.isArray(v)) throw new Error(`${{v}} is an array`);\n"
+                f"        if (v == null) throw new Error(`${{v}} is not an object it is null`);\n"
                 f"        if (typeof v !== 'object') throw new Error(`${{v}} is not an object it is a ${{typeof v}}`);\n"
-                f"        const attr_asa=function(name:string, asa):any{{\n"
+                f"        const attr_asa=function(name:string, asa:any):any{{\n"
                 f"            try{{\n"
                 f"                asa(v[name]);\n"
                 f"            }}\n"
-                f"            catch(e){{\n"
+                f"            catch(e:any){{\n"
                 f"                throw new Error(`attribute ${{name}} is invalid because ${{e}}`);\n"
                 f"            }}\n"
                 f"        }}\n" +
-                ''.join([f"        attr_asa('{attr_name}',(x)=>{indent(8,attr_codec.get_typescript_asa('x',namespace,back_refs))});\n"
+                ''.join([f"        attr_asa('{attr_name}',(x:any)=>{indent(8,attr_codec.get_typescript_asa('x',namespace,back_refs))});\n"
                          for attr_name, attr_codec in self.attr_codecs.items()])+
                 f"        return v as {tt};\n"
                 f"    }}\n"
-                f"    catch(e){{\n"
+                f"    catch(e:any){{\n"
                 f"        throw new Error(`${{v}} is not a {tt} because ${{e}}`);\n"
                 f"    }}\n"
                 f"}}")
             target_namespace.defs[TypeScriptUQN(f"isInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
                 f"function isInstanceOf{typescript_type_name}(v:any): v is {tt}\n"
                 f"{{\n"
                 f"    return (\n"
-                f"        Array.isArray(v) &&\n"
+                f"        !Array.isArray(v) &&\n"
+                f"        v !== null &&"+
                 f"        typeof v === 'object'"+
-                ''.join([f" &&\n        {indent(8,attr_codec.get_typescript_isa('v[{attr_name}]',namespace,back_refs))}"
+                ''.join([" &&\n        "+indent(8,attr_codec.get_typescript_isa(f'v["{attr_name}"]',namespace,back_refs))
                          for attr_name, attr_codec in self.attr_codecs.items()])+")"
                 f"}}")
             pass
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        if self.custom_codec is not None:
+            return self.custom_codec.xju_json_codec_get_typescript_isa(expression,namespace)
         self.ensure_typescript_defs(namespace)
         fqn=self.get_type_fqn().split('.')
         return TypeScriptSourceCode('.'.join(fqn[0:-1]+[f"isInstanceOf{fqn[-1]}({expression})"]))
 
     def get_typescript_asa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        if self.custom_codec is not None:
+            return self.custom_codec.xju_json_codec_get_typescript_asa(expression,namespace)
         self.ensure_typescript_defs(namespace)
         fqn=self.get_type_fqn().split('.')
         fqn=self.get_type_fqn().split('.')
         return TypeScriptSourceCode('.'.join(fqn[0:-1]+[f"asInstanceOf{fqn[-1]}({expression})"]))
     pass
 
 class SelfCodec:
@@ -1000,57 +1230,89 @@
             expression:TypeScriptSourceCode,
             namespace: TypeScriptNamespace,
             back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         assert back_refs is not None
         return back_refs.asa_back_ref(expression)
     pass
     
-def _explodeSchema(t:type):
-    '''explode type {t!r} into a tree of codecs'''
+def _explodeSchema(t:type|NewType|TypeVar|GenericAlias|UnionType|_LiteralGenericAlias|_GenericAlias,
+                   type_var_map:dict[TypeVar,Any]|None):
+    '''explode type {t!r} into a tree of codecs using map {type_var_map} to resolve any generic type refs i.e. TypeVars'''
     try:
-        if t is float:
+        if type(t) is TypeVar:
+            assert type_var_map is not None
+            assert t in type_var_map, type_var_map.keys()
+            return _explodeSchema(type_var_map[t],type_var_map)
+        if t is float or (isinstance(t,NewType) and t.__supertype__ is float):
             return NoopCodec[float](float)
-        if t is int:
+        if t is int or (isinstance(t,NewType) and t.__supertype__ is int):
             return NoopCodec[int](int)
-        if t is str:
+        if t is str or (isinstance(t,NewType) and t.__supertype__ is str):
             return NoopCodec[str](str)
-        if t is bool:
+        if t is bool or (isinstance(t,NewType) and t.__supertype__ is bool):
             return NoopCodec[bool](bool)
         if t is None or t is NoneType:
             return NoneCodec()
         if t is list:
             return AnyListCodec()
-        if type(t) is GenericAlias and getattr(t, '__origin__') is list:
-            return ListCodec(_explodeSchema(getattr(t,'__args__')[0]))
+        if type(t) is GenericAlias and get_origin(t) is list:
+            return ListCodec(_explodeSchema(get_args(t)[0],type_var_map))
+        if type(t) is _LiteralGenericAlias and len(t.__args__)==1:
+            return _explode_literal(t.__args__[0])
         if type(t) is _LiteralGenericAlias:
-            value = t.__args__[0]
-            if not isinstance(value,str):
-                raise Exception(f'{t!r} literal type is not supported (only string is implemented)')
-            return LiteralStrCodec(value)
-        if type(t) is GenericAlias and getattr(t, '__origin__') is tuple:
-            return TupleCodec([_explodeSchema(_) for _ in getattr(t,'__args__')])
+            return UnionCodec(get_args(t),
+                              {t:_explode_literal(t) for t in get_args(t)})
+        if type(t) is GenericAlias and get_origin(t) is tuple:
+            return TupleCodec([_explodeSchema(_,type_var_map) for _ in get_args(t)])
         if t is dict:
             return AnyDictCodec()
-        if type(t) is GenericAlias and getattr(t, '__origin__') is dict:
-            return DictCodec(*[_explodeSchema(_) for _ in getattr(t,'__args__')])
+        if type(t) is GenericAlias and get_origin(t) is dict:
+            return DictCodec(*[_explodeSchema(_, type_var_map) for _ in get_args(t)])
         if type(t) is UnionType:
-            return UnionCodec(getattr(t,'__args__'))
+            return UnionCodec(get_args(t),
+                              {t:_explodeSchema(t, type_var_map) for t in get_args(t)})
         if type(t) is _UnionGenericAlias:
-            return UnionCodec(getattr(t,'__args__'))
+            return UnionCodec(get_args(t),
+                              {t:_explodeSchema(t, type_var_map) for t in get_args(t)})
         if t is Self:
             return SelfCodec()
+        if type(t) is _GenericAlias:
+            local_type_var_map={
+                type_var: value
+                for type_var, value in
+                list((type_var_map or {}).items())+list(zip(get_origin(t).__parameters__, get_args(t)))
+            }
+            return ClassCodec(
+                get_origin(t),
+                { n: _explodeSchema(nt,local_type_var_map)
+                  for n,nt in get_type_hints(get_origin(t)).items()})
+        assert isinstance(t,type), t
         if issubclass(t,xju.newtype.Int):
             return NewIntCodec(t)
         if issubclass(t,xju.newtype.Float):
             return NewFloatCodec(t)
         if issubclass(t,xju.newtype.Str):
             return NewStrCodec(t)
         return ClassCodec(
-            t,{n: _explodeSchema(nt) for n,nt in get_type_hints(t).items()})
+            t,{n: _explodeSchema(nt,type_var_map) for n,nt in get_type_hints(t).items()})
     except Exception:
         raise in_function_context(_explodeSchema,vars()) from None
     pass
 
+def _explode_literal(value: Any):
+    '''create codec for literal value {value!r}'''
+    try:
+        if type(value) is str:
+            return LiteralStrCodec(value)
+        if type(value) is bool:
+            return LiteralBoolCodec(value)
+        if type(value) is int:
+            return LiteralIntCodec(value)
+        t=type(value)
+        raise Exception(f'{t} literals are not supported (only support str, int, bool)')
+    except:
+        raise in_function_context(_explode_literal, vars())
+    pass
 
 def indent(n: int, s:TypeScriptSourceCode)->str:
     lines=s.splitlines()
     return '\n'.join([lines[0].value()]+[(' '*n)+l.value() for l in lines[1:]])
```

### Comparing `xju-1.2.9/src/xju/json_codec.py.test` & `xju-1.3.0/src/xju/json_codec.py.test`

 * *Files 24% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 from sys import path
+import ipaddress
 from os.path import dirname
 if path[0]==dirname(__file__): path.pop(0)
 
 from xju.json_codec import codec, Codec, JsonType, AnyJsonCodec, SelfCodec
+from xju.json_codec import TypeScriptSourceCode, TypeScriptNamespace, CustomClassCodec
 
-from typing import cast, Type, Literal, Any, Self
+from typing import cast, Type, Literal, Any, Self, NewType, Generic, TypeVar
 from types import NoneType
 from dataclasses import dataclass, field
 import re
 import sys
+import ipaddress
 
 from xju.assert_ import Assert
 import xju.newtype
 from xju.xn import readable_repr
+from xju.time import Timestamp
 
 x:Any
 
 
 # int,str,bool,float,None map directly
 
 Assert(codec(int).decode(3))==3
@@ -44,15 +48,31 @@
 
 Assert(codec(int).encode(3))==3
 Assert(codec(str).encode('fred'))=='fred'
 Assert(codec(bool).encode(True))==True
 Assert(codec(float).encode(5.5))==5.5
 Assert(codec(float).encode(5))==5
 
-# note None is a bit weird, sometimes it acts as as a type, others not
+# and can use typing.NewType of int,str,bool,float
+Colour = NewType('Colour',str)
+Assert(codec(Colour).decode('red'))==Colour('red')
+Assert(codec(Colour).encode(Colour('red')))=='red'
+Milligrams = NewType('Milligrams',float)
+Assert(codec(Milligrams).decode(7.6))==Milligrams(7.6)
+Assert(codec(Milligrams).encode(Milligrams(7.6)))==7.6
+Votes = NewType('Votes',int)
+Assert(codec(Votes).decode(7))==Votes(7)
+Assert(codec(Votes).encode(Votes(7)))==7
+Enabled = NewType('Enabled',bool)
+Assert(codec(Enabled).decode(True))==Enabled(True)
+Assert(codec(Enabled).decode(False))==Enabled(False)
+Assert(codec(Enabled).encode(Enabled(True)))==True
+Assert(codec(Enabled).encode(Enabled(False)))==False
+
+# note None is a not a type, it's type can only be got via type(None)
 Assert(codec(type(None)).decode(None))==None
 Assert(codec(type(None)).encode(None))==None
 
 
 # list maps to list...
 Assert(codec(list).decode([5, 'fred']))==[5, 'fred']
 Assert(codec(list).encode([5, 'fred']))==[5, 'fred']
@@ -145,18 +165,25 @@
     pass
 
 
 # dict with no type hints allows any keys with any value types (key must be string)
 Assert(codec(dict).decode({'fred':5, 'jock': 'nine'}))=={'fred':5, 'jock':'nine'}
 Assert(codec(dict).encode({'fred':5, 'jock': 'nine'}))=={'fred':5, 'jock':'nine'}
 
-# dict with specific value type...
+# dict with specific value type, keys can be str...
 Assert(codec(dict[str,int]).decode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
 Assert(codec(dict[str,int]).encode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
 
+#... or xju.newtype.Str or anything that with str encoding
+class SurnameTag:pass
+class Surname(xju.newtype.Str[SurnameTag]):pass
+
+Assert(codec(dict[Surname,int]).encode({Surname('fred'):5, Surname('jock'): 9}))=={'fred':5, 'jock':9}
+Assert(codec(dict[Surname,int]).decode({'fred':5, 'jock':9}))=={Surname('fred'):5, Surname('jock'): 9}
+
 # ... must be given a dict...
 try:
     x=codec(dict).decode(7)
 except Exception as e:
     Assert("7 is not a dict").isIn(str(e))
 else:
     assert False, x
@@ -174,15 +201,15 @@
     x=codec(dict[str,int]).decode({'jock': 'fred'})
 except Exception as e:
     Assert("'fred' (of type <class 'str'>) is not a <class 'int'>").isIn(str(e))
 else:
     assert False, x
     pass
 
-# dict keys must be strings...
+# dict keys must be strings or xju.newtype.Str...
 try:
     x=codec(dict).encode({6: 'fred'})
 except Exception as e:
     Assert(str(e)).matches("6 is not a <class 'str'>")
 else:
     assert False, x
     pass
@@ -255,17 +282,14 @@
 except Exception as e:
     Assert("'fred' is not a <class '__main__.Metres'>").isIn(str(e))
 else:
     assert False, x
     pass
 
 #xju.newtype.Str support
-class SurnameTag:pass
-class Surname(xju.newtype.Str[SurnameTag]):pass
-
 Assert(codec(Surname).decode('Ang'))==Surname('Ang')
 Assert(codec(Surname).encode(Surname('Ang')))=='Ang'
 
 try:
     x=codec(Surname).decode(17)
 except Exception as e:
     Assert("17 (of type <class 'int'>) is not an str").isIn(str(e))
@@ -301,32 +325,35 @@
     Assert(str(e)).matches("failed to decode 5.7 to a str | int because.*failed to decode as <class 'str'> because 5.7 (of type <class 'float'>) is not a <class 'str'> and failed to decode as <class 'int'> because 5.7 (of type <class 'float'>) is not a <class 'int'>")
 else:
     assert False, x
     pass
 
 
 # class (object) support:
-#   encoding is dictionary containing each objct attribute (except that string literal
-#   attributes are treated specially, see string literal attributes below)
+#   - encoding is dictionary containing each object attribute (except that string literal
+#     attributes are treated specially, see string literal attributes below)
+#   - when decoding, class is always initialised via keyword args (note that
+#     dataclass generates __init__ function that supports keyword args)
+#   - class may implement CustomClassCodec protocol for custom encodings, see
+#     IpAddr below
+@dataclass
+class Address:
+    street:'Street'
+    suburb:'Suburb'
+    postcode:'Postcode'
+
 class StreetTag:pass
 class Street(xju.newtype.Str[StreetTag]):pass
 
 class SuburbTag:pass
 class Suburb(xju.newtype.Str[SuburbTag]):pass
 
 class PostcodeTag:pass
 class Postcode(xju.newtype.Int[PostcodeTag]):pass
 
-@dataclass
-class Address:
-    street:Street
-    suburb:Suburb
-    postcode:Postcode
-
-
 Assert(codec(Address).decode({
     'street':'alba',
     'suburb': 'bocca',
     'postcode': 3365}))==Address(Street('alba'),Suburb('bocca'),Postcode(3365))
         
 Assert(codec(Address).encode(Address(Street('alba'),Suburb('bocca'),Postcode(3365))))=={
     'street':'alba',
@@ -370,30 +397,23 @@
     b: int
 
 # class inheritance...
 @dataclass
 class UnitAddress(Address,ManagerName):
     unit:Unit
 
-# ... __init__ argument order is assumed to be that used by dataclass, i.e. classes in
-# reverse-mro (see python mro() and __mro__) with attributes of each class in usual order, so
-# order of UnitAddress __init__ args is
-# ManagerName attrs in order (i.e. a, b) then Address attrs in order (i.e. street, suburb, postcode)
-# then UnitAddress attributes in order (i.e. unit), so in total:
-# a, b, street, suburb, postcode.
-# Decode does not care about json dict order...
 Assert(codec(UnitAddress).decode({
     'street':'alba',
     'suburb': 'bocca',
     'postcode': 3365,
     'unit': '17a',
     'a': 'fred',
     'b': 17}))==UnitAddress('fred',17,Street('alba'),Suburb('bocca'),Postcode(3365),Unit('17a'))
 
-# ... encode will order attrs per description above
+# ... encode will order attrs per python mro()
 Assert(codec(UnitAddress).encode(
     UnitAddress('fred',17,Street('alba'),Suburb('bocca'),Postcode(3365),unit=Unit('17a'))))=={
         'a': 'fred',
         'b': 17,
         'street':'alba',
         'suburb': 'bocca',
         'postcode': 3365,
@@ -402,72 +422,236 @@
     UnitAddress('fred',17,Street('alba'),Suburb('bocca'),Postcode(3365),unit=Unit('17a')))).keys()))==[
         'a',
         'b',
         'street',
         'suburb',
         'postcode',
         'unit']
-        
 
-# string Literal
+# custom class encoding by implementing CustomClassCodec protocol, for example
+# to support encoding of external types with control over their json representation
+class IpV4Addr(ipaddress.IPv4Address):
+    __xju_json_codec=codec(str)
+
+    @staticmethod
+    def xju_json_codec_encode(x:object) -> JsonType:
+        assert isinstance(x,IpV4Addr)
+        return IpV4Addr.__xju_json_codec.encode(x.exploded)
+    @staticmethod
+    def xju_json_codec_decode(x:JsonType) -> object:
+        return IpV4Addr(IpV4Addr.__xju_json_codec.decode(x))
+    @staticmethod
+    def xju_json_codec_get_json_schema(definitions:dict[str,dict]) -> dict:
+        '''return json schema for T'''
+        '''- may add any supporting definitions to definitions'''
+        return IpV4Addr.__xju_json_codec.get_json_schema()
+    @staticmethod
+    def xju_json_codec_get_typescript_isa(
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace) -> TypeScriptSourceCode:
+        '''return typescript source code that turns {expression} into a bool indicating whether the expression is a T'''
+        '''- may add any supporting definitions to namespace, e.g. type for T itself'''
+        return IpV4Addr.__xju_json_codec.get_typescript_isa(expression,namespace)
+
+    @staticmethod
+    def xju_json_codec_get_typescript_asa(
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace) -> TypeScriptSourceCode:
+        '''return typescript source code that safely casts {expression} to a T, throwing an Error if {expression} is not valid as a T'''
+        '''- may add any supporting definitions to namespace, e.g. type for T itself'''
+        return IpV4Addr.__xju_json_codec.get_typescript_asa(expression,namespace)
+    pass
+
+Assert(IpV4Addr).isSubclassOf(CustomClassCodec)
+Assert(codec(IpV4Addr).encode(IpV4Addr('172.18.12.1')))=='172.18.12.1'
+Assert(codec(IpV4Addr).decode('172.18.12.1')).isInstanceOf(IpV4Addr)
+Assert(codec(IpV4Addr).decode('172.18.12.1'))==IpV4Addr('172.18.12.1')
+
+
+# REVISIT: adjust IpAddrWithPrefix to generate a typescript alias
+@dataclass
+class IpAddrWithPrefix(ipaddress.IPv4Interface):
+    """An IP host address in a network, e.g. 10.1.1.49/24"""
+    if_str: str
+    __codec=codec(str)
+    def __post_init__(self):
+        super().__init__(self.if_str)
+    @staticmethod
+    def xju_json_codec_decode(x:JsonType) -> object:
+        return IpAddrWithPrefix(IpAddrWithPrefix.__codec.decode(x))
+    @staticmethod
+    def xju_json_codec_encode(x:object) -> JsonType:
+        assert isinstance(x,IpAddrWithPrefix)
+        return IpAddrWithPrefix.__codec.encode(x.if_str)
+    @staticmethod
+    def xju_json_codec_get_json_schema(definitions:dict[str,dict]) -> dict:
+        '''return json schema for T'''
+        '''- may add any supporting definitions to definitions'''
+        return IpAddrWithPrefix.__codec.get_json_schema()
+    @staticmethod
+    def xju_json_codec_get_typescript_isa(
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace) -> TypeScriptSourceCode:
+        '''return typescript source code that turns {expression} into a bool indicating whether the expression is a T'''
+        '''- may add any supporting definitions to namespace, e.g. type for T itself'''
+        return IpAddrWithPrefix.__codec.get_typescript_isa(expression,namespace)
+
+    @staticmethod
+    def xju_json_codec_get_typescript_asa(
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace) -> TypeScriptSourceCode:
+        '''return typescript source code that safely casts {expression} to a T, throwing an Error if {expression} is not valid as a T'''
+        '''- may add any supporting definitions to namespace, e.g. type for T itself'''
+        return IpAddrWithPrefix.__codec.get_typescript_asa(expression,namespace)
+
+@dataclass
+class Router:
+    name: str
+    ifv4: IpAddrWithPrefix
+
+Assert(codec(Router).decode({'name':'fred','ifv4':'10.1.7.44/22'}))==Router(name='fred',ifv4=IpAddrWithPrefix('10.1.7.44/22'))
+Assert(codec(Router).decode({'name':'fred','ifv4':'10.1.7.44/22'}).ifv4.network)==ipaddress.IPv4Network("10.1.4.0/22")
+Assert(codec(Router).encode(Router(name='fred',ifv4=IpAddrWithPrefix('10.1.7.44/22'))))=={'name':'fred','ifv4':'10.1.7.44/22'}
+
+
+# string/int/bool literals
 #mypy 1.0.0 bug:
-#Codec[Literal['fred']](Literal['fred'])
+#codec(Literal['fred'])
 # ... says:
 #  error: Argument 1 to "Codec" has incompatible type "object"; expected "Type[Literal['fred']]"  [arg-type]
 
 Assert(codec(Literal['fred']).decode('fred'))=='fred' # type: ignore
 Assert(codec(Literal['fred']).encode('fred'))=='fred' # type: ignore
 
-#non-string literal not yet implemented
+Assert(codec(Literal['fred','jock']).decode('fred'))=='fred' # type: ignore
+Assert(codec(Literal['fred','jock']).decode('jock'))=='jock' # type: ignore
+Assert(codec(Literal['fred','jock']).encode('fred'))=='fred' # type: ignore
+Assert(codec(Literal['fred','jock']).encode('jock'))=='jock' # type: ignore
+
+Assert(codec(Literal[7]).decode(7))==7 # type: ignore
+Assert(codec(Literal[7]).encode(7))==7 # type: ignore
+
+Assert(codec(Literal[7,8]).decode(7))==7 # type: ignore
+Assert(codec(Literal[7,8]).decode(8))==8 # type: ignore
+Assert(codec(Literal[7,8]).encode(7))==7 # type: ignore
+Assert(codec(Literal[7,8]).encode(8))==8 # type: ignore
+
+Assert(codec(Literal[True]).decode(True))==True # type: ignore
+Assert(codec(Literal[False]).encode(False))==False # type: ignore
+
+Assert(codec(Literal[True,False]).decode(True))==True # type: ignore
+Assert(codec(Literal[True,False]).decode(False))==False # type: ignore
+Assert(codec(Literal[True,False]).encode(True))==True # type: ignore
+Assert(codec(Literal[True,False]).encode(False))==False # type: ignore
+
+
+Assert(codec(Literal[6,'jock']).decode(6))==6 # type: ignore
+Assert(codec(Literal[6,'jock']).decode('jock'))=='jock' # type: ignore
+Assert(codec(Literal[6,'jock']).encode(6))==6 # type: ignore
+Assert(codec(Literal[6,'jock']).encode('jock'))=='jock' # type: ignore
+
+
+#float literal not yet implemented
 try:
-    x=codec(Literal[7]).decode(7) # type: ignore
+    x=codec(Literal[7.6]).decode(7.6) # type: ignore
 except Exception as e:
-    Assert("typing.Literal[7] literal type is not supported (only string is implemented)").isIn(str(e))
+    Assert("failed to create codec for literal value 7.6 because\n<class 'float'> literals are not supported (only support str, int, bool)").isIn(readable_repr(e))
 else:
     assert False, x
     pass
 
 
 #encode wrong type
 try:
-    x=codec(Literal['fred']).encode(7) # type: ignore
+    x=codec(Literal['fred','jock']).encode(7) # type: ignore
 except Exception as e:
     Assert("7 is not 'fred'").isIn(str(e))
 else:
     assert False, x
     pass
+try:
+    x=codec(Literal[7,8]).encode(True) # type: ignore
+except Exception as e:
+    Assert("True is not 7").isIn(str(e))
+else:
+    assert False, x
+    pass
+try:
+    x=codec(Literal[False,True]).encode('fred') # type: ignore
+except Exception as e:
+    Assert("'fred' is not False").isIn(str(e))
+else:
+    assert False, x
+    pass
 #decode wrong type
 try:
     x=codec(Literal['fred']).decode(7) # type: ignore
 except Exception as e:
     Assert("7 is not a string").isIn(str(e))
 else:
     assert False, x
     pass
+try:
+    x=codec(Literal[7]).decode('fred') # type: ignore
+except Exception as e:
+    Assert("'fred' is not a int").isIn(str(e))
+else:
+    assert False, x
+    pass
+try:
+    x=codec(Literal[False]).decode(7) # type: ignore
+except Exception as e:
+    Assert("7 is not a boolean").isIn(str(e))
+else:
+    assert False, x
+    pass
 
-# string literal attributes match that string literal...
+# decode wrong value
+try:
+    x=codec(Literal['fred','ann']).decode('jock') # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to decode jock to a typing.Literal['fred', 'ann'] because\nfailed to decode 'jock' as one of ('fred', 'ann') because\nfailed to decode as 'fred' because 'jock' is not 'fred' and failed to decode as 'ann' because 'jock' is not 'ann'."
+else:
+    assert False, x
+    pass
+try:
+    x=codec(Literal[6,7]).decode(8) # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to decode 8 to a typing.Literal[6, 7] because\nfailed to decode 8 as one of (6, 7) because\nfailed to decode as 6 because 8 is not 6 and failed to decode as 7 because 8 is not 7."
+else:
+    assert False, x
+    pass
+try:
+    x=codec(Literal[False]).decode(True) # type: ignore
+except Exception as e:
+    Assert("True is not False").isIn(str(e))
+else:
+    assert False, x
+    pass
+
+# literal attributes match that string literal...
 @dataclass
 class Add:
     a:int
     b:int
-    op_type: Literal['add'] = 'add'  # note default value not required but recommended, see below
+    op_type: Literal['add'] # = 'add' not recommended - see Caution below
 
 Assert(codec(Add).decode(
     {
         'op_type':'add',
         'a': 7,
         'b': 8
-    }))==Add(7,8)
+    }))==Add(7,8,op_type='add')
         
 Assert(codec(Add).decode({
     'op_type':'add',
     'a': 7,
     'b': 8}).op_type)=='add'
         
-Assert(codec(Add).encode(Add(7,8))=={
+Assert(codec(Add).encode(Add(7,8,op_type='add'))=={
     'op_type':'add',
     'a': 7,
     'b': 8})
         
 # ... and rejected other values...
 try:
     x=codec(Add).decode({
@@ -478,26 +662,14 @@
     Assert(str(e)).contains("'subtract' is not 'add'")
 else:
     assert False, x
     pass
 
 # ... allowing them to be used as type descriminators...
 @dataclass
-class Sub:
-    a:int
-    b:int
-    op_type: Literal['sub'] = 'sub'
-
-Assert(codec(Add|Sub).decode({  # type: ignore
-    'op_type':'sub',
-    'a': 7,
-    'b': 8}))==Sub(7,8)
-
-# ... without defaults, string literal attributes still work...
-@dataclass
 class MissingDefault:
     op_type: Literal['op']
     sub_type: Literal['plus']
     a:int
     b:int
     pass
 
@@ -505,14 +677,29 @@
     'op_type':'op',
     'sub_type':'plus',
     'a': 7,
     'b': 8}))==MissingDefault('op', 'plus', 7, 8)
 
 # ... but always need to be passed literal value.
 
+# Caution, giving the literal attribute a default seems
+# like a useful shortcut since we know exactly what value
+# to give it:
+@dataclass
+class Sub:
+    a:int
+    b:int
+    op_type: Literal['sub'] = 'sub'
+
+# ... but that will also match json with no op_type:
+Assert(codec(Add|Sub).decode({  # type: ignore
+    'a': 7,
+    'b': 8}))==Sub(7,8)
+
+
 
 # misc coverage
 Assert(repr(codec(int)))=="<class 'int'> json codec"
 
 
 Assert(codec(int|None).decode(None))==None # type: ignore
 Assert(codec(int|None).encode(None))==None # type: ignore
@@ -560,23 +747,26 @@
 Assert(codec(AgeInYears).get_json_schema())=={'description': 'AgeInYears', 'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Street).get_json_schema())=={'description': 'Street', 'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Metres).get_json_schema())=={'description': 'Metres', 'type': 'number', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Literal['fred']).get_json_schema())=={'type': 'string', 'enum': ['fred'], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
+Assert(codec(Literal[7]).get_json_schema())=={'type': 'number', 'enum': [7], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
+Assert(codec(Literal[False]).get_json_schema())=={'type': 'boolean', 'enum': [False], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
 
 Assert(codec(Address).get_json_schema())=={
     '$ref': '#/definitions/Address',
     '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema',
     'definitions':{
         'Address':{
             'description': 'Address',
             'type': 'object',
             'properties': {'street': {'description': 'Street', 'type': 'string'}, 'suburb': {'description': 'Suburb', 'type': 'string'}, 'postcode': {'description': 'Postcode', 'type': 'integer'}}}}}
+Assert(codec(IpV4Addr).get_json_schema())=={'type': 'string', '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema', 'definitions': {}}
 
 
 
 # recursive via Self
 class LeafTag:pass
 class Leaf(xju.newtype.Int[LeafTag]):pass
 
@@ -800,21 +990,141 @@
     pass
 
 Assert(codec(Person).decode({'first_name':'fred','last_name':'jones'}))==Person(first_name='fred',last_name='jones')
 Assert(codec(Person).decode({'first_name':'fred','phobias':['spiders'],'last_name':'jones'}))==Person(first_name='fred',last_name='jones',phobias=['spiders'])
 Assert(codec(Person).decode({'first_name':'fred','middle_names':['arachnid'],'last_name':'jones'}))==Person(first_name='fred',last_name='jones',middle_names=['arachnid'])
 
 
-# not-present optional attribute must still appear in json (with value null)
+# non-defaulted "optional" attribute (of type X|None) must still appear in json (with value null)
 @dataclass
 class Opt:
     x: str|None
     pass
 
 Assert(codec(Opt).decode({'x':None}))==Opt(x=None)
 try:
     codec(Opt).decode({})
 except Exception as e:
     Assert(readable_repr(e)).contains("Failed to decode {} to a <class '__main__.Opt'> because\nfailed to deocde {} as a <class '__main__.Opt'> because\nfailed to init <class '__main__.Opt'> with keyword arguments {} because\nOpt.__init__() missing 1 required positional argument: 'x'.")
 else:
     assert False
     pass
+
+
+# specialisation based on descriminator
+@dataclass
+class Court:
+    width:Metres
+    length:Metres
+    game:str
+    pass
+
+@dataclass
+class NetballCourt(Court):
+    game:Literal['netball'] = 'netball'
+    pass
+
+@dataclass
+class BasketballCourt(Court):
+    game:Literal['basketball'] = 'basketball'
+    pass
+
+court_codec=codec(NetballCourt|BasketballCourt|Court) # type: ignore  # mypy 1.2.0 bug
+Assert(court_codec.decode({'game':'netball', 'width':8, 'length': 10})).isInstanceOf(NetballCourt)
+Assert(court_codec.decode({'game':'basketball', 'width':8, 'length': 10})).isInstanceOf(BasketballCourt)
+Assert(court_codec.decode({'game':'badminton', 'width':8, 'length': 10})).isInstanceOf(Court)
+Assert(court_codec.encode(NetballCourt(width=Metres(8),length=Metres(10)))=={'game':'netball', 'width':8, 'length': 10})
+Assert(court_codec.encode(BasketballCourt(width=Metres(8),length=Metres(10)))=={'game':'basketball', 'width':8, 'length': 10})
+Assert(court_codec.encode(Court(game='badminton',width=Metres(8),length=Metres(10)))=={'game':'badminton', 'width':8, 'length': 10})
+
+
+# generic class codecs are supported, for example a messages might
+# carry generic payloads:
+
+@dataclass
+class Msg:
+    msg_type: str
+    pass
+
+Payload=TypeVar('Payload')
+
+@dataclass
+class SetMsg(Generic[Payload],Msg):
+    msg_type: Literal['set_new_value']
+    new_value: Payload
+    pass
+
+SetSurnameMsg=SetMsg[Surname]
+
+Assert(codec(SetSurnameMsg).decode({'msg_type':'set_new_value','new_value':'knox'}))==SetSurnameMsg(msg_type='set_new_value',new_value=Surname('knox'))
+
+@dataclass
+class SetMultiMsg(Generic[Payload],Msg):
+    msg_type: Literal['set_new_values']
+    new_values: list[Payload]
+    pass
+
+SetSurnamesMsg=SetMultiMsg[Surname]
+
+Assert(codec(SetSurnamesMsg).decode({'msg_type':'set_new_values','new_values':['knox','garden']}))==SetSurnamesMsg(msg_type='set_new_values',new_values=[Surname('knox'),Surname('garden')])
+
+
+# codec can generate a typescript "cast" ("as-a") and "type guard" ("is a") matching its
+# json encoding. Non-class codecs generate inline typescript source code, see
+# codec.get_typescripte_asa() and codec.get_typescript_isa(). For classes, codec
+# also generates functions in corresponding namespace, for example:
+
+typescript_namespace=TypeScriptNamespace({})
+
+timestamp_codec=codec(Timestamp)
+# ensure typescript_namespace has as-a and is-a functions for xju.time.Timestamp,
+# xju.time.asInstanceOfTimestamp(), xju.time.isInstanceOfTimestamp():
+timestamp_codec.ensure_typescript_defs(typescript_namespace)
+
+Assert(codec(IpV4Addr).get_typescript_isa(TypeScriptSourceCode('7'),typescript_namespace))==TypeScriptSourceCode("(typeof (7) == 'string')")
+Assert(codec(IpV4Addr).get_typescript_asa(TypeScriptSourceCode('7'),typescript_namespace))==TypeScriptSourceCode("""((v: any): string => {
+    if (typeof v !== 'string') throw new Error(`${v} is not a string it is a ${typeof v}`);
+    return v as string;
+})(7)""")
+       
+# ... get_formatted_defs() generates the typescript source code:
+Assert(typescript_namespace.get_formatted_defs())==TypeScriptSourceCode(
+    '''\
+namespace xju {
+    export namespace time {
+        export type Timestamp = {
+            _Timestamp__value: number;
+        };
+        export function asInstanceOfTimestamp(v: any): xju.time.Timestamp
+        {
+            try{
+                if (Array.isArray(v)) throw new Error(`${v} is an array`);
+                if (v == null) throw new Error(`${v} is not an object it is null`);
+                if (typeof v !== \'object\') throw new Error(`${v} is not an object it is a ${typeof v}`);
+                const attr_asa=function(name:string, asa:any):any{
+                    try{
+                        asa(v[name]);
+                    }
+                    catch(e:any){
+                        throw new Error(`attribute ${name} is invalid because ${e}`);
+                    }
+                }
+                attr_asa(\'_Timestamp__value\',(x:any)=>((v: any): number => {
+                    if (typeof v !== \'number\') throw new Error(`${v} is not a number it is a ${typeof v}`);
+                    return v as number;
+                })(x));
+                return v as xju.time.Timestamp;
+            }
+            catch(e:any){
+                throw new Error(`${v} is not a xju.time.Timestamp because ${e}`);
+            }
+        }
+        export function isInstanceOfTimestamp(v:any): v is xju.time.Timestamp
+        {
+            return (
+                !Array.isArray(v) &&
+                v !== null &&        typeof v === \'object\' &&
+                (typeof (v["_Timestamp__value"]) == \'number\'))}
+    }
+}
+''')
+
```

### Comparing `xju-1.2.9/src/xju/jsonschema.py` & `xju-1.3.0/src/xju/jsonschema.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/jsonschema.py.test` & `xju-1.3.0/src/xju/jsonschema.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/misc.py` & `xju-1.3.0/src/xju/misc.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/misc.py.test` & `xju-1.3.0/src/xju/misc.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/newtype.py` & `xju-1.3.0/src/xju/newtype.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,75 +26,73 @@
 #  class HoursTag:pass
 #  class Hours(Int[HoursTag]):pass
 #
 # ... note do not use 'Hours=Int[HoursTag]' because that is an alias to a generic and
 # therefore has not run-time presence and therefore cannot be used with isinstance.
 #
 from typing import Iterable,Sized,Container,Collection,Reversible,Protocol,Type,overload,TypeVar
-from typing import Generic,Tuple,Mapping,Optional,List,Literal,Union,Any,Self
+from typing import Generic,Tuple,Mapping,Optional,List,Literal,Union,Any,Self,Never
+from types import NotImplementedType
 
 Tag=TypeVar('Tag',covariant=True)
 
-def verify_same_type(x:Any,y:Any):
-    if x.__class__ is not y.__class__:
-        raise Exception(f"{x!r}'s type {x.__class__} is not the same as {y!r}'s type {y.__class__}")
-    pass
-
-def eq(x:Any,y:Any)->bool:
-    verify_same_type(x,y)
-    return x.value().__eq__(y.value())
-
 class Int(Generic[Tag]):
     __value:int
 
     def __init__(self, value:int):
         self.__value=value
         pass
 
     def value(self)->int:
         return self.__value
 
-    def __eq__(self,other)->bool:
-        '''equality test, only valid for two object of exactly the same class; except that
-           python insists supporting __eq__ for objects of any type, so this function's signature
-           allows it and calls out all nonsense at runtime'''
+    # note the following type: ignore is to get the desired behaviour from mypy --strict-equality
+    # (as at mypy 1.3.0) i.e. forbid comparison of Int[XTag] and Int[YTag], noting:
+    # - python itself insists on being able to compare values of unrelated type (for example
+    #   to implement x in y)
+    # - the type: ignore avoid mypy error for non-liskoff substitutability (because
+    #   python's Object.__eq__ has other as Any)
+    # - with other: Any, mypy --strict-equality gives no error at all
+    # - magically (incorrectly?), the type: ignore does not suppress checks on type of other, but
+    #   does suppress the substitution error
+    def __eq__(self,other:Self)->bool:  # type: ignore
+        '''equality test, self and other have the same type and same value'''
         '''i.e. recommend stick to using Int[X] like:
               class Hours(Int[HoursTag]):pass
            ... and not inherit from Hours.
            If you choose to inherit from Hours, make sure you write your own __eq__'''
-        return eq(self,other)
+        if type(other) is not type(self):
+            return False
+        return self.value().__eq__(other.value())
 
-    def __ne__(self,other)->bool:
-        return not eq(self,other)
+    def __ne__(self,other:Self)->bool:  # type: ignore
+        return not self.__eq__(other)
 
     def __str__(self)->str:
         return str(self.value())
 
     def __repr__(self)->str:
         return repr(self.value())
 
     def __format__(self, format_spec:str)->str:
         return self.value().__format__(format_spec)
 
     def __float__(self)->float:
         return self.value().__float__()
     
-    def conjugate(self):
-        return self.value().conjugate()
-
     @overload
     def __divmod__(self, x:int) -> Tuple[Self,Self]:
         pass
     @overload
     def __divmod__(self, x:float) -> Tuple[float,float]:
         pass
     @overload
     def __divmod__(self, x:Self) -> Tuple[int,int]:
         pass
-    def __divmod__(self, x):
+    def __divmod__(self, x:Any) -> Any:
         if isinstance(x,int):
             q,r=self.value().__divmod__(x)
             return self.__class__(q),self.__class__(r)
         if isinstance(x,float):
             return divmod(self.value(),x)
         else:
             return divmod(self.value(),x.value())
@@ -105,15 +103,15 @@
         pass
     @overload
     def __floordiv__(self, x:float) -> float:
         pass
     @overload
     def __floordiv__(self, x:Self) -> int:
         pass
-    def __floordiv__(self, x):
+    def __floordiv__(self, x:Any) -> Any:
         if isinstance(x,int):
             return self.__class__(self.value()//x)
         elif isinstance(x,float):
             return self.value()//x
         else:
             return self.value()//x.value()
         pass
@@ -125,30 +123,28 @@
             return self.value()/x.value()
         pass
     
     @overload
     def __mul__(self, x:int) -> Self:
         pass
     @overload
-    def __mul__(self, x:Any):  # -> NotImplemented:
+    def __mul__(self, x:float) -> NotImplementedType:
         pass
-    def __mul__(self, x):
+    def __mul__(self, x:Any) -> Any:
         if isinstance(x,int):
             return self.__class__(self.value()*x)
-        else:
-            return NotImplemented
-        pass
+        return NotImplemented
 
     @overload
-    def __rmul__(self, x:int):  # -> Self:
+    def __rmul__(self, x:int) -> Self:
         pass
     @overload
-    def __rmul__(self, x:Any):  # -> NotImplemented
+    def __rmul__(self, x:float)-> float:
         pass
-    def __rmul__(self, x):
+    def __rmul__(self, x:Any)->Any:
         if isinstance(x,int):
             return self.__class__(x*self.value())
         else:
             return NotImplemented
         pass
 
     @overload
@@ -156,15 +152,15 @@
         pass
     @overload
     def __mod__(self, other:float)->float:
         pass
     @overload
     def __mod__(self, other:Self)->int:
         pass
-    def __mod__(self, other):
+    def __mod__(self, other:Any)->Any:
         if type(other) is int:
             return self.__class__(self.value()%other)
         if type(other) is float:
             return self.value()%other
         else:
             return self.value()%other.value()
 
@@ -244,26 +240,35 @@
     def __init__(self, value:float):
         self.__value=value
         pass
 
     def value(self)->float:
         return self.__value
 
-    def __eq__(self,other)->bool:
-        '''equality test, only valid for two object of exactly the same class; except
-           that python insists on supporting __eq__ for objects of any type, so this
-           function's signature allows it and calls out all nonsense at runtime'''
-        '''i.e. recommend stick to using Float[X] like:
-              class Timestamp(Float[TimestampTag]):pass
-           ... and not inherit from Timestamp.
-           If you choose to inherit from Timestamp, make sure you write your own __eq__'''
-        return eq(self,other)
+    # note the following type: ignore is to get the desired behaviour from mypy --strict-equality
+    # (as at mypy 1.3.0) i.e. forbid comparison of Int[XTag] and Int[YTag], noting:
+    # - python itself insists on being able to compare values of unrelated type (for example
+    #   to implement x in y)
+    # - the type: ignore avoid mypy error for non-liskoff substitutability (because
+    #   python's Object.__eq__ has other as Any)
+    # - with other: Any, mypy --strict-equality gives no error at all
+    # - magically (incorrectly?), the type: ignore does not suppress checks on type of other, but
+    #   does suppress the substitution error
+    def __eq__(self,other:Self)->bool:  # type: ignore
+        '''equality test, self and other have the same type and same value'''
+        '''i.e. recommend stick to using Int[X] like:
+              class Hours(Int[HoursTag]):pass
+           ... and not inherit from Hours.
+           If you choose to inherit from Hours, make sure you write your own __eq__'''
+        if type(other) is not type(self):
+            return False
+        return self.value().__eq__(other.value())
 
-    def __ne__(self,other)->bool:
-        return not eq(self,other)
+    def __ne__(self,other:Self)->bool:  # type: ignore
+        return not self.__eq__(other)
 
     def __str__(self)->str:
         return str(self.value())
 
     def __repr__(self)->str:
         return repr(self.value())
 
@@ -275,27 +280,24 @@
     
     def __float__(self)->float:
         return self.value().__float__()
     
     def hex(self)->str:
         return self.value().hex()
     
-    def conjugate(self):
-        return self.value().conjugate()
-
     @overload
     def __divmod__(self, x:int) -> Tuple[Self,Self]:
         pass
     @overload
     def __divmod__(self, x:float) -> Tuple[Self,Self]:
         pass
     @overload
     def __divmod__(self, x:Self) -> Tuple[float,float]:
         pass
-    def __divmod__(self, x):
+    def __divmod__(self, x:Any) -> Any:
         if isinstance(x,int) or isinstance(x,float):
             q,r=self.value().__divmod__(x)
             return self.__class__(q),self.__class__(r)
         else:
             return divmod(self.value(),x.value())
         pass
 
@@ -304,62 +306,62 @@
         pass
     @overload
     def __floordiv__(self, x:float) -> Self:
         pass
     @overload
     def __floordiv__(self, x:Self) -> float:
         pass
-    def __floordiv__(self, x):
+    def __floordiv__(self, x:Any) -> Any:
         if isinstance(x,int) or isinstance(x,float):
             return self.__class__(self.value()//x)
         else:
             return self.value()//x.value()
         pass
 
     @overload
     def __truediv__(self, x:Union[float,int]) -> Self:
         pass
     @overload
     def __truediv__(self, x:Self) -> float:
         pass
-    def __truediv__(self, x):
+    def __truediv__(self, x:Any) -> Any:
         if isinstance(x,int) or isinstance(x,float):
             return self.__class__(self.value()/x)
         else:
             return self.value()/x.value()
         pass
     
     @overload
     def __mul__(self, x:int) -> Self:
         pass
     @overload
     def __mul__(self, x:float) -> Self:
         pass
-    def __mul__(self, x):
+    def __mul__(self, x:Any) -> Any:
         return self.__class__(self.value()*x)
 
     @overload
     def __rmul__(self, x:int) -> Self:
         pass
     @overload
     def __rmul__(self, x:float) -> Self:
         pass
-    def __rmul__(self, x):
+    def __rmul__(self, x:Any)->Any:
         return self.__class__(x*self.value())
 
     @overload
     def __mod__(self, other:int)->Self:
         pass
     @overload
     def __mod__(self, other:float)->Self:
         pass
     @overload
     def __mod__(self, other:Self)->float:
         pass
-    def __mod__(self, other):
+    def __mod__(self, other:Any)->Any:
         if isinstance(other,int) or isinstance(other,float):
             return self.__class__(self.value()%other)
         else:
             return self.value()%other.value()
 
     def __round__(self, ndigits:int=0)->Self:
         return self.__class__(self.value().__round__(ndigits))
@@ -412,59 +414,67 @@
     def __init__(self, value:str):
         self.__value=value
         pass
 
     def value(self)->str:
         return self.__value
 
-    def __eq__(self,other)->bool:
-        '''equality test ignores possible subclass relationships, i.e. only valid
-           for two object of exactly the same class; except that python insists
-           supporting __eq__ for objects of any type, so this functions allows
-           comparing any Str[X] with anything but calls out nonsense at runtime'''
-        '''i.e. recommend stick to using Str[X] like:
-              class FirstName(Str[FirstNameTag]):pass
-           ... and not inherit from FirstName.
-           If you choose to inherit from Timestamp, make sure you write your own __eq__'''
-        return eq(self,other)
+    # note the following type: ignore is to get the desired behaviour from mypy --strict-equality
+    # (as at mypy 1.3.0) i.e. forbid comparison of Int[XTag] and Int[YTag], noting:
+    # - python itself insists on being able to compare values of unrelated type (for example
+    #   to implement x in y)
+    # - the type: ignore avoid mypy error for non-liskoff substitutability (because
+    #   python's Object.__eq__ has other as Any)
+    # - with other: Any, mypy --strict-equality gives no error at all
+    # - magically (incorrectly?), the type: ignore does not suppress checks on type of other, but
+    #   does suppress the substitution error
+    def __eq__(self,other:Self)->bool:  # type: ignore
+        '''equality test, self and other have the same type and same value'''
+        '''i.e. recommend stick to using Int[X] like:
+              class Hours(Int[HoursTag]):pass
+           ... and not inherit from Hours.
+           If you choose to inherit from Hours, make sure you write your own __eq__'''
+        if type(other) is not type(self):
+            return False
+        return self.value().__eq__(other.value())
 
-    def __ne__(self,other)->bool:
-        return not eq(self,other)
+    def __ne__(self,other:Self)->bool:  # type: ignore
+        return not self.__eq__(other)
 
     def __str__(self)->str:
         return str(self.value())
 
     def __repr__(self)->str:
         return repr(self.value())
 
     def __format__(self, format_spec:str)->str:
         return self.value().__format__(format_spec)
 
-    def splitlines(self,keepends=False)->List:
+    def splitlines(self,keepends:bool=False)->List[Self]:
         return [self.__class__(_) for _ in self.value().splitlines()]
 
     def encode(self,encoding:str='utf-8', errors:str='strict')->bytes:
         return self.value().encode()
 
     def __contains__(self,other:str)->bool:
         return self.value().__contains__(other)
 
     def zfill(self,width:int)->Self:
         return self.__class__(self.value().zfill(width))
 
-    def format_map(self,mapping:Mapping):
+    def format_map(self,mapping:Mapping[Any,Any]) -> Self:
         return self.__class__(self.value().format_map(mapping))
 
-    def format(self,*args,**kwargs):
+    def format(self,*args:Any,**kwargs:Any) -> Any:
         return self.__class__(self.value().format(*args,**kwargs))
     
-    def expandtabs(self,tabsize=8)->Self:
+    def expandtabs(self,tabsize:int=8)->Self:
         return self.__class__(self.value().expandtabs(tabsize))
 
-    def __getitem__(self,key):
+    def __getitem__(self,key:Any) -> Any:
         return self.value().__getitem__(key)
 
     
     def capitalize(self)->Self:
         return self.__class__(self.value().capitalize())
     def lower(self)->Self:
         return self.__class__(self.value().lower())
@@ -525,104 +535,104 @@
         pass
     @overload
     def rfind(self, sub:str, start:int)->int:
         pass
     @overload
     def rfind(self, sub:str, start:int, end:int)->int:
         pass
-    def rfind(self, sub, *args):
-        return self.value().rfind(sub,*args)
+    def rfind(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().rfind(*args)
     @overload
     def find(self, sub:str) -> int:
         pass
     @overload
     def find(self, sub:str, start:int)->int:
         pass
     @overload
     def find(self, sub:str, start:int, end:int)->int:
         pass
-    def find(self, sub, *args):
-        return self.value().find(sub,*args)
+    def find(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().find(*args)
     @overload
     def rindex(self, sub:str) -> int:
         pass
     @overload
     def rindex(self, sub:str, start:int)->int:
         pass
     @overload
     def rindex(self, sub:str, start:int, end:int)->int:
         pass
-    def rindex(self, sub, *args):
-        return self.value().rindex(sub,*args)
+    def rindex(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().rindex(*args)
     @overload
     def index(self, sub:str) -> int:
         pass
     @overload
     def index(self, sub:str, start:int)->int:
         pass
     @overload
     def index(self, sub:str, start:int, end:int)->int:
         pass
-    def index(self, sub, *args):
-        return self.value().index(sub,*args)
+    def index(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().index(*args)
     @overload
     def count(self, sub:str) -> int:
         pass
     @overload
     def count(self, sub:str, start:int)->int:
         pass
     @overload
     def count(self, sub:str, start:int, end:int)->int:
         pass
-    def count(self, sub, *args):
-        return self.value().count(sub,*args)
+    def count(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().count(*args)
     @overload
     def translate(self, sub:str) -> int:
         pass
     @overload
     def translate(self, sub:str, start:int)->int:
         pass
     @overload
     def translate(self, sub:str, start:int, end:int)->int:
         pass
-    def translate(self, sub, *args):
-        return self.value().translate(sub,*args)
+    def translate(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().translate(*args)
     @overload
     def endswith(self, s:str) -> bool:
         pass
     @overload
     def endswith(self, s:str, start:int)->bool:
         pass
     @overload
     def endswith(self, s:str, start:int, end:int)->bool:
         pass
-    def endswith(self, s, *args):
-        return self.value().endswith(s,*args)
+    def endswith(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().endswith(*args)
     @overload
     def startswith(self, s:str) -> bool:
         pass
     @overload
     def startswith(self, s:str, start:int)->bool:
         pass
     @overload
     def startswith(self, s:str, start:int, end:int)->bool:
         pass
-    def startswith(self, s, *args):
-        return self.value().startswith(s,*args)
-    def strip(self, chars:Optional[str]=None)->Self:
+    def startswith(self, *args:Any, **kwargs:Any) -> Any:
+        return self.value().startswith(*args)
+    def strip(self, chars:str|None=None)->Self:
         return self.__class__(self.value().strip(chars))
-    def lstrip(self, chars:Optional[str]=None)->Self:
+    def lstrip(self, chars:str|None=None)->Self:
         return self.__class__(self.value().lstrip(chars))
-    def rstrip(self, chars:Optional[str]=None)->Self:
+    def rstrip(self, chars:str|None=None)->Self:
         return self.__class__(self.value().rstrip(chars))
-    def replace(self, old:str, new:str, count=-1)->Self:
+    def replace(self, old:str, new:str, count:int=-1)->Self:
         return self.__class__(self.value().replace(old,new,count))
-    def split(self, sep:Optional[str]=None, max_split=-1)->List[str]:
+    def split(self, sep:Optional[str]=None, max_split:int=-1)->List[str]:
         return self.value().split(sep,max_split)
-    def rsplit(self, sep:Optional[str]=None, max_split=-1)->List[str]:
+    def rsplit(self, sep:Optional[str]=None, max_split:int=-1)->List[str]:
         return self.value().rsplit(sep,max_split)
     def partition(self,sep:str) -> Tuple[str,str,str]:
         return self.value().partition(sep)
     def rpartition(self,sep:str) -> Tuple[str,str,str]:
         return self.value().rpartition(sep)
     def removeprefix(self,sub:str)->Self:
         return self.__class__(self.value().removeprefix(sub))
```

### Comparing `xju-1.2.9/src/xju/newtype.py.test` & `xju-1.3.0/src/xju/newtype.py.test`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
 
 Assert(str(h1))=='7'
 Assert(repr(h1))=='7'
 Assert('{:02d}'.format(h1))=='07'
 Assert(h1.__float__())==7.0
 Assert(abs(Hours(-5)))==Hours(5)
 Assert(~h1)==Hours(~h1.value())
-Assert(h1.conjugate())==h1.value().conjugate()
 Assert(divmod(h1,Hours(2)))==(3,1)
 Assert(divmod(h1,2))==(Hours(3),Hours(1))
 Assert(divmod(h1,1.5))==(4.0,1.0)
 # floordiv
 Assert(h1//3)==Hours(2)
 Assert(h1//Hours(3))==2
 Assert(h1//2.5)==7//2.5
@@ -187,15 +186,15 @@
     h2*2.5
 except TypeError as e:
     Assert("unsupported operand type(s) for *: 'Hours' and 'float'").isIn(readable_repr(e))
 else:
     assert False
     pass
 try:
-    Hours(3)*Hours(4)
+    Hours(3)*Hours(4)  # type: ignore # or mypy rightly rejects
 except TypeError as e:
     Assert("unsupported operand type(s) for *: 'Hours' and 'Hours'").isIn(readable_repr(e))
 else:
     assert False
     pass
 # rmull
 Assert(3*Hours(4))==Hours(12)
@@ -241,22 +240,14 @@
 Assert(h1|h2)==Hours(7|8)
 Assert(h1.__xor__(h2))==Hours(7^8)
 Assert(h1.as_integer_ratio())==h1.value().as_integer_ratio()
 
 Assert(Hours(7)!=Hours(8))==True
 
 try:
-    Hours(7)==7
-except Exception as e:
-    Assert(readable_repr(e))=="7's type <class '__main__.Hours'> is not the same as 7's type <class 'int'>"
-else:
-    assert False
-    pass
-
-try:
     Hours(7)+cast(Hours,7)
 except Exception as e:
     Assert("unsupported operand type(s) for +: 'Hours' and 'int'").isIn(readable_repr(e))
 else:
     assert False
     pass
 
@@ -336,15 +327,14 @@
 Assert(l2)>=l1
 Assert(str(l1))==str(7.5)
 Assert(repr(l1))==repr(7.5)
 Assert(f'{l1:0.2f}')=='7.50'
 Assert(int(l1))==7
 Assert(float(l1))==7.5
 Assert(l1.hex())==float(7.5).hex()
-Assert(l1.conjugate())==float(7.5).conjugate()
 Assert(divmod(l1,2))==tuple(Length(x) for x in divmod(7.5,2))
 Assert(divmod(l1,1.5))==tuple(Length(x) for x in divmod(7.5,1.5))
 Assert(divmod(l1,l2))==divmod(7.5,10.0)
 #floordiv
 Assert(l1//2)==Length(7.5//2)
 Assert(l1//2.6)==Length(7.5//2.6)
 Assert(l1//l2)==7.5//10.0
@@ -413,7 +403,12 @@
     cast(Length,7)-Length(7)
 except Exception as e:
     Assert("unsupported operand type(s) for -: 'int' and 'Length'").isIn(readable_repr(e))
 else:
     assert False
     pass
 
+y:list[LastName|Weight|Hours] = [ LastName('fred'), Weight(7.8), Hours(9) ]
+
+Assert(LastName('jock') not in y)==True
+Assert(Hours(2) not in y)==True
+Assert(Weight(2.1) not in y)==True
```

### Comparing `xju-1.2.9/src/xju/patch.py` & `xju-1.3.0/src/xju/patch.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/patch.py.test` & `xju-1.3.0/src/xju/patch.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/pq.py` & `xju-1.3.0/src/xju/pq.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/pq.py.test` & `xju-1.3.0/src/xju/pq.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/rfc2616.py` & `xju-1.3.0/src/xju/rfc2616.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/rfc2616.py.test` & `xju-1.3.0/src/xju/rfc2616.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/time.py` & `xju-1.3.0/src/xju/time.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/time.py.test` & `xju-1.3.0/src/xju/time.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.9/src/xju/xn.py` & `xju-1.3.0/src/xju/xn.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,40 +13,41 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 import traceback
 import sys
 import string
-from typing import Sequence,Callable,Literal,Dict,List,Tuple
+from typing import Sequence,Callable,Literal,Dict,List,Tuple,Any,Type
+from types import TracebackType
 
 class FileAndLine(object):
-    def __init__(self,file=None,line=None,readable:bool=True):
+    def __init__(self,file:str|None=None,line:int|None=None,readable:bool=True)->None:
         self.file=file
         self.line=line
         self.readable=readable
         pass
-    def setTo(self,file,line)->None:
+    def setTo(self,file:str,line:int)->None:
         self.file=file
         self.line=line
         pass
     def __str__(self)->str:
         if self.file:
             return '{file}:{line}: '.format(**self.__dict__)
         return ''
     pass
 
 class Xn:
     """Capture cause and context.
     """
-    def __init__(self, cause:object):
+    def __init__(self, cause:object)->None:
         '''cause is convertable to a string using str'''
         ''' e.g. cause can be an exception or a string like "file not found"'''
-        '''cause can also have a readable_repr() method, in which case that'''
-        '''will be used by readable_repr() below'''
+        '''cause can also have a xju_xn_readable_repr() method, in which case that'''
+        '''will be used by xju_xn_readable_repr() below'''
         self.cause = (cause,FileAndLine()) # file,line set below
         self.context:List[Tuple[str,FileAndLine]] = [] # (text,FileAndLine)
         pass
 
     def __str__(self)->str:
         '''programmer friendly format, each context and cause includes
         file and line, and intermediate stack entries are included
@@ -54,61 +55,70 @@
         result = ''
         x = ''.join([
             '{fl}failed to {s} because\n'.format(**vars())
             for s,fl in reversed(self.context)])
         y = '{cause[1]}{cause[0]}'.format(**vars(self))
         return x+y
 
-    def readable_repr(self)->str:
+    def xju_xn_readable_repr(self)->str:
         '''human (non-programmer) readable representation, omitting file
         and line, omitting intermediate stack entries, and producing a
         proper sentence i.e. capitalised and ending in full stop
         - see unit test below for example'''
         result = ''
         x:str = ''.join([
             'failed to {s} because\n'.format(**vars())
             for s,fl in reversed(self.context)
             if fl.readable])
-        if hasattr(self.cause[0], 'readable_repr'):
-            y:str=self.cause[0].readable_repr()
+        if hasattr(self.cause[0], 'xju_xn_readable_repr'):
+            y:str=self.cause[0].xju_xn_readable_repr()
         else:
             y = str(self.cause[0])
             pass
         return capitalise(x+y+'.')
     pass
 
-def readable_repr(e)->str:
-    if callable(getattr(e,'readable_repr',None)):
-        return e.readable_repr()
+def readable_repr(e:BaseException)->str:
+    r=getattr(e,'xju_xn_readable_repr',None)
+    if callable(r):
+        return str(r())
     return str(e)
 
 def capitalise(s:str)->str:
     if s and s[0]!=s[0].upper():
         return s[0].upper()+s[1:]
     return s
 
-def in_function_context(function:Callable, vars:Dict={}, exceptionInfo=None, fl=None)->Exception:
+def in_function_context(function:Callable,
+                        vars:Dict[str,Any]={},
+                        exceptionInfo:None|tuple[Type[BaseException],BaseException,TracebackType]=None,
+                        fl:None|tuple[str,int]=None)->BaseException:
     """Make a Xn that includes exception info and context as first_line_of(f.__doc__).format(**vars()).
-    If exceptionInfo[1] is already a Xn just add context,
-    otherwise use exceptionInfo as cause for a new Xn.
-
-    exceptionInfo is as returned by sys.exc_info()
+       - if exceptionInfo[1] is already a Xn just add context
+       - otherwise use exceptionInfo as cause for a new Xn
+       - exceptionInfo defaults to sys.exc_info()
     """
     return in_context(first_line_of(function.__doc__).format(**vars),
                       exceptionInfo=exceptionInfo,
                       fl=fl)
 
-def in_context(context:str, exceptionInfo=None, fl=None)->Exception:
+def in_context(context:str,
+               exceptionInfo:None|tuple[Type[BaseException],BaseException,TracebackType]=None,
+               fl:None|tuple[str,int]=None)->BaseException:
     """Make a Xn that includes exception info and context.
-    If exceptionInfo[1] is already a Xn just add context,
-    otherwise use exceptionInfo as cause for a new Xn.
-
-    exceptionInfo is as returned by sys.exc_info()
+       - if exceptionInfo[1] is already a Xn just add context
+       - otherwise use exceptionInfo as cause for a new Xn
+       - exceptionInfo defaults to sys.exc_info()
     """
-    if exceptionInfo is None: exceptionInfo=sys.exc_info()
+    if exceptionInfo is None:
+        t, e, b = sys.exc_info()
+        assert t is not None
+        assert e is not None
+        assert b is not None
+        exceptionInfo=(t,e,b)
     exceptionType,r,traceBack=exceptionInfo
 
     if not isinstance(r,Xn):
         #build new exception type derived from both original and Xn
         name=exceptionType.__name__
         def init(self,v):
             Xn.__init__(self,v)
@@ -117,27 +127,28 @@
                     setattr(self,a,getattr(v,a))
                 except AttributeError:
                     pass
                 pass
             pass
         def str_(self)->str:
             return Xn.__str__(self)
-        def readable_repr(self)->str:
-            return Xn.readable_repr(self)
+        def xju_xn_readable_repr(self)->str:
+            return Xn.xju_xn_readable_repr(self)
         r=type(name,
                (Xn,exceptionType),
                {
                    '__init__':init,
                    '__str__':str_,
-                   'readable_repr':readable_repr
+                   'xju_xn_readable_repr':xju_xn_readable_repr
                })(r)
     
     st=[tuple(_) for _ in traceback.extract_tb(traceBack)]
     # fill in most recent file,line (latest context or cause if no context)
     f,l=st[-1][0:2]
+    assert isinstance(r, Xn)
     if r.context:
         if not r.context[-1][1].file:
             r.context[-1][1].file=f
             pass
         if not r.context[-1][1].line:
             r.context[-1][1].file=l
             pass
@@ -152,54 +163,32 @@
     f2=fl[0] if fl else None
     l2=fl[1] if fl else None
     r.context.append( (context,FileAndLine(f2,l2)) )
     traceBack.tb_next=None
     return r
 
 
-def first_line_of(x)->str:
-    '''return first line of str({x})'''
-    return str(x).split('\n')[0]
+def first_line_of(x:Any)->str:
+    '''return first non-empty line of str({x}) stripped of leading and trailing whitespace'''
+    return str(x).strip().split('\n')[0].strip()
 
 def desentence(s:str)->str:
     '''remove any trailing '.' and down-case first characters of {s}'''
     if s.endswith('.'): s=s[:-1]
     return s[0:1].lower()+s[1:]
 
 def indent(prefix:str,s:str)->str:
     '''prefix all but first line of s by specified prefix'''
     return s.replace('\n','\n'+prefix)
 
-class AllFailed(Exception):
-    def __init__(self,causes:Sequence[Exception]):
+class AllFailed(BaseException):
+    def __init__(self,causes:Sequence[BaseException])->None:
         self.causes=causes
         pass
-    def __str__(self):
+    def __str__(self)->str:
         return ', and\n'.join([str(cause) for cause in self.causes])
-    def readable_repr(self)->str:
+    def xju_xn_readable_repr(self)->str:
         return '; and\n'.join(['- '+
                                indent('  ',desentence(readable_repr(cause)))
                                for cause in self.causes])
     pass
 
-class Scope:
-    def __init__(self,description,
-                 log=lambda s: print('INFO: {s}'.format(**vars()))):
-        self.description=description
-        self.log=log
-        self.result_=None
-        log('+ '+self.description)
-        pass
-    def __enter__(self):
-        return self
-    def __exit__(self,eType,eVal,eTrc):
-        self.log('- '+self.description+' = '+ (str(eType) if eType else repr(self.result_)))
-        description=self.description
-        self.description=None
-        if eType:
-            raise in_context(description, (eType,eVal,eTrc)) from None
-        return False
-    def result(self,result):
-        self.result_=result
-        return result
-    pass
-
```

### Comparing `xju-1.2.9/src/xju/xn.py.test` & `xju-1.3.0/src/xju/xn.py.test`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 from sys import path
 from os.path import dirname
 if path[0]==dirname(__file__): path.pop(0)
-from xju.xn import in_context,readable_repr,AllFailed,in_function_context,Scope,Xn,capitalise
+from xju.xn import in_context,readable_repr,AllFailed,in_function_context,Xn,capitalise
 from xju.assert_ import Assert
 from typing import cast
 
 import io
 import sys
 
 from xju.assert_ import Assert
@@ -150,16 +150,18 @@
 fred.\
 '''
     pass
 
 def test6():
     class X:
         def jump(self, height:int):
-            '''jump {height}m in the air
-               - from a standing start'''
+            '''
+            jump {height}m in the air
+            - from a standing start
+            '''
             try:
                 raise Exception('I have lead feet')
             except Exception as e:
                 raise in_function_context(X.jump,vars()) from None
             pass
         pass
     try:
@@ -167,48 +169,14 @@
     except Exception as e:
         Assert(readable_repr(e))=='Failed to jump 10m in the air because\nI have lead feet.'
     else:
         assert False, 'should not be here'
         pass
     pass
 
-sys.stdout=io.StringIO()
-with Scope('do some stuff') as scope:
-    pass
-Assert(sys.stdout.getvalue())=='''\
-INFO: + do some stuff
-INFO: - do some stuff = None
-'''
-sys.stdout=io.StringIO()
-def f():
-    with Scope('do some stuff') as scope:
-        return scope.result(77)
-    pass
-
-Assert(f())==77
-Assert(sys.stdout.getvalue())=='''\
-INFO: + do some stuff
-INFO: - do some stuff = 77
-'''
-def f2():
-    with Scope('do some stuff') as scope:
-        raise Exception('did not work')
-    pass
-try:
-    f2()
-except Exception as e:
-    ee:Xn=cast(Xn,e)
-    Assert(ee.readable_repr())=='''\
-Failed to do some stuff because
-did not work.'''
-else:
-    assert False,'should not reach'
-    pass
-
-
 def test8():
     Assert(capitalise('Fred'))=='Fred'
     pass
 
 def test9():
     Assert(str(AllFailed([Exception('fred'),Exception('jock')])))=="fred, and\njock"
     pass
```

### Comparing `xju-1.2.9/src/xju.egg-info/PKG-INFO` & `xju-1.3.0/src/xju.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.2.9
+Version: 1.3.0
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -53,14 +53,34 @@
 * see `xju/cmc/cmclass.py.test <xju/cmc/cmclass.py.test>`_ for sample code
 
 
 `xju.cmc.Dict <xju/cmc/__init__.py>`_ - dictionary that is a context manager for its (context manager) values
 
 * see `xju/cmc/Dict.py.test <xju/cmc/Dict.py.test>`_ for sample code
 
+`xju.cmc.Opt <xju/cmc/__init__.py>`_ - context manager for its optional (context manager) value
+
+* see `xju/cmc/Opt.py.test <xju/cmc/Opt.py.test>`_ for sample code
+
+`xju.cmc.async_cmclass <xju/cmc/__init__.py>`_  - provides async context management for class attributes that are async / sync context managers
+
+* managing multiple resource attributes is clumsy with AsyncExitStack, this module implements
+  \__aenter__ and \__aexit__ automatically to ensure correct ordering and cleanup on exceptions
+
+* see `xju/cmc/async_cmclass.py.test <xju/cmc/async_cmclass.py.test>`_ for sample code
+
+
+`xju.cmc.AsyncDict <xju/cmc/__init__.py>`_ - dictionary that is a async context manager for its (async context manager) values
+
+* see `xju/cmc/AsyncDict.py.test <xju/cmc/AsyncDict.py.test>`_ for sample code
+
+`xju.cmc.AsyncOpt <xju/cmc/__init__.py>`_ - async context manager for its optional (async context manager) value
+
+* see `xju/cmc/AsyncOpt.py.test <xju/cmc/AsyncOpt.py.test>`_ for sample code
+
 
 `xju.cmc.io <xju/cmc/io/__init__.py>`_ - pure context management for e.g. file reading and writing, non-blocking io
 
 * see unit tests for sample code:
   *  `FileLock.py.test <xju/cmc/io/FileLock.py.test>`_
   *  `FileMode.py.test <xju/cmc/io/FileMode.py.test>`_
   *  `FilePosition.py.test <xju/cmc/io/FilePosition.py.test>`_
@@ -86,19 +106,19 @@
 `xju.cmc.Thread/Mutex/Lock/Condition <xju/cmc/__init__.py>`_
 
 * threading primitives that encourage correct design
 
 * see `xju/cmc/ThreadMutexLockCondition.py.test <xju/cmc/ThreadMutexLockCondition.py.test>`_ for sample code
 
 
-`xju.cmc.Task <xju/cmc/__init__.py>`_
+`xju.cmc.AsyncTask/Mutex/Lock/Condition <xju/cmc/__init__.py>`_
 
-* asyncio Task context manager
+* asyncio Task/Mutex/Lock/Condition context managers
 
-* see `xju/cmc/Task.py.test <xju/cmc/Task.py.test>`_ for sample code
+* see `xju/cmc/Task.py.test <xju/cmc/AsyncTaskMutexLockCondition.py.test>`_ for sample code
 
 
 `xju.cmc.AsyncServiceQueue <xju/cmc/__init__.py>`_
 
 * asyncio thread-safe service queue, allows any thread to queue a coroutine on an event loop
   so it is executed by a task in that event loop
 
@@ -134,14 +154,16 @@
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
 * generates typescript code (types, type-guards and dynamic casts) equivalents
 
+* extensible with custom encodings
+
 * see `xju/json_codec.py.test <xju/json_codec.py.test>`_ for full sample code
 
 
 `xju.jsonschema <xju/jsonschema.py>`_
 
 * represents JSON schemas as straight-foward, easy-to-read python data structures, because life's too short for jsonschema.org
 
@@ -166,14 +188,31 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
+- 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
+- 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
+- 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
+- 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
+- 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
+- 1.2.13 xju.newtype eq/neq now follows python "you can compare apples to oranges", rely on mypy --strict-equality (which for what it's worth is broken at mypy 1.3.0)
+- 1.2.13 now compatible with mypy --strict-equality
+- 1.2.13 add xju.cmc.AsyncTask/Mutex/Condition/Lock (thread equivalents for asyncio); note Task deprecated, use AsyncTask
+- 1.2.13 add custom encoding facility to xju.json_codec
+- 1.2.13 add typescript aliases to json_codec generated code for xju.newtype Str/Int/Float
+- 1.2.12 fixes typescript null v object handling
+- 1.2.12 adds typescript aliases for NewStr, NewInt, NewFloat
+- 1.2.11 adds typescript --strict support and fixes typescript code generation bugs
+- 1.2.11 xju.json_codec supports Literal[int] and Literal[bool]
+- 1.2.11 xju.json_codec supports generic classes
+- 1.2.10 xju.json_codec supports typing.NewType str/int/bool/float
 - 1.2.9 xju.json_codec generates typescript equivalents
 - 1.2.9 xju.json_codec adds codec() convenience method
 - 1.2.9 xju.json_codec uses kw_args to construct classes
 
 - 1.2.8 xju.json_codec supports string type-hints (for foward definitions)
 - 1.2.8 xju.json_codec adds typing.Self support (for recursive types)
 - 1.2.8 xju.json_codec requires python 3.11, tested with mypy 1.1.1
```

### Comparing `xju-1.2.9/src/xju.egg-info/SOURCES.txt` & `xju-1.3.0/src/xju.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,23 @@
 src/xju/time.py.test
 src/xju/xn.py
 src/xju/xn.py.test
 src/xju.egg-info/PKG-INFO
 src/xju.egg-info/SOURCES.txt
 src/xju.egg-info/dependency_links.txt
 src/xju.egg-info/top_level.txt
+src/xju/cmc/AsyncDict.py.test
+src/xju/cmc/AsyncOpt.py.test
 src/xju/cmc/AsyncServiceQueue.py.test
+src/xju/cmc/AsyncTaskMutexLockCondition.py.test
 src/xju/cmc/Dict.py.test
+src/xju/cmc/Opt.py.test
 src/xju/cmc/ThreadMutexLockCondition.py.test
 src/xju/cmc/__init__.py
+src/xju/cmc/async_cmclass.py.test
 src/xju/cmc/cmc.py.test
 src/xju/cmc/cmclass.py.test
 src/xju/cmc/perflog.py
 src/xju/cmc/perflog.py.test
 src/xju/cmc/signal.py
 src/xju/cmc/signal.py.test
 src/xju/cmc/tstore.py
```

