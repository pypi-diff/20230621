# Comparing `tmp/s2and-0.17.tar.gz` & `tmp/s2and-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2and-0.17.tar", last modified: Wed Jun 21 11:22:07 2023, max compression
+gzip compressed data, was "s2and-0.18.tar", last modified: Wed Jun 21 11:29:59 2023, max compression
```

## Comparing `s2and-0.17.tar` & `s2and-0.18.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:22:07.132662 s2and-0.17/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.17/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 11:22:07.132526 s2and-0.17/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9477 2023-06-14 16:26:22.000000 s2and-0.17/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:22:07.130206 s2and-0.17/s2and/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.17/s2and/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1762 2023-06-05 12:41:33.000000 s2and-0.17/s2and/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.17/s2and/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    42587 2023-06-20 21:51:56.000000 s2and-0.17/s2and/eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.17/s2and/featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.17/s2and/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1096 2023-06-21 11:18:36.000000 s2and-0.17/s2and/inference.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    48439 2023-06-20 21:51:36.000000 s2and-0.17/s2and/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.17/s2and/plotting_utils.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.17/s2and/s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.17/s2and/sampling.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.17/s2and/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:22:07.130804 s2and-0.17/s2and.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 11:22:07.000000 s2and-0.17/s2and.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-21 11:22:07.000000 s2and-0.17/s2and.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-21 11:22:07.000000 s2and-0.17/s2and.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-21 11:22:07.000000 s2and-0.17/s2and.egg-info/top_level.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-21 11:22:07.132700 s2and-0.17/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-21 11:21:49.000000 s2and-0.17/setup.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:22:07.132339 s2and-0.17/tests/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.17/tests/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_cluster.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_cluster_incremental.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_cluster_incremental_incompatible.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.17/tests/test_text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:29:59.590323 s2and-0.18/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.18/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 11:29:59.590193 s2and-0.18/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9477 2023-06-14 16:26:22.000000 s2and-0.18/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:29:59.588465 s2and-0.18/s2and/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.18/s2and/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1762 2023-06-05 12:41:33.000000 s2and-0.18/s2and/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.18/s2and/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    42587 2023-06-20 21:51:56.000000 s2and-0.18/s2and/eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.18/s2and/featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.18/s2and/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1096 2023-06-21 11:29:51.000000 s2and-0.18/s2and/inference.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    48439 2023-06-20 21:51:36.000000 s2and-0.18/s2and/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.18/s2and/plotting_utils.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.18/s2and/s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.18/s2and/sampling.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.18/s2and/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:29:59.588977 s2and-0.18/s2and.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 11:29:59.000000 s2and-0.18/s2and.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-21 11:29:59.000000 s2and-0.18/s2and.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-21 11:29:59.000000 s2and-0.18/s2and.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-21 11:29:59.000000 s2and-0.18/s2and.egg-info/top_level.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-21 11:29:59.590362 s2and-0.18/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-21 11:29:23.000000 s2and-0.18/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:29:59.590034 s2and-0.18/tests/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.18/tests/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_cluster.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_cluster_incremental.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_cluster_incremental_incompatible.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.18/tests/test_text.py
```

### Comparing `s2and-0.17/LICENSE` & `s2and-0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `s2and-0.17/README.md` & `s2and-0.18/README.md`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/consts.py` & `s2and-0.18/s2and/consts.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/data.py` & `s2and-0.18/s2and/data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/eval.py` & `s2and-0.18/s2and/eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/featurizer.py` & `s2and-0.18/s2and/featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/file_cache.py` & `s2and-0.18/s2and/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/inference.py` & `s2and-0.18/s2and/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os.path import join
 import pickle
 import pprint
 from s2and.data import ANDData
 
 
-def run(path_to_data, dataset_name="pubmed", batch_size=100000000, use_cache=True, n_jobs=96):
+def run(path_to_data, dataset_name="pubmed", batch_size=100000000, use_cache=True, n_jobs=64):
     parent_dir = join(path_to_data, dataset_name)
 
     signatures = join(parent_dir, f"{dataset_name}_signatures.json")
     papers = join(parent_dir, f"{dataset_name}_papers.json")
 
     with open(join(path_to_data, "production_model.pickle"), "rb") as _pkl_file:
         clusterer = pickle.load(_pkl_file)['clusterer']
```

### Comparing `s2and-0.17/s2and/model.py` & `s2and-0.18/s2and/model.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/plotting_utils.py` & `s2and-0.18/s2and/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/s2_funcs.py` & `s2and-0.18/s2and/s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/sampling.py` & `s2and-0.18/s2and/sampling.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and/text.py` & `s2and-0.18/s2and/text.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/s2and.egg-info/SOURCES.txt` & `s2and-0.18/s2and.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_cluster.py` & `s2and-0.18/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_cluster_incremental.py` & `s2and-0.18/tests/test_cluster_incremental.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_cluster_incremental_incompatible.py` & `s2and-0.18/tests/test_cluster_incremental_incompatible.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_data.py` & `s2and-0.18/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_eval.py` & `s2and-0.18/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_featurizer.py` & `s2and-0.18/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_s2_funcs.py` & `s2and-0.18/tests/test_s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.17/tests/test_text.py` & `s2and-0.18/tests/test_text.py`

 * *Files identical despite different names*

