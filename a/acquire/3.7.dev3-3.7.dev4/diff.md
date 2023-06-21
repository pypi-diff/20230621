# Comparing `tmp/acquire-3.7.dev3.tar.gz` & `tmp/acquire-3.7.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.7.dev3.tar", last modified: Mon Jun 19 15:52:55 2023, max compression
+gzip compressed data, was "acquire-3.7.dev4.tar", last modified: Wed Jun 21 07:17:43 2023, max compression
```

## Comparing `acquire-3.7.dev3.tar` & `acquire-3.7.dev4.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-19 15:52:41.000000 acquire-3.7.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-19 15:52:41.000000 acquire-3.7.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 15:52:41.000000 acquire-3.7.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-19 15:52:55.142928 acquire-3.7.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-19 15:52:41.000000 acquire-3.7.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76017 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-19 15:52:45.000000 acquire-3.7.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:52:55.142928 acquire-3.7.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.976532 acquire-3.7.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-21 07:17:27.000000 acquire-3.7.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-21 07:17:27.000000 acquire-3.7.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 07:17:27.000000 acquire-3.7.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-21 07:17:43.976532 acquire-3.7.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-21 07:17:27.000000 acquire-3.7.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.964532 acquire-3.7.dev4/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76017 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.968532 acquire-3.7.dev4/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.968532 acquire-3.7.dev4/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.972532 acquire-3.7.dev4/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.972532 acquire-3.7.dev4/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.972532 acquire-3.7.dev4/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-21 07:17:27.000000 acquire-3.7.dev4/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-21 07:17:43.000000 acquire-3.7.dev4/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.968532 acquire-3.7.dev4/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-21 07:17:43.000000 acquire-3.7.dev4/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-21 07:17:43.000000 acquire-3.7.dev4/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:17:43.000000 acquire-3.7.dev4/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 07:17:43.000000 acquire-3.7.dev4/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 07:17:43.000000 acquire-3.7.dev4/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 07:17:43.000000 acquire-3.7.dev4/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-21 07:17:34.000000 acquire-3.7.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:17:43.976532 acquire-3.7.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.976532 acquire-3.7.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:17:43.976532 acquire-3.7.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-21 07:17:27.000000 acquire-3.7.dev4/tox.ini
```

### Comparing `acquire-3.7.dev3/LICENSE` & `acquire-3.7.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/PKG-INFO` & `acquire-3.7.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.7.dev3
+Version: 3.7.dev4
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.7.dev3/README.md` & `acquire-3.7.dev4/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/acquire.py` & `acquire-3.7.dev4/acquire/acquire.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/collector.py` & `acquire-3.7.dev4/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/crypt.py` & `acquire-3.7.dev4/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/dynamic/windows/collect.py` & `acquire-3.7.dev4/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/dynamic/windows/handles.py` & `acquire-3.7.dev4/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/dynamic/windows/named_objects.py` & `acquire-3.7.dev4/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/dynamic/windows/ntdll.py` & `acquire-3.7.dev4/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/dynamic/windows/types.py` & `acquire-3.7.dev4/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/esxi.py` & `acquire-3.7.dev4/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/hashes.py` & `acquire-3.7.dev4/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/log.py` & `acquire-3.7.dev4/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/outputs/base.py` & `acquire-3.7.dev4/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/outputs/dir.py` & `acquire-3.7.dev4/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/outputs/tar.py` & `acquire-3.7.dev4/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/tools/decrypter.py` & `acquire-3.7.dev4/acquire/tools/decrypter.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import io
 import json
 import logging
 import multiprocessing
 import os
 import signal
 import sys
-from collections import deque
+import textwrap
+from collections import defaultdict, deque
 from concurrent.futures import ProcessPoolExecutor
 from datetime import datetime, timezone
 from pathlib import Path
 from queue import Empty as QueueEmptyError
 from urllib import request
 from urllib.error import HTTPError
 from urllib.parse import urljoin
@@ -339,27 +340,28 @@
     args = parser.parse_args()
 
     setup_logging(log, args.verbose)
 
     if not progress:
         log.info("`rich` is not installed, progress will not be shown")
 
-    if args.output and len(args.files) > 1:
-        parser.exit("--output is only allowed when decrypting a single file")
+    if args.output and args.output.is_file() and len(args.files) > 1:
+        parser.exit("--output should be a directory when decrypting multiple files.")
 
-    if not args.output:
-        for path in args.files:
-            if path.suffix != ".enc":
-                parser.exit(f"File doesn't have .enc extension: {path}")
+    files = find_enc_files(args.files)
 
     if args.output:
-        outputs = [args.output.resolve()]
+        resolv_path = args.output.resolve()
+        outputs = [resolv_path / path.stem for path in files] if args.output.is_dir() else [resolv_path]
     else:
         # Strip .enc extension
-        outputs = [path.with_suffix("") for path in args.files]
+        outputs = [path.with_suffix("") for path in files]
+
+    if len(set(outputs)) != len(outputs):
+        show_duplicates(args.output, files)
 
     if not args.key_file and not args.key_server:
         parser.exit("Need either --key-file or --key-server")
 
     if args.key_file:
         if not args.key_file.is_file():
             parser.exit(f"{args.key_file} doesn't exist or is not a file")
@@ -374,15 +376,15 @@
     with ctx:
         signal_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
         with multiprocessing.Manager() as mp, ProcessPoolExecutor(max_workers=args.workers) as executor:
             stop_event = mp.Event()
             status_queue = mp.Queue()
             tasks = []
 
-            for in_path, out_path in zip(args.files, outputs):
+            for in_path, out_path in zip(files, outputs):
                 task_id = (
                     progress.add_task("decrypt", start=False, visible=False, filename=in_path.name)
                     if progress
                     else len(tasks)
                 )
                 executor.submit(
                     worker,
@@ -420,12 +422,47 @@
                 except (QueueEmptyError, KeyboardInterrupt):
                     (progress.console.log if progress else log.info)("Stopping...")
                     stop_event.set()
                     executor.shutdown(wait=True, cancel_futures=True)
                     break
 
 
+def show_duplicates(output_directory: Path, files: list[Path]) -> None:
+    # Gather all files that could cause duplicates in `args.output`.
+    input_files = defaultdict(list)
+    for input_file in files:
+        input_files[input_file.name].append(input_file)
+
+    # Find all duplicates
+    duplicate_generator = (file_paths for file_paths in input_files.values() if len(file_paths) > 1)
+    duplicates = "\n\n".join(
+        textwrap.indent(
+            "\n".join(str(file) for file in file_paths),
+            prefix="  - ",
+        )
+        for file_paths in duplicate_generator
+    )
+    log.warning(
+        "Two or more encrypted files have the same name. "
+        f"This will skip decrypting the file if it already exists in '{output_directory}'\n"
+        f"The files with the same names are:\n"
+        f"{duplicates}"
+    )
+
+
+def find_enc_files(files: list[Path]) -> list[Path]:
+    encrypted_files = []
+    for path in files:
+        if path.is_file() and path.suffix == ".enc":
+            encrypted_files.append(path)
+        elif path.is_dir():
+            encrypted_files.extend(path.rglob("*.enc"))
+        else:
+            log.info(f"File {path!r} does not have the .enc extension. skipping.")
+    return encrypted_files
+
+
 if __name__ == "__main__":
     try:
         sys.exit(main())
     except KeyboardInterrupt:
         pass
```

### Comparing `acquire-3.7.dev3/acquire/uploaders/minio.py` & `acquire-3.7.dev4/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/uploaders/plugin.py` & `acquire-3.7.dev4/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/uploaders/plugin_registry.py` & `acquire-3.7.dev4/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire/utils.py` & `acquire-3.7.dev4/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/acquire.egg-info/PKG-INFO` & `acquire-3.7.dev4/acquire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.7.dev3
+Version: 3.7.dev4
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.7.dev3/acquire.egg-info/SOURCES.txt` & `acquire-3.7.dev4/acquire.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 acquire/uploaders/minio.py
 acquire/uploaders/plugin.py
 acquire/uploaders/plugin_registry.py
 tests/__init__.py
 tests/conftest.py
 tests/test_acquire_command.py
 tests/test_collector.py
+tests/test_decryptor_funcs.py
 tests/test_esxi_memory.py
 tests/test_file_sorting.py
 tests/test_minio_uploader.py
 tests/test_plugin.py
 tests/test_utils.py
 tests/docs/Makefile
 tests/docs/conf.py
```

### Comparing `acquire-3.7.dev3/pyproject.toml` & `acquire-3.7.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/conftest.py` & `acquire-3.7.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/docs/Makefile` & `acquire-3.7.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/docs/conf.py` & `acquire-3.7.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/test_acquire_command.py` & `acquire-3.7.dev4/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/test_collector.py` & `acquire-3.7.dev4/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/test_esxi_memory.py` & `acquire-3.7.dev4/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/test_file_sorting.py` & `acquire-3.7.dev4/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/test_minio_uploader.py` & `acquire-3.7.dev4/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/test_plugin.py` & `acquire-3.7.dev4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tests/test_utils.py` & `acquire-3.7.dev4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev3/tox.ini` & `acquire-3.7.dev4/tox.ini`

 * *Files identical despite different names*

