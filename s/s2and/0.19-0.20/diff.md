# Comparing `tmp/s2and-0.19.tar.gz` & `tmp/s2and-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2and-0.19.tar", last modified: Wed Jun 21 11:39:48 2023, max compression
+gzip compressed data, was "s2and-0.20.tar", last modified: Wed Jun 21 15:48:44 2023, max compression
```

## Comparing `s2and-0.19.tar` & `s2and-0.20.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:39:48.686677 s2and-0.19/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.19/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 11:39:48.686555 s2and-0.19/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9477 2023-06-14 16:26:22.000000 s2and-0.19/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:39:48.684702 s2and-0.19/s2and/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.19/s2and/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1762 2023-06-05 12:41:33.000000 s2and-0.19/s2and/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.19/s2and/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    42587 2023-06-20 21:51:56.000000 s2and-0.19/s2and/eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.19/s2and/featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.19/s2and/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1119 2023-06-21 11:39:33.000000 s2and-0.19/s2and/inference.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    48439 2023-06-20 21:51:36.000000 s2and-0.19/s2and/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.19/s2and/plotting_utils.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.19/s2and/s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.19/s2and/sampling.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.19/s2and/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:39:48.685233 s2and-0.19/s2and.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 11:39:48.000000 s2and-0.19/s2and.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-21 11:39:48.000000 s2and-0.19/s2and.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-21 11:39:48.000000 s2and-0.19/s2and.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-21 11:39:48.000000 s2and-0.19/s2and.egg-info/top_level.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-21 11:39:48.686720 s2and-0.19/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-21 11:39:46.000000 s2and-0.19/setup.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 11:39:48.686389 s2and-0.19/tests/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.19/tests/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_cluster.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_cluster_incremental.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_cluster_incremental_incompatible.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.19/tests/test_text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 15:48:44.034801 s2and-0.20/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.20/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 15:48:44.034678 s2and-0.20/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10741 2023-06-21 14:47:32.000000 s2and-0.20/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 15:48:44.032558 s2and-0.20/s2and/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.20/s2and/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1751 2023-06-21 15:46:46.000000 s2and-0.20/s2and/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.20/s2and/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    42587 2023-06-20 21:51:56.000000 s2and-0.20/s2and/eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.20/s2and/featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.20/s2and/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1119 2023-06-21 11:39:33.000000 s2and-0.20/s2and/inference.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    48439 2023-06-20 21:51:36.000000 s2and-0.20/s2and/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.20/s2and/plotting_utils.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.20/s2and/s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.20/s2and/sampling.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.20/s2and/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 15:48:44.033116 s2and-0.20/s2and.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-21 15:48:44.000000 s2and-0.20/s2and.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-21 15:48:44.000000 s2and-0.20/s2and.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-21 15:48:44.000000 s2and-0.20/s2and.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-21 15:48:44.000000 s2and-0.20/s2and.egg-info/top_level.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-21 15:48:44.034840 s2and-0.20/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-21 15:48:34.000000 s2and-0.20/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-21 15:48:44.034489 s2and-0.20/tests/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.20/tests/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_cluster.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_cluster_incremental.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_cluster_incremental_incompatible.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.20/tests/test_text.py
```

### Comparing `s2and-0.19/LICENSE` & `s2and-0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `s2and-0.19/README.md` & `s2and-0.20/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 # Using this fork
 First, following installation instructions below.
 After using my Redshift SQL query to pull papers from the database to a file called *raw_signatures.json*,
 running *process_signatures.py* will create the *clusters.json* (ground truth) and *signatures.json* files, as well as some other JSONs used for creating the *papers.json* file in *create_papers.py*, which should be run after. These JSONs (all three) can be used in *adam_train.py* to train a clusterer model, returning precision, recall, and F1-score metrics. They (*signatures.json* and *papers.json*) can also be used in inference, returning a dictionary of author names (with number suffixes for duplicate names) to lists of signature IDs they are predicted to have contributed to on the papers. Inference can be run with a resulting clusterer model pickle file (or the provided production model) using *adam_test2.py*. 
 
 *adam_prediction_test.py* can be used to test if your setup is working for S2AND inference.
 
+## Creating input JSON files
+First, consult with Ghamut to receive the appropriate queries to generate the necessary files on S3.
+
+Following this, place *raw_signatures.json* in the root directory and just run the Python scripts to do the rest.
+
+### Running the JSON-creating Python scripts
+If *aff_map.json* is not present or provided to you, run
+*create_ror_map.py* and then *create_aff_map.py*. This will take several hours. It is used to map institution IDs to ROR affiliation names using S2AFF results.
+
+The first script to run is *process_signatures.py*. This will create the initial signatures and clusters JSON files as well as some intermediate files.
+
+Next, if *abstracts.json* is not present or provided to you, run *create_abstracts.py*. This will take many hours.
+
+The second script to run is *create_papers.py*. This creates the initial *papers.json* file. It will take many hours.
+
+Following this, you should run *add_abstracts.py* and *add_citations.py* to add abstracts and citations to the *papers.json* file, respectively.
+
+Finally, you should run *prune_signatures.py* to ensure that S2AND will properly process the input JSON files. 
+
+When finished, you will have three, valid S2AND-ready input JSON files (in *data/adam-orcids* by default)!
+
 --------------------------------------------------------------------------------
 
 # S2AND
 This repository provides access to the S2AND dataset and S2AND reference model described in the paper [S2AND: A Benchmark and Evaluation System for Author Name Disambiguation](https://api.semanticscholar.org/CorpusID:232233421) by Shivashankar Subramanian, Daniel King, Doug Downey, Sergey Feldman.
 
 The reference model is live on semanticscholar.org, and the trained model is available now as part of the data download (see below).
```

### Comparing `s2and-0.19/s2and/consts.py` & `s2and-0.20/s2and/consts.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     NAME_COUNTS_PATH = "https://s3-us-west-2.amazonaws.com/ai2-s2-research-public/s2and-release/name_counts.pickle"
 
 FASTTEXT_PATH = os.path.join(CONFIG["main_data_dir"], "lid.176.bin")
 if not os.path.exists(FASTTEXT_PATH):
     FASTTEXT_PATH = "https://s3-us-west-2.amazonaws.com/ai2-s2-research-public/s2and-release/lid.176.bin"
 
 # feature caching related consts
-CACHE_ROOT = Path(os.getenv("S2AND_CACHE", str(Path.home() / ".s2and")))
+CACHE_ROOT = Path(os.getenv("S2AND_CACHE", "/shared/.s2and"))
 """
 Incrementation history
 1 - initial version
 2 - changed to SPECTERv2
 """
 FEATURIZER_VERSION = 2
```

### Comparing `s2and-0.19/s2and/data.py` & `s2and-0.20/s2and/data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/eval.py` & `s2and-0.20/s2and/eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/featurizer.py` & `s2and-0.20/s2and/featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/file_cache.py` & `s2and-0.20/s2and/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/inference.py` & `s2and-0.20/s2and/inference.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/model.py` & `s2and-0.20/s2and/model.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/plotting_utils.py` & `s2and-0.20/s2and/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/s2_funcs.py` & `s2and-0.20/s2and/s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/sampling.py` & `s2and-0.20/s2and/sampling.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and/text.py` & `s2and-0.20/s2and/text.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/s2and.egg-info/SOURCES.txt` & `s2and-0.20/s2and.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_cluster.py` & `s2and-0.20/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_cluster_incremental.py` & `s2and-0.20/tests/test_cluster_incremental.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_cluster_incremental_incompatible.py` & `s2and-0.20/tests/test_cluster_incremental_incompatible.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_data.py` & `s2and-0.20/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_eval.py` & `s2and-0.20/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_featurizer.py` & `s2and-0.20/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_s2_funcs.py` & `s2and-0.20/tests/test_s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.19/tests/test_text.py` & `s2and-0.20/tests/test_text.py`

 * *Files identical despite different names*

