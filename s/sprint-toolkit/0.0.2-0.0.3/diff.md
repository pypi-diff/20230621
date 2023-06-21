# Comparing `tmp/sprint-toolkit-0.0.2.tar.gz` & `tmp/sprint-toolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprint-toolkit-0.0.2.tar", last modified: Wed Jun 21 18:36:06 2023, max compression
+gzip compressed data, was "sprint-toolkit-0.0.3.tar", last modified: Wed Jun 21 18:40:05 2023, max compression
```

## Comparing `sprint-toolkit-0.0.2.tar` & `sprint-toolkit-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.870297 sprint-toolkit-0.0.2/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    11348 2023-03-31 16:14:19.000000 sprint-toolkit-0.0.2/LICENSE
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9674 2023-06-21 18:36:06.870297 sprint-toolkit-0.0.2/PKG-INFO
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     8869 2023-06-21 17:02:38.000000 sprint-toolkit-0.0.2/README.md
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       79 2023-06-21 18:36:06.870297 sprint-toolkit-0.0.2/setup.cfg
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1117 2023-06-21 18:36:03.000000 sprint-toolkit-0.0.2/setup.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.862297 sprint-toolkit-0.0.2/sprint_toolkit/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       50 2023-06-21 18:02:32.000000 sprint-toolkit-0.0.2/sprint_toolkit/__init__.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/inference/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       36 2023-03-16 18:11:55.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/__init__.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7441 2023-03-16 18:16:31.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/aio.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1463 2023-03-16 18:25:20.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/data_iters.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6745 2023-03-16 18:37:18.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/encode.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3749 2023-02-18 19:47:29.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/encoder_builders.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2916 2023-06-19 17:12:28.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/evaluate.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2146 2023-01-10 15:57:46.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/index.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      405 2023-03-16 18:11:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/logging.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      327 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/__init__.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    13043 2023-03-16 17:11:56.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/deepimpact.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5812 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/sparta.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5015 2023-03-02 19:25:37.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/splade.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9631 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/tildev2.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7559 2023-02-18 14:25:57.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/unicoil.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5049 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/quantize.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1313 2023-02-18 19:48:23.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/reformat_query.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5164 2023-02-02 15:27:55.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/rerank.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    15528 2023-02-15 16:41:17.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/search.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1010 2023-01-31 15:31:10.000000 sprint-toolkit-0.0.2/sprint_toolkit/inference/utils.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       34 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/__init__.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1231 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/MSMARCODataLoader.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3877 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/MSMARCOGroupedDataLoader.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      108 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/__init__.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1940 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/MarginMSELoss.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3203 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/MultipleNegativeRankingLoss.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      122 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/__init__.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      847 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/losses/utils.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.866297 sprint-toolkit-0.0.2/sprint_toolkit/train/models/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      127 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/__init__.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6036 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/deepimpact.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2453 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/sparta.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     8792 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/splade.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4105 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/tilde.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9426 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/unicoil.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3192 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/models/utils.py
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3695 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.2/sprint_toolkit/train/trainer.py
-drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:36:06.862297 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9674 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1674 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        1 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       14 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/requires.txt
--rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       15 2023-06-21 18:36:06.000000 sprint-toolkit-0.0.2/sprint_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.817342 sprint-toolkit-0.0.3/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    11348 2023-03-31 16:14:19.000000 sprint-toolkit-0.0.3/LICENSE
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9674 2023-06-21 18:40:05.817342 sprint-toolkit-0.0.3/PKG-INFO
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     8869 2023-06-21 17:02:38.000000 sprint-toolkit-0.0.3/README.md
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       79 2023-06-21 18:40:05.817342 sprint-toolkit-0.0.3/setup.cfg
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1117 2023-06-21 18:39:54.000000 sprint-toolkit-0.0.3/setup.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.809342 sprint-toolkit-0.0.3/sprint_toolkit/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:39:28.000000 sprint-toolkit-0.0.3/sprint_toolkit/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.813342 sprint-toolkit-0.0.3/sprint_toolkit/inference/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       36 2023-03-16 18:11:55.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7441 2023-03-16 18:16:31.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/aio.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1463 2023-03-16 18:25:20.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/data_iters.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6745 2023-03-16 18:37:18.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/encode.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3749 2023-02-18 19:47:29.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/encoder_builders.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2916 2023-06-19 17:12:28.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/evaluate.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2146 2023-01-10 15:57:46.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/index.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      405 2023-03-16 18:11:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/logging.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.813342 sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      327 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    13043 2023-03-16 17:11:56.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/deepimpact.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5812 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/sparta.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5015 2023-03-02 19:25:37.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/splade.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9631 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/tildev2.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7559 2023-02-18 14:25:57.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/unicoil.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5049 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/quantize.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1313 2023-02-18 19:48:23.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/reformat_query.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5164 2023-02-02 15:27:55.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/rerank.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    15528 2023-02-15 16:41:17.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/search.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1010 2023-01-31 15:31:10.000000 sprint-toolkit-0.0.3/sprint_toolkit/inference/utils.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.813342 sprint-toolkit-0.0.3/sprint_toolkit/train/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       34 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.813342 sprint-toolkit-0.0.3/sprint_toolkit/train/dataloaders/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1231 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/dataloaders/MSMARCODataLoader.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3877 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/dataloaders/MSMARCOGroupedDataLoader.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      108 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/dataloaders/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.813342 sprint-toolkit-0.0.3/sprint_toolkit/train/losses/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1940 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/losses/MarginMSELoss.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3203 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/losses/MultipleNegativeRankingLoss.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      122 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/losses/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      847 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/losses/utils.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.817342 sprint-toolkit-0.0.3/sprint_toolkit/train/models/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      127 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/models/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6036 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/models/deepimpact.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2453 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/models/sparta.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     8792 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/models/splade.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4105 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/models/tilde.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9426 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/models/unicoil.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3192 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/models/utils.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3695 2022-05-03 16:06:35.000000 sprint-toolkit-0.0.3/sprint_toolkit/train/trainer.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-06-21 18:40:05.813342 sprint-toolkit-0.0.3/sprint_toolkit.egg-info/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9674 2023-06-21 18:40:05.000000 sprint-toolkit-0.0.3/sprint_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1674 2023-06-21 18:40:05.000000 sprint-toolkit-0.0.3/sprint_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        1 2023-06-21 18:40:05.000000 sprint-toolkit-0.0.3/sprint_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       14 2023-06-21 18:40:05.000000 sprint-toolkit-0.0.3/sprint_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       15 2023-06-21 18:40:05.000000 sprint-toolkit-0.0.3/sprint_toolkit.egg-info/top_level.txt
```

### Comparing `sprint-toolkit-0.0.2/LICENSE` & `sprint-toolkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/PKG-INFO` & `sprint-toolkit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint-toolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: SPRINT: A Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse Retrieval
 Home-page: https://github.com/thakur-nandan/sprint
 Author: Nandan Thakur
 Author-email: nandant@gmail.com
 Project-URL: Bug Tracker, https://github.com/thakur-nandan/sprint/issues
 Keywords: Information Retrieval Toolkit Sparse Retrievers Networks BERT PyTorch IR NLP deep learning
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprint-toolkit Version: 0.0.2 Summary: SPRINT: A
+Metadata-Version: 2.1 Name: sprint-toolkit Version: 0.0.3 Summary: SPRINT: A
 Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse
 Retrieval Home-page: https://github.com/thakur-nandan/sprint Author: Nandan
 Thakur Author-email: nandant@gmail.com Project-URL: Bug Tracker, https://
 github.com/thakur-nandan/sprint/issues Keywords: Information Retrieval Toolkit
 Sparse Retrievers Networks BERT PyTorch IR NLP deep learning Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
```

### Comparing `sprint-toolkit-0.0.2/README.md` & `sprint-toolkit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/setup.py` & `sprint-toolkit-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 setup(
     name="sprint-toolkit",
-    version="0.0.2",
+    version="0.0.3",
     author="Nandan Thakur",
     author_email="nandant@gmail.com",
     description="SPRINT: A Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse Retrieval",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/thakur-nandan/sprint",
     project_urls={
```

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/aio.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/aio.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/data_iters.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/data_iters.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/encode.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/encode.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/encoder_builders.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/encoder_builders.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/evaluate.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/evaluate.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/index.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/index.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/deepimpact.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/deepimpact.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/sparta.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/sparta.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/splade.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/splade.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/tildev2.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/tildev2.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/methods/unicoil.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/methods/unicoil.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/quantize.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/quantize.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/reformat_query.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/reformat_query.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/rerank.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/rerank.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/search.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/search.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/inference/utils.py` & `sprint-toolkit-0.0.3/sprint_toolkit/inference/utils.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/MSMARCODataLoader.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/dataloaders/MSMARCODataLoader.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/dataloaders/MSMARCOGroupedDataLoader.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/dataloaders/MSMARCOGroupedDataLoader.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/losses/MarginMSELoss.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/losses/MarginMSELoss.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/losses/MultipleNegativeRankingLoss.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/losses/MultipleNegativeRankingLoss.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/losses/utils.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/losses/utils.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/models/deepimpact.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/models/deepimpact.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/models/sparta.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/models/sparta.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/models/splade.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/models/splade.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/models/tilde.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/models/tilde.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/models/unicoil.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/models/unicoil.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/models/utils.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/models/utils.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit/train/trainer.py` & `sprint-toolkit-0.0.3/sprint_toolkit/train/trainer.py`

 * *Files identical despite different names*

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit.egg-info/PKG-INFO` & `sprint-toolkit-0.0.3/sprint_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint-toolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: SPRINT: A Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse Retrieval
 Home-page: https://github.com/thakur-nandan/sprint
 Author: Nandan Thakur
 Author-email: nandant@gmail.com
 Project-URL: Bug Tracker, https://github.com/thakur-nandan/sprint/issues
 Keywords: Information Retrieval Toolkit Sparse Retrievers Networks BERT PyTorch IR NLP deep learning
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprint-toolkit Version: 0.0.2 Summary: SPRINT: A
+Metadata-Version: 2.1 Name: sprint-toolkit Version: 0.0.3 Summary: SPRINT: A
 Unified Toolkit for Evaluating and Demystifying Zero-shot Neural Sparse
 Retrieval Home-page: https://github.com/thakur-nandan/sprint Author: Nandan
 Thakur Author-email: nandant@gmail.com Project-URL: Bug Tracker, https://
 github.com/thakur-nandan/sprint/issues Keywords: Information Retrieval Toolkit
 Sparse Retrievers Networks BERT PyTorch IR NLP deep learning Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
```

### Comparing `sprint-toolkit-0.0.2/sprint_toolkit.egg-info/SOURCES.txt` & `sprint-toolkit-0.0.3/sprint_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

