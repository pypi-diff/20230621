# Comparing `tmp/nkululeko-0.48.1.tar.gz` & `tmp/nkululeko-0.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.48.1.tar", last modified: Thu Jun 15 08:43:08 2023, max compression
+gzip compressed data, was "nkululeko-0.49.0.tar", last modified: Wed Jun 21 11:55:16 2023, max compression
```

## Comparing `nkululeko-0.48.1.tar` & `nkululeko-0.49.0.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-15 08:43:08.480520 nkululeko-0.48.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6507 2023-06-15 08:23:15.000000 nkululeko-0.48.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.48.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18233 2023-06-15 08:43:08.480520 nkululeko-0.48.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.48.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-15 08:43:08.480520 nkululeko-0.48.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.48.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.48.1/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.48.1/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.48.1/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.48.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-15 08:22:24.000000 nkululeko-0.48.1/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21705 2023-06-15 08:31:25.000000 nkululeko-0.48.1/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.48.1/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.48.1/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.48.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.48.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20319 2023-05-23 12:09:53.000000 nkululeko-0.48.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.48.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.48.1/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.48.1/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.48.1/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.48.1/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.48.1/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.48.1/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3756 2023-06-14 15:21:48.000000 nkululeko-0.48.1/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.48.1/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3012 2023-06-14 15:21:48.000000 nkululeko-0.48.1/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.48.1/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.48.1/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.48.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.48.1/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19509 2023-05-25 16:45:46.000000 nkululeko-0.48.1/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.48.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.48.1/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.48.1/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.48.1/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.48.1/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.48.1/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.48.1/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.48.1/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.48.1/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.48.1/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.48.1/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.48.1/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.48.1/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.48.1/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.48.1/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.48.1/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.48.1/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.48.1/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.48.1/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.48.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.48.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.48.1/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.48.1/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.48.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.48.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.48.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.48.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.48.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8967 2023-05-23 11:38:09.000000 nkululeko-0.48.1/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-15 08:43:08.480520 nkululeko-0.48.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18233 2023-06-15 08:43:08.000000 nkululeko-0.48.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1594 2023-06-15 08:43:08.000000 nkululeko-0.48.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-15 08:43:08.000000 nkululeko-0.48.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-15 08:43:08.000000 nkululeko-0.48.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-15 08:43:08.000000 nkululeko-0.48.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.48.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-15 08:43:08.480520 nkululeko-0.48.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.48.1/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-21 11:55:16.825416 nkululeko-0.49.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6562 2023-06-21 11:38:47.000000 nkululeko-0.49.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.49.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18288 2023-06-21 11:55:16.825416 nkululeko-0.49.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.49.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-21 11:55:16.825416 nkululeko-0.49.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.49.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-06-19 14:49:48.000000 nkululeko-0.49.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2404 2023-06-21 11:09:59.000000 nkululeko-0.49.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.49.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.49.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-21 11:36:09.000000 nkululeko-0.49.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21705 2023-06-15 08:31:25.000000 nkululeko-0.49.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.49.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.49.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.49.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.49.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21185 2023-06-19 14:52:26.000000 nkululeko-0.49.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.49.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.49.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.49.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.49.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.49.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.49.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.49.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3756 2023-06-14 15:21:48.000000 nkululeko-0.49.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.49.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3012 2023-06-14 15:21:48.000000 nkululeko-0.49.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.49.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.49.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.49.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.49.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-21 11:41:47.000000 nkululeko-0.49.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.49.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.49.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.49.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.49.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.49.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.49.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.49.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.49.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.49.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.49.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.49.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.49.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.49.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.49.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.49.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.49.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.49.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.49.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.49.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.49.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.49.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2659 2023-06-21 11:28:55.000000 nkululeko-0.49.0/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-21 11:03:40.000000 nkululeko-0.49.0/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.49.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.49.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.49.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.49.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.49.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.49.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.49.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8967 2023-05-23 11:38:09.000000 nkululeko-0.49.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-21 11:55:16.825416 nkululeko-0.49.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18288 2023-06-21 11:55:16.000000 nkululeko-0.49.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-06-21 11:55:16.000000 nkululeko-0.49.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-21 11:55:16.000000 nkululeko-0.49.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-21 11:55:16.000000 nkululeko-0.49.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-21 11:55:16.000000 nkululeko-0.49.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.49.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-21 11:55:16.825416 nkululeko-0.49.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.49.0/setup.py
```

### Comparing `nkululeko-0.48.1/CHANGELOG.md` & `nkululeko-0.49.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.49.0
+--------------
+* added random-splicing
+
 Version 0.48.1
 --------------
 * bugfix: database object was not loaded when dataframe was reused
 
 Version 0.48.0
 --------------
 * enabled specific feature selection for praat and opensmile features
```

### Comparing `nkululeko-0.48.1/LICENSE` & `nkululeko-0.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/PKG-INFO` & `nkululeko-0.49.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.48.1
+Version: 0.49.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -210,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.49.0
+--------------
+* added random-splicing
+
 Version 0.48.1
 --------------
 * bugfix: database object was not loaded when dataframe was reused
 
 Version 0.48.0
 --------------
 * enabled specific feature selection for praat and opensmile features
```

### Comparing `nkululeko-0.48.1/README.md` & `nkululeko-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/augment.py` & `nkululeko-0.49.0/nkululeko/nkululeko.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-# augment.py
-# augment the training sets
+# nkululeko.py
+# Entry script to do a Nkululeko experiment
 
-from nkululeko.experiment import Experiment
+import nkululeko.experiment as exp
 import configparser
 from nkululeko.util import Util
-from  nkululeko.constants import VERSION
+import os.path
+from nkululeko.constants import VERSION
 import argparse
-import os
 
 def main(src_dir):
     parser = argparse.ArgumentParser(description='Call the nkululeko framework.')
     parser.add_argument('--config', default='exp.ini', help='The base configuration')
     args = parser.parse_args()
     if args.config is not None:
         config_file = args.config    
     else:
         config_file = f'{src_dir}/exp.ini'
 
     # test if the configuration file exists
     if not os.path.isfile(config_file):
         print(f'ERROR: no such file: {config_file}')
         exit()
-        
+
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
+    
     # create a new experiment
-    expr = Experiment(config)
+    expr = exp.Experiment(config)
     util = Util()
-    util.debug(f'running {expr.name}, nkululeko version {VERSION}')
+    util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
     util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
 
-    # augment
-    expr.augment()
+    # extract features
+    expr.extract_feats()
 
-    print('DONE')
+    # initialize a run manager
+    expr.init_runmanager()
 
+    # run the experiment
+    expr.run()
+
+    print('DONE')
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
-    main(cwd) # use this if you want to state the config file path on command line
+    main(cwd) # use this if you want to state the config file path on command line
```

### Comparing `nkululeko-0.48.1/nkululeko/augmenter.py` & `nkululeko-0.49.0/nkululeko/augmenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from audformat.utils import map_file_path
 import audeer
 
 class Augmenter:
     """
         augmenting the train split
     """
-    def __init__(self, train_df):
-        self.train_df = train_df
+    def __init__(self, df):
+        self.df = df
         self.util = Util()
         # Define a standard transformation that randomly add augmentations to files
         self.audioment = Compose([
             AddGaussianNoise(min_amplitude=0.001, max_amplitude=0.015, p=0.5),
             TimeStretch(min_rate=0.8, max_rate=1.25, p=0.5),
             PitchShift(min_semitones=-4, max_semitones=4, p=0.5),
             Shift(min_fraction=-0.5, max_fraction=0.5, p=0.5),
@@ -26,35 +26,35 @@
     def changepath(self, fp, np):
 #        parent = os.path.dirname(fp).split('/')[-1]
         fullpath = os.path.dirname(fp)
  #       newpath = f'{np}{parent}'
  #       audeer.mkdir(newpath)
         return fp.replace(fullpath, np)
 
-    def augment(self):
+    def augment(self, sample_selection):
         """
         augment the training files and return a dataframe with new files index.
         """
-        files = self.train_df.index.get_level_values(0).values
+        files = self.df.index.get_level_values(0).values
         store = self.util.get_path('store')
         filepath = f'{store}augmentations/'
         audeer.mkdir(filepath)
-        self.util.debug(f'augmenting the training set to {filepath}')
+        self.util.debug(f'augmenting {sample_selection} samples to {filepath}')
         newpath = ''
         for i, f in enumerate(files):
             signal, sr = audiofile.read(f)
             filename = os.path.basename(f)
             parent = os.path.dirname(f).split('/')[-1]
             sig_aug = self.audioment(samples = signal, sample_rate = sr)
             newpath = f'{filepath}/{parent}/'
             audeer.mkdir(newpath)
             audiofile.write(f'{newpath}{filename}', signal=sig_aug, sampling_rate=sr)
             if i%10==0:
                 print(f'augmented {i} of {len(files)}')
-        df_ret = self.train_df.copy()
+        df_ret = self.df.copy()
         df_ret = df_ret.set_index(map_file_path(df_ret.index, lambda x: self.changepath(x, newpath)))
-        aug_db_filename = self.util.config_val('DATA', 'augment', 'augment.csv')
+        aug_db_filename = self.util.config_val('DATA', 'augment_result', 'augment.csv')
         target = self.util.config_val('DATA', 'target', 'emotion')
         df_ret[target] = df_ret['class_label']
         df_ret = df_ret.drop(columns=['class_label'])
         df_ret.to_csv(aug_db_filename)
         return df_ret
```

### Comparing `nkululeko-0.48.1/nkululeko/cacheddataset.py` & `nkululeko-0.49.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/dataset.py` & `nkululeko-0.49.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/dataset_csv.py` & `nkululeko-0.49.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/dataset_ravdess.py` & `nkululeko-0.49.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/demo.py` & `nkululeko-0.49.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/demo_predictor.py` & `nkululeko-0.49.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/experiment.py` & `nkululeko-0.49.0/nkululeko/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,26 +288,46 @@
         self.feats_test = self.feature_extractor.extract()
         self.util.debug(f'All features: train shape : {self.feats_train.shape}, test shape:{self.feats_test.shape}')
 
         self._check_scale()
 
     def augment(self):
         """
-        Augment the training set
+        Augment the selected samples
         """
         from nkululeko.augmenter import Augmenter
-        augmenter = Augmenter(self.df_train)
-        augmenter.augment()
+        sample_selection = self.util.config_val(' DATA', 'augment', 'train')
+        if sample_selection=='all':
+            df = pd.concat([self.df_train, self.df_test])
+        elif sample_selection=='train':
+            df = self.df_train
+        elif sample_selection=='test':
+            df = self.df_test
+        else:
+            self.util.error(f'unknown augmentation selection specifier {sample_selection}, should be [all | train | test]')
 
-    # def augment_train(self):
-    #     """Augment the train dataframe"""
-    #     from nkululeko.augmenter import Augmenter
-    #     augment_train = Augmenter(self.df_train)
-    #     df_train_aug = augment_train.augment()
-    #     self.df_train = self.df_train.append(df_train_aug)
+        augmenter = Augmenter(df)
+        augmenter.augment(sample_selection)
+
+    def random_splice(self):
+        """
+        Random-splice the selected samples
+        """
+        from nkululeko.randomsplicer import Randomsplicer
+        sample_selection = self.util.config_val(' DATA', 'random_splice', 'train')
+        if sample_selection=='all':
+            df = pd.concat([self.df_train, self.df_test])
+        elif sample_selection=='train':
+            df = self.df_train
+        elif sample_selection=='test':
+            df = self.df_test
+        else:
+            self.util.error(f'unknown augmentation selection specifier {sample_selection}, should be [all | train | test]')
+        randomsplicer = Randomsplicer(df)
+        randomsplicer.run(sample_selection)
 
 
     def analyse_features(self, needs_feats):
         """
         Do a feature exploration
         
         """
```

### Comparing `nkululeko-0.48.1/nkululeko/explore.py` & `nkululeko-0.49.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_analyser.py` & `nkululeko-0.49.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_audmodel.py` & `nkululeko-0.49.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.49.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_clap.py` & `nkululeko-0.49.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_import.py` & `nkululeko-0.49.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_mld.py` & `nkululeko-0.49.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_opensmile.py` & `nkululeko-0.49.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_oxbow.py` & `nkululeko-0.49.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_praat.py` & `nkululeko-0.49.0/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_trill.py` & `nkululeko-0.49.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feats_wav2vec2.py` & `nkululeko-0.49.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feature_extractor.py` & `nkululeko-0.49.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/featureset.py` & `nkululeko-0.49.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/feinberg_praat.py` & `nkululeko-0.49.0/nkululeko/feinberg_praat.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         x[np.isnan(x)] = 0
     if np.any(np.isfinite(x)):
         print (f'Warning: {np.count_nonzero(np.isfinite(x))} infinite in x')
     
     # PCA
     pca = PCA(n_components=2)
     principalComponents = pca.fit_transform(x)
-    print(type(principalComponents))
     if np.any(np.isnan(principalComponents)):
         print ('pc is nan')
         print(f'count: {np.count_nonzero(np.isnan(principalComponents))}')
         print(principalComponents)
         principalComponents=np.nan_to_num(principalComponents)
 
     principalDf = pd.DataFrame(data = principalComponents, columns = ['JitterPCA', 'ShimmerPCA'])
```

### Comparing `nkululeko-0.48.1/nkululeko/filter_data.py` & `nkululeko-0.49.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/loss_ccc.py` & `nkululeko-0.49.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/loss_softf1loss.py` & `nkululeko-0.49.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model.py` & `nkululeko-0.49.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model_cnn.py` & `nkululeko-0.49.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model_gmm.py` & `nkululeko-0.49.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model_knn.py` & `nkululeko-0.49.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model_knn_reg.py` & `nkululeko-0.49.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model_mlp.py` & `nkululeko-0.49.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model_mlp_regression.py` & `nkululeko-0.49.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/model_svm.py` & `nkululeko-0.49.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/modelrunner.py` & `nkululeko-0.49.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/nkululeko.py` & `nkululeko-0.49.0/nkululeko/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-# nkululeko.py
-# Entry script to do a Nkululeko experiment
+# test.py
+# Just use a database as test
 
-import nkululeko.experiment as exp
+from nkululeko.experiment import Experiment
 import configparser
 from nkululeko.util import Util
-import os.path
-from nkululeko.constants import VERSION
+from  nkululeko.constants import VERSION
 import argparse
+import os
 
 def main(src_dir):
     parser = argparse.ArgumentParser(description='Call the nkululeko framework.')
     parser.add_argument('--config', default='exp.ini', help='The base configuration')
+    parser.add_argument('--outfile', default='my_results.csv', help='File name to store the predictions')
+
     args = parser.parse_args()
-    if args.config is not None:
-        config_file = args.config    
-    else:
-        config_file = f'{src_dir}/exp.ini'
+
+    config_file = args.config    
 
     # test if the configuration file exists
     if not os.path.isfile(config_file):
         print(f'ERROR: no such file: {config_file}')
         exit()
-
+        
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     
     # create a new experiment
-    expr = exp.Experiment(config)
+    expr = Experiment(config)
     util = Util()
     util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
-    # load the data
-    expr.load_datasets()
-
-    # split into train and test
-    expr.fill_train_and_tests()
-    util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
-
-    # extract features
-    expr.extract_feats()
-
-    # initialize a run manager
-    expr.init_runmanager()
-
-    # run the experiment
-    expr.run()
+    # load the experiment
+    expr.load(f'{util.get_save_name()}')
+    expr.fill_tests()
+    expr.extract_test_feats()
+    expr.predict_test_and_save(args.outfile)
 
     print('DONE')
 
+
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
-    main(cwd) # use this if you want to state the config file path on command line
+    main(cwd) # use this if you want to state the config file path on command line
```

### Comparing `nkululeko-0.48.1/nkululeko/plots.py` & `nkululeko-0.49.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/reporter.py` & `nkululeko-0.49.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/runmanager.py` & `nkululeko-0.49.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/scaler.py` & `nkululeko-0.49.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.49.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/test.py` & `nkululeko-0.49.0/nkululeko/augment.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,54 @@
-# test.py
-# Just use a database as test
+# augment.py
+# augment the training sets
 
 from nkululeko.experiment import Experiment
 import configparser
 from nkululeko.util import Util
 from  nkululeko.constants import VERSION
 import argparse
 import os
 
 def main(src_dir):
     parser = argparse.ArgumentParser(description='Call the nkululeko framework.')
     parser.add_argument('--config', default='exp.ini', help='The base configuration')
-    parser.add_argument('--outfile', default='my_results.csv', help='File name to store the predictions')
-
     args = parser.parse_args()
-
-    config_file = args.config    
+    if args.config is not None:
+        config_file = args.config    
+    else:
+        config_file = f'{src_dir}/exp.ini'
 
     # test if the configuration file exists
     if not os.path.isfile(config_file):
         print(f'ERROR: no such file: {config_file}')
         exit()
         
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
-    
     # create a new experiment
     expr = Experiment(config)
     util = Util()
-    util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
+    util.debug(f'running {expr.name}, nkululeko version {VERSION}')
 
-    # load the experiment
-    expr.load(f'{util.get_save_name()}')
-    expr.fill_tests()
-    expr.extract_test_feats()
-    expr.predict_test_and_save(args.outfile)
+    # load the data
+    expr.load_datasets()
+
+    # split into train and test
+    expr.fill_train_and_tests()
+    util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
+
+    # augment
+    augmenting = util.config_val('DATA', 'augment', False)
+    if augmenting:
+        expr.augment()
+    
+    random_splicing = util.config_val('DATA', 'random_splice', False)
+    if random_splicing:
+        expr.random_splice()
 
     print('DONE')
 
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
     main(cwd) # use this if you want to state the config file path on command line
```

### Comparing `nkululeko-0.48.1/nkululeko/test_predictor.py` & `nkululeko-0.49.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko/util.py` & `nkululeko-0.49.0/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.48.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.49.0/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.48.1
+Version: 0.49.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -210,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.49.0
+--------------
+* added random-splicing
+
 Version 0.48.1
 --------------
 * bugfix: database object was not loaded when dataframe was reused
 
 Version 0.48.0
 --------------
 * enabled specific feature selection for praat and opensmile features
```

### Comparing `nkululeko-0.48.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.49.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 nkululeko/model_tree.py
 nkululeko/model_tree_reg.py
 nkululeko/model_xgb.py
 nkululeko/model_xgr.py
 nkululeko/modelrunner.py
 nkululeko/nkululeko.py
 nkululeko/plots.py
+nkululeko/randomsplicer.py
+nkululeko/randomsplicing.py
 nkululeko/reporter.py
 nkululeko/result.py
 nkululeko/runmanager.py
 nkululeko/scaler.py
 nkululeko/syllable_nuclei.py
 nkululeko/test.py
 nkululeko/test_predictor.py
```

### Comparing `nkululeko-0.48.1/setup.cfg` & `nkululeko-0.49.0/setup.cfg`

 * *Files identical despite different names*

