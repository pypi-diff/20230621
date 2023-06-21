# Comparing `tmp/dcnum-0.0.7.tar.gz` & `tmp/dcnum-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.7.tar", last modified: Fri Jun 16 13:44:31 2023, max compression
+gzip compressed data, was "dcnum-0.0.8.tar", last modified: Wed Jun 21 21:09:59 2023, max compression
```

## Comparing `dcnum-0.0.7.tar` & `dcnum-0.0.8.tar`

### file list

```diff
@@ -1,82 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.934601 dcnum-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-16 13:44:19.000000 dcnum-0.0.7/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-16 13:44:19.000000 dcnum-0.0.7/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-16 13:44:19.000000 dcnum-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-16 13:44:19.000000 dcnum-0.0.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-16 13:44:19.000000 dcnum-0.0.7/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 13:44:19.000000 dcnum-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-16 13:44:31.942601 dcnum-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-16 13:44:19.000000 dcnum-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/brightness/bright_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/haralick/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/haralick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/haralick/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/haralick/tex_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/feat/moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/feat/moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/segm/segmenter_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/write/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-16 13:44:19.000000 dcnum-0.0.7/dcnum/write/writer_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.938601 dcnum-0.0.7/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:44:31.000000 dcnum-0.0.7/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 13:44:19.000000 dcnum-0.0.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-16 13:44:19.000000 dcnum-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:44:31.942601 dcnum-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:44:31.942601 dcnum-0.0.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_write_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 13:44:19.000000 dcnum-0.0.7/tests/test_write_writer_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.576246 dcnum-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.564245 dcnum-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 21:09:46.000000 dcnum-0.0.8/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 21:09:46.000000 dcnum-0.0.8/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-21 21:09:46.000000 dcnum-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 21:09:46.000000 dcnum-0.0.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-21 21:09:46.000000 dcnum-0.0.8/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-21 21:09:46.000000 dcnum-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 21:09:59.576246 dcnum-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 21:09:46.000000 dcnum-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 21:09:46.000000 dcnum-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:09:59.576246 dcnum-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.576246 dcnum-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.576246 dcnum-0.0.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_write_writer.py
```

### Comparing `dcnum-0.0.7/.github/workflows/check.yml` & `dcnum-0.0.8/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/.github/workflows/deploy_pypi.yml` & `dcnum-0.0.8/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/.gitignore` & `dcnum-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/LICENSE` & `dcnum-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/PKG-INFO` & `dcnum-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.7
+Version: 0.0.8
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.7/README.rst` & `dcnum-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/feat/background/base.py` & `dcnum-0.0.8/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/feat/background/bg_roll_median.py` & `dcnum-0.0.8/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/feat/background/bg_sparse_median.py` & `dcnum-0.0.8/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/feat/moments/mt_legacy.py` & `dcnum-0.0.8/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/meta/ppid.py` & `dcnum-0.0.8/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/read/cache.py` & `dcnum-0.0.8/dcnum/read/cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,22 +21,26 @@
         loaded, decompressed and from that one image extracted. The
         `HDF5ImageCache` class caches the chunks from the HDF5 files
         into memory, making single-image-access very fast.
         """
         # TODO:
         # - adjust chunking to multiples of the chunks in the dataset
         #   (which will slightly speed up things)
+        chunk_size = min(h5ds.shape[0], chunk_size)
         self.h5ds = h5ds
         self.chunk_size = chunk_size
         self.boolean = boolean
         self.cache_size = cache_size
         #: This is a FILO cache for the chunks
         self.cache = collections.OrderedDict()
         self.shape = h5ds.shape
-        self._len = len(self.h5ds)
+        self.image_shape = self.shape[1:]
+        self.chunk_shape = (chunk_size,) + self.shape[1:]
+        self._len = self.shape[0]
+        self.num_chunks = int(np.ceil(self._len / self.chunk_size))
 
     def _get_chunk_index_for_index(self, index):
         if index < 0:
             index = len(self.h5ds) + index
         chunk_index = index // self.chunk_size
         sub_index = index % self.chunk_size
         return chunk_index, sub_index
@@ -78,16 +82,18 @@
 class ImageCorrCache:
     def __init__(self,
                  image: HDF5ImageCache,
                  image_bg: HDF5ImageCache):
         self.image = image
         self.image_bg = image_bg
         self.chunk_size = image.chunk_size
+        self.num_chunks = image.num_chunks
         self.h5ds = image.h5ds
         self.shape = image.shape
+        self.chunk_shape = image.chunk_shape
         #: This is a FILO cache for the corrected image chunks
         self.cache = collections.OrderedDict()
         self.cache_size = image.cache_size
 
     def _get_chunk_index_for_index(self, index):
         if index < 0:
             index = len(self.h5ds) + index
@@ -100,15 +106,16 @@
         return self.get_chunk(chunk_index)[sub_index]
 
     def __len__(self):
         return len(self.image)
 
     def get_chunk(self, chunk_index):
         if chunk_index not in self.cache:
-            data = np.array(self.image.get_chunk(chunk_index), dtype=int) \
+            data = np.array(
+                self.image.get_chunk(chunk_index), dtype=np.int16) \
                 - self.image_bg.get_chunk(chunk_index)
             self.cache[chunk_index] = data
             if len(self.cache) > self.cache_size:
                 # Remove the first item
                 self.cache.popitem(last=False)
         return self.cache[chunk_index]
```

### Comparing `dcnum-0.0.7/dcnum/read/hdf5_data.py` & `dcnum-0.0.8/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/segm/segm_thresh.py` & `dcnum-0.0.8/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/segm/segmenter.py` & `dcnum-0.0.8/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/dcnum/segm/segmenter_cpu.py` & `dcnum-0.0.8/dcnum/segm/segmenter_cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import multiprocessing as mp
+import os
 import time
 import threading
 
 import numpy as np
 
 from .segmenter import Segmenter
 
@@ -116,15 +117,15 @@
           images, then `image_data` must already be background-corrected.
         """
         if stop is None or start is None:
             start = 0
             stop = len(image_data)
 
         batch_size = stop - start
-        size = np.prod(image_data[0]) * batch_size
+        size = np.prod(image_data.shape[1:]) * batch_size
 
         if self.image_shape is None:
             self.image_shape = image_data[0].shape
 
         if self._mp_image_np is not None and self._mp_image_np.size != size:
             # reset image data
             self._mp_image_np = None
@@ -228,14 +229,15 @@
         self.labels_data_raw = segmenter.mp_labels_raw
         # The shape of one image
         self.image_shape = segmenter.image_shape
         self.sl_start = sl_start
         self.sl_stop = sl_stop
 
     def run(self):
+        print(f"Running {self} in PID {os.getpid()}")
         # We have to create the numpy-versions of the mp.RawArrays here,
         # otherwise we only get some kind of copy in the new process
         # when we use "spawn" instead of "fork".
         labels_data = np.ctypeslib.as_array(self.labels_data_raw).reshape(
             -1, self.image_shape[0], self.image_shape[1])
         image_data = np.ctypeslib.as_array(self.image_data_raw).reshape(
             -1, self.image_shape[0], self.image_shape[1])
@@ -264,9 +266,9 @@
 
 class CPUSegmenterWorkerProcess(CPUSegmenterWorker, mp.Process):
     def __init__(self, *args, **kwargs):
         super(CPUSegmenterWorkerProcess, self).__init__(*args, **kwargs)
 
 
 class CPUSegmenterWorkerThread(CPUSegmenterWorker, threading.Thread):
-    def __init__(self, *args):
-        super(CPUSegmenterWorkerThread, self).__init__(*args)
+    def __init__(self, *args, **kwargs):
+        super(CPUSegmenterWorkerThread, self).__init__(*args, **kwargs)
```

### Comparing `dcnum-0.0.7/dcnum/write/writer.py` & `dcnum-0.0.8/dcnum/write/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,13 +71,15 @@
 
     def store_feature_chunk(self, feat, data):
         """Store feature data
 
         The "chunk" implies that always chunks of data are stored,
         never single events.
         """
+        if feat == "mask" and data.dtype == bool:
+            data = 255 * np.array(data, dtype=np.uint8)
         ds, offset = self.require_feature(feat=feat,
                                           item_shape=data.shape[1:],
                                           dtype=data.dtype)
         dsize = data.shape[0]
         ds.resize(offset + dsize, axis=0)
         ds[offset:offset + dsize] = data
```

### Comparing `dcnum-0.0.7/dcnum/write/writer_thread.py` & `dcnum-0.0.8/dcnum/write/deque_writer_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 import threading
 import time
 
 from .writer import HDF5Writer
 
 
-class HDF5WriterThread(threading.Thread):
+class DequeWriterThread(threading.Thread):
     def __init__(self,
                  path_out: pathlib.Path,
                  dq: collections.deque,
                  ds_kwds: dict = None,
                  mode: str = "a",
                  *args, **kwargs):
         """Convenience class for writing to data outside the main loop
@@ -19,15 +19,15 @@
         ----------
         path_out:
             Path to the output HDF5 file
         dq:
             `collections.deque` object from which data are taken
             using `popleft()`.
         """
-        super(HDF5WriterThread, self).__init__(*args, **kwargs)
+        super(DequeWriterThread, self).__init__(*args, **kwargs)
         self.writer = HDF5Writer(path_out, mode=mode, ds_kwds=ds_kwds)
         self.dq = dq
         self.may_stop_loop = False
         self.must_stop_loop = False
 
     def abort_loop(self):
         """Force aborting the loop as soon as possible"""
@@ -39,15 +39,14 @@
 
     def run(self):
         while True:
             if self.must_stop_loop:
                 break
             elif len(self.dq):
                 feat, data = self.dq.popleft()
-                self.writer.store_feature_chunk(feat=feat,
-                                                data=data)
+                self.writer.store_feature_chunk(feat=feat, data=data)
             elif self.may_stop_loop:
                 break
             else:
                 # wait for the next item to arrive
                 time.sleep(.5)
         self.writer.close()
```

### Comparing `dcnum-0.0.7/dcnum.egg-info/PKG-INFO` & `dcnum-0.0.8/dcnum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.7
+Version: 0.0.8
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.7/dcnum.egg-info/SOURCES.txt` & `dcnum-0.0.8/dcnum.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,39 +10,45 @@
 dcnum/_version.py
 dcnum.egg-info/PKG-INFO
 dcnum.egg-info/SOURCES.txt
 dcnum.egg-info/dependency_links.txt
 dcnum.egg-info/requires.txt
 dcnum.egg-info/top_level.txt
 dcnum/feat/__init__.py
-dcnum/feat/background/__init__.py
-dcnum/feat/background/base.py
-dcnum/feat/background/bg_roll_median.py
-dcnum/feat/background/bg_sparse_median.py
-dcnum/feat/brightness/__init__.py
-dcnum/feat/brightness/bright_all.py
-dcnum/feat/haralick/__init__.py
-dcnum/feat/haralick/common.py
-dcnum/feat/haralick/tex_all.py
-dcnum/feat/moments/__init__.py
-dcnum/feat/moments/ct_opencv.py
-dcnum/feat/moments/mt_legacy.py
+dcnum/feat/event_extractor_manager_thread.py
+dcnum/feat/gate.py
+dcnum/feat/queue_event_extractor.py
+dcnum/feat/feat_background/__init__.py
+dcnum/feat/feat_background/base.py
+dcnum/feat/feat_background/bg_roll_median.py
+dcnum/feat/feat_background/bg_sparse_median.py
+dcnum/feat/feat_brightness/__init__.py
+dcnum/feat/feat_brightness/bright_all.py
+dcnum/feat/feat_brightness/common.py
+dcnum/feat/feat_moments/__init__.py
+dcnum/feat/feat_moments/ct_opencv.py
+dcnum/feat/feat_moments/mt_legacy.py
+dcnum/feat/feat_texture/__init__.py
+dcnum/feat/feat_texture/common.py
+dcnum/feat/feat_texture/tex_all.py
 dcnum/meta/__init__.py
 dcnum/meta/ppid.py
 dcnum/read/__init__.py
 dcnum/read/cache.py
 dcnum/read/const.py
 dcnum/read/hdf5_data.py
 dcnum/segm/__init__.py
 dcnum/segm/segm_thresh.py
 dcnum/segm/segmenter.py
 dcnum/segm/segmenter_cpu.py
+dcnum/segm/segmenter_manager_thread.py
 dcnum/write/__init__.py
+dcnum/write/deque_writer_thread.py
+dcnum/write/queue_collector_thread.py
 dcnum/write/writer.py
-dcnum/write/writer_thread.py
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/extensions/github_changelog.py
 tests/conftest.py
 tests/helper_methods.py
 tests/requirements.txt
@@ -52,11 +58,11 @@
 tests/test_feat_moments_based.py
 tests/test_init.py
 tests/test_ppid.py
 tests/test_ppid_segm.py
 tests/test_read_concat_hdf5.py
 tests/test_read_hdf5.py
 tests/test_segm_thresh.py
+tests/test_write_deque_writer_thread.py
 tests/test_write_writer.py
-tests/test_write_writer_thread.py
 tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
 tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
```

### Comparing `dcnum-0.0.7/docs/conf.py` & `dcnum-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/docs/extensions/github_changelog.py` & `dcnum-0.0.8/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/pyproject.toml` & `dcnum-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/helper_methods.py` & `dcnum-0.0.8/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.0.8/tests/test_feat_background_bg_roll_median.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import h5py
 import numpy as np
 import pytest
 
-from dcnum.feat.background import bg_roll_median
+from dcnum.feat.feat_background import bg_roll_median
 
 
 def test_compute_median_for_slice():
     # events in shared arrays: 100
     # image shape: 5 * 7
     shared_input = np.arange(5*7).reshape(1, 5*7) * np.ones((100, 1))
     assert shared_input.size == 100 * 5 * 7
```

### Comparing `dcnum-0.0.7/tests/test_feat_brightness.py` & `dcnum-0.0.8/tests/test_feat_brightness.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pathlib
 
 import h5py
 import numpy as np
 
-from dcnum.feat import brightness
+from dcnum.feat import feat_brightness
 
 from helper_methods import retrieve_data
 
 data_path = pathlib.Path(__file__).parent / "data"
 
 
 def test_basic_brightness():
     # This original file was generated with dcevent for reference.
     path = retrieve_data(data_path /
                          "fmt-hdf5_cytoshot_full-features_2023.zip")
     # Make data available
     with h5py.File(path) as h5:
-        data = brightness.brightness_features(
+        data = feat_brightness.brightness_features(
             image=h5["events/image"][:],
             image_bg=h5["events/image_bg"][:],
             mask=h5["events/mask"][:],
         )
 
         assert np.allclose(data["bright_bc_avg"][1],
                            -43.75497215592681,
                            atol=0, rtol=1e-10)
-        for feat in brightness.brightness_names:
+        for feat in feat_brightness.brightness_names:
             assert np.allclose(h5["events"][feat][:],
                                data[feat]), f"Feature {feat} mismatch!"
         # control test
         assert not np.allclose(h5["events"]["bright_perc_10"][:],
                                data["bright_perc_90"])
```

### Comparing `dcnum-0.0.7/tests/test_feat_haralick.py` & `dcnum-0.0.8/tests/test_feat_haralick.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pathlib
 
 import h5py
 import numpy as np
 
-from dcnum.feat import haralick
+from dcnum.feat import feat_texture
 
 from helper_methods import retrieve_data
 
 data_path = pathlib.Path(__file__).parent / "data"
 
 
 def test_basic_haralick():
     # This original file was generated with dcevent for reference.
     path = retrieve_data(data_path /
                          "fmt-hdf5_cytoshot_full-features_2023.zip")
     # Make data available
     with h5py.File(path) as h5:
-        ret_arr = haralick.haralick_texture_features(
+        ret_arr = feat_texture.haralick_texture_features(
             image=h5["events/image"][:],
             image_bg=h5["events/image_bg"][:],
             mask=h5["events/mask"][:],
         )
 
         assert np.allclose(ret_arr["tex_asm_avg"][1],
                            0.001514295993357114,
                            atol=0, rtol=1e-10)
-        for feat in haralick.haralick_names:
+        for feat in feat_texture.haralick_names:
             assert np.allclose(h5["events"][feat],
                                ret_arr[feat])
         # control test
         assert not np.allclose(h5["events"]["tex_asm_avg"],
                                ret_arr["tex_asm_ptp"])
```

### Comparing `dcnum-0.0.7/tests/test_feat_moments_based.py` & `dcnum-0.0.8/tests/test_feat_moments_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 
 import h5py
 import numpy as np
 
-from dcnum.feat import moments
+from dcnum.feat import feat_moments
 
 from helper_methods import retrieve_data
 
 data_path = pathlib.Path(__file__).parent / "data"
 
 
 def test_moments_based_features():
@@ -28,15 +28,15 @@
         "inert_ratio_cvx",
         "inert_ratio_raw",
         "inert_ratio_prnc",
     ]
 
     # Make data available
     with h5py.File(path) as h5:
-        data = moments.moments_based_features(
+        data = feat_moments.moments_based_features(
             mask=h5["events/mask"][:],
             pixel_size=0.2645
         )
         for feat in feats:
             if feat.count("inert"):
                 rtol = 2e-5
                 atol = 1e-8
```

### Comparing `dcnum-0.0.7/tests/test_ppid.py` & `dcnum-0.0.8/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/test_read_concat_hdf5.py` & `dcnum-0.0.8/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/test_read_hdf5.py` & `dcnum-0.0.8/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/test_segm_thresh.py` & `dcnum-0.0.8/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/test_write_writer.py` & `dcnum-0.0.8/tests/test_write_writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.7/tests/test_write_writer_thread.py` & `dcnum-0.0.8/tests/test_write_deque_writer_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def test_writer_thread_basic():
     path = retrieve_data(data_path /
                          "fmt-hdf5_cytoshot_full-features_2023.zip")
     path_wrt = path.with_name("written.hdf5")
     dq = collections.deque()
 
-    wrthr = write.HDF5WriterThread(path_out=path_wrt, dq=dq)
+    wrthr = write.DequeWriterThread(path_out=path_wrt, dq=dq)
     wrthr.start()
 
     with h5py.File(path) as h5:
         deform = h5["events"]["deform"][:]
         image = h5["events"]["image"][:]
 
         dq.append(("deform", deform))
```

