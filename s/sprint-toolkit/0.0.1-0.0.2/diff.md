# Comparing `tmp/sprint-toolkit-0.0.1.tar.gz` & `tmp/sprint-toolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprint-toolkit-0.0.1.tar", last modified: Wed Jun 21 14:03:38 2023, max compression
+gzip compressed data, was "sprint-toolkit-0.0.2.tar", last modified: Wed Jun 21 18:36:06 2023, max compression
```

## Comparing `sprint-toolkit-0.0.1.tar` & `sprint-toolkit-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,55 @@
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 14:03:38.605491 sprint-toolkit-0.0.1/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    11348 2023-03-31 16:14:19.000000 sprint-toolkit-0.0.1/LICENSE
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7574 2023-06-21 14:03:38.605491 sprint-toolkit-0.0.1/PKG-INFO
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6732 2023-06-21 13:55:06.000000 sprint-toolkit-0.0.1/README.md
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       38 2023-06-21 14:03:38.605491 sprint-toolkit-0.0.1/setup.cfg
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1117 2023-06-21 14:02:31.000000 sprint-toolkit-0.0.1/setup.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 14:03:38.605491 sprint-toolkit-0.0.1/sprint_toolkit.egg-info/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7574 2023-06-21 14:03:38.000000 sprint-toolkit-0.0.1/sprint_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      215 2023-06-21 14:03:38.000000 sprint-toolkit-0.0.1/sprint_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        1 2023-06-21 14:03:38.000000 sprint-toolkit-0.0.1/sprint_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       14 2023-06-21 14:03:38.000000 sprint-toolkit-0.0.1/sprint_toolkit.egg-info/requires.txt
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        1 2023-06-21 14:03:38.000000 sprint-toolkit-0.0.1/sprint_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.870297 sprint-toolkit-0.0.2/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    11348 2023-03-31 16:14:19.000000 sprint-toolkit-0.0.2/LICENSE
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9674 2023-06-21 18:36:06.870297 sprint-toolkit-0.0.2/PKG-INFO
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     8869 2023-06-21 17:02:38.000000 sprint-toolkit-0.0.2/README.md
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       79 2023-06-21 18:36:06.870297 sprint-toolkit-0.0.2/setup.cfg
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1117 2023-06-21 18:36:03.000000 sprint-toolkit-0.0.2/setup.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.862297 sprint-toolkit-0.0.2/sprint_toolkit/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       50 2023-06-21 18:02:32.000000 sprint-toolkit-0.0.2/sprint_toolkit/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/inference/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       36 2023-03-16 18:11:55.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7441 2023-03-16 18:16:31.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/aio.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1463 2023-03-16 18:25:20.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/data_iters.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6745 2023-03-16 18:37:18.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/encode.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3749 2023-02-18 19:47:29.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/encoder_builders.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2916 2023-06-19 17:12:28.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/evaluate.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2146 2023-01-10 15:57:46.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/index.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      405 2023-03-16 18:11:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/logging.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      327 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    13043 2023-03-16 17:11:56.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/deepimpact.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5812 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/sparta.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5015 2023-03-02 19:25:37.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/splade.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9631 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/tildev2.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7559 2023-02-18 14:25:57.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/unicoil.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5049 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/quantize.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1313 2023-02-18 19:48:23.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/reformat_query.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5164 2023-02-02 15:27:55.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/rerank.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    15528 2023-02-15 16:41:17.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/search.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1010 2023-01-31 15:31:10.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/utils.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       34 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1231 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/MSMARCODataLoader.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3877 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/MSMARCOGroupedDataLoader.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      108 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1940 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/MarginMSELoss.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3203 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/MultipleNegativeRankingLoss.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      122 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      847 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/utils.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/models/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      127 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6036 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/deepimpact.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2453 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/sparta.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     8792 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/splade.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4105 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/tilde.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9426 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/unicoil.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3192 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/utils.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3695 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/trainer.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.862297 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9674 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1674 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        1 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       14 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       15 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/top_level.txt
```

### Comparing `sprint-toolkit-0.0.1/LICENSE` & `sprint-toolkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.1/PKG-INFO` & `sprint-toolkit-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-Metadata-Version: 2.1
-Name: sprint-toolkit
-Version: 0.0.1
-Summary: SPRINT: A Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse Retrieval
-Home-page: https://github.com/thakur-nandan/sprint
-Author: Nandan Thakur
-Author-email: nandant@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/thakur-nandan/sprint/issues
-Keywords: Information Retrieval Toolkit Sparse Retrievers Networks BERT PyTorch IR NLP deep learning
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
 <img style="vertical-align:middle" width="620" height="120" src="./images/sprint-logo.png" />
 </h1>
 
-A Unified Repository to evaluate diverse state-of-the-art neural sparse-retrieval methods in one-click.
+<p align="center">
+    <a href="https://github.com/thakur-nandan/sprint/releases">
+        <img alt="GitHub release" src="https://img.shields.io/badge/release-v0.0.1-blue">
+    </a>
+    <a href="https://www.python.org/">
+            <img alt="Build" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg?color=purple">
+    </a>
+    <a href="https://github.com/thakur-nandan/sprint/blob/master/LICENSE">
+        <img alt="License" src="https://img.shields.io/github/license/thakur-nandan/sprint.svg?color=green">
+    </a>
+    <!-- <a href="https://colab.research.google.com/drive/1HfutiEhHMJLXiWGT8pcipxT5L2TpYEdt?usp=sharing">
+        <img alt="Open In Colab" src="https://colab.research.google.com/assets/colab-badge.svg">
+    </a> -->
+    <a href="https://pepy.tech/project/sprint-toolkit">
+        <img alt="Downloads" src="https://static.pepy.tech/personalized-badge/sprint?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads">
+    </a>
+    <a href="https://github.com/thakur-nandan/sprint/">
+        <img alt="Downloads" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103">
+    </a>
+</p>
+
+<h3 align="center">
+    <a href="https://uwaterloo.ca"><img style="float: left; padding: 2px 7px 2px 7px;" width="213" height="67" src="./images/uwaterloo.png" /></a>
+    <a href="http://www.ukp.tu-darmstadt.de"><img style="float: middle; padding: 2px 7px 2px 7px;" width="147" height="67" src="./images/ukp.png" /></a>
+    <a href="https://www.tu-darmstadt.de/"><img style="float: right; padding: 2px 7px 2px 7px;" width="167.7" height="60" src="./images/tu-darmstadt.png" /></a>
+</h3>
+
+### SPRINT provides a _unified_ repository to easily _evaluate_ diverse state-of-the-art neural (BERT-based) sparse-retrieval models.
+
+SPRINT toolkit allows you to easily search or evaluate any neural sparse retriever across **any** dataset in the BEIR benchmark (or your own dataset). The toolkit is built around as a useful wrapper around Pyserini. The toolkit provides evaluation of seven diverse (neural) sparse retrieval models: [SPLADEv2](https://arxiv.org/abs/2109.10086), [BT-SPLADE-L](https://arxiv.org/abs/2207.03834), [uniCOIL](https://arxiv.org/abs/2106.14807), [TILDEv2](https://arxiv.org/abs/2108.08513), [DeepImpact](https://arxiv.org/abs/2104.12016), [DocT5query](https://cs.uwaterloo.ca/~jimmylin/publications/Nogueira_Lin_2019_docTTTTTquery-v2.pdf) and [SPARTA](https://aclanthology.org/2021.naacl-main.47/).
+
+
+
 
-## Getting Started
-This repo is backed by Pyserini/Anserini, both which relies on Java. To make all the things eaiser, we recommend to follow the steps below via `conda`:
+If you want to read more about the SPRINT toolkit, or wish to know which model to use, please refer to our paper for more details:
+
+* [**SPRINT: A Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse Retrieval**]() (Accepted at SIGIR'23 Resource Track)
+
+## :runner: Getting Started
+SPRINT is backed by Pyserini which relies on Java. To make the installation eaiser, we recommend to follow the steps below via `conda`:
 
 ```bash
 #### Create a new conda environment using conda ####
 $ conda create -n sprint_env python=3.8
 $ conda activate sprint_env
 
 # Install JDK 11 via conda
 $ conda install -c conda-forge openjdk=11
 
-# Install Pyserini, BEIR using PyPI
-$ pip install pyserini
-$ pip install beir
-
-#### Git clone this repository
-$ git clone https://github.com/thakur-nandan/sprint.git
-$ cd sprint
-$ pip install -e .
+# Install SPRINT toolkit using PyPI
+$ pip install sprint-toolkit
 ```
 
+## :runner: Quickstart with SPRINT Toolkit
 
-```bash
-conda env create -f environment.yml  # The Java/JDK dependency will also be installed by running this
-```
-This will create a conda environment named `sparse-retrieval`. So if you want other names, please change the `name` argument in [environment.yml](environment.yml).
-
-To install this repo, just go into the repo and do:  (This is required to run the examples)
-```
-pip install -e .
-```
-
-
-## Inference
 ### Quick start
 For a quick start, we can go to the [example](examples/inference/distilsplade_max/beir_scifact/all_in_one.sh) for evaluating SPLADE (`distilsplade_max`) on the BeIR/SciFact dataset:
 ```bash
 cd examples/inference/distilsplade_max/beir_scifact
 bash all_in_one.sh
 ```
 This will go over the whole pipeline and give the final evaluation results in `beir_scifact-distilsplade_max-quantized/evaluation/metrics.json`:
@@ -175,9 +174,7 @@
 Will be added.
 
 ## Contacts
 The main contributors of this repository are:
 
 - [Nandan Thakur](https://github.com/Nthakur20)
 - [Kexin Wang](https://github.com/kwang2049)
-
-
```

### Comparing `sprint-toolkit-0.0.1/setup.py` & `sprint-toolkit-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 setup(
     name="sprint-toolkit",
-    version="0.0.1",
+    version="0.0.2",
     author="Nandan Thakur",
     author_email="nandant@gmail.com",
     description="SPRINT: A Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse Retrieval",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/thakur-nandan/sprint",
     project_urls={
```

### Comparing `sprint-toolkit-0.0.1/sprint_toolkit.egg-info/PKG-INFO` & `sprint-toolkit-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,474 +1,605 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7370 7269  : 2.1.Name: spri
 00000020: 6e74 2d74 6f6f 6c6b 6974 0a56 6572 7369  nt-toolkit.Versi
-00000030: 6f6e 3a20 302e 302e 310a 5375 6d6d 6172  on: 0.0.1.Summar
+00000030: 6f6e 3a20 302e 302e 320a 5375 6d6d 6172  on: 0.0.2.Summar
 00000040: 793a 2053 5052 494e 543a 2041 2055 6e69  y: SPRINT: A Uni
 00000050: 6669 6564 2054 6f6f 6c6b 6974 2066 6f72  fied Toolkit for
 00000060: 2045 7661 6c75 6174 696e 6720 616e 6420   Evaluating and 
 00000070: 4465 6d79 7374 6966 7969 6e67 205a 6572  Demystifying Zer
 00000080: 6f2d 7368 6f74 204e 6575 7261 6c20 5370  o-shot Neural Sp
 00000090: 6172 7365 2052 6574 7269 6576 616c 0a48  arse Retrieval.H
 000000a0: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
 000000b0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6861  //github.com/tha
 000000c0: 6b75 722d 6e61 6e64 616e 2f73 7072 696e  kur-nandan/sprin
 000000d0: 740a 4175 7468 6f72 3a20 4e61 6e64 616e  t.Author: Nandan
 000000e0: 2054 6861 6b75 720a 4175 7468 6f72 2d65   Thakur.Author-e
 000000f0: 6d61 696c 3a20 6e61 6e64 616e 7440 676d  mail: nandant@gm
-00000100: 6169 6c2e 636f 6d0a 4c69 6365 6e73 653a  ail.com.License:
-00000110: 2055 4e4b 4e4f 574e 0a50 726f 6a65 6374   UNKNOWN.Project
-00000120: 2d55 524c 3a20 4275 6720 5472 6163 6b65  -URL: Bug Tracke
-00000130: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
-00000140: 622e 636f 6d2f 7468 616b 7572 2d6e 616e  b.com/thakur-nan
-00000150: 6461 6e2f 7370 7269 6e74 2f69 7373 7565  dan/sprint/issue
-00000160: 730a 4b65 7977 6f72 6473 3a20 496e 666f  s.Keywords: Info
-00000170: 726d 6174 696f 6e20 5265 7472 6965 7661  rmation Retrieva
-00000180: 6c20 546f 6f6c 6b69 7420 5370 6172 7365  l Toolkit Sparse
-00000190: 2052 6574 7269 6576 6572 7320 4e65 7477   Retrievers Netw
-000001a0: 6f72 6b73 2042 4552 5420 5079 546f 7263  orks BERT PyTorc
-000001b0: 6820 4952 204e 4c50 2064 6565 7020 6c65  h IR NLP deep le
-000001c0: 6172 6e69 6e67 0a50 6c61 7466 6f72 6d3a  arning.Platform:
-000001d0: 2055 4e4b 4e4f 574e 0a43 6c61 7373 6966   UNKNOWN.Classif
-000001e0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000001f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000200: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
-00000210: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000220: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000230: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
-00000240: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
-00000250: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000260: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000270: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
-00000280: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
-00000290: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-000002a0: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
-000002b0: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
-000002c0: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-000002d0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000002e0: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
-000002f0: 680a 5265 7175 6972 6573 2d50 7974 686f  h.Requires-Pytho
-00000300: 6e3a 203e 3d33 2e37 0a44 6573 6372 6970  n: >=3.7.Descrip
-00000310: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00000320: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00000330: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-00000340: 4943 454e 5345 0a0a 3c68 3120 616c 6967  ICENSE..<h1 alig
-00000350: 6e3d 2263 656e 7465 7222 3e0a 3c69 6d67  n="center">.<img
-00000360: 2073 7479 6c65 3d22 7665 7274 6963 616c   style="vertical
-00000370: 2d61 6c69 676e 3a6d 6964 646c 6522 2077  -align:middle" w
-00000380: 6964 7468 3d22 3632 3022 2068 6569 6768  idth="620" heigh
-00000390: 743d 2231 3230 2220 7372 633d 222e 2f69  t="120" src="./i
-000003a0: 6d61 6765 732f 7370 7269 6e74 2d6c 6f67  mages/sprint-log
-000003b0: 6f2e 706e 6722 202f 3e0a 3c2f 6831 3e0a  o.png" />.</h1>.
-000003c0: 0a41 2055 6e69 6669 6564 2052 6570 6f73  .A Unified Repos
-000003d0: 6974 6f72 7920 746f 2065 7661 6c75 6174  itory to evaluat
-000003e0: 6520 6469 7665 7273 6520 7374 6174 652d  e diverse state-
-000003f0: 6f66 2d74 6865 2d61 7274 206e 6575 7261  of-the-art neura
-00000400: 6c20 7370 6172 7365 2d72 6574 7269 6576  l sparse-retriev
-00000410: 616c 206d 6574 686f 6473 2069 6e20 6f6e  al methods in on
-00000420: 652d 636c 6963 6b2e 0a0a 2323 2047 6574  e-click...## Get
-00000430: 7469 6e67 2053 7461 7274 6564 0a54 6869  ting Started.Thi
-00000440: 7320 7265 706f 2069 7320 6261 636b 6564  s repo is backed
-00000450: 2062 7920 5079 7365 7269 6e69 2f41 6e73   by Pyserini/Ans
-00000460: 6572 696e 692c 2062 6f74 6820 7768 6963  erini, both whic
-00000470: 6820 7265 6c69 6573 206f 6e20 4a61 7661  h relies on Java
-00000480: 2e20 546f 206d 616b 6520 616c 6c20 7468  . To make all th
-00000490: 6520 7468 696e 6773 2065 6169 7365 722c  e things eaiser,
-000004a0: 2077 6520 7265 636f 6d6d 656e 6420 746f   we recommend to
-000004b0: 2066 6f6c 6c6f 7720 7468 6520 7374 6570   follow the step
-000004c0: 7320 6265 6c6f 7720 7669 6120 6063 6f6e  s below via `con
-000004d0: 6461 603a 0a0a 6060 6062 6173 680a 2323  da`:..```bash.##
-000004e0: 2323 2043 7265 6174 6520 6120 6e65 7720  ## Create a new 
-000004f0: 636f 6e64 6120 656e 7669 726f 6e6d 656e  conda environmen
-00000500: 7420 7573 696e 6720 636f 6e64 6120 2323  t using conda ##
-00000510: 2323 0a24 2063 6f6e 6461 2063 7265 6174  ##.$ conda creat
-00000520: 6520 2d6e 2073 7072 696e 745f 656e 7620  e -n sprint_env 
-00000530: 7079 7468 6f6e 3d33 2e38 0a24 2063 6f6e  python=3.8.$ con
-00000540: 6461 2061 6374 6976 6174 6520 7370 7269  da activate spri
-00000550: 6e74 5f65 6e76 0a0a 2320 496e 7374 616c  nt_env..# Instal
-00000560: 6c20 4a44 4b20 3131 2076 6961 2063 6f6e  l JDK 11 via con
-00000570: 6461 0a24 2063 6f6e 6461 2069 6e73 7461  da.$ conda insta
-00000580: 6c6c 202d 6320 636f 6e64 612d 666f 7267  ll -c conda-forg
-00000590: 6520 6f70 656e 6a64 6b3d 3131 0a0a 2320  e openjdk=11..# 
-000005a0: 496e 7374 616c 6c20 5079 7365 7269 6e69  Install Pyserini
-000005b0: 2c20 4245 4952 2075 7369 6e67 2050 7950  , BEIR using PyP
-000005c0: 490a 2420 7069 7020 696e 7374 616c 6c20  I.$ pip install 
-000005d0: 7079 7365 7269 6e69 0a24 2070 6970 2069  pyserini.$ pip i
-000005e0: 6e73 7461 6c6c 2062 6569 720a 0a23 2323  nstall beir..###
-000005f0: 2320 4769 7420 636c 6f6e 6520 7468 6973  # Git clone this
-00000600: 2072 6570 6f73 6974 6f72 790a 2420 6769   repository.$ gi
-00000610: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
-00000620: 6769 7468 7562 2e63 6f6d 2f74 6861 6b75  github.com/thaku
-00000630: 722d 6e61 6e64 616e 2f73 7072 696e 742e  r-nandan/sprint.
-00000640: 6769 740a 2420 6364 2073 7072 696e 740a  git.$ cd sprint.
-00000650: 2420 7069 7020 696e 7374 616c 6c20 2d65  $ pip install -e
-00000660: 202e 0a60 6060 0a0a 0a60 6060 6261 7368   ..```...```bash
-00000670: 0a63 6f6e 6461 2065 6e76 2063 7265 6174  .conda env creat
-00000680: 6520 2d66 2065 6e76 6972 6f6e 6d65 6e74  e -f environment
-00000690: 2e79 6d6c 2020 2320 5468 6520 4a61 7661  .yml  # The Java
-000006a0: 2f4a 444b 2064 6570 656e 6465 6e63 7920  /JDK dependency 
-000006b0: 7769 6c6c 2061 6c73 6f20 6265 2069 6e73  will also be ins
-000006c0: 7461 6c6c 6564 2062 7920 7275 6e6e 696e  talled by runnin
-000006d0: 6720 7468 6973 0a60 6060 0a54 6869 7320  g this.```.This 
-000006e0: 7769 6c6c 2063 7265 6174 6520 6120 636f  will create a co
-000006f0: 6e64 6120 656e 7669 726f 6e6d 656e 7420  nda environment 
-00000700: 6e61 6d65 6420 6073 7061 7273 652d 7265  named `sparse-re
-00000710: 7472 6965 7661 6c60 2e20 536f 2069 6620  trieval`. So if 
-00000720: 796f 7520 7761 6e74 206f 7468 6572 206e  you want other n
-00000730: 616d 6573 2c20 706c 6561 7365 2063 6861  ames, please cha
-00000740: 6e67 6520 7468 6520 606e 616d 6560 2061  nge the `name` a
-00000750: 7267 756d 656e 7420 696e 205b 656e 7669  rgument in [envi
-00000760: 726f 6e6d 656e 742e 796d 6c5d 2865 6e76  ronment.yml](env
-00000770: 6972 6f6e 6d65 6e74 2e79 6d6c 292e 0a0a  ironment.yml)...
-00000780: 546f 2069 6e73 7461 6c6c 2074 6869 7320  To install this 
-00000790: 7265 706f 2c20 6a75 7374 2067 6f20 696e  repo, just go in
-000007a0: 746f 2074 6865 2072 6570 6f20 616e 6420  to the repo and 
-000007b0: 646f 3a20 2028 5468 6973 2069 7320 7265  do:  (This is re
-000007c0: 7175 6972 6564 2074 6f20 7275 6e20 7468  quired to run th
-000007d0: 6520 6578 616d 706c 6573 290a 6060 600a  e examples).```.
-000007e0: 7069 7020 696e 7374 616c 6c20 2d65 202e  pip install -e .
-000007f0: 0a60 6060 0a0a 0a23 2320 496e 6665 7265  .```...## Infere
-00000800: 6e63 650a 2323 2320 5175 6963 6b20 7374  nce.### Quick st
-00000810: 6172 740a 466f 7220 6120 7175 6963 6b20  art.For a quick 
-00000820: 7374 6172 742c 2077 6520 6361 6e20 676f  start, we can go
-00000830: 2074 6f20 7468 6520 5b65 7861 6d70 6c65   to the [example
-00000840: 5d28 6578 616d 706c 6573 2f69 6e66 6572  ](examples/infer
-00000850: 656e 6365 2f64 6973 7469 6c73 706c 6164  ence/distilsplad
-00000860: 655f 6d61 782f 6265 6972 5f73 6369 6661  e_max/beir_scifa
-00000870: 6374 2f61 6c6c 5f69 6e5f 6f6e 652e 7368  ct/all_in_one.sh
-00000880: 2920 666f 7220 6576 616c 7561 7469 6e67  ) for evaluating
-00000890: 2053 504c 4144 4520 2860 6469 7374 696c   SPLADE (`distil
-000008a0: 7370 6c61 6465 5f6d 6178 6029 206f 6e20  splade_max`) on 
-000008b0: 7468 6520 4265 4952 2f53 6369 4661 6374  the BeIR/SciFact
-000008c0: 2064 6174 6173 6574 3a0a 6060 6062 6173   dataset:.```bas
-000008d0: 680a 6364 2065 7861 6d70 6c65 732f 696e  h.cd examples/in
-000008e0: 6665 7265 6e63 652f 6469 7374 696c 7370  ference/distilsp
-000008f0: 6c61 6465 5f6d 6178 2f62 6569 725f 7363  lade_max/beir_sc
-00000900: 6966 6163 740a 6261 7368 2061 6c6c 5f69  ifact.bash all_i
-00000910: 6e5f 6f6e 652e 7368 0a60 6060 0a54 6869  n_one.sh.```.Thi
-00000920: 7320 7769 6c6c 2067 6f20 6f76 6572 2074  s will go over t
-00000930: 6865 2077 686f 6c65 2070 6970 656c 696e  he whole pipelin
-00000940: 6520 616e 6420 6769 7665 2074 6865 2066  e and give the f
-00000950: 696e 616c 2065 7661 6c75 6174 696f 6e20  inal evaluation 
-00000960: 7265 7375 6c74 7320 696e 2060 6265 6972  results in `beir
-00000970: 5f73 6369 6661 6374 2d64 6973 7469 6c73  _scifact-distils
-00000980: 706c 6164 655f 6d61 782d 7175 616e 7469  plade_max-quanti
-00000990: 7a65 642f 6576 616c 7561 7469 6f6e 2f6d  zed/evaluation/m
-000009a0: 6574 7269 6373 2e6a 736f 6e60 3a0a 0a3c  etrics.json`:..<
-000009b0: 6465 7461 696c 733e 0a20 203c 7375 6d6d  details>.  <summ
-000009c0: 6172 793e 5265 7375 6c74 733a 2064 6973  ary>Results: dis
-000009d0: 7469 6c73 706c 6164 655f 6d61 7820 6f6e  tilsplade_max on
-000009e0: 2042 6549 522f 5363 6946 6163 743c 2f73   BeIR/SciFact</s
-000009f0: 756d 6d61 7279 3e0a 2020 0a20 2060 6060  ummary>.  .  ```
-00000a00: 6261 7368 0a20 2020 2020 6361 7420 6265  bash.     cat be
-00000a10: 6972 5f73 6369 6661 6374 2d64 6973 7469  ir_scifact-disti
-00000a20: 6c73 706c 6164 655f 6d61 782d 7175 616e  lsplade_max-quan
-00000a30: 7469 7a65 642f 6576 616c 7561 7469 6f6e  tized/evaluation
-00000a40: 2f6d 6574 7269 6373 2e6a 736f 6e20 0a20  /metrics.json . 
-00000a50: 2020 2020 2320 7b0a 2020 2020 2023 2020      # {.     #  
-00000a60: 2020 2022 6e44 4347 223a 207b 0a20 2020     "nDCG": {.   
-00000a70: 2020 2320 2020 2020 2020 2020 224e 4443    #         "NDC
-00000a80: 4740 3122 3a20 302e 3630 3333 332c 0a20  G@1": 0.60333,. 
-00000a90: 2020 2020 2320 2020 2020 2020 2020 224e      #         "N
-00000aa0: 4443 4740 3322 3a20 302e 3635 3936 392c  DCG@3": 0.65969,
-00000ab0: 0a20 2020 2020 2320 2020 2020 2020 2020  .     #         
-00000ac0: 224e 4443 4740 3522 3a20 302e 3637 3230  "NDCG@5": 0.6720
-00000ad0: 342c 0a20 2020 2020 2320 2020 2020 2020  4,.     #       
-00000ae0: 2020 224e 4443 4740 3130 223a 2030 2e36    "NDCG@10": 0.6
-00000af0: 3932 352c 0a20 2020 2020 2320 2020 2020  925,.     #     
-00000b00: 2020 2020 224e 4443 4740 3130 3022 3a20      "NDCG@100": 
-00000b10: 302e 3732 3032 2c0a 2020 2020 2023 2020  0.7202,.     #  
-00000b20: 2020 2020 2020 2022 4e44 4347 4031 3030         "NDCG@100
-00000b30: 3022 3a20 302e 3732 3735 330a 2020 2020  0": 0.72753.    
-00000b40: 2023 2020 2020 207d 2c0a 2020 2020 2023   #     },.     #
-00000b50: 2020 2020 2022 4d41 5022 3a20 7b0a 2020       "MAP": {.  
-00000b60: 2020 2023 2020 2020 2020 2020 2022 4d41     #         "MA
-00000b70: 5040 3122 3a20 302e 3537 3231 372c 0a20  P@1": 0.57217,. 
-00000b80: 2020 2020 2320 2020 2020 2e2e 2e0a 2020      #     ....  
-00000b90: 2020 2023 207d 0a20 2060 6060 0a3c 2f64     # }.  ```.</d
-00000ba0: 6574 6169 6c73 3e0a 0a4f 7220 6966 2079  etails>..Or if y
-00000bb0: 6f75 206c 696b 6520 7275 6e6e 696e 6720  ou like running 
-00000bc0: 7079 7468 6f6e 2064 6972 6563 746c 792c  python directly,
-00000bd0: 206a 7573 7420 7275 6e20 7468 6520 636f   just run the co
-00000be0: 6465 2073 6e69 7070 6574 2062 656c 6f77  de snippet below
-00000bf0: 2066 6f72 2065 7661 6c75 6174 696e 6720   for evaluating 
-00000c00: 6063 6173 746f 7269 6e69 2f75 6e69 636f  `castorini/unico
-00000c10: 696c 2d6e 6f65 7870 2d6d 736d 6172 636f  il-noexp-msmarco
-00000c20: 2d70 6173 7361 6765 6020 6f6e 2060 4265  -passage` on `Be
-00000c30: 4952 2f53 6369 4661 6374 603a 0a60 6060  IR/SciFact`:.```
-00000c40: 7079 7468 6f6e 0a66 726f 6d20 7370 7269  python.from spri
-00000c50: 6e74 2e69 6e66 6572 656e 6365 2069 6d70  nt.inference imp
-00000c60: 6f72 7420 6169 6f0a 0a0a 6966 205f 5f6e  ort aio...if __n
-00000c70: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-00000c80: 5f5f 273a 2020 2320 6169 6f2e 7275 6e20  __':  # aio.run 
-00000c90: 6361 6e20 6f6e 6c79 2062 6520 6361 6c6c  can only be call
-00000ca0: 6564 2077 6974 6869 6e20 5f5f 6d61 696e  ed within __main
-00000cb0: 5f5f 0a20 2020 2061 696f 2e72 756e 280a  __.    aio.run(.
-00000cc0: 2020 2020 2020 2020 656e 636f 6465 725f          encoder_
-00000cd0: 6e61 6d65 3d27 756e 6963 6f69 6c27 2c0a  name='unicoil',.
-00000ce0: 2020 2020 2020 2020 636b 7074 5f6e 616d          ckpt_nam
-00000cf0: 653d 2763 6173 746f 7269 6e69 2f75 6e69  e='castorini/uni
-00000d00: 636f 696c 2d6e 6f65 7870 2d6d 736d 6172  coil-noexp-msmar
-00000d10: 636f 2d70 6173 7361 6765 272c 0a20 2020  co-passage',.   
-00000d20: 2020 2020 2064 6174 615f 6e61 6d65 3d27       data_name='
-00000d30: 6265 6972 2f73 6369 6661 6374 272c 0a20  beir/scifact',. 
-00000d40: 2020 2020 2020 2067 7075 733d 5b30 2c20         gpus=[0, 
-00000d50: 315d 2c0a 2020 2020 2020 2020 6f75 7470  1],.        outp
-00000d60: 7574 5f64 6972 3d27 6265 6972 5f73 6369  ut_dir='beir_sci
-00000d70: 6661 6374 2d75 6e69 636f 696c 5f6e 6f65  fact-unicoil_noe
-00000d80: 7870 272c 0a20 2020 2020 2020 2064 6f5f  xp',.        do_
-00000d90: 7175 616e 7469 7a61 7469 6f6e 3d54 7275  quantization=Tru
-00000da0: 652c 0a20 2020 2020 2020 2071 7561 6e74  e,.        quant
-00000db0: 697a 6174 696f 6e5f 6d65 7468 6f64 3d27  ization_method='
-00000dc0: 7261 6e67 652d 6e62 6974 7327 2c20 2023  range-nbits',  #
-00000dd0: 2053 6f20 7468 6520 646f 6320 7465 726d   So the doc term
-00000de0: 2077 6569 6768 7473 2077 696c 6c20 6265   weights will be
-00000df0: 2071 7561 6e74 697a 6564 2062 7920 6028   quantized by `(
-00000e00: 7465 726d 5f77 6569 6768 7473 202f 2035  term_weights / 5
-00000e10: 2920 2a20 2832 202a 2a20 3829 600a 2020  ) * (2 ** 8)`.  
-00000e20: 2020 2020 2020 6f72 6967 696e 616c 5f73        original_s
-00000e30: 636f 7265 5f72 616e 6765 3d35 2c0a 2020  core_range=5,.  
-00000e40: 2020 2020 2020 7175 616e 7469 7a61 7469        quantizati
-00000e50: 6f6e 5f6e 6269 7473 3d38 2c0a 2020 2020  on_nbits=8,.    
-00000e60: 2020 2020 6f72 6967 696e 616c 5f71 7565      original_que
-00000e70: 7279 5f66 6f72 6d61 743d 2762 6569 7227  ry_format='beir'
-00000e80: 2c0a 2020 2020 2020 2020 746f 7069 635f  ,.        topic_
-00000e90: 7370 6c69 743d 2774 6573 7427 0a20 2020  split='test'.   
-00000ea0: 2029 0a20 2020 2023 2059 6f75 2077 6f75   ).    # You wou
-00000eb0: 6c64 2067 6574 2022 4e44 4347 4031 3022  ld get "NDCG@10"
-00000ec0: 3a20 302e 3638 3536 330a 6060 600a 2323  : 0.68563.```.##
-00000ed0: 2320 5374 6570 2062 7920 7374 6570 0a4f  # Step by step.O
-00000ee0: 6e65 2063 616e 2061 6c73 6f20 7275 6e20  ne can also run 
-00000ef0: 7468 6520 6162 6f76 6520 7072 6f63 6573  the above proces
-00000f00: 7320 696e 2036 2073 6570 6172 6174 6520  s in 6 separate 
-00000f10: 7374 6570 7320 756e 6465 7220 7468 6520  steps under the 
-00000f20: 5b73 7465 705f 6279 5f73 7465 705d 2865  [step_by_step](e
-00000f30: 7861 6d70 6c65 732f 696e 6665 7265 6e63  xamples/inferenc
-00000f40: 652f 6469 7374 696c 7370 6c61 6465 5f6d  e/distilsplade_m
-00000f50: 6178 2f62 6569 725f 7363 6966 6163 742f  ax/beir_scifact/
-00000f60: 7374 6570 5f62 795f 7374 6570 2920 666f  step_by_step) fo
-00000f70: 6c64 6572 3a0a 312e 205b 656e 636f 6465  lder:.1. [encode
-00000f80: 5d28 6578 616d 706c 6573 2f69 6e66 6572  ](examples/infer
-00000f90: 656e 6365 2f64 6973 7469 6c73 706c 6164  ence/distilsplad
-00000fa0: 655f 6d61 782f 6265 6972 5f73 6369 6661  e_max/beir_scifa
-00000fb0: 6374 2f73 7465 705f 6279 5f73 7465 702f  ct/step_by_step/
-00000fc0: 312e 656e 636f 6465 2e62 6569 725f 7363  1.encode.beir_sc
-00000fd0: 6966 6163 742d 6469 7374 696c 7370 6c61  ifact-distilspla
-00000fe0: 6465 5f6d 6178 2d66 6c6f 6174 2e73 6829  de_max-float.sh)
-00000ff0: 3a20 456e 636f 6465 2064 6f63 756d 656e  : Encode documen
-00001000: 7473 2069 6e74 6f20 7465 726d 2077 6569  ts into term wei
-00001010: 6768 7473 2062 7920 6d75 6c74 6970 726f  ghts by multipro
-00001020: 6365 7373 696e 6720 6f6e 206d 7574 6c69  cessing on mutli
-00001030: 706c 6520 4750 5573 3b0a 322e 205b 7175  ple GPUs;.2. [qu
-00001040: 616e 7469 7a65 5d28 6578 616d 706c 6573  antize](examples
-00001050: 2f69 6e66 6572 656e 6365 2f64 6973 7469  /inference/disti
-00001060: 6c73 706c 6164 655f 6d61 782f 6265 6972  lsplade_max/beir
-00001070: 5f73 6369 6661 6374 2f73 7465 705f 6279  _scifact/step_by
-00001080: 5f73 7465 702f 322e 7175 616e 7469 7a65  _step/2.quantize
-00001090: 2e62 6569 725f 7363 6966 6163 742d 6469  .beir_scifact-di
-000010a0: 7374 696c 7370 6c61 6465 5f6d 6178 2d32  stilsplade_max-2
-000010b0: 6469 6769 7473 2e73 6829 3a20 5175 616e  digits.sh): Quan
-000010c0: 7469 7a65 2074 6865 2064 6f63 756d 656e  tize the documen
-000010d0: 7420 7465 726d 2077 6569 6768 7473 2069  t term weights i
-000010e0: 6e74 6f20 696e 7465 6765 7273 2028 6361  nto integers (ca
-000010f0: 6e20 6265 2073 6361 7065 6429 3b0a 332e  n be scaped);.3.
-00001100: 205b 696e 6465 785d 2865 7861 6d70 6c65   [index](example
-00001110: 732f 696e 6665 7265 6e63 652f 6469 7374  s/inference/dist
-00001120: 696c 7370 6c61 6465 5f6d 6178 2f62 6569  ilsplade_max/bei
-00001130: 725f 7363 6966 6163 742f 7374 6570 5f62  r_scifact/step_b
-00001140: 795f 7374 6570 2f33 2e69 6e64 6578 2e62  y_step/3.index.b
-00001150: 6569 725f 7363 6966 6163 742d 6469 7374  eir_scifact-dist
-00001160: 696c 7370 6c61 6465 5f6d 6178 2d32 6469  ilsplade_max-2di
-00001170: 6769 7473 2e73 6829 3a20 496e 6465 7820  gits.sh): Index 
-00001180: 7468 6520 7465 726d 2077 6569 6768 7473  the term weights
-00001190: 2069 6e20 746f 204c 7563 656e 6520 696e   in to Lucene in
-000011a0: 6465 7820 2862 6163 6b65 6e64 6564 2062  dex (backended b
-000011b0: 7920 5079 7365 7269 6e69 293b 0a34 2e20  y Pyserini);.4. 
-000011c0: 5b72 6566 6f72 6d61 745d 2865 7861 6d70  [reformat](examp
-000011d0: 6c65 732f 696e 6665 7265 6e63 652f 6469  les/inference/di
-000011e0: 7374 696c 7370 6c61 6465 5f6d 6178 2f62  stilsplade_max/b
-000011f0: 6569 725f 7363 6966 6163 742f 7374 6570  eir_scifact/step
-00001200: 5f62 795f 7374 6570 2f34 2e72 6566 6f72  _by_step/4.refor
-00001210: 6d61 745f 7175 6572 792e 6265 6972 5f73  mat_query.beir_s
-00001220: 6369 6661 6374 2e73 6829 3a20 5265 666f  cifact.sh): Refo
-00001230: 726d 6174 2074 6865 2071 7565 7269 6573  rmat the queries
-00001240: 2066 696c 6520 2865 2e67 2e20 7468 6520   file (e.g. the 
-00001250: 6f6e 6573 2066 726f 6d20 4265 4952 2920  ones from BeIR) 
-00001260: 696e 746f 2074 6865 2050 7973 6572 696e  into the Pyserin
-00001270: 6920 666f 726d 6174 3b0a 352e 205b 7365  i format;.5. [se
-00001280: 6172 6368 5d28 6578 616d 706c 6573 2f69  arch](examples/i
-00001290: 6e66 6572 656e 6365 2f64 6973 7469 6c73  nference/distils
-000012a0: 706c 6164 655f 6d61 782f 6265 6972 5f73  plade_max/beir_s
-000012b0: 6369 6661 6374 2f73 7465 705f 6279 5f73  cifact/step_by_s
-000012c0: 7465 702f 352e 7365 6172 6368 2e62 6569  tep/5.search.bei
-000012d0: 725f 7363 6966 6163 742d 6469 7374 696c  r_scifact-distil
-000012e0: 7370 6c61 6465 5f6d 6178 2d32 6469 6769  splade_max-2digi
-000012f0: 7473 2e73 6829 3a20 5265 7472 6965 7665  ts.sh): Retrieve
-00001300: 2074 6865 2072 656c 6576 616e 7420 646f   the relevant do
-00001310: 6375 6d65 6e74 7320 2862 6163 6b65 6e64  cuments (backend
-00001320: 6564 2062 7920 5079 7365 7269 6e69 293b  ed by Pyserini);
-00001330: 0a36 2e20 5b65 7661 6c75 6174 655d 2865  .6. [evaluate](e
-00001340: 7861 6d70 6c65 732f 696e 6665 7265 6e63  xamples/inferenc
-00001350: 652f 6469 7374 696c 7370 6c61 6465 5f6d  e/distilsplade_m
-00001360: 6178 2f62 6569 725f 7363 6966 6163 742f  ax/beir_scifact/
-00001370: 7374 6570 5f62 795f 7374 6570 2f36 2e65  step_by_step/6.e
-00001380: 7661 6c75 6174 652e 6265 6972 5f73 6369  valuate.beir_sci
-00001390: 6661 6374 2d64 6973 7469 6c73 706c 6164  fact-distilsplad
-000013a0: 655f 6d61 782d 3264 6967 6974 732e 7368  e_max-2digits.sh
-000013b0: 293a 2045 7661 6c75 6174 6520 7468 6520  ): Evaluate the 
-000013c0: 7265 7375 6c74 7320 6167 6169 6e73 7420  results against 
-000013d0: 6120 6365 7274 6169 6e20 6c61 6265 6c65  a certain labele
-000013e0: 6420 6461 7461 2c20 652e 672e 7468 6520  d data, e.g.the 
-000013f0: 7172 656c 7320 7573 6564 2069 6e20 4265  qrels used in Be
-00001400: 4952 2028 6261 636b 656e 6465 6420 6279  IR (backended by
-00001410: 2042 6549 5229 0a0a 4375 7272 656e 746c   BeIR)..Currentl
-00001420: 7920 6974 202a 2a64 6972 6563 746c 792a  y it **directly*
-00001430: 2a20 7375 7070 6f72 7473 206d 6574 686f  * supports metho
-00001440: 6473 2028 7769 7468 2072 6570 726f 6475  ds (with reprodu
-00001450: 6374 696f 6e20 7665 7269 6669 6564 293a  ction verified):
-00001460: 0a2d 2075 6e69 434f 494c 3b0a 2d20 5350  .- uniCOIL;.- SP
-00001470: 4c41 4445 3a20 476f 2074 6f20 5b65 7861  LADE: Go to [exa
-00001480: 6d70 6c65 732f 696e 6665 7265 6e63 652f  mples/inference/
-00001490: 6469 7374 696c 7370 6c61 6465 5f6d 6178  distilsplade_max
-000014a0: 2f62 6569 725f 7363 6966 6163 745d 2865  /beir_scifact](e
-000014b0: 7861 6d70 6c65 732f 696e 6665 7265 6e63  xamples/inferenc
-000014c0: 652f 6469 7374 696c 7370 6c61 6465 5f6d  e/distilsplade_m
-000014d0: 6178 2f62 6569 725f 7363 6966 6163 7429  ax/beir_scifact)
-000014e0: 2066 6f72 2066 6173 7420 7265 7072 6f64   for fast reprod
-000014f0: 7563 696e 6720 6064 6973 7469 6c73 706c  ucing `distilspl
-00001500: 6164 655f 6d61 7860 206f 6e20 5363 6946  ade_max` on SciF
-00001510: 6163 743b 0a2d 2053 5041 5254 413b 0a2d  act;.- SPARTA;.-
-00001520: 2054 494c 4445 7632 3a20 476f 2074 6f20   TILDEv2: Go to 
-00001530: 5b65 7861 6d70 6c65 732f 696e 6665 7265  [examples/infere
-00001540: 6e63 652f 7469 6c64 6576 322d 6e6f 6578  nce/tildev2-noex
-00001550: 702f 7472 6563 646c 3230 3139 5d28 6578  p/trecdl2019](ex
-00001560: 616d 706c 6573 2f69 6e66 6572 656e 6365  amples/inference
-00001570: 2f74 696c 6465 7632 2d6e 6f65 7870 2f74  /tildev2-noexp/t
-00001580: 7265 6364 6c32 3031 3929 2066 6f72 2066  recdl2019) for f
-00001590: 6173 7420 7265 7072 6f64 7563 696e 6720  ast reproducing 
-000015a0: 6069 656c 6162 2f54 494c 4445 7632 2d6e  `ielab/TILDEv2-n
-000015b0: 6f45 7870 6020 7265 7261 6e6b 696e 6720  oExp` reranking 
-000015c0: 6f6e 2054 5245 432d 444c 2032 3031 393b  on TREC-DL 2019;
-000015d0: 0a2d 2044 6565 7049 6d70 6163 740a 0a43  .- DeepImpact..C
-000015e0: 7572 7265 6e74 6c79 2069 7420 7375 7070  urrently it supp
-000015f0: 6f72 7473 2064 6174 6120 666f 726d 6174  orts data format
-00001600: 7320 2862 7920 646f 776e 6c6f 6164 696e  s (by downloadin
-00001610: 6720 6175 746f 6d61 7469 6361 6c6c 7929  g automatically)
-00001620: 3a0a 2d20 4265 4952 0a0a 4f74 6865 7220  :.- BeIR..Other 
-00001630: 6d6f 6465 6c73 2061 6e64 2064 6174 6120  models and data 
-00001640: 2866 6f72 6d61 7473 2920 7769 6c6c 2062  (formats) will b
-00001650: 6520 6164 6465 642e 0a0a 2323 2320 4375  e added...### Cu
-00001660: 7374 6f6d 2065 6e63 6f64 6572 730a 546f  stom encoders.To
-00001670: 2061 6464 2061 2063 7573 746f 6d20 656e   add a custom en
-00001680: 636f 6465 722c 206f 6e65 2063 616e 2072  coder, one can r
-00001690: 6566 6572 2074 6f20 7468 6520 6578 616d  efer to the exam
-000016a0: 706c 6520 5b65 7861 6d70 6c65 732f 696e  ple [examples/in
-000016b0: 6665 7265 6e63 652f 6375 7374 6f6d 5f65  ference/custom_e
-000016c0: 6e63 6f64 6572 2f62 6569 725f 7363 6966  ncoder/beir_scif
-000016d0: 6163 745d 2865 7861 6d70 6c65 732f 696e  act](examples/in
-000016e0: 6665 7265 6e63 652f 6375 7374 6f6d 5f65  ference/custom_e
-000016f0: 6e63 6f64 6572 2f62 6569 725f 7363 6966  ncoder/beir_scif
-00001700: 6163 7429 2c20 7768 6572 6520 6064 6973  act), where `dis
-00001710: 7469 6c73 706c 6164 655f 6d61 7860 2069  tilsplade_max` i
-00001720: 7320 6576 616c 7561 7465 6420 6f6e 2060  s evaluated on `
-00001730: 4265 4952 2f53 6369 4661 6374 6020 2a2a  BeIR/SciFact` **
-00001740: 7769 7468 2073 746f 7077 6f72 6473 2066  with stopwords f
-00001750: 696c 7465 7265 6420 6f75 742a 2a2e 0a0a  iltered out**...
-00001760: 496e 2064 6574 6169 6c2c 206f 6e65 206a  In detail, one j
-00001770: 7573 7420 6e65 6564 7320 746f 2064 6566  ust needs to def
-00001780: 696e 6520 796f 7572 2063 7573 746f 6d20  ine your custom 
-00001790: 656e 636f 6465 7220 636c 6173 7320 616e  encoder class an
-000017a0: 6420 7772 6974 6520 6120 6e65 7720 656e  d write a new en
-000017b0: 636f 6465 7220 6275 696c 6465 7220 6675  coder builder fu
-000017c0: 6e63 7469 6f6e 3a0a 6060 6070 7974 686f  nction:.```pytho
-000017d0: 6e0a 6672 6f6d 2074 7970 696e 6720 696d  n.from typing im
-000017e0: 706f 7274 2044 6963 742c 204c 6973 740a  port Dict, List.
-000017f0: 6672 6f6d 2070 7973 6572 696e 692e 656e  from pyserini.en
-00001800: 636f 6465 2069 6d70 6f72 7420 5175 6572  code import Quer
-00001810: 7945 6e63 6f64 6572 2c20 446f 6375 6d65  yEncoder, Docume
-00001820: 6e74 456e 636f 6465 720a 0a63 6c61 7373  ntEncoder..class
-00001830: 2043 7573 746f 6d51 7565 7279 456e 636f   CustomQueryEnco
-00001840: 6465 7228 5175 6572 7945 6e63 6f64 6572  der(QueryEncoder
-00001850: 293a 0a0a 2020 2020 6465 6620 656e 636f  ):..    def enco
-00001860: 6465 2873 656c 662c 2074 6578 742c 202a  de(self, text, *
-00001870: 2a6b 7761 7267 7329 202d 3e20 4469 6374  *kwargs) -> Dict
-00001880: 5b73 7472 2c20 666c 6f61 745d 3a0a 2020  [str, float]:.  
-00001890: 2020 2020 2020 2320 4a75 7374 2061 6e20        # Just an 
-000018a0: 6578 616d 706c 653a 0a20 2020 2020 2020  example:.       
-000018b0: 2074 6572 6d73 203d 2074 6578 742e 7370   terms = text.sp
-000018c0: 6c69 7428 290a 2020 2020 2020 2020 7465  lit().        te
-000018d0: 726d 5f77 6569 6768 7473 203d 207b 7465  rm_weights = {te
-000018e0: 726d 3a20 3120 666f 7220 7465 726d 2069  rm: 1 for term i
-000018f0: 6e20 7465 726d 737d 0a20 2020 2020 2020  n terms}.       
-00001900: 2072 6574 7572 6e20 7465 726d 5f77 6569   return term_wei
-00001910: 6768 7473 2020 2320 4469 6374 206f 626a  ghts  # Dict obj
-00001920: 6563 742c 2077 6865 7265 206b 6579 732f  ect, where keys/
-00001930: 7661 6c75 6573 2061 7265 2074 6572 6d73  values are terms
-00001940: 2f74 6572 6d20 7363 6f72 6573 2c20 7265  /term scores, re
-00001950: 7370 2e0a 0a63 6c61 7373 2043 7573 746f  sp...class Custo
-00001960: 6d44 6f63 756d 656e 7445 6e63 6f64 6572  mDocumentEncoder
-00001970: 2844 6f63 756d 656e 7445 6e63 6f64 6572  (DocumentEncoder
-00001980: 293a 0a0a 2020 2020 6465 6620 656e 636f  ):..    def enco
-00001990: 6465 2873 656c 662c 2074 6578 7473 2c20  de(self, texts, 
-000019a0: 2a2a 6b77 6172 6773 2920 2d3e 204c 6973  **kwargs) -> Lis
-000019b0: 745b 4469 6374 5b73 7472 2c20 666c 6f61  t[Dict[str, floa
-000019c0: 745d 5d3a 0a20 2020 2020 2020 2023 204a  t]]:.        # J
-000019d0: 7573 7420 616e 2065 7861 6d70 6c65 3a0a  ust an example:.
-000019e0: 2020 2020 2020 2020 7465 726d 5f77 6569          term_wei
-000019f0: 6768 7473 5f62 6174 6368 203d 205b 5d0a  ghts_batch = [].
-00001a00: 2020 2020 2020 2020 666f 7220 7465 7874          for text
-00001a10: 2069 6e20 7465 7874 733a 0a20 2020 2020   in texts:.     
-00001a20: 2020 2020 2020 2074 6572 6d73 203d 2074         terms = t
-00001a30: 6578 742e 7370 6c69 7428 290a 2020 2020  ext.split().    
-00001a40: 2020 2020 2020 2020 7465 726d 5f77 6569          term_wei
-00001a50: 6768 7473 203d 207b 7465 726d 3a20 3120  ghts = {term: 1 
-00001a60: 666f 7220 7465 726d 2069 6e20 7465 726d  for term in term
-00001a70: 737d 0a20 2020 2020 2020 2020 2020 2074  s}.            t
-00001a80: 6572 6d5f 7765 6967 6874 735f 6261 7463  erm_weights_batc
-00001a90: 682e 6170 7065 6e64 2874 6572 6d5f 7765  h.append(term_we
-00001aa0: 6967 6874 7329 0a20 2020 2020 2020 2072  ights).        r
-00001ab0: 6574 7572 6e20 7465 726d 5f77 6569 6768  eturn term_weigh
-00001ac0: 7473 5f62 6174 6368 200a 0a64 6566 2063  ts_batch ..def c
-00001ad0: 7573 746f 6d5f 656e 636f 6465 725f 6275  ustom_encoder_bu
-00001ae0: 696c 6465 7228 636b 7074 5f6e 616d 652c  ilder(ckpt_name,
-00001af0: 2065 7479 7065 2c20 6465 7669 6365 3d27   etype, device='
-00001b00: 6370 7527 293a 0a20 2020 2069 6620 6574  cpu'):.    if et
-00001b10: 7970 6520 3d3d 2027 7175 6572 7927 3a0a  ype == 'query':.
-00001b20: 2020 2020 2020 2020 7265 7475 726e 2043          return C
-00001b30: 7573 746f 6d51 7565 7279 456e 636f 6465  ustomQueryEncode
-00001b40: 7228 636b 7074 5f6e 616d 652c 2064 6576  r(ckpt_name, dev
-00001b50: 6963 653d 6465 7669 6365 2920 2020 2020  ice=device)     
-00001b60: 2020 200a 2020 2020 656c 6966 2065 7479     .    elif ety
-00001b70: 7065 203d 3d20 2764 6f63 756d 656e 7427  pe == 'document'
-00001b80: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00001b90: 2043 7573 746f 6d44 6f63 756d 656e 7445   CustomDocumentE
-00001ba0: 6e63 6f64 6572 2863 6b70 745f 6e61 6d65  ncoder(ckpt_name
-00001bb0: 2c20 6465 7669 6365 3d64 6576 6963 6529  , device=device)
-00001bc0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00001bd0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00001be0: 726f 720a 6060 600a 5468 656e 2072 6567  ror.```.Then reg
-00001bf0: 6973 7465 7220 6063 7573 746f 6d5f 656e  ister `custom_en
-00001c00: 636f 6465 725f 6275 696c 6465 7260 2077  coder_builder` w
-00001c10: 6974 6820 6073 7072 696e 742e 696e 6665  ith `sprint.infe
-00001c20: 7265 6e63 652e 656e 636f 6465 725f 6275  rence.encoder_bu
-00001c30: 696c 6465 7273 2e72 6567 6973 7465 7260  ilders.register`
-00001c40: 2062 6566 6f72 6520 7573 6167 653a 0a60   before usage:.`
-00001c50: 6060 7079 7468 6f6e 0a66 726f 6d20 7370  ``python.from sp
-00001c60: 7269 6e74 2e69 6e66 6572 656e 6365 2e65  rint.inference.e
-00001c70: 6e63 6f64 6572 5f62 7569 6c64 6572 7320  ncoder_builders 
-00001c80: 696d 706f 7274 2072 6567 6973 7465 720a  import register.
-00001c90: 0a72 6567 6973 7465 7228 2763 7573 746f  .register('custo
-00001ca0: 6d5f 656e 636f 6465 725f 6275 696c 6465  m_encoder_builde
-00001cb0: 7227 2c20 6375 7374 6f6d 5f65 6e63 6f64  r', custom_encod
-00001cc0: 6572 5f62 7569 6c64 6572 290a 6060 600a  er_builder).```.
-00001cd0: 0a23 2320 5472 6169 6e69 6e67 2028 4578  .## Training (Ex
-00001ce0: 7065 7269 6d65 6e74 616c 290a 5769 6c6c  perimental).Will
-00001cf0: 2062 6520 6164 6465 642e 0a0a 2323 2043   be added...## C
-00001d00: 6f6e 7461 6374 730a 5468 6520 6d61 696e  ontacts.The main
-00001d10: 2063 6f6e 7472 6962 7574 6f72 7320 6f66   contributors of
-00001d20: 2074 6869 7320 7265 706f 7369 746f 7279   this repository
-00001d30: 2061 7265 3a0a 0a2d 205b 4e61 6e64 616e   are:..- [Nandan
-00001d40: 2054 6861 6b75 725d 2868 7474 7073 3a2f   Thakur](https:/
-00001d50: 2f67 6974 6875 622e 636f 6d2f 4e74 6861  /github.com/Ntha
-00001d60: 6b75 7232 3029 0a2d 205b 4b65 7869 6e20  kur20).- [Kexin 
-00001d70: 5761 6e67 5d28 6874 7470 733a 2f2f 6769  Wang](https://gi
-00001d80: 7468 7562 2e63 6f6d 2f6b 7761 6e67 3230  thub.com/kwang20
-00001d90: 3439 290a 0a0a                           49)...
+00000100: 6169 6c2e 636f 6d0a 5072 6f6a 6563 742d  ail.com.Project-
+00000110: 5552 4c3a 2042 7567 2054 7261 636b 6572  URL: Bug Tracker
+00000120: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+00000130: 2e63 6f6d 2f74 6861 6b75 722d 6e61 6e64  .com/thakur-nand
+00000140: 616e 2f73 7072 696e 742f 6973 7375 6573  an/sprint/issues
+00000150: 0a4b 6579 776f 7264 733a 2049 6e66 6f72  .Keywords: Infor
+00000160: 6d61 7469 6f6e 2052 6574 7269 6576 616c  mation Retrieval
+00000170: 2054 6f6f 6c6b 6974 2053 7061 7273 6520   Toolkit Sparse 
+00000180: 5265 7472 6965 7665 7273 204e 6574 776f  Retrievers Netwo
+00000190: 726b 7320 4245 5254 2050 7954 6f72 6368  rks BERT PyTorch
+000001a0: 2049 5220 4e4c 5020 6465 6570 206c 6561   IR NLP deep lea
+000001b0: 726e 696e 670a 436c 6173 7369 6669 6572  rning.Classifier
+000001c0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000001d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001e0: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+000001f0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+00000200: 5349 2041 7070 726f 7665 6420 3a3a 2041  SI Approved :: A
+00000210: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
+00000220: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
+00000230: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+00000240: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000250: 6e64 656e 740a 436c 6173 7369 6669 6572  ndent.Classifier
+00000260: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
+00000270: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000280: 6720 3a3a 2041 7274 6966 6963 6961 6c20  g :: Artificial 
+00000290: 496e 7465 6c6c 6967 656e 6365 0a43 6c61  Intelligence.Cla
+000002a0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+000002b0: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
+000002c0: 6965 6e63 652f 5265 7365 6172 6368 0a52  ience/Research.R
+000002d0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+000002e0: 3e3d 332e 370a 4465 7363 7269 7074 696f  >=3.7.Descriptio
+000002f0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000300: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
+00000310: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+00000320: 4e53 450a 0a3c 6831 2061 6c69 676e 3d22  NSE..<h1 align="
+00000330: 6365 6e74 6572 223e 0a3c 696d 6720 7374  center">.<img st
+00000340: 796c 653d 2276 6572 7469 6361 6c2d 616c  yle="vertical-al
+00000350: 6967 6e3a 6d69 6464 6c65 2220 7769 6474  ign:middle" widt
+00000360: 683d 2236 3230 2220 6865 6967 6874 3d22  h="620" height="
+00000370: 3132 3022 2073 7263 3d22 2e2f 696d 6167  120" src="./imag
+00000380: 6573 2f73 7072 696e 742d 6c6f 676f 2e70  es/sprint-logo.p
+00000390: 6e67 2220 2f3e 0a3c 2f68 313e 0a0a 3c70  ng" />.</h1>..<p
+000003a0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000003b0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000003c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000003d0: 2f74 6861 6b75 722d 6e61 6e64 616e 2f73  /thakur-nandan/s
+000003e0: 7072 696e 742f 7265 6c65 6173 6573 223e  print/releases">
+000003f0: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
+00000400: 743d 2247 6974 4875 6220 7265 6c65 6173  t="GitHub releas
+00000410: 6522 2073 7263 3d22 6874 7470 733a 2f2f  e" src="https://
+00000420: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000430: 6164 6765 2f72 656c 6561 7365 2d76 302e  adge/release-v0.
+00000440: 302e 312d 626c 7565 223e 0a20 2020 203c  0.1-blue">.    <
+00000450: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+00000460: 2268 7474 7073 3a2f 2f77 7777 2e70 7974  "https://www.pyt
+00000470: 686f 6e2e 6f72 672f 223e 0a20 2020 2020  hon.org/">.     
+00000480: 2020 2020 2020 203c 696d 6720 616c 743d         <img alt=
+00000490: 2242 7569 6c64 2220 7372 633d 2268 7474  "Build" src="htt
+000004a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000004b0: 2e69 6f2f 6261 6467 652f 4d61 6465 2532  .io/badge/Made%2
+000004c0: 3077 6974 682d 5079 7468 6f6e 2d31 6634  0with-Python-1f4
+000004d0: 3235 662e 7376 673f 636f 6c6f 723d 7075  25f.svg?color=pu
+000004e0: 7270 6c65 223e 0a20 2020 203c 2f61 3e0a  rple">.    </a>.
+000004f0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000500: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000510: 7468 616b 7572 2d6e 616e 6461 6e2f 7370  thakur-nandan/sp
+00000520: 7269 6e74 2f62 6c6f 622f 6d61 7374 6572  rint/blob/master
+00000530: 2f4c 4943 454e 5345 223e 0a20 2020 2020  /LICENSE">.     
+00000540: 2020 203c 696d 6720 616c 743d 224c 6963     <img alt="Lic
+00000550: 656e 7365 2220 7372 633d 2268 7474 7073  ense" src="https
+00000560: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000570: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+00000580: 2f74 6861 6b75 722d 6e61 6e64 616e 2f73  /thakur-nandan/s
+00000590: 7072 696e 742e 7376 673f 636f 6c6f 723d  print.svg?color=
+000005a0: 6772 6565 6e22 3e0a 2020 2020 3c2f 613e  green">.    </a>
+000005b0: 0a20 2020 203c 212d 2d20 3c61 2068 7265  .    <!-- <a hre
+000005c0: 663d 2268 7474 7073 3a2f 2f63 6f6c 6162  f="https://colab
+000005d0: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+000005e0: 2e63 6f6d 2f64 7269 7665 2f31 4866 7574  .com/drive/1Hfut
+000005f0: 6945 6848 4d4a 4c58 6957 4754 3870 6369  iEhHMJLXiWGT8pci
+00000600: 7078 5435 4c32 5470 5945 6474 3f75 7370  pxT5L2TpYEdt?usp
+00000610: 3d73 6861 7269 6e67 223e 0a20 2020 2020  =sharing">.     
+00000620: 2020 203c 696d 6720 616c 743d 224f 7065     <img alt="Ope
+00000630: 6e20 496e 2043 6f6c 6162 2220 7372 633d  n In Colab" src=
+00000640: 2268 7474 7073 3a2f 2f63 6f6c 6162 2e72  "https://colab.r
+00000650: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00000660: 6f6d 2f61 7373 6574 732f 636f 6c61 622d  om/assets/colab-
+00000670: 6261 6467 652e 7376 6722 3e0a 2020 2020  badge.svg">.    
+00000680: 3c2f 613e 202d 2d3e 0a20 2020 203c 6120  </a> -->.    <a 
+00000690: 6872 6566 3d22 6874 7470 733a 2f2f 7065  href="https://pe
+000006a0: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
+000006b0: 7370 7269 6e74 2d74 6f6f 6c6b 6974 223e  sprint-toolkit">
+000006c0: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
+000006d0: 743d 2244 6f77 6e6c 6f61 6473 2220 7372  t="Downloads" sr
+000006e0: 633d 2268 7474 7073 3a2f 2f73 7461 7469  c="https://stati
+000006f0: 632e 7065 7079 2e74 6563 682f 7065 7273  c.pepy.tech/pers
+00000700: 6f6e 616c 697a 6564 2d62 6164 6765 2f73  onalized-badge/s
+00000710: 7072 696e 743f 7065 7269 6f64 3d74 6f74  print?period=tot
+00000720: 616c 2675 6e69 7473 3d69 6e74 6572 6e61  al&units=interna
+00000730: 7469 6f6e 616c 5f73 7973 7465 6d26 6c65  tional_system&le
+00000740: 6674 5f63 6f6c 6f72 3d67 7265 7926 7269  ft_color=grey&ri
+00000750: 6768 745f 636f 6c6f 723d 6f72 616e 6765  ght_color=orange
+00000760: 266c 6566 745f 7465 7874 3d44 6f77 6e6c  &left_text=Downl
+00000770: 6f61 6473 223e 0a20 2020 203c 2f61 3e0a  oads">.    </a>.
+00000780: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000790: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000007a0: 7468 616b 7572 2d6e 616e 6461 6e2f 7370  thakur-nandan/sp
+000007b0: 7269 6e74 2f22 3e0a 2020 2020 2020 2020  rint/">.        
+000007c0: 3c69 6d67 2061 6c74 3d22 446f 776e 6c6f  <img alt="Downlo
+000007d0: 6164 7322 2073 7263 3d22 6874 7470 733a  ads" src="https:
+000007e0: 2f2f 6261 6467 6573 2e66 7261 7073 6f66  //badges.frapsof
+000007f0: 742e 636f 6d2f 6f73 2f76 312f 6f70 656e  t.com/os/v1/open
+00000800: 2d73 6f75 7263 652e 7376 673f 763d 3130  -source.svg?v=10
+00000810: 3322 3e0a 2020 2020 3c2f 613e 0a3c 2f70  3">.    </a>.</p
+00000820: 3e0a 0a3c 6833 2061 6c69 676e 3d22 6365  >..<h3 align="ce
+00000830: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000840: 6566 3d22 6874 7470 733a 2f2f 7577 6174  ef="https://uwat
+00000850: 6572 6c6f 6f2e 6361 223e 3c69 6d67 2073  erloo.ca"><img s
+00000860: 7479 6c65 3d22 666c 6f61 743a 206c 6566  tyle="float: lef
+00000870: 743b 2070 6164 6469 6e67 3a20 3270 7820  t; padding: 2px 
+00000880: 3770 7820 3270 7820 3770 783b 2220 7769  7px 2px 7px;" wi
+00000890: 6474 683d 2232 3133 2220 6865 6967 6874  dth="213" height
+000008a0: 3d22 3637 2220 7372 633d 222e 2f69 6d61  ="67" src="./ima
+000008b0: 6765 732f 7577 6174 6572 6c6f 6f2e 706e  ges/uwaterloo.pn
+000008c0: 6722 202f 3e3c 2f61 3e0a 2020 2020 3c61  g" /></a>.    <a
+000008d0: 2068 7265 663d 2268 7474 703a 2f2f 7777   href="http://ww
+000008e0: 772e 756b 702e 7475 2d64 6172 6d73 7461  w.ukp.tu-darmsta
+000008f0: 6474 2e64 6522 3e3c 696d 6720 7374 796c  dt.de"><img styl
+00000900: 653d 2266 6c6f 6174 3a20 6d69 6464 6c65  e="float: middle
+00000910: 3b20 7061 6464 696e 673a 2032 7078 2037  ; padding: 2px 7
+00000920: 7078 2032 7078 2037 7078 3b22 2077 6964  px 2px 7px;" wid
+00000930: 7468 3d22 3134 3722 2068 6569 6768 743d  th="147" height=
+00000940: 2236 3722 2073 7263 3d22 2e2f 696d 6167  "67" src="./imag
+00000950: 6573 2f75 6b70 2e70 6e67 2220 2f3e 3c2f  es/ukp.png" /></
+00000960: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000970: 6874 7470 733a 2f2f 7777 772e 7475 2d64  https://www.tu-d
+00000980: 6172 6d73 7461 6474 2e64 652f 223e 3c69  armstadt.de/"><i
+00000990: 6d67 2073 7479 6c65 3d22 666c 6f61 743a  mg style="float:
+000009a0: 2072 6967 6874 3b20 7061 6464 696e 673a   right; padding:
+000009b0: 2032 7078 2037 7078 2032 7078 2037 7078   2px 7px 2px 7px
+000009c0: 3b22 2077 6964 7468 3d22 3136 372e 3722  ;" width="167.7"
+000009d0: 2068 6569 6768 743d 2236 3022 2073 7263   height="60" src
+000009e0: 3d22 2e2f 696d 6167 6573 2f74 752d 6461  ="./images/tu-da
+000009f0: 726d 7374 6164 742e 706e 6722 202f 3e3c  rmstadt.png" /><
+00000a00: 2f61 3e0a 3c2f 6833 3e0a 0a23 2323 2053  /a>.</h3>..### S
+00000a10: 5052 494e 5420 7072 6f76 6964 6573 2061  PRINT provides a
+00000a20: 205f 756e 6966 6965 645f 2072 6570 6f73   _unified_ repos
+00000a30: 6974 6f72 7920 746f 2065 6173 696c 7920  itory to easily 
+00000a40: 5f65 7661 6c75 6174 655f 2064 6976 6572  _evaluate_ diver
+00000a50: 7365 2073 7461 7465 2d6f 662d 7468 652d  se state-of-the-
+00000a60: 6172 7420 6e65 7572 616c 2028 4245 5254  art neural (BERT
+00000a70: 2d62 6173 6564 2920 7370 6172 7365 2d72  -based) sparse-r
+00000a80: 6574 7269 6576 616c 206d 6f64 656c 732e  etrieval models.
+00000a90: 0a0a 5350 5249 4e54 2074 6f6f 6c6b 6974  ..SPRINT toolkit
+00000aa0: 2061 6c6c 6f77 7320 796f 7520 746f 2065   allows you to e
+00000ab0: 6173 696c 7920 7365 6172 6368 206f 7220  asily search or 
+00000ac0: 6576 616c 7561 7465 2061 6e79 206e 6575  evaluate any neu
+00000ad0: 7261 6c20 7370 6172 7365 2072 6574 7269  ral sparse retri
+00000ae0: 6576 6572 2061 6372 6f73 7320 2a2a 616e  ever across **an
+00000af0: 792a 2a20 6461 7461 7365 7420 696e 2074  y** dataset in t
+00000b00: 6865 2042 4549 5220 6265 6e63 686d 6172  he BEIR benchmar
+00000b10: 6b20 286f 7220 796f 7572 206f 776e 2064  k (or your own d
+00000b20: 6174 6173 6574 292e 2054 6865 2074 6f6f  ataset). The too
+00000b30: 6c6b 6974 2069 7320 6275 696c 7420 6172  lkit is built ar
+00000b40: 6f75 6e64 2061 7320 6120 7573 6566 756c  ound as a useful
+00000b50: 2077 7261 7070 6572 2061 726f 756e 6420   wrapper around 
+00000b60: 5079 7365 7269 6e69 2e20 5468 6520 746f  Pyserini. The to
+00000b70: 6f6c 6b69 7420 7072 6f76 6964 6573 2065  olkit provides e
+00000b80: 7661 6c75 6174 696f 6e20 6f66 2073 6576  valuation of sev
+00000b90: 656e 2064 6976 6572 7365 2028 6e65 7572  en diverse (neur
+00000ba0: 616c 2920 7370 6172 7365 2072 6574 7269  al) sparse retri
+00000bb0: 6576 616c 206d 6f64 656c 733a 205b 5350  eval models: [SP
+00000bc0: 4c41 4445 7632 5d28 6874 7470 733a 2f2f  LADEv2](https://
+00000bd0: 6172 7869 762e 6f72 672f 6162 732f 3231  arxiv.org/abs/21
+00000be0: 3039 2e31 3030 3836 292c 205b 4254 2d53  09.10086), [BT-S
+00000bf0: 504c 4144 452d 4c5d 2868 7474 7073 3a2f  PLADE-L](https:/
+00000c00: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00000c10: 3230 372e 3033 3833 3429 2c20 5b75 6e69  207.03834), [uni
+00000c20: 434f 494c 5d28 6874 7470 733a 2f2f 6172  COIL](https://ar
+00000c30: 7869 762e 6f72 672f 6162 732f 3231 3036  xiv.org/abs/2106
+00000c40: 2e31 3438 3037 292c 205b 5449 4c44 4576  .14807), [TILDEv
+00000c50: 325d 2868 7474 7073 3a2f 2f61 7278 6976  2](https://arxiv
+00000c60: 2e6f 7267 2f61 6273 2f32 3130 382e 3038  .org/abs/2108.08
+00000c70: 3531 3329 2c20 5b44 6565 7049 6d70 6163  513), [DeepImpac
+00000c80: 745d 2868 7474 7073 3a2f 2f61 7278 6976  t](https://arxiv
+00000c90: 2e6f 7267 2f61 6273 2f32 3130 342e 3132  .org/abs/2104.12
+00000ca0: 3031 3629 2c20 5b44 6f63 5435 7175 6572  016), [DocT5quer
+00000cb0: 795d 2868 7474 7073 3a2f 2f63 732e 7577  y](https://cs.uw
+00000cc0: 6174 6572 6c6f 6f2e 6361 2f7e 6a69 6d6d  aterloo.ca/~jimm
+00000cd0: 796c 696e 2f70 7562 6c69 6361 7469 6f6e  ylin/publication
+00000ce0: 732f 4e6f 6775 6569 7261 5f4c 696e 5f32  s/Nogueira_Lin_2
+00000cf0: 3031 395f 646f 6354 5454 5454 7175 6572  019_docTTTTTquer
+00000d00: 792d 7632 2e70 6466 2920 616e 6420 5b53  y-v2.pdf) and [S
+00000d10: 5041 5254 415d 2868 7474 7073 3a2f 2f61  PARTA](https://a
+00000d20: 636c 616e 7468 6f6c 6f67 792e 6f72 672f  clanthology.org/
+00000d30: 3230 3231 2e6e 6161 636c 2d6d 6169 6e2e  2021.naacl-main.
+00000d40: 3437 2f29 2e0a 0a0a 0a0a 4966 2079 6f75  47/)......If you
+00000d50: 2077 616e 7420 746f 2072 6561 6420 6d6f   want to read mo
+00000d60: 7265 2061 626f 7574 2074 6865 2053 5052  re about the SPR
+00000d70: 494e 5420 746f 6f6c 6b69 742c 206f 7220  INT toolkit, or 
+00000d80: 7769 7368 2074 6f20 6b6e 6f77 2077 6869  wish to know whi
+00000d90: 6368 206d 6f64 656c 2074 6f20 7573 652c  ch model to use,
+00000da0: 2070 6c65 6173 6520 7265 6665 7220 746f   please refer to
+00000db0: 206f 7572 2070 6170 6572 2066 6f72 206d   our paper for m
+00000dc0: 6f72 6520 6465 7461 696c 733a 0a0a 2a20  ore details:..* 
+00000dd0: 5b2a 2a53 5052 494e 543a 2041 2055 6e69  [**SPRINT: A Uni
+00000de0: 6669 6564 2054 6f6f 6c6b 6974 2066 6f72  fied Toolkit for
+00000df0: 2045 7661 6c75 6174 696e 6720 616e 6420   Evaluating and 
+00000e00: 4465 6d79 7374 6966 7969 6e67 205a 6572  Demystifying Zer
+00000e10: 6f2d 7368 6f74 204e 6575 7261 6c20 5370  o-shot Neural Sp
+00000e20: 6172 7365 2052 6574 7269 6576 616c 2a2a  arse Retrieval**
+00000e30: 5d28 2920 2841 6363 6570 7465 6420 6174  ]() (Accepted at
+00000e40: 2053 4947 4952 2732 3320 5265 736f 7572   SIGIR'23 Resour
+00000e50: 6365 2054 7261 636b 290a 0a23 2320 3a72  ce Track)..## :r
+00000e60: 756e 6e65 723a 2047 6574 7469 6e67 2053  unner: Getting S
+00000e70: 7461 7274 6564 0a53 5052 494e 5420 6973  tarted.SPRINT is
+00000e80: 2062 6163 6b65 6420 6279 2050 7973 6572   backed by Pyser
+00000e90: 696e 6920 7768 6963 6820 7265 6c69 6573  ini which relies
+00000ea0: 206f 6e20 4a61 7661 2e20 546f 206d 616b   on Java. To mak
+00000eb0: 6520 7468 6520 696e 7374 616c 6c61 7469  e the installati
+00000ec0: 6f6e 2065 6169 7365 722c 2077 6520 7265  on eaiser, we re
+00000ed0: 636f 6d6d 656e 6420 746f 2066 6f6c 6c6f  commend to follo
+00000ee0: 7720 7468 6520 7374 6570 7320 6265 6c6f  w the steps belo
+00000ef0: 7720 7669 6120 6063 6f6e 6461 603a 0a0a  w via `conda`:..
+00000f00: 6060 6062 6173 680a 2323 2323 2043 7265  ```bash.#### Cre
+00000f10: 6174 6520 6120 6e65 7720 636f 6e64 6120  ate a new conda 
+00000f20: 656e 7669 726f 6e6d 656e 7420 7573 696e  environment usin
+00000f30: 6720 636f 6e64 6120 2323 2323 0a24 2063  g conda ####.$ c
+00000f40: 6f6e 6461 2063 7265 6174 6520 2d6e 2073  onda create -n s
+00000f50: 7072 696e 745f 656e 7620 7079 7468 6f6e  print_env python
+00000f60: 3d33 2e38 0a24 2063 6f6e 6461 2061 6374  =3.8.$ conda act
+00000f70: 6976 6174 6520 7370 7269 6e74 5f65 6e76  ivate sprint_env
+00000f80: 0a0a 2320 496e 7374 616c 6c20 4a44 4b20  ..# Install JDK 
+00000f90: 3131 2076 6961 2063 6f6e 6461 0a24 2063  11 via conda.$ c
+00000fa0: 6f6e 6461 2069 6e73 7461 6c6c 202d 6320  onda install -c 
+00000fb0: 636f 6e64 612d 666f 7267 6520 6f70 656e  conda-forge open
+00000fc0: 6a64 6b3d 3131 0a0a 2320 496e 7374 616c  jdk=11..# Instal
+00000fd0: 6c20 5350 5249 4e54 2074 6f6f 6c6b 6974  l SPRINT toolkit
+00000fe0: 2075 7369 6e67 2050 7950 490a 2420 7069   using PyPI.$ pi
+00000ff0: 7020 696e 7374 616c 6c20 7370 7269 6e74  p install sprint
+00001000: 2d74 6f6f 6c6b 6974 0a60 6060 0a0a 2323  -toolkit.```..##
+00001010: 203a 7275 6e6e 6572 3a20 5175 6963 6b73   :runner: Quicks
+00001020: 7461 7274 2077 6974 6820 5350 5249 4e54  tart with SPRINT
+00001030: 2054 6f6f 6c6b 6974 0a0a 2323 2320 5175   Toolkit..### Qu
+00001040: 6963 6b20 7374 6172 740a 466f 7220 6120  ick start.For a 
+00001050: 7175 6963 6b20 7374 6172 742c 2077 6520  quick start, we 
+00001060: 6361 6e20 676f 2074 6f20 7468 6520 5b65  can go to the [e
+00001070: 7861 6d70 6c65 5d28 6578 616d 706c 6573  xample](examples
+00001080: 2f69 6e66 6572 656e 6365 2f64 6973 7469  /inference/disti
+00001090: 6c73 706c 6164 655f 6d61 782f 6265 6972  lsplade_max/beir
+000010a0: 5f73 6369 6661 6374 2f61 6c6c 5f69 6e5f  _scifact/all_in_
+000010b0: 6f6e 652e 7368 2920 666f 7220 6576 616c  one.sh) for eval
+000010c0: 7561 7469 6e67 2053 504c 4144 4520 2860  uating SPLADE (`
+000010d0: 6469 7374 696c 7370 6c61 6465 5f6d 6178  distilsplade_max
+000010e0: 6029 206f 6e20 7468 6520 4265 4952 2f53  `) on the BeIR/S
+000010f0: 6369 4661 6374 2064 6174 6173 6574 3a0a  ciFact dataset:.
+00001100: 6060 6062 6173 680a 6364 2065 7861 6d70  ```bash.cd examp
+00001110: 6c65 732f 696e 6665 7265 6e63 652f 6469  les/inference/di
+00001120: 7374 696c 7370 6c61 6465 5f6d 6178 2f62  stilsplade_max/b
+00001130: 6569 725f 7363 6966 6163 740a 6261 7368  eir_scifact.bash
+00001140: 2061 6c6c 5f69 6e5f 6f6e 652e 7368 0a60   all_in_one.sh.`
+00001150: 6060 0a54 6869 7320 7769 6c6c 2067 6f20  ``.This will go 
+00001160: 6f76 6572 2074 6865 2077 686f 6c65 2070  over the whole p
+00001170: 6970 656c 696e 6520 616e 6420 6769 7665  ipeline and give
+00001180: 2074 6865 2066 696e 616c 2065 7661 6c75   the final evalu
+00001190: 6174 696f 6e20 7265 7375 6c74 7320 696e  ation results in
+000011a0: 2060 6265 6972 5f73 6369 6661 6374 2d64   `beir_scifact-d
+000011b0: 6973 7469 6c73 706c 6164 655f 6d61 782d  istilsplade_max-
+000011c0: 7175 616e 7469 7a65 642f 6576 616c 7561  quantized/evalua
+000011d0: 7469 6f6e 2f6d 6574 7269 6373 2e6a 736f  tion/metrics.jso
+000011e0: 6e60 3a0a 0a3c 6465 7461 696c 733e 0a20  n`:..<details>. 
+000011f0: 203c 7375 6d6d 6172 793e 5265 7375 6c74   <summary>Result
+00001200: 733a 2064 6973 7469 6c73 706c 6164 655f  s: distilsplade_
+00001210: 6d61 7820 6f6e 2042 6549 522f 5363 6946  max on BeIR/SciF
+00001220: 6163 743c 2f73 756d 6d61 7279 3e0a 2020  act</summary>.  
+00001230: 0a20 2060 6060 6261 7368 0a20 2020 2020  .  ```bash.     
+00001240: 6361 7420 6265 6972 5f73 6369 6661 6374  cat beir_scifact
+00001250: 2d64 6973 7469 6c73 706c 6164 655f 6d61  -distilsplade_ma
+00001260: 782d 7175 616e 7469 7a65 642f 6576 616c  x-quantized/eval
+00001270: 7561 7469 6f6e 2f6d 6574 7269 6373 2e6a  uation/metrics.j
+00001280: 736f 6e20 0a20 2020 2020 2320 7b0a 2020  son .     # {.  
+00001290: 2020 2023 2020 2020 2022 6e44 4347 223a     #     "nDCG":
+000012a0: 207b 0a20 2020 2020 2320 2020 2020 2020   {.     #       
+000012b0: 2020 224e 4443 4740 3122 3a20 302e 3630    "NDCG@1": 0.60
+000012c0: 3333 332c 0a20 2020 2020 2320 2020 2020  333,.     #     
+000012d0: 2020 2020 224e 4443 4740 3322 3a20 302e      "NDCG@3": 0.
+000012e0: 3635 3936 392c 0a20 2020 2020 2320 2020  65969,.     #   
+000012f0: 2020 2020 2020 224e 4443 4740 3522 3a20        "NDCG@5": 
+00001300: 302e 3637 3230 342c 0a20 2020 2020 2320  0.67204,.     # 
+00001310: 2020 2020 2020 2020 224e 4443 4740 3130          "NDCG@10
+00001320: 223a 2030 2e36 3932 352c 0a20 2020 2020  ": 0.6925,.     
+00001330: 2320 2020 2020 2020 2020 224e 4443 4740  #         "NDCG@
+00001340: 3130 3022 3a20 302e 3732 3032 2c0a 2020  100": 0.7202,.  
+00001350: 2020 2023 2020 2020 2020 2020 2022 4e44     #         "ND
+00001360: 4347 4031 3030 3022 3a20 302e 3732 3735  CG@1000": 0.7275
+00001370: 330a 2020 2020 2023 2020 2020 207d 2c0a  3.     #     },.
+00001380: 2020 2020 2023 2020 2020 2022 4d41 5022       #     "MAP"
+00001390: 3a20 7b0a 2020 2020 2023 2020 2020 2020  : {.     #      
+000013a0: 2020 2022 4d41 5040 3122 3a20 302e 3537     "MAP@1": 0.57
+000013b0: 3231 372c 0a20 2020 2020 2320 2020 2020  217,.     #     
+000013c0: 2e2e 2e0a 2020 2020 2023 207d 0a20 2060  ....     # }.  `
+000013d0: 6060 0a3c 2f64 6574 6169 6c73 3e0a 0a4f  ``.</details>..O
+000013e0: 7220 6966 2079 6f75 206c 696b 6520 7275  r if you like ru
+000013f0: 6e6e 696e 6720 7079 7468 6f6e 2064 6972  nning python dir
+00001400: 6563 746c 792c 206a 7573 7420 7275 6e20  ectly, just run 
+00001410: 7468 6520 636f 6465 2073 6e69 7070 6574  the code snippet
+00001420: 2062 656c 6f77 2066 6f72 2065 7661 6c75   below for evalu
+00001430: 6174 696e 6720 6063 6173 746f 7269 6e69  ating `castorini
+00001440: 2f75 6e69 636f 696c 2d6e 6f65 7870 2d6d  /unicoil-noexp-m
+00001450: 736d 6172 636f 2d70 6173 7361 6765 6020  smarco-passage` 
+00001460: 6f6e 2060 4265 4952 2f53 6369 4661 6374  on `BeIR/SciFact
+00001470: 603a 0a60 6060 7079 7468 6f6e 0a66 726f  `:.```python.fro
+00001480: 6d20 7370 7269 6e74 2e69 6e66 6572 656e  m sprint.inferen
+00001490: 6365 2069 6d70 6f72 7420 6169 6f0a 0a0a  ce import aio...
+000014a0: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
+000014b0: 5f5f 6d61 696e 5f5f 273a 2020 2320 6169  __main__':  # ai
+000014c0: 6f2e 7275 6e20 6361 6e20 6f6e 6c79 2062  o.run can only b
+000014d0: 6520 6361 6c6c 6564 2077 6974 6869 6e20  e called within 
+000014e0: 5f5f 6d61 696e 5f5f 0a20 2020 2061 696f  __main__.    aio
+000014f0: 2e72 756e 280a 2020 2020 2020 2020 656e  .run(.        en
+00001500: 636f 6465 725f 6e61 6d65 3d27 756e 6963  coder_name='unic
+00001510: 6f69 6c27 2c0a 2020 2020 2020 2020 636b  oil',.        ck
+00001520: 7074 5f6e 616d 653d 2763 6173 746f 7269  pt_name='castori
+00001530: 6e69 2f75 6e69 636f 696c 2d6e 6f65 7870  ni/unicoil-noexp
+00001540: 2d6d 736d 6172 636f 2d70 6173 7361 6765  -msmarco-passage
+00001550: 272c 0a20 2020 2020 2020 2064 6174 615f  ',.        data_
+00001560: 6e61 6d65 3d27 6265 6972 2f73 6369 6661  name='beir/scifa
+00001570: 6374 272c 0a20 2020 2020 2020 2067 7075  ct',.        gpu
+00001580: 733d 5b30 2c20 315d 2c0a 2020 2020 2020  s=[0, 1],.      
+00001590: 2020 6f75 7470 7574 5f64 6972 3d27 6265    output_dir='be
+000015a0: 6972 5f73 6369 6661 6374 2d75 6e69 636f  ir_scifact-unico
+000015b0: 696c 5f6e 6f65 7870 272c 0a20 2020 2020  il_noexp',.     
+000015c0: 2020 2064 6f5f 7175 616e 7469 7a61 7469     do_quantizati
+000015d0: 6f6e 3d54 7275 652c 0a20 2020 2020 2020  on=True,.       
+000015e0: 2071 7561 6e74 697a 6174 696f 6e5f 6d65   quantization_me
+000015f0: 7468 6f64 3d27 7261 6e67 652d 6e62 6974  thod='range-nbit
+00001600: 7327 2c20 2023 2053 6f20 7468 6520 646f  s',  # So the do
+00001610: 6320 7465 726d 2077 6569 6768 7473 2077  c term weights w
+00001620: 696c 6c20 6265 2071 7561 6e74 697a 6564  ill be quantized
+00001630: 2062 7920 6028 7465 726d 5f77 6569 6768   by `(term_weigh
+00001640: 7473 202f 2035 2920 2a20 2832 202a 2a20  ts / 5) * (2 ** 
+00001650: 3829 600a 2020 2020 2020 2020 6f72 6967  8)`.        orig
+00001660: 696e 616c 5f73 636f 7265 5f72 616e 6765  inal_score_range
+00001670: 3d35 2c0a 2020 2020 2020 2020 7175 616e  =5,.        quan
+00001680: 7469 7a61 7469 6f6e 5f6e 6269 7473 3d38  tization_nbits=8
+00001690: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
+000016a0: 616c 5f71 7565 7279 5f66 6f72 6d61 743d  al_query_format=
+000016b0: 2762 6569 7227 2c0a 2020 2020 2020 2020  'beir',.        
+000016c0: 746f 7069 635f 7370 6c69 743d 2774 6573  topic_split='tes
+000016d0: 7427 0a20 2020 2029 0a20 2020 2023 2059  t'.    ).    # Y
+000016e0: 6f75 2077 6f75 6c64 2067 6574 2022 4e44  ou would get "ND
+000016f0: 4347 4031 3022 3a20 302e 3638 3536 330a  CG@10": 0.68563.
+00001700: 6060 600a 2323 2320 5374 6570 2062 7920  ```.### Step by 
+00001710: 7374 6570 0a4f 6e65 2063 616e 2061 6c73  step.One can als
+00001720: 6f20 7275 6e20 7468 6520 6162 6f76 6520  o run the above 
+00001730: 7072 6f63 6573 7320 696e 2036 2073 6570  process in 6 sep
+00001740: 6172 6174 6520 7374 6570 7320 756e 6465  arate steps unde
+00001750: 7220 7468 6520 5b73 7465 705f 6279 5f73  r the [step_by_s
+00001760: 7465 705d 2865 7861 6d70 6c65 732f 696e  tep](examples/in
+00001770: 6665 7265 6e63 652f 6469 7374 696c 7370  ference/distilsp
+00001780: 6c61 6465 5f6d 6178 2f62 6569 725f 7363  lade_max/beir_sc
+00001790: 6966 6163 742f 7374 6570 5f62 795f 7374  ifact/step_by_st
+000017a0: 6570 2920 666f 6c64 6572 3a0a 312e 205b  ep) folder:.1. [
+000017b0: 656e 636f 6465 5d28 6578 616d 706c 6573  encode](examples
+000017c0: 2f69 6e66 6572 656e 6365 2f64 6973 7469  /inference/disti
+000017d0: 6c73 706c 6164 655f 6d61 782f 6265 6972  lsplade_max/beir
+000017e0: 5f73 6369 6661 6374 2f73 7465 705f 6279  _scifact/step_by
+000017f0: 5f73 7465 702f 312e 656e 636f 6465 2e62  _step/1.encode.b
+00001800: 6569 725f 7363 6966 6163 742d 6469 7374  eir_scifact-dist
+00001810: 696c 7370 6c61 6465 5f6d 6178 2d66 6c6f  ilsplade_max-flo
+00001820: 6174 2e73 6829 3a20 456e 636f 6465 2064  at.sh): Encode d
+00001830: 6f63 756d 656e 7473 2069 6e74 6f20 7465  ocuments into te
+00001840: 726d 2077 6569 6768 7473 2062 7920 6d75  rm weights by mu
+00001850: 6c74 6970 726f 6365 7373 696e 6720 6f6e  ltiprocessing on
+00001860: 206d 7574 6c69 706c 6520 4750 5573 3b0a   mutliple GPUs;.
+00001870: 322e 205b 7175 616e 7469 7a65 5d28 6578  2. [quantize](ex
+00001880: 616d 706c 6573 2f69 6e66 6572 656e 6365  amples/inference
+00001890: 2f64 6973 7469 6c73 706c 6164 655f 6d61  /distilsplade_ma
+000018a0: 782f 6265 6972 5f73 6369 6661 6374 2f73  x/beir_scifact/s
+000018b0: 7465 705f 6279 5f73 7465 702f 322e 7175  tep_by_step/2.qu
+000018c0: 616e 7469 7a65 2e62 6569 725f 7363 6966  antize.beir_scif
+000018d0: 6163 742d 6469 7374 696c 7370 6c61 6465  act-distilsplade
+000018e0: 5f6d 6178 2d32 6469 6769 7473 2e73 6829  _max-2digits.sh)
+000018f0: 3a20 5175 616e 7469 7a65 2074 6865 2064  : Quantize the d
+00001900: 6f63 756d 656e 7420 7465 726d 2077 6569  ocument term wei
+00001910: 6768 7473 2069 6e74 6f20 696e 7465 6765  ghts into intege
+00001920: 7273 2028 6361 6e20 6265 2073 6361 7065  rs (can be scape
+00001930: 6429 3b0a 332e 205b 696e 6465 785d 2865  d);.3. [index](e
+00001940: 7861 6d70 6c65 732f 696e 6665 7265 6e63  xamples/inferenc
+00001950: 652f 6469 7374 696c 7370 6c61 6465 5f6d  e/distilsplade_m
+00001960: 6178 2f62 6569 725f 7363 6966 6163 742f  ax/beir_scifact/
+00001970: 7374 6570 5f62 795f 7374 6570 2f33 2e69  step_by_step/3.i
+00001980: 6e64 6578 2e62 6569 725f 7363 6966 6163  ndex.beir_scifac
+00001990: 742d 6469 7374 696c 7370 6c61 6465 5f6d  t-distilsplade_m
+000019a0: 6178 2d32 6469 6769 7473 2e73 6829 3a20  ax-2digits.sh): 
+000019b0: 496e 6465 7820 7468 6520 7465 726d 2077  Index the term w
+000019c0: 6569 6768 7473 2069 6e20 746f 204c 7563  eights in to Luc
+000019d0: 656e 6520 696e 6465 7820 2862 6163 6b65  ene index (backe
+000019e0: 6e64 6564 2062 7920 5079 7365 7269 6e69  nded by Pyserini
+000019f0: 293b 0a34 2e20 5b72 6566 6f72 6d61 745d  );.4. [reformat]
+00001a00: 2865 7861 6d70 6c65 732f 696e 6665 7265  (examples/infere
+00001a10: 6e63 652f 6469 7374 696c 7370 6c61 6465  nce/distilsplade
+00001a20: 5f6d 6178 2f62 6569 725f 7363 6966 6163  _max/beir_scifac
+00001a30: 742f 7374 6570 5f62 795f 7374 6570 2f34  t/step_by_step/4
+00001a40: 2e72 6566 6f72 6d61 745f 7175 6572 792e  .reformat_query.
+00001a50: 6265 6972 5f73 6369 6661 6374 2e73 6829  beir_scifact.sh)
+00001a60: 3a20 5265 666f 726d 6174 2074 6865 2071  : Reformat the q
+00001a70: 7565 7269 6573 2066 696c 6520 2865 2e67  ueries file (e.g
+00001a80: 2e20 7468 6520 6f6e 6573 2066 726f 6d20  . the ones from 
+00001a90: 4265 4952 2920 696e 746f 2074 6865 2050  BeIR) into the P
+00001aa0: 7973 6572 696e 6920 666f 726d 6174 3b0a  yserini format;.
+00001ab0: 352e 205b 7365 6172 6368 5d28 6578 616d  5. [search](exam
+00001ac0: 706c 6573 2f69 6e66 6572 656e 6365 2f64  ples/inference/d
+00001ad0: 6973 7469 6c73 706c 6164 655f 6d61 782f  istilsplade_max/
+00001ae0: 6265 6972 5f73 6369 6661 6374 2f73 7465  beir_scifact/ste
+00001af0: 705f 6279 5f73 7465 702f 352e 7365 6172  p_by_step/5.sear
+00001b00: 6368 2e62 6569 725f 7363 6966 6163 742d  ch.beir_scifact-
+00001b10: 6469 7374 696c 7370 6c61 6465 5f6d 6178  distilsplade_max
+00001b20: 2d32 6469 6769 7473 2e73 6829 3a20 5265  -2digits.sh): Re
+00001b30: 7472 6965 7665 2074 6865 2072 656c 6576  trieve the relev
+00001b40: 616e 7420 646f 6375 6d65 6e74 7320 2862  ant documents (b
+00001b50: 6163 6b65 6e64 6564 2062 7920 5079 7365  ackended by Pyse
+00001b60: 7269 6e69 293b 0a36 2e20 5b65 7661 6c75  rini);.6. [evalu
+00001b70: 6174 655d 2865 7861 6d70 6c65 732f 696e  ate](examples/in
+00001b80: 6665 7265 6e63 652f 6469 7374 696c 7370  ference/distilsp
+00001b90: 6c61 6465 5f6d 6178 2f62 6569 725f 7363  lade_max/beir_sc
+00001ba0: 6966 6163 742f 7374 6570 5f62 795f 7374  ifact/step_by_st
+00001bb0: 6570 2f36 2e65 7661 6c75 6174 652e 6265  ep/6.evaluate.be
+00001bc0: 6972 5f73 6369 6661 6374 2d64 6973 7469  ir_scifact-disti
+00001bd0: 6c73 706c 6164 655f 6d61 782d 3264 6967  lsplade_max-2dig
+00001be0: 6974 732e 7368 293a 2045 7661 6c75 6174  its.sh): Evaluat
+00001bf0: 6520 7468 6520 7265 7375 6c74 7320 6167  e the results ag
+00001c00: 6169 6e73 7420 6120 6365 7274 6169 6e20  ainst a certain 
+00001c10: 6c61 6265 6c65 6420 6461 7461 2c20 652e  labeled data, e.
+00001c20: 672e 7468 6520 7172 656c 7320 7573 6564  g.the qrels used
+00001c30: 2069 6e20 4265 4952 2028 6261 636b 656e   in BeIR (backen
+00001c40: 6465 6420 6279 2042 6549 5229 0a0a 4375  ded by BeIR)..Cu
+00001c50: 7272 656e 746c 7920 6974 202a 2a64 6972  rrently it **dir
+00001c60: 6563 746c 792a 2a20 7375 7070 6f72 7473  ectly** supports
+00001c70: 206d 6574 686f 6473 2028 7769 7468 2072   methods (with r
+00001c80: 6570 726f 6475 6374 696f 6e20 7665 7269  eproduction veri
+00001c90: 6669 6564 293a 0a2d 2075 6e69 434f 494c  fied):.- uniCOIL
+00001ca0: 3b0a 2d20 5350 4c41 4445 3a20 476f 2074  ;.- SPLADE: Go t
+00001cb0: 6f20 5b65 7861 6d70 6c65 732f 696e 6665  o [examples/infe
+00001cc0: 7265 6e63 652f 6469 7374 696c 7370 6c61  rence/distilspla
+00001cd0: 6465 5f6d 6178 2f62 6569 725f 7363 6966  de_max/beir_scif
+00001ce0: 6163 745d 2865 7861 6d70 6c65 732f 696e  act](examples/in
+00001cf0: 6665 7265 6e63 652f 6469 7374 696c 7370  ference/distilsp
+00001d00: 6c61 6465 5f6d 6178 2f62 6569 725f 7363  lade_max/beir_sc
+00001d10: 6966 6163 7429 2066 6f72 2066 6173 7420  ifact) for fast 
+00001d20: 7265 7072 6f64 7563 696e 6720 6064 6973  reproducing `dis
+00001d30: 7469 6c73 706c 6164 655f 6d61 7860 206f  tilsplade_max` o
+00001d40: 6e20 5363 6946 6163 743b 0a2d 2053 5041  n SciFact;.- SPA
+00001d50: 5254 413b 0a2d 2054 494c 4445 7632 3a20  RTA;.- TILDEv2: 
+00001d60: 476f 2074 6f20 5b65 7861 6d70 6c65 732f  Go to [examples/
+00001d70: 696e 6665 7265 6e63 652f 7469 6c64 6576  inference/tildev
+00001d80: 322d 6e6f 6578 702f 7472 6563 646c 3230  2-noexp/trecdl20
+00001d90: 3139 5d28 6578 616d 706c 6573 2f69 6e66  19](examples/inf
+00001da0: 6572 656e 6365 2f74 696c 6465 7632 2d6e  erence/tildev2-n
+00001db0: 6f65 7870 2f74 7265 6364 6c32 3031 3929  oexp/trecdl2019)
+00001dc0: 2066 6f72 2066 6173 7420 7265 7072 6f64   for fast reprod
+00001dd0: 7563 696e 6720 6069 656c 6162 2f54 494c  ucing `ielab/TIL
+00001de0: 4445 7632 2d6e 6f45 7870 6020 7265 7261  DEv2-noExp` rera
+00001df0: 6e6b 696e 6720 6f6e 2054 5245 432d 444c  nking on TREC-DL
+00001e00: 2032 3031 393b 0a2d 2044 6565 7049 6d70   2019;.- DeepImp
+00001e10: 6163 740a 0a43 7572 7265 6e74 6c79 2069  act..Currently i
+00001e20: 7420 7375 7070 6f72 7473 2064 6174 6120  t supports data 
+00001e30: 666f 726d 6174 7320 2862 7920 646f 776e  formats (by down
+00001e40: 6c6f 6164 696e 6720 6175 746f 6d61 7469  loading automati
+00001e50: 6361 6c6c 7929 3a0a 2d20 4265 4952 0a0a  cally):.- BeIR..
+00001e60: 4f74 6865 7220 6d6f 6465 6c73 2061 6e64  Other models and
+00001e70: 2064 6174 6120 2866 6f72 6d61 7473 2920   data (formats) 
+00001e80: 7769 6c6c 2062 6520 6164 6465 642e 0a0a  will be added...
+00001e90: 2323 2320 4375 7374 6f6d 2065 6e63 6f64  ### Custom encod
+00001ea0: 6572 730a 546f 2061 6464 2061 2063 7573  ers.To add a cus
+00001eb0: 746f 6d20 656e 636f 6465 722c 206f 6e65  tom encoder, one
+00001ec0: 2063 616e 2072 6566 6572 2074 6f20 7468   can refer to th
+00001ed0: 6520 6578 616d 706c 6520 5b65 7861 6d70  e example [examp
+00001ee0: 6c65 732f 696e 6665 7265 6e63 652f 6375  les/inference/cu
+00001ef0: 7374 6f6d 5f65 6e63 6f64 6572 2f62 6569  stom_encoder/bei
+00001f00: 725f 7363 6966 6163 745d 2865 7861 6d70  r_scifact](examp
+00001f10: 6c65 732f 696e 6665 7265 6e63 652f 6375  les/inference/cu
+00001f20: 7374 6f6d 5f65 6e63 6f64 6572 2f62 6569  stom_encoder/bei
+00001f30: 725f 7363 6966 6163 7429 2c20 7768 6572  r_scifact), wher
+00001f40: 6520 6064 6973 7469 6c73 706c 6164 655f  e `distilsplade_
+00001f50: 6d61 7860 2069 7320 6576 616c 7561 7465  max` is evaluate
+00001f60: 6420 6f6e 2060 4265 4952 2f53 6369 4661  d on `BeIR/SciFa
+00001f70: 6374 6020 2a2a 7769 7468 2073 746f 7077  ct` **with stopw
+00001f80: 6f72 6473 2066 696c 7465 7265 6420 6f75  ords filtered ou
+00001f90: 742a 2a2e 0a0a 496e 2064 6574 6169 6c2c  t**...In detail,
+00001fa0: 206f 6e65 206a 7573 7420 6e65 6564 7320   one just needs 
+00001fb0: 746f 2064 6566 696e 6520 796f 7572 2063  to define your c
+00001fc0: 7573 746f 6d20 656e 636f 6465 7220 636c  ustom encoder cl
+00001fd0: 6173 7320 616e 6420 7772 6974 6520 6120  ass and write a 
+00001fe0: 6e65 7720 656e 636f 6465 7220 6275 696c  new encoder buil
+00001ff0: 6465 7220 6675 6e63 7469 6f6e 3a0a 6060  der function:.``
+00002000: 6070 7974 686f 6e0a 6672 6f6d 2074 7970  `python.from typ
+00002010: 696e 6720 696d 706f 7274 2044 6963 742c  ing import Dict,
+00002020: 204c 6973 740a 6672 6f6d 2070 7973 6572   List.from pyser
+00002030: 696e 692e 656e 636f 6465 2069 6d70 6f72  ini.encode impor
+00002040: 7420 5175 6572 7945 6e63 6f64 6572 2c20  t QueryEncoder, 
+00002050: 446f 6375 6d65 6e74 456e 636f 6465 720a  DocumentEncoder.
+00002060: 0a63 6c61 7373 2043 7573 746f 6d51 7565  .class CustomQue
+00002070: 7279 456e 636f 6465 7228 5175 6572 7945  ryEncoder(QueryE
+00002080: 6e63 6f64 6572 293a 0a0a 2020 2020 6465  ncoder):..    de
+00002090: 6620 656e 636f 6465 2873 656c 662c 2074  f encode(self, t
+000020a0: 6578 742c 202a 2a6b 7761 7267 7329 202d  ext, **kwargs) -
+000020b0: 3e20 4469 6374 5b73 7472 2c20 666c 6f61  > Dict[str, floa
+000020c0: 745d 3a0a 2020 2020 2020 2020 2320 4a75  t]:.        # Ju
+000020d0: 7374 2061 6e20 6578 616d 706c 653a 0a20  st an example:. 
+000020e0: 2020 2020 2020 2074 6572 6d73 203d 2074         terms = t
+000020f0: 6578 742e 7370 6c69 7428 290a 2020 2020  ext.split().    
+00002100: 2020 2020 7465 726d 5f77 6569 6768 7473      term_weights
+00002110: 203d 207b 7465 726d 3a20 3120 666f 7220   = {term: 1 for 
+00002120: 7465 726d 2069 6e20 7465 726d 737d 0a20  term in terms}. 
+00002130: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+00002140: 726d 5f77 6569 6768 7473 2020 2320 4469  rm_weights  # Di
+00002150: 6374 206f 626a 6563 742c 2077 6865 7265  ct object, where
+00002160: 206b 6579 732f 7661 6c75 6573 2061 7265   keys/values are
+00002170: 2074 6572 6d73 2f74 6572 6d20 7363 6f72   terms/term scor
+00002180: 6573 2c20 7265 7370 2e0a 0a63 6c61 7373  es, resp...class
+00002190: 2043 7573 746f 6d44 6f63 756d 656e 7445   CustomDocumentE
+000021a0: 6e63 6f64 6572 2844 6f63 756d 656e 7445  ncoder(DocumentE
+000021b0: 6e63 6f64 6572 293a 0a0a 2020 2020 6465  ncoder):..    de
+000021c0: 6620 656e 636f 6465 2873 656c 662c 2074  f encode(self, t
+000021d0: 6578 7473 2c20 2a2a 6b77 6172 6773 2920  exts, **kwargs) 
+000021e0: 2d3e 204c 6973 745b 4469 6374 5b73 7472  -> List[Dict[str
+000021f0: 2c20 666c 6f61 745d 5d3a 0a20 2020 2020  , float]]:.     
+00002200: 2020 2023 204a 7573 7420 616e 2065 7861     # Just an exa
+00002210: 6d70 6c65 3a0a 2020 2020 2020 2020 7465  mple:.        te
+00002220: 726d 5f77 6569 6768 7473 5f62 6174 6368  rm_weights_batch
+00002230: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00002240: 7220 7465 7874 2069 6e20 7465 7874 733a  r text in texts:
+00002250: 0a20 2020 2020 2020 2020 2020 2074 6572  .            ter
+00002260: 6d73 203d 2074 6578 742e 7370 6c69 7428  ms = text.split(
+00002270: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
+00002280: 726d 5f77 6569 6768 7473 203d 207b 7465  rm_weights = {te
+00002290: 726d 3a20 3120 666f 7220 7465 726d 2069  rm: 1 for term i
+000022a0: 6e20 7465 726d 737d 0a20 2020 2020 2020  n terms}.       
+000022b0: 2020 2020 2074 6572 6d5f 7765 6967 6874       term_weight
+000022c0: 735f 6261 7463 682e 6170 7065 6e64 2874  s_batch.append(t
+000022d0: 6572 6d5f 7765 6967 6874 7329 0a20 2020  erm_weights).   
+000022e0: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
+000022f0: 5f77 6569 6768 7473 5f62 6174 6368 200a  _weights_batch .
+00002300: 0a64 6566 2063 7573 746f 6d5f 656e 636f  .def custom_enco
+00002310: 6465 725f 6275 696c 6465 7228 636b 7074  der_builder(ckpt
+00002320: 5f6e 616d 652c 2065 7479 7065 2c20 6465  _name, etype, de
+00002330: 7669 6365 3d27 6370 7527 293a 0a20 2020  vice='cpu'):.   
+00002340: 2069 6620 6574 7970 6520 3d3d 2027 7175   if etype == 'qu
+00002350: 6572 7927 3a0a 2020 2020 2020 2020 7265  ery':.        re
+00002360: 7475 726e 2043 7573 746f 6d51 7565 7279  turn CustomQuery
+00002370: 456e 636f 6465 7228 636b 7074 5f6e 616d  Encoder(ckpt_nam
+00002380: 652c 2064 6576 6963 653d 6465 7669 6365  e, device=device
+00002390: 2920 2020 2020 2020 200a 2020 2020 656c  )        .    el
+000023a0: 6966 2065 7479 7065 203d 3d20 2764 6f63  if etype == 'doc
+000023b0: 756d 656e 7427 3a0a 2020 2020 2020 2020  ument':.        
+000023c0: 7265 7475 726e 2043 7573 746f 6d44 6f63  return CustomDoc
+000023d0: 756d 656e 7445 6e63 6f64 6572 2863 6b70  umentEncoder(ckp
+000023e0: 745f 6e61 6d65 2c20 6465 7669 6365 3d64  t_name, device=d
+000023f0: 6576 6963 6529 0a20 2020 2065 6c73 653a  evice).    else:
+00002400: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00002410: 616c 7565 4572 726f 720a 6060 600a 5468  alueError.```.Th
+00002420: 656e 2072 6567 6973 7465 7220 6063 7573  en register `cus
+00002430: 746f 6d5f 656e 636f 6465 725f 6275 696c  tom_encoder_buil
+00002440: 6465 7260 2077 6974 6820 6073 7072 696e  der` with `sprin
+00002450: 742e 696e 6665 7265 6e63 652e 656e 636f  t.inference.enco
+00002460: 6465 725f 6275 696c 6465 7273 2e72 6567  der_builders.reg
+00002470: 6973 7465 7260 2062 6566 6f72 6520 7573  ister` before us
+00002480: 6167 653a 0a60 6060 7079 7468 6f6e 0a66  age:.```python.f
+00002490: 726f 6d20 7370 7269 6e74 2e69 6e66 6572  rom sprint.infer
+000024a0: 656e 6365 2e65 6e63 6f64 6572 5f62 7569  ence.encoder_bui
+000024b0: 6c64 6572 7320 696d 706f 7274 2072 6567  lders import reg
+000024c0: 6973 7465 720a 0a72 6567 6973 7465 7228  ister..register(
+000024d0: 2763 7573 746f 6d5f 656e 636f 6465 725f  'custom_encoder_
+000024e0: 6275 696c 6465 7227 2c20 6375 7374 6f6d  builder', custom
+000024f0: 5f65 6e63 6f64 6572 5f62 7569 6c64 6572  _encoder_builder
+00002500: 290a 6060 600a 0a23 2320 5472 6169 6e69  ).```..## Traini
+00002510: 6e67 2028 4578 7065 7269 6d65 6e74 616c  ng (Experimental
+00002520: 290a 5769 6c6c 2062 6520 6164 6465 642e  ).Will be added.
+00002530: 0a0a 2323 2043 6f6e 7461 6374 730a 5468  ..## Contacts.Th
+00002540: 6520 6d61 696e 2063 6f6e 7472 6962 7574  e main contribut
+00002550: 6f72 7320 6f66 2074 6869 7320 7265 706f  ors of this repo
+00002560: 7369 746f 7279 2061 7265 3a0a 0a2d 205b  sitory are:..- [
+00002570: 4e61 6e64 616e 2054 6861 6b75 725d 2868  Nandan Thakur](h
+00002580: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002590: 6d2f 4e74 6861 6b75 7232 3029 0a2d 205b  m/Nthakur20).- [
+000025a0: 4b65 7869 6e20 5761 6e67 5d28 6874 7470  Kexin Wang](http
+000025b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+000025c0: 7761 6e67 3230 3439 290a                 wang2049).
```

