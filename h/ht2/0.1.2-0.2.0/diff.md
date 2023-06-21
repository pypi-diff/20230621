# Comparing `tmp/ht2-0.1.2.tar.gz` & `tmp/ht2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht2-0.1.2.tar", last modified: Thu Jun 15 10:48:40 2023, max compression
+gzip compressed data, was "ht2-0.2.0.tar", last modified: Wed Jun 21 08:32:56 2023, max compression
```

## Comparing `ht2-0.1.2.tar` & `ht2-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.138352 ht2-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-06-12 07:05:14.000000 ht2-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      775 2023-06-15 10:48:40.138352 ht2-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2023-06-15 08:25:10.000000 ht2-0.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)      713 2023-06-15 10:47:36.000000 ht2-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 10:48:40.138352 ht2-0.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.134352 ht2-0.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.138352 ht2-0.1.2/src/ht2/
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-15 10:32:09.000000 ht2-0.1.2/src/ht2/__init__.py
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-12 07:05:14.000000 ht2-0.1.2/src/ht2/example.py
--rw-r--r--   0 root         (0) root         (0)     6351 2023-06-15 06:22:24.000000 ht2-0.1.2/src/ht2/files.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-13 07:59:41.000000 ht2-0.1.2/src/ht2/image.py
--rw-r--r--   0 root         (0) root         (0)      467 2023-06-15 10:31:54.000000 ht2-0.1.2/src/ht2/misc.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-12 09:33:27.000000 ht2-0.1.2/src/ht2/os.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-06-12 07:05:14.000000 ht2-0.1.2/src/ht2/text.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-12 07:05:14.000000 ht2-0.1.2/src/ht2/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.138352 ht2-0.1.2/src/ht2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      775 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:32:56.638401 ht2-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-06-12 07:05:14.000000 ht2-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-21 08:32:56.638401 ht2-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-15 10:51:16.000000 ht2-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      713 2023-06-21 08:30:18.000000 ht2-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 08:32:56.638401 ht2-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:32:56.638401 ht2-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:32:56.638401 ht2-0.2.0/src/ht2/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-21 06:44:04.000000 ht2-0.2.0/src/ht2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:32:56.638401 ht2-0.2.0/src/ht2/snippets/
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-21 07:20:40.000000 ht2-0.2.0/src/ht2/snippets/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:32:56.638401 ht2-0.2.0/src/ht2/utils_dev/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-12 07:05:14.000000 ht2-0.2.0/src/ht2/utils_dev/example.py
+-rw-r--r--   0 root         (0) root         (0)     6341 2023-06-21 08:18:44.000000 ht2-0.2.0/src/ht2/utils_dev/files.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-13 07:59:41.000000 ht2-0.2.0/src/ht2/utils_dev/image.py
+-rw-r--r--   0 root         (0) root         (0)      467 2023-06-15 10:31:54.000000 ht2-0.2.0/src/ht2/utils_dev/misc.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-12 09:33:27.000000 ht2-0.2.0/src/ht2/utils_dev/os.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-12 07:05:14.000000 ht2-0.2.0/src/ht2/utils_dev/text.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-12 07:05:14.000000 ht2-0.2.0/src/ht2/utils_dev/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 08:32:56.638401 ht2-0.2.0/src/ht2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-21 08:32:56.000000 ht2-0.2.0/src/ht2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      424 2023-06-21 08:32:56.000000 ht2-0.2.0/src/ht2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 08:32:56.000000 ht2-0.2.0/src/ht2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-21 08:32:56.000000 ht2-0.2.0/src/ht2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-21 08:32:56.000000 ht2-0.2.0/src/ht2.egg-info/top_level.txt
```

### Comparing `ht2-0.1.2/LICENSE` & `ht2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ht2-0.1.2/PKG-INFO` & `ht2-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ht2
-Version: 0.1.2
+Version: 0.2.0
 Summary: Just a bag of quality of life tools for Machine Learning Engineers
 Author-email: Haotian Zhang <z.haotian@columbia.edu>
 Project-URL: Homepage, https://github.com/htplex/ht2
 Project-URL: Bug Tracker, https://github.com/htplex/ht2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,10 @@
 ## install
 `pip install ht2 ` or
 `pip install ht2 --index-url https://pypi.org/simple`
 
 ## post upgrades
 `python3 -m build`
 `python3 -m twine upload --repository pypi dist/*`
+
+## TODO
+* sphinx documentation
```

### Comparing `ht2-0.1.2/pyproject.toml` & `ht2-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ht2"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Haotian Zhang", email="z.haotian@columbia.edu" },
 ]
 description = "Just a bag of quality of life tools for Machine Learning Engineers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ht2-0.1.2/src/ht2/files.py` & `ht2-0.2.0/src/ht2/utils_dev/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def write_cache(env, cache):
         with env.begin(write=True) as txn:
             for k, v in cache.items():
                 txn.put(k, v)
     
     os.makedirs(export_path, exist_ok=True)
     env = lmdb.open(export_path, map_size=2**40)
-    for i, data in enumerate(tqdm(data_list)):
+    for i, data in enumerate(data_list):
         data_id = str(i).zfill(13)
         data = encoder(data)
         for key,value in data.items():
             if "_" in key:
                 raise ValueError("_ can not be in key, to avoid loading errors")
             cache[f"{data_id}_{key}".encode('utf-8')] = value
 
@@ -58,15 +58,15 @@
     lmdb_env = lmdb.open(data_dir)
     lmdb_txn = lmdb_env.begin()
     lmdb_cursor = lmdb_txn.cursor()
 
     # start loading
     data_list = []
     current_data_id = ""
-    for key, value in tqdm(lmdb_cursor):
+    for key, value in lmdb_cursor:
         data_id,key = key.decode().split("_")
         
         if data_id != current_data_id: # new data line
             if current_data_id:
                 data = decoder(data)
                 data_list.append(data)
             current_data_id = data_id
@@ -115,17 +115,19 @@
         else:
             decoded_dict[key]=value.decode()
 
     return decoded_dict
 
 # generalized encoder/decoder
 
+
+
 def obj_to_bin(obj):
     pickled_data = pickle.dumps(obj)
-    compressed_pickle = zlib.compress(pickled_data, level = 9)
+    compressed_pickle = zlib.compress(pickled_data, level = 1)
     return compressed_pickle
 
 def bin_to_obj(bin):
     depressed_pickle = zlib.decompress(bin)
     obj = pickle.loads(depressed_pickle)
     return obj
```

### Comparing `ht2-0.1.2/src/ht2/image.py` & `ht2-0.2.0/src/ht2/utils_dev/image.py`

 * *Files identical despite different names*

### Comparing `ht2-0.1.2/src/ht2/text.py` & `ht2-0.2.0/src/ht2/utils_dev/text.py`

 * *Files identical despite different names*

### Comparing `ht2-0.1.2/src/ht2.egg-info/PKG-INFO` & `ht2-0.2.0/src/ht2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ht2
-Version: 0.1.2
+Version: 0.2.0
 Summary: Just a bag of quality of life tools for Machine Learning Engineers
 Author-email: Haotian Zhang <z.haotian@columbia.edu>
 Project-URL: Homepage, https://github.com/htplex/ht2
 Project-URL: Bug Tracker, https://github.com/htplex/ht2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,10 @@
 ## install
 `pip install ht2 ` or
 `pip install ht2 --index-url https://pypi.org/simple`
 
 ## post upgrades
 `python3 -m build`
 `python3 -m twine upload --repository pypi dist/*`
+
+## TODO
+* sphinx documentation
```

