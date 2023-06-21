# Comparing `tmp/fastxtend-0.1.3.tar.gz` & `tmp/fastxtend-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastxtend-0.1.3.tar", last modified: Wed Jun  7 16:45:08 2023, max compression
+gzip compressed data, was "fastxtend-0.1.4.tar", last modified: Wed Jun 21 06:18:41 2023, max compression
```

## Comparing `fastxtend-0.1.3.tar` & `fastxtend-0.1.4.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.373530 fastxtend-0.1.3/
--rw-r--r--   0 benja     (1000) benja     (1000)     1072 2023-02-21 17:38:09.000000 fastxtend-0.1.3/LICENSE
--rw-rw-r--   0 benja     (1000) benja     (1000)     7778 2023-06-07 16:45:08.373530 fastxtend-0.1.3/PKG-INFO
--rw-rw-r--   0 benja     (1000) benja     (1000)     6853 2023-06-07 15:14:37.000000 fastxtend-0.1.3/README.md
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.361530 fastxtend-0.1.3/fastxtend/
--rw-rw-r--   0 benja     (1000) benja     (1000)       22 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/__init__.py
--rw-rw-r--   0 benja     (1000) benja     (1000)   209914 2023-06-07 16:16:41.000000 fastxtend-0.1.3/fastxtend/_modidx.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend/audio/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/audio/__init__.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      493 2023-03-11 21:10:32.000000 fastxtend-0.1.3/fastxtend/audio/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)    30135 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/augment.py
--rw-r--r--   0 benja     (1000) benja     (1000)     6870 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/core.py
--rw-r--r--   0 benja     (1000) benja     (1000)    11546 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/data.py
--rw-r--r--   0 benja     (1000) benja     (1000)     3500 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/learner.py
--rw-r--r--   0 benja     (1000) benja     (1000)    11276 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/mixup.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2728 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/basics.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend/callback/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/callback/__init__.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      248 2023-03-11 21:10:32.000000 fastxtend-0.1.3/fastxtend/callback/all.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     1707 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/channelslast.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    14473 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/compiler.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    17890 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/cutmixup.py
--rw-r--r--   0 benja     (1000) benja     (1000)    10936 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/ema.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     4583 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/lr_finder.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    21973 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/profiler.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    17703 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/progresize.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      160 2023-03-20 20:46:25.000000 fastxtend-0.1.3/fastxtend/callback/simpleprofiler.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2815 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/tracker.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend/data/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/data/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)       25 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/data/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2332 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/data/transforms.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/ffcv/
--rw-rw-r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/ffcv/__init__.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      326 2023-03-27 07:41:32.000000 fastxtend-0.1.3/fastxtend/ffcv/all.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     3945 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/epoch_iterator.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     6469 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/fields.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      148 2023-03-27 07:41:32.000000 fastxtend-0.1.3/fastxtend/ffcv/fx.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     4885 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/inference.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    12850 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/loader.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     4556 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/operations.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    35082 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/transforms.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     2838 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/utils.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     4310 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/writer.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      837 2023-03-27 07:41:33.000000 fastxtend-0.1.3/fastxtend/imports.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     6746 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/losses.py
--rw-r--r--   0 benja     (1000) benja     (1000)    41980 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/metrics.py
--rw-r--r--   0 benja     (1000) benja     (1000)    12155 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/multiloss.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/optimizer/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/optimizer/__init__.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    11746 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/adan.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      163 2023-06-06 06:08:24.000000 fastxtend-0.1.3/fastxtend/optimizer/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)    20144 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/eightbit.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    15451 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/foreach.py
--rw-r--r--   0 benja     (1000) benja     (1000)    22375 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/fused.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     5012 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/lion.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     9351 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/sophia.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     7601 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/stableadam.py
--rw-rw-r--   0 benja     (1000) benja     (1000)    15022 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/torchscript.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     2987 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/patches.py
--rw-r--r--   0 benja     (1000) benja     (1000)     7538 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/schedulers.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     1993 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/test_utils.py
--rw-rw-r--   0 benja     (1000) benja     (1000)      857 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/torch_core.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     2643 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/transform.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     4545 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/utils.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/vision/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)      324 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/vision/all.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/vision/augment/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/augment/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)       46 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/vision/augment/all.py
--rw-rw-r--   0 benja     (1000) benja     (1000)     7734 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/vision/augment/batch.py
--rw-r--r--   0 benja     (1000) benja     (1000)     6251 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/vision/augment/itemtensor.py
--rw-r--r--   0 benja     (1000) benja     (1000)     1865 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/data.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.373530 fastxtend-0.1.3/fastxtend/vision/models/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)       78 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/vision/models/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)     4796 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/attention_modules.py
--rw-r--r--   0 benja     (1000) benja     (1000)     1560 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/pooling.py
--rw-r--r--   0 benja     (1000) benja     (1000)    15564 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/xresnet.py
-drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend.egg-info/
--rw-r--r--   0 benja     (1000) benja     (1000)     7778 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/PKG-INFO
--rw-r--r--   0 benja     (1000) benja     (1000)     2136 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/SOURCES.txt
--rw-r--r--   0 benja     (1000) benja     (1000)        1 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/dependency_links.txt
--rw-r--r--   0 benja     (1000) benja     (1000)       40 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/entry_points.txt
--rw-r--r--   0 benja     (1000) benja     (1000)        1 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend.egg-info/not-zip-safe
--rw-r--r--   0 benja     (1000) benja     (1000)      611 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/requires.txt
--rw-r--r--   0 benja     (1000) benja     (1000)       10 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/top_level.txt
--rw-rw-r--   0 benja     (1000) benja     (1000)       38 2023-06-07 16:45:08.373530 fastxtend-0.1.3/setup.cfg
--rw-rw-r--   0 benja     (1000) benja     (1000)     3243 2023-03-27 07:41:33.000000 fastxtend-0.1.3/setup.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.438599 fastxtend-0.1.4/
+-rw-r--r--   0 benja     (1000) benja     (1000)     1072 2023-02-21 17:38:09.000000 fastxtend-0.1.4/LICENSE
+-rw-r--r--   0 benja     (1000) benja     (1000)     7778 2023-06-21 06:18:41.438599 fastxtend-0.1.4/PKG-INFO
+-rw-rw-r--   0 benja     (1000) benja     (1000)     6853 2023-06-07 15:14:37.000000 fastxtend-0.1.4/README.md
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.378599 fastxtend-0.1.4/fastxtend/
+-rw-rw-r--   0 benja     (1000) benja     (1000)       22 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)   223552 2023-06-21 06:18:32.000000 fastxtend-0.1.4/fastxtend/_modidx.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.398599 fastxtend-0.1.4/fastxtend/audio/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/audio/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      493 2023-03-11 21:10:32.000000 fastxtend-0.1.4/fastxtend/audio/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    30135 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/audio/augment.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     6870 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/audio/core.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    11546 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/audio/data.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     3500 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/audio/learner.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    11276 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/audio/mixup.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     2728 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/basics.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.418599 fastxtend-0.1.4/fastxtend/callback/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/callback/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      188 2023-06-17 19:39:19.000000 fastxtend-0.1.4/fastxtend/callback/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     3934 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/amp.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     1923 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/channelslast.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    14458 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/compiler.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    17890 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/cutmixup.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     9980 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/ema.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     5528 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/gradaccum.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4583 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/lr_finder.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    21192 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/profiler.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    17050 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/progresize.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      160 2023-03-20 20:46:25.000000 fastxtend-0.1.4/fastxtend/callback/simpleprofiler.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     2815 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/tracker.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     6670 2023-06-21 06:02:49.000000 fastxtend-0.1.4/fastxtend/callback/utils.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.418599 fastxtend-0.1.4/fastxtend/data/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/data/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)       25 2023-02-21 17:38:10.000000 fastxtend-0.1.4/fastxtend/data/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     2332 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/data/transforms.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.438599 fastxtend-0.1.4/fastxtend/ffcv/
+-rw-rw-r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      326 2023-03-27 07:41:32.000000 fastxtend-0.1.4/fastxtend/ffcv/all.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     3945 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/epoch_iterator.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     6469 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/fields.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      148 2023-03-27 07:41:32.000000 fastxtend-0.1.4/fastxtend/ffcv/fx.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4885 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/inference.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    12955 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/loader.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4556 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/operations.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    35082 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/transforms.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     2838 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/utils.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4310 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/ffcv/writer.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      837 2023-03-27 07:41:33.000000 fastxtend-0.1.4/fastxtend/imports.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     6746 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/losses.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    41980 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/metrics.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    12155 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/multiloss.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.438599 fastxtend-0.1.4/fastxtend/optimizer/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    11746 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/adan.py
+-rw-r--r--   0 benja     (1000) benja     (1000)      163 2023-06-21 06:18:28.000000 fastxtend-0.1.4/fastxtend/optimizer/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    20144 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/eightbit.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    15451 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/foreach.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    22375 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/fused.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     5012 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/lion.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     9351 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/sophia.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     7670 2023-06-21 06:18:25.000000 fastxtend-0.1.4/fastxtend/optimizer/stableadam.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    15022 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/optimizer/torchscript.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     2987 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/patches.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     7538 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/schedulers.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     1993 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/test_utils.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      857 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/torch_core.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     2643 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/transform.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     4702 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/utils.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.438599 fastxtend-0.1.4/fastxtend/vision/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)      324 2023-02-21 17:38:10.000000 fastxtend-0.1.4/fastxtend/vision/all.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.438599 fastxtend-0.1.4/fastxtend/vision/augment/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/augment/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)       46 2023-02-21 17:38:10.000000 fastxtend-0.1.4/fastxtend/vision/augment/all.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     7734 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/augment/batch.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     6251 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/augment/itemtensor.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     1865 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/data.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.438599 fastxtend-0.1.4/fastxtend/vision/models/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/models/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)       78 2023-02-21 17:38:10.000000 fastxtend-0.1.4/fastxtend/vision/models/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     4796 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/models/attention_modules.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     1560 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/models/pooling.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    15564 2023-06-21 06:02:50.000000 fastxtend-0.1.4/fastxtend/vision/models/xresnet.py
+drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-06-21 06:18:41.388599 fastxtend-0.1.4/fastxtend.egg-info/
+-rw-r--r--   0 benja     (1000) benja     (1000)     7778 2023-06-21 06:18:41.000000 fastxtend-0.1.4/fastxtend.egg-info/PKG-INFO
+-rw-r--r--   0 benja     (1000) benja     (1000)     2222 2023-06-21 06:18:41.000000 fastxtend-0.1.4/fastxtend.egg-info/SOURCES.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)        1 2023-06-21 06:18:41.000000 fastxtend-0.1.4/fastxtend.egg-info/dependency_links.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)       40 2023-06-21 06:18:41.000000 fastxtend-0.1.4/fastxtend.egg-info/entry_points.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)        1 2023-02-21 17:38:10.000000 fastxtend-0.1.4/fastxtend.egg-info/not-zip-safe
+-rw-r--r--   0 benja     (1000) benja     (1000)      611 2023-06-21 06:18:41.000000 fastxtend-0.1.4/fastxtend.egg-info/requires.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)       10 2023-06-21 06:18:41.000000 fastxtend-0.1.4/fastxtend.egg-info/top_level.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)       38 2023-06-21 06:18:41.438599 fastxtend-0.1.4/setup.cfg
+-rw-rw-r--   0 benja     (1000) benja     (1000)     3243 2023-03-27 07:41:33.000000 fastxtend-0.1.4/setup.py
```

### Comparing `fastxtend-0.1.3/LICENSE` & `fastxtend-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/PKG-INFO` & `fastxtend-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastxtend
-Version: 0.1.3
+Version: 0.1.4
 Summary: Train fastai models faster (and other useful tools)
 Home-page: https://github.com/warner-benjamin/fastxtend
 Author: Benjamin Warner
 Author-email: me@benjaminwarner.dev
 License: MIT License
 Project-URL: Documentation, https://fastxtend.benjaminwarner.dev/
 Keywords: fastai pytorch extensions
```

### Comparing `fastxtend-0.1.3/README.md` & `fastxtend-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/_modidx.py` & `fastxtend-0.1.4/fastxtend/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,47 @@
                                                                                       'fastxtend/audio/mixup.py'),
                                        'fastxtend.audio.mixup.AudioMixUp.before_batch': ( 'audio.05_mixup.html#audiomixup.before_batch',
                                                                                           'fastxtend/audio/mixup.py')},
             'fastxtend.basics': { 'fastxtend.basics.is_listish': ('basics.html#is_listish', 'fastxtend/basics.py'),
                                   'fastxtend.basics.listify_store_attr': ('basics.html#listify_store_attr', 'fastxtend/basics.py'),
                                   'fastxtend.basics.show_batch': ('basics.html#show_batch', 'fastxtend/basics.py')},
             'fastxtend.callback.all': {},
+            'fastxtend.callback.amp': { 'fastxtend.callback.amp.AMPMode': ('callback.amp.html#ampmode', 'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.Learner.to_bf16': ( 'callback.amp.html#learner.to_bf16',
+                                                                                    'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.Learner.to_fp16': ( 'callback.amp.html#learner.to_fp16',
+                                                                                    'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.Learner.to_fp32': ( 'callback.amp.html#learner.to_fp32',
+                                                                                    'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision': ( 'callback.amp.html#mixedprecision',
+                                                                                   'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.__init__': ( 'callback.amp.html#mixedprecision.__init__',
+                                                                                            'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.after_cancel_fit': ( 'callback.amp.html#mixedprecision.after_cancel_fit',
+                                                                                                    'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.after_fit': ( 'callback.amp.html#mixedprecision.after_fit',
+                                                                                             'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.after_loss': ( 'callback.amp.html#mixedprecision.after_loss',
+                                                                                              'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.after_pred': ( 'callback.amp.html#mixedprecision.after_pred',
+                                                                                              'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.after_step': ( 'callback.amp.html#mixedprecision.after_step',
+                                                                                              'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.before_backward': ( 'callback.amp.html#mixedprecision.before_backward',
+                                                                                                   'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.before_batch': ( 'callback.amp.html#mixedprecision.before_batch',
+                                                                                                'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.before_fit': ( 'callback.amp.html#mixedprecision.before_fit',
+                                                                                              'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.before_step': ( 'callback.amp.html#mixedprecision.before_step',
+                                                                                               'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.param_groups': ( 'callback.amp.html#mixedprecision.param_groups',
+                                                                                                'fastxtend/callback/amp.py'),
+                                        'fastxtend.callback.amp.MixedPrecision.step': ( 'callback.amp.html#mixedprecision.step',
+                                                                                        'fastxtend/callback/amp.py')},
             'fastxtend.callback.channelslast': { 'fastxtend.callback.channelslast.ChannelsLast': ( 'callback.channelslast.html#channelslast',
                                                                                                    'fastxtend/callback/channelslast.py'),
                                                  'fastxtend.callback.channelslast.ChannelsLast.before_fit': ( 'callback.channelslast.html#channelslast.before_fit',
                                                                                                               'fastxtend/callback/channelslast.py'),
                                                  'fastxtend.callback.channelslast.Learner.to_channelslast': ( 'callback.channelslast.html#learner.to_channelslast',
                                                                                                               'fastxtend/callback/channelslast.py'),
                                                  'fastxtend.callback.channelslast.Learner.to_contiguous': ( 'callback.channelslast.html#learner.to_contiguous',
@@ -380,22 +413,50 @@
                                                                                                'fastxtend/callback/ema.py'),
                                         'fastxtend.callback.ema.EMACallback.before_batch': ( 'callback.ema.html#emacallback.before_batch',
                                                                                              'fastxtend/callback/ema.py'),
                                         'fastxtend.callback.ema.EMACallback.before_fit': ( 'callback.ema.html#emacallback.before_fit',
                                                                                            'fastxtend/callback/ema.py'),
                                         'fastxtend.callback.ema.EMACallback.before_validate': ( 'callback.ema.html#emacallback.before_validate',
                                                                                                 'fastxtend/callback/ema.py'),
+                                        'fastxtend.callback.ema.EMASchedule': ( 'callback.ema.html#emaschedule',
+                                                                                'fastxtend/callback/ema.py'),
+                                        'fastxtend.callback.ema.EMASchedule.__init__': ( 'callback.ema.html#emaschedule.__init__',
+                                                                                         'fastxtend/callback/ema.py'),
+                                        'fastxtend.callback.ema.EMASchedule.after_batch': ( 'callback.ema.html#emaschedule.after_batch',
+                                                                                            'fastxtend/callback/ema.py'),
+                                        'fastxtend.callback.ema.EMASchedule.before_fit': ( 'callback.ema.html#emaschedule.before_fit',
+                                                                                           'fastxtend/callback/ema.py'),
                                         'fastxtend.callback.ema.EMAWarmupCallback': ( 'callback.ema.html#emawarmupcallback',
                                                                                       'fastxtend/callback/ema.py'),
                                         'fastxtend.callback.ema.EMAWarmupCallback.__init__': ( 'callback.ema.html#emawarmupcallback.__init__',
-                                                                                               'fastxtend/callback/ema.py'),
-                                        'fastxtend.callback.ema.EMAWarmupCallback.after_batch': ( 'callback.ema.html#emawarmupcallback.after_batch',
-                                                                                                  'fastxtend/callback/ema.py'),
-                                        'fastxtend.callback.ema.EMAWarmupCallback.before_fit': ( 'callback.ema.html#emawarmupcallback.before_fit',
-                                                                                                 'fastxtend/callback/ema.py')},
+                                                                                               'fastxtend/callback/ema.py')},
+            'fastxtend.callback.gradaccum': { 'fastxtend.callback.gradaccum.GradientAccumulation': ( 'callback.gradaccum.html#gradientaccumulation',
+                                                                                                     'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulation.__init__': ( 'callback.gradaccum.html#gradientaccumulation.__init__',
+                                                                                                              'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulation._run_loggers': ( 'callback.gradaccum.html#gradientaccumulation._run_loggers',
+                                                                                                                  'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulation.after_epoch': ( 'callback.gradaccum.html#gradientaccumulation.after_epoch',
+                                                                                                                 'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulation.after_loss': ( 'callback.gradaccum.html#gradientaccumulation.after_loss',
+                                                                                                                'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulation.before_fit': ( 'callback.gradaccum.html#gradientaccumulation.before_fit',
+                                                                                                                'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulation.before_step': ( 'callback.gradaccum.html#gradientaccumulation.before_step',
+                                                                                                                 'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulationSchedule': ( 'callback.gradaccum.html#gradientaccumulationschedule',
+                                                                                                             'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulationSchedule.__init__': ( 'callback.gradaccum.html#gradientaccumulationschedule.__init__',
+                                                                                                                      'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulationSchedule._run_loggers': ( 'callback.gradaccum.html#gradientaccumulationschedule._run_loggers',
+                                                                                                                          'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulationSchedule.before_batch': ( 'callback.gradaccum.html#gradientaccumulationschedule.before_batch',
+                                                                                                                          'fastxtend/callback/gradaccum.py'),
+                                              'fastxtend.callback.gradaccum.GradientAccumulationSchedule.before_fit': ( 'callback.gradaccum.html#gradientaccumulationschedule.before_fit',
+                                                                                                                        'fastxtend/callback/gradaccum.py')},
             'fastxtend.callback.lr_finder': { 'fastxtend.callback.lr_finder.LRFinder': ( 'callback.lr_finder.html#lrfinder',
                                                                                          'fastxtend/callback/lr_finder.py'),
                                               'fastxtend.callback.lr_finder.LRFinder.__init__': ( 'callback.lr_finder.html#lrfinder.__init__',
                                                                                                   'fastxtend/callback/lr_finder.py'),
                                               'fastxtend.callback.lr_finder.LRFinder.after_batch': ( 'callback.lr_finder.html#lrfinder.after_batch',
                                                                                                      'fastxtend/callback/lr_finder.py'),
                                               'fastxtend.callback.lr_finder.LRFinder.after_fit': ( 'callback.lr_finder.html#lrfinder.after_fit',
@@ -456,14 +517,18 @@
                                                                                                                     'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputCallback._create_overview_row': ( 'callback.profiler.html#throughputcallback._create_overview_row',
                                                                                                                       'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputCallback._display_report': ( 'callback.profiler.html#throughputcallback._display_report',
                                                                                                                  'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputCallback._generate_report': ( 'callback.profiler.html#throughputcallback._generate_report',
                                                                                                                   'fastxtend/callback/profiler.py'),
+                                             'fastxtend.callback.profiler.ThroughputCallback._log_after_batch': ( 'callback.profiler.html#throughputcallback._log_after_batch',
+                                                                                                                  'fastxtend/callback/profiler.py'),
+                                             'fastxtend.callback.profiler.ThroughputCallback._log_after_fit': ( 'callback.profiler.html#throughputcallback._log_after_fit',
+                                                                                                                'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputCallback._samples_per_second': ( 'callback.profiler.html#throughputcallback._samples_per_second',
                                                                                                                      'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputCallback.before_batch': ( 'callback.profiler.html#throughputcallback.before_batch',
                                                                                                               'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputCallback.before_draw': ( 'callback.profiler.html#throughputcallback.before_draw',
                                                                                                              'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputCallback.before_epoch': ( 'callback.profiler.html#throughputcallback.before_epoch',
@@ -489,25 +554,25 @@
                                              'fastxtend.callback.profiler.ThroughputPostCallback.after_fit': ( 'callback.profiler.html#throughputpostcallback.after_fit',
                                                                                                                'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.after_train': ( 'callback.profiler.html#throughputpostcallback.after_train',
                                                                                                                  'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.after_validate': ( 'callback.profiler.html#throughputpostcallback.after_validate',
                                                                                                                     'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.before_fit': ( 'callback.profiler.html#throughputpostcallback.before_fit',
-                                                                                                                'fastxtend/callback/profiler.py'),
-                                             'fastxtend.callback.profiler.convert_to_int': ( 'callback.profiler.html#convert_to_int',
-                                                                                             'fastxtend/callback/profiler.py')},
+                                                                                                                'fastxtend/callback/profiler.py')},
             'fastxtend.callback.progresize': { 'fastxtend.callback.progresize.IncreaseMode': ( 'callback.progresize.html#increasemode',
                                                                                                'fastxtend/callback/progresize.py'),
                                                'fastxtend.callback.progresize.ProgressiveResize': ( 'callback.progresize.html#progressiveresize',
                                                                                                     'fastxtend/callback/progresize.py'),
                                                'fastxtend.callback.progresize.ProgressiveResize.__init__': ( 'callback.progresize.html#progressiveresize.__init__',
                                                                                                              'fastxtend/callback/progresize.py'),
                                                'fastxtend.callback.progresize.ProgressiveResize._increase_size': ( 'callback.progresize.html#progressiveresize._increase_size',
                                                                                                                    'fastxtend/callback/progresize.py'),
+                                               'fastxtend.callback.progresize.ProgressiveResize._log_size': ( 'callback.progresize.html#progressiveresize._log_size',
+                                                                                                              'fastxtend/callback/progresize.py'),
                                                'fastxtend.callback.progresize.ProgressiveResize._process_pipeline': ( 'callback.progresize.html#progressiveresize._process_pipeline',
                                                                                                                       'fastxtend/callback/progresize.py'),
                                                'fastxtend.callback.progresize.ProgressiveResize.after_epoch': ( 'callback.progresize.html#progressiveresize.after_epoch',
                                                                                                                 'fastxtend/callback/progresize.py'),
                                                'fastxtend.callback.progresize.ProgressiveResize.before_batch': ( 'callback.progresize.html#progressiveresize.before_batch',
                                                                                                                  'fastxtend/callback/progresize.py'),
                                                'fastxtend.callback.progresize.ProgressiveResize.before_fit': ( 'callback.progresize.html#progressiveresize.before_fit',
@@ -543,14 +608,44 @@
                                                                                                      'fastxtend/callback/tracker.py'),
                                             'fastxtend.callback.tracker.SaveModelAtEnd.before_fit': ( 'callback.tracker.html#savemodelatend.before_fit',
                                                                                                       'fastxtend/callback/tracker.py'),
                                             'fastxtend.callback.tracker.TerminateOnTrainNaN': ( 'callback.tracker.html#terminateontrainnan',
                                                                                                 'fastxtend/callback/tracker.py'),
                                             'fastxtend.callback.tracker.TerminateOnTrainNaN.after_batch': ( 'callback.tracker.html#terminateontrainnan.after_batch',
                                                                                                             'fastxtend/callback/tracker.py')},
+            'fastxtend.callback.utils': { 'fastxtend.callback.utils.CallbackScheduler': ( 'callback.utils.html#callbackscheduler',
+                                                                                          'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.CallbackScheduler.schedule_step': ( 'callback.utils.html#callbackscheduler.schedule_step',
+                                                                                                        'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.CallbackScheduler.setup_schedule': ( 'callback.utils.html#callbackscheduler.setup_schedule',
+                                                                                                         'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.Learner._log_dict': ( 'callback.utils.html#learner._log_dict',
+                                                                                          'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.Learner._log_values': ( 'callback.utils.html#learner._log_values',
+                                                                                            'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch': ( 'callback.utils.html#logdispatch',
+                                                                                    'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch._log_tensorboard': ( 'callback.utils.html#logdispatch._log_tensorboard',
+                                                                                                     'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch._log_wandb': ( 'callback.utils.html#logdispatch._log_wandb',
+                                                                                               'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch._update_dict': ( 'callback.utils.html#logdispatch._update_dict',
+                                                                                                 'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch._update_values': ( 'callback.utils.html#logdispatch._update_values',
+                                                                                                   'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch.after_batch': ( 'callback.utils.html#logdispatch.after_batch',
+                                                                                                'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch.after_epoch': ( 'callback.utils.html#logdispatch.after_epoch',
+                                                                                                'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch.before_fit': ( 'callback.utils.html#logdispatch.before_fit',
+                                                                                               'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch.log_wandb_summary': ( 'callback.utils.html#logdispatch.log_wandb_summary',
+                                                                                                      'fastxtend/callback/utils.py'),
+                                          'fastxtend.callback.utils.LogDispatch.log_wandb_table': ( 'callback.utils.html#logdispatch.log_wandb_table',
+                                                                                                    'fastxtend/callback/utils.py')},
             'fastxtend.data.all': {},
             'fastxtend.data.transforms': { 'fastxtend.data.transforms.GreatGrandparentSplitter': ( 'data.transforms.html#greatgrandparentsplitter',
                                                                                                    'fastxtend/data/transforms.py'),
                                            'fastxtend.data.transforms.KFoldColSplitter': ( 'data.transforms.html#kfoldcolsplitter',
                                                                                            'fastxtend/data/transforms.py'),
                                            'fastxtend.data.transforms.ParentSplitter': ( 'data.transforms.html#parentsplitter',
                                                                                          'fastxtend/data/transforms.py'),
@@ -634,14 +729,15 @@
                                                                                    'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader._pipeline_device': ( 'ffcv.loader.html#loader._pipeline_device',
                                                                                           'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader._pre_show_batch': ( 'ffcv.loader.html#loader._pre_show_batch',
                                                                                          'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader._retain_dl': ( 'ffcv.loader.html#loader._retain_dl',
                                                                                     'fastxtend/ffcv/loader.py'),
+                                       'fastxtend.ffcv.loader.Loader.bs': ('ffcv.loader.html#loader.bs', 'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.decode': ( 'ffcv.loader.html#loader.decode',
                                                                                 'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.decode_batch': ( 'ffcv.loader.html#loader.decode_batch',
                                                                                       'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.device': ( 'ffcv.loader.html#loader.device',
                                                                                 'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.n_inp': ('ffcv.loader.html#loader.n_inp', 'fastxtend/ffcv/loader.py'),
@@ -1341,14 +1437,15 @@
                                                                                           'fastxtend/transform.py'),
                                      'fastxtend.transform.BatchRandTransform._do_f': ( 'transform.html#batchrandtransform._do_f',
                                                                                        'fastxtend/transform.py'),
                                      'fastxtend.transform.BatchRandTransform.before_call': ( 'transform.html#batchrandtransform.before_call',
                                                                                              'fastxtend/transform.py')},
             'fastxtend.utils': { 'fastxtend.utils.clean_ipython_hist': ('utils.html#clean_ipython_hist', 'fastxtend/utils.py'),
                                  'fastxtend.utils.clean_traceback': ('utils.html#clean_traceback', 'fastxtend/utils.py'),
+                                 'fastxtend.utils.convert_to_int': ('utils.html#convert_to_int', 'fastxtend/utils.py'),
                                  'fastxtend.utils.free_gpu_memory': ('utils.html#free_gpu_memory', 'fastxtend/utils.py'),
                                  'fastxtend.utils.less_random': ('utils.html#less_random', 'fastxtend/utils.py'),
                                  'fastxtend.utils.pil_to_numpy': ('utils.html#pil_to_numpy', 'fastxtend/utils.py'),
                                  'fastxtend.utils.scale_time': ('utils.html#scale_time', 'fastxtend/utils.py')},
             'fastxtend.vision.all': {},
             'fastxtend.vision.augment.all': {},
             'fastxtend.vision.augment.batch': { 'fastxtend.vision.augment.batch.ChannelDrop': ( 'vision.augment.batch.html#channeldrop',
```

### Comparing `fastxtend-0.1.3/fastxtend/audio/augment.py` & `fastxtend-0.1.4/fastxtend/audio/augment.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/audio/core.py` & `fastxtend-0.1.4/fastxtend/audio/core.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/audio/data.py` & `fastxtend-0.1.4/fastxtend/audio/data.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/audio/learner.py` & `fastxtend-0.1.4/fastxtend/audio/learner.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/audio/mixup.py` & `fastxtend-0.1.4/fastxtend/audio/mixup.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/basics.py` & `fastxtend-0.1.4/fastxtend/basics.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/callback/compiler.py` & `fastxtend-0.1.4/fastxtend/callback/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 import torch._dynamo as dynamo
 from torch.serialization import FILE_LIKE
 
 from fastai.learner import Learner, save_model, join_path_file, _cast_tensor
 from fastai.callback import schedule
 from fastai.callback.core import Callback, TrainEvalCallback, CancelFitException
-from fastai.callback.fp16 import MixedPrecision
+
+from .amp import MixedPrecision
 
 try:
     from fastxtend.ffcv.loader import Loader
     FFCV = True
 except ImportError:
     FFCV = False
```

### Comparing `fastxtend-0.1.3/fastxtend/callback/cutmixup.py` & `fastxtend-0.1.4/fastxtend/callback/cutmixup.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/callback/ema.py` & `fastxtend-0.1.4/fastxtend/callback/ema.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 from copy import deepcopy
 
 from fastai.callback.core import Callback
 from fastai.callback.fp16 import MixedPrecision
 from fastai.callback.schedule import SchedCos, _Annealer
 
+from .utils import *
 from ..imports import *
 
 # %% auto 0
-__all__ = ['EMACallback', 'EMAWarmupCallback']
+__all__ = ['EMACallback', 'EMASchedule', 'EMAWarmupCallback']
 
 # %% ../../nbs/callback.ema.ipynb 6
 class EMACallback(Callback):
     "Exponential Moving Average (EMA) of model weights with a fused update step"
     order,run_valid = MixedPrecision.order+1,False
     def __init__(self,
         decay:float=0.9998, # EMA decay value
@@ -141,15 +142,15 @@
         if self.replace_weights:
             self.learn.model = self.ema_model
             self.ema_model = None
         else:
             self.learn.model_ema = self.ema_model
 
 # %% ../../nbs/callback.ema.ipynb 9
-class EMAWarmupCallback(EMACallback):
+class EMASchedule(EMACallback, CallbackScheduler):
     "Exponential Moving Average (EMA) of model weights with a warmup schedule and fused update step"
     order,run_valid = MixedPrecision.order+1,False
     def __init__(self,
         start_decay:float=0.9, # Initial EMA decay value
         final_decay:float=0.9998, # Final EMA decay value
         start:Numeric=0, # Start EMA warmup in percent of training steps (float) or epochs (int, index 0)
         finish:Numeric=0.3, # Finish EMA warmup in percent of training steps (float) or epochs (int, index 0)
@@ -158,65 +159,48 @@
         validate_ema:bool=True, # Run validation metrics using EMA weights instead of model weights. If true, `ema_device` must match model device
         replace_weights:bool=False, # Replace model weights with EMA weights when finished training. If false, set `Learner.model_ema` to EMA weights
         foreach:bool|None=None, # Fuse EMA update step with PyTorch ForEach methods or use a standard for loop. Defaults to true if PyTorch 1.12+ and Cuda device detected
         resume:bool=False, # Resume from EMA weights from previous training saved to `Learner.model_ema`
         all_parameters:bool=False, # Apply EMA step to all parameters or only those with `requires_grad`
         all_buffers:bool=False, # Apply EMA step to persistent model buffers or all buffers
         skip_ema:bool=True, # Skip EMA step if callbacks, such as GradientAccumulation or MixedPrecision, skip the Optimizer update step
-        logger_callback:str='wandb', # Log EMA decay to `logger_callback` using `Callback.name` if available
     ):
-        super().__init__(decay=final_decay, start=start, ema_device=ema_device,
-                         validate_ema=validate_ema, replace_weights=replace_weights,
-                         foreach=foreach, resume=resume, all_parameters=all_parameters,
-                         all_buffers=all_buffers, skip_ema=skip_ema)
-        store_attr(names='start_decay,final_decay,finish,logger_callback')
-        self.schedule = schedule(start_decay, final_decay)
+        EMACallback.__init__(self,
+            decay=final_decay,
+            start=start,
+            ema_device=ema_device,
+            validate_ema=validate_ema,
+            replace_weights=replace_weights,
+            foreach=foreach,
+            resume=resume,
+            all_parameters=all_parameters,
+            all_buffers=all_buffers,
+            skip_ema=skip_ema)
 
-    def before_fit(self):
-        if self.finish - self.start <= 0:
-            warn(f'EMA Warmup start={self.start} is less or equal to final={self.epoch} which negates warmup')
+        CallbackScheduler.__init__(self)
+        store_attr(names='start_decay,final_decay,finish,schedule')
 
+    def before_fit(self):
+        super().setup_schedule(self.n_epoch, len(self.dls.train), self.start_decay,
+                               self.final_decay, self.start, self.finish, self.schedule,
+                               callback_name='EMA Schedule')
         super().before_fit()
 
-        if self.finish >= 1 and isinstance(self.finish, int):
-            self.finish = self.finish/self.n_epoch
-        if self.finish >= 1:
-            warn(f'EMA Warmup finish {self.finish} is equal or greater than one and will not finish in this training run')
-
-        if self.resume and self.n_epoch < self.finish*self.n_epoch:
-            warn("Resuming EMA Warmup before the warmup is finished is not supported")
-
         # negate decay so at least one ema scheduling step will occur
         self.decay = -1*self.decay
-        self.warmup_pct = 0.
-        self._warmup_sched = 1/(len(self.dls.train) * self.n_epoch * (self.finish - self.start))
-
-        self._log_ema_decay = getattr(self, f'_{self.logger_callback}_log_ema_decay', noop)
-        self.has_logger = hasattr(self.learn, self.logger_callback) and self._log_ema_decay != noop
 
     def after_batch(self):
         if self._do_ema:
-            if self.pct_train >= self.start and self.decay != self.final_decay:
-                if self.pct_train >= self.finish:
-                    self.decay = self.final_decay
-                else:
-                    self.decay = self.schedule(self.warmup_pct)
-                    self.warmup_pct += self._warmup_sched
-                self.inverse_decay = 1-self.decay
+            self.decay = super().schedule_step(self.decay, self.pct_train)
+            self.inverse_decay = 1-self.decay
 
             super().after_batch()
 
-        if self.has_logger:
-            if self._do_ema:
-                self._log_ema_decay(self.decay)
-            else:
-                self._log_ema_decay(0.)
+        self.learn._log_values(ema_decay=self.decay if self._do_ema else 0)
 
-# %% ../../nbs/callback.ema.ipynb 13
-try:
-    import wandb
-
-    @patch
-    def _wandb_log_ema_decay(self:EMAWarmupCallback, decay:float):
-        wandb.log({'ema_decay': decay}, self.learn.wandb._wandb_step+1)
-except:
-    pass
+# %% ../../nbs/callback.ema.ipynb 11
+class EMAWarmupCallback(EMASchedule):
+    "EMAWarmpCallback has been renamed to EMASchedule"
+    @delegates(EMASchedule.__init__)
+    def __init__(self, **kwargs):
+        warn("EMAWarmpCallback has been renamed to EMASchedule")
+        super().__init__(**kwargs)
```

### Comparing `fastxtend-0.1.3/fastxtend/callback/lr_finder.py` & `fastxtend-0.1.4/fastxtend/callback/lr_finder.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/callback/profiler.py` & `fastxtend-0.1.4/fastxtend/callback/profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from fastcore.foundation import docs
 from fastcore.basics import mk_class, noop, in_notebook
 
 import fastai
 from fastai.learner import Learner, Recorder
 from fastai.callback.core import *
 
+from .utils import *
 from ..imports import *
-from ..utils import scale_time
+from ..utils import scale_time, convert_to_int
 
 if in_notebook():
     from IPython.display import display
 
 # %% ../../nbs/callback.profiler.ipynb 10
 if parse(fastai.__version__) >= parse('2.7.0'):
     _inner_loop = "before_draw before_batch after_pred after_loss before_backward after_cancel_backward after_backward before_step after_step after_cancel_batch after_batch".split()
@@ -121,26 +122,28 @@
         show_report:bool=True, # Display formatted report post profile
         plain:bool=False, # For Jupyter Notebooks, display plain report
         markdown:bool=False, # Display markdown formatted report
         save_csv:bool=False,  # Save raw results to csv
         csv_name:str='throughput.csv', # CSV save location
         rolling_average:int=10, # Number of batches to average throughput over
         drop_first_batch:bool=True, # Drop the first batch from profiling
-        logger_callback='wandb' # Log report and samples/second to `logger_callback` using `Callback.name`
     ):
         store_attr(but='csv_name,average,drop_first_batch')
         self.csv_name = Path(csv_name)
         self._drop = int(drop_first_batch)
         self._rolling_average = rolling_average
-        self._log_after_batch = getattr(self, f'_{logger_callback}_log_after_batch', noop)
-        self._log_after_fit   = getattr(self, f'_{logger_callback}_log_after_fit', noop)
         self._phase, self._train, self._valid = _phase, _train_short, _valid_short
 
     def before_fit(self):
-        self.has_logger = hasattr(self.learn, self.logger_callback) and not hasattr(self.learn, 'lr_finder') and not hasattr(self, "gather_preds")
+        if hasattr(self.learn, 'wandb') and not hasattr(self.learn, 'lr_finder') and not hasattr(self, "gather_preds"):
+            self._log_summary = self.learn.log_dispatch.log_wandb_summary
+            self._log_table = self.learn.log_dispatch.log_wandb_table
+        else:
+            self._log_summary = noop
+            self._log_table = noop
         self._raw_values, self._processed_samples = {}, {}
         for p in _phase:
             self._raw_values[p] = []
         for p in _epoch:
             for a in getattr(self, f'_{p}'):
                 if a!='samples':
                     self._raw_values[f'{p}_{a}'] = []
@@ -256,24 +259,45 @@
         else:
             bs = np.array(bs[self._drop:])
             self._processed_samples[f'{phase}_{action}'] = bs/input
             sam_per_sec = f'{int(np.around(self._processed_samples[f"{phase}_{action}"].mean())):,d}'
         return [phase, action, np.mean(input), np.std(input), len(input), sam_per_sec,
                 np.sum(input), f'{self._calc_percent(np.sum(input)):.0%}']
 
+    def _log_after_batch(self, actions):
+        bs = np.mean(self._raw_values[f'train_bs'][-self._rolling_average:])
+        self.learn._log_dict({f'throughput/{action}': self._samples_per_second(bs, action) for action in actions})
+
+    def _log_after_fit(self):
+        if self._log_summary.__name__ != 'noop' and self._log_table.__name__ != 'noop':
+            for t in self.learn.profile_results.itertuples():
+                if isinstance(convert_to_int(t._6), int):
+                    self._log_summary(f'{t.Phase}/{t.Action}_throughput', self._processed_samples[f'{t.Phase}_{t.Action}'])
+
+                if t.Phase=='fit':
+                    values = self._raw_values[f'{t.Phase}']
+                    log = f'{t.Phase}/duration' if t.Action == 'fit' else f'{t.Phase}/{t.Action}_duration'
+                else:
+                    # Optionally drop first batch if train/valid phase
+                    values = self._raw_values[f'{t.Phase}_{t.Action}'][self._drop:]
+                    log = f'{t.Phase}/{t.Action}_duration'
+                self._log_summary(log, np.array(values))
+
+            self._log_table("profile_report", dataframe=self.learn.profile_report)
+            self._log_table("profile_results", dataframe=self.learn.profile_results)
+
 # %% ../../nbs/callback.profiler.ipynb 23
 class ThroughputPostCallback(Callback):
     "Required pair with `ThroughputCallback` to profile training performance. Removes itself after training is over."
     order,remove_on_fetch = Recorder.order-1,True
     def __init__(self):
         self._log_full = False
         self._phase, self._train, self._valid = _phase, _train_short, _train_short
 
     def _before_fit(self):
-        self.has_logger = self.profiler.has_logger
         self._start_train_logging, self._start_valid_logging = False, False
         self.n_train_batches = len(self.dls.train)
         self.n_valid_batches = len(self.dls.valid)
         self._rolling_average = self.profiler._rolling_average
         self._iter = -self.profiler._drop
 
     def before_fit(self):
@@ -286,28 +310,28 @@
     def after_validate(self):
         self.profiler._raw_values['valid'].append(time.perf_counter() - self.profiler._validate_start)
 
     def after_batch(self):
         if self.training:
             self.profiler._raw_values['train_batch'].append(time.perf_counter() - self.profiler._train_batch_start)
             self.profiler._raw_values['train_bs'].append(find_bs(self.learn.yb))
-            if self.has_logger and self._iter >= self._rolling_average and self._iter % self._rolling_average == 0:
+            if self._iter >= self._rolling_average and self._iter % self._rolling_average == 0:
                 self.profiler._log_after_batch(self._train)
             self._iter += 1
         else:
             self.profiler._raw_values['valid_batch'].append(time.perf_counter() - self.profiler._valid_batch_start)
             self.profiler._raw_values['valid_bs'].append(find_bs(self.learn.yb))
 
     def after_epoch(self):
         self.profiler._raw_values['epoch'].append(time.perf_counter() - self.profiler._epoch_start)
 
     def _after_fit(self, callbacks):
         self.profiler._raw_values['fit'].append(time.perf_counter() - self.profiler._fit_start)
         self.profiler._generate_report()
-        if self.has_logger: self.profiler._log_after_fit()
+        self.profiler._log_after_fit()
         if not hasattr(self.learn, 'lr_finder'):
             self.profiler._display_report()
             self.learn.remove_cbs(callbacks)
 
     def after_fit(self):
         self._after_fit([ThroughputCallback, ThroughputPostCallback])
 
@@ -325,19 +349,17 @@
         show_report:bool=True, # Display formatted report post profile
         plain:bool=False, # For Jupyter Notebooks, display plain report
         markdown:bool=False, # Display markdown formatted report
         save_csv:bool=False,  # Save raw results to csv
         csv_name:str='simpleprofiler.csv', # CSV save location
         rolling_average:int=10, # Number of batches to average throughput over
         drop_first_batch:bool=True, # Drop the first batch from profiling
-        logger_callback='wandb' # Log report and samples/second to `logger_callback` using `Callback.name`
     ):
         super().__init__(show_report=show_report, plain=plain, markdown=markdown, save_csv=save_csv,
-                         csv_name=csv_name, rolling_average=rolling_average, drop_first_batch=drop_first_batch,
-                         logger_callback=logger_callback)
+                         csv_name=csv_name, rolling_average=rolling_average, drop_first_batch=drop_first_batch)
         self._phase, self._train, self._valid = _phase, _train_full, _valid_full
 
     def before_backward(self):
         self._backward_start = time.perf_counter()
 
     def before_step(self):
         self._raw_values['train_backward'].append(time.perf_counter() - self._backward_start)
@@ -390,66 +412,25 @@
 @patch
 def profile(self:Learner,
         mode:ProfileMode=ProfileMode.Throughput, # Which profiler to use. Throughput or Simple.
         show_report:bool=True, # Display formatted report post profile
         plain:bool=False, # For Jupyter Notebooks, display plain report
         markdown:bool=False, # Display markdown formatted report
         save_csv:bool=False,  # Save raw results to csv
-        csv_name:str='simpleprofiler.csv', # CSV save location
+        csv_name:str='profiler.csv', # CSV save location
         rolling_average:int=10, # Number of batches to average throughput over
         drop_first_batch:bool=True, # Drop the first batch from profiling
-        logger_callback='wandb' # Log report and samples/second to `logger_callback` using `Callback.name`
     ):
     "Run a fastxtend profiler which removes itself when finished training."
     if mode == ProfileMode.Throughput:
-        self.add_cbs([ThroughputCallback(show_report=show_report, plain=plain, markdown=markdown, 
-                                         save_csv=save_csv, csv_name=csv_name, rolling_average=rolling_average, 
-                                         drop_first_batch=drop_first_batch, logger_callback=logger_callback),
+        self.add_cbs([ThroughputCallback(show_report=show_report, plain=plain, markdown=markdown,
+                                         save_csv=save_csv, csv_name=csv_name, rolling_average=rolling_average,
+                                         drop_first_batch=drop_first_batch),
                       ThroughputPostCallback()
                 ])
     if mode == ProfileMode.Simple:
-        self.add_cbs([SimpleProfilerCallback(show_report=show_report, plain=plain, markdown=markdown, 
-                                             save_csv=save_csv, csv_name=csv_name, rolling_average=rolling_average, 
-                                             drop_first_batch=drop_first_batch, logger_callback=logger_callback),
+        self.add_cbs([SimpleProfilerCallback(show_report=show_report, plain=plain, markdown=markdown,
+                                             save_csv=save_csv, csv_name=csv_name, rolling_average=rolling_average,
+                                             drop_first_batch=drop_first_batch),
                       SimpleProfilerPostCallback()
                 ])
     return self
-
-# %% ../../nbs/callback.profiler.ipynb 42
-def convert_to_int(s):
-    try:
-        return int(s.replace(",", ""))
-    except ValueError:
-        return s
-
-# %% ../../nbs/callback.profiler.ipynb 43
-try:
-    import wandb
-
-    @patch
-    def _wandb_log_after_batch(self:ThroughputCallback, actions:list[str]):
-        bs = np.mean(self._raw_values[f'train_bs'][-self._rolling_average:])
-        logs = {f'throughput/{action}': self._samples_per_second(bs, action) for action in actions}
-        wandb.log(logs, self.learn.wandb._wandb_step+1)
-
-    @patch
-    def _wandb_log_after_fit(self:ThroughputCallback):
-        for t in self.learn.profile_results.itertuples():
-            if isinstance(convert_to_int(t._6), int):
-                wandb.summary[f'{t.Phase}/{t.Action}_throughput'] = self._processed_samples[f'{t.Phase}_{t.Action}']
-            
-            if t.Phase=='fit':
-                values = self._raw_values[f'{t.Phase}']
-                log = f'{t.Phase}/duration' if t.Action == 'fit' else f'{t.Phase}/{t.Action}_duration'
-            else:
-                # Optionally drop first batch if train/valid phase
-                values = self._raw_values[f'{t.Phase}_{t.Action}'][self._drop:]
-                log = f'{t.Phase}/{t.Action}_duration'
-            wandb.summary[log] = np.array(values)
-
-        report  = wandb.Table(dataframe=self.learn.profile_report)
-        results = wandb.Table(dataframe=self.learn.profile_results)
-
-        wandb.log({"profile_report": report})
-        wandb.log({"profile_results": results})
-except:
-    pass
```

### Comparing `fastxtend-0.1.3/fastxtend/callback/progresize.py` & `fastxtend-0.1.4/fastxtend/callback/progresize.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 try:
     from fastxtend.ffcv.loader import Loader
     FFCV = True
 except ImportError:
     FFCV = False
 
+from .utils import *
 from ..imports import *
 
 # %% auto 0
 __all__ = ['IncreaseMode', 'ProgressiveResize']
 
 # %% ../../nbs/callback.progresize.ipynb 4
 _resize_augs = (AffineCoordTfm, RandomResizedCropGPU)
@@ -76,15 +77,14 @@
         resize_valid:bool=True, # Apply progressive resizing to valid dataset
         final_size:tuple[int,int]|None=None, # Final image size. Set if using a non-fastai DataLoaders, automatically detected from fastai DataLoader with batch_tfms
         add_resize:bool=False, # Add a separate resize step. Use for non-fastai DataLoaders or fastai DataLoader without batch_tfms
         resize_targ:bool=False, # Applies the separate resize step to targets
         preallocate_bs:int|None=None, # Preallocation batch size. Set if the valid DataLoader has a larger batch size than the train DataLoader.
         empty_cache:bool=False, # Call `torch.cuda.empty_cache()` before a resizing epoch. May prevent Cuda & Magma errors. Don't use with multiple GPUs
         verbose:bool=True, # Print a summary of the progressive resizing schedule
-        logger_callback:str='wandb', # Log image size to `logger_callback` using `Callback.name` if available
     ):
         store_attr()
         self.run_valid = resize_valid
         if resize_targ and not add_resize:
             warn(f'`resize_targ` requires `add_resize` set to True')
         if empty_cache and increase_mode==IncreaseMode.Batch:
             warn(f'`empty_cache` requires `increase_mode` set to Epoch')
@@ -92,16 +92,14 @@
     def before_fit(self):
         "Sets up Progressive Resizing"
         if hasattr(self.learn, 'lr_finder') or hasattr(self.learn, "gather_preds"):
             self.run = False
             return
 
         self._resize, self._remove_resize, self._null_resize, self._remove_cutmix = [], False, True, False
-        self._log_size = getattr(self, f'_{self.logger_callback}_log_size', noop)
-        self.has_logger = hasattr(self.learn, self.logger_callback) and self._log_size != noop
         self.increase_by = tensor(self.increase_by)
         self.resize_batch = self.increase_mode == IncreaseMode.Batch
 
         # Dry run at full resolution to pre-allocate memory
         # See https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html#pre-allocate-memory-in-case-of-variable-input-length
         states = get_random_states()
         try:
@@ -259,37 +257,31 @@
         if self.add_resize:
             self.learn.xb = (self._added_resize(self.x, scale_factor=(self.current_size/self.final_size)[0]),)
             if self.resize_targ:
                 self.learn.yb = (self._added_resize(self.y, scale_factor=(self.current_size/self.final_size)[0]),)
 
     def before_train(self):
         "Increases the image size before the training epoch if set to ProgSizeMode.Epoch"
-        if self.epoch==0 and self.has_logger:
-            self._log_size(False)
+        if self.epoch==0:
+            self._log_size()
 
         if not self.resize_batch and len(self.step_epochs) > 0 and self.epoch >= self.step_epochs[0]:
             _ = self.step_epochs.pop(0)
             self._increase_size()
 
     def after_epoch(self):
         "Calls `torch.cuda.empty_cache()` if `empty_cache=True` before a resizing epoch if set to ProgSizeMode.Epoch. May slightly increase single GPU training speed."
         if not self.resize_batch and self.empty_cache and len(self.step_epochs) > 0 and self.epoch+1 >= self.step_epochs[0]:
             del self.learn.xb
             del self.learn.yb
             del self.learn.pred
             torch.cuda.empty_cache()
 
-        if self.epoch+1==self.n_epoch and self.has_logger:
-            self._log_size(False)
-
     def _increase_size(self):
         "Increase the input size"
-        if self.has_logger:
-            self._log_size(False)
-
         self.current_size += self.increase_by
         for i, resize in enumerate(self._resize):
             if (self.current_size < self.final_size).all():
                 resize.size = _to_size(self.current_size)
                 if self._has_cutmixupaug:
                     self.learn.cut_mix_up_augment._size = _to_size(self.current_size)
             else:
@@ -303,31 +295,22 @@
                     resize.mode = self._orig_modes[i]
 
         if (self.current_size == self.final_size).all() and self._remove_resize:
                 self.add_resize = False
                 if self._remove_cutmix:
                     self.learn.cut_mix_up_augment._cutmixaugs_pipe = Pipeline([])
                     self.learn.cut_mix_up_augment._docutmixaug = False
-
-        if self.has_logger:
-            self._log_size()
+        self._log_size()
 
     def _process_pipeline(self, pipe, null_resize=None):
         'Helper method for processing augmentation pipelines'
         for p in pipe:
             if isinstance(p, _resize_augs):
                 self._resize.append(p)
                 if null_resize is None:
                     self._null_resize = self._null_resize and p.size is None
                 else:
                     self._null_resize = null_resize
 
-# %% ../../nbs/callback.progresize.ipynb 46
-try:
-    import wandb
-
-    @patch
-    def _wandb_log_size(self:ProgressiveResize, next_step=True):
+    def _log_size(self):
         size = _to_size(self.current_size)
-        wandb.log({'progressive_resize_size': size[0]}, self.learn.wandb._wandb_step+int(next_step))
-except:
-    pass
+        self.learn._log_values(progressive_resize_size=size[0])
```

### Comparing `fastxtend-0.1.3/fastxtend/callback/tracker.py` & `fastxtend-0.1.4/fastxtend/callback/tracker.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/data/transforms.py` & `fastxtend-0.1.4/fastxtend/data/transforms.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/epoch_iterator.py` & `fastxtend-0.1.4/fastxtend/ffcv/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/fields.py` & `fastxtend-0.1.4/fastxtend/ffcv/fields.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/inference.py` & `fastxtend-0.1.4/fastxtend/ffcv/inference.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/loader.py` & `fastxtend-0.1.4/fastxtend/ffcv/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,19 @@
 
     @property
     def n_inp(self) -> int:
         "Number of elements in a batch for model input"
         return self._n_inp
 
     @property
+    def bs(self) -> int:
+        "Number of items a batch"
+        return self.batch_size
+
+    @property
     def device(self):
         return self._device
 
     @device.setter
     def device(self, device:int|str|torch.device):
         # parse device
         device, *_ = torch._C._nn._parse_to(device=device)
```

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/operations.py` & `fastxtend-0.1.4/fastxtend/ffcv/operations.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/transforms.py` & `fastxtend-0.1.4/fastxtend/ffcv/transforms.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/utils.py` & `fastxtend-0.1.4/fastxtend/ffcv/utils.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/ffcv/writer.py` & `fastxtend-0.1.4/fastxtend/ffcv/writer.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/imports.py` & `fastxtend-0.1.4/fastxtend/imports.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/losses.py` & `fastxtend-0.1.4/fastxtend/losses.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/metrics.py` & `fastxtend-0.1.4/fastxtend/metrics.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/multiloss.py` & `fastxtend-0.1.4/fastxtend/multiloss.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/adan.py` & `fastxtend-0.1.4/fastxtend/optimizer/adan.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/eightbit.py` & `fastxtend-0.1.4/fastxtend/optimizer/eightbit.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/foreach.py` & `fastxtend-0.1.4/fastxtend/optimizer/foreach.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/fused.py` & `fastxtend-0.1.4/fastxtend/optimizer/fused.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/lion.py` & `fastxtend-0.1.4/fastxtend/optimizer/lion.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/sophia.py` & `fastxtend-0.1.4/fastxtend/optimizer/sophia.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/stableadam.py` & `fastxtend-0.1.4/fastxtend/optimizer/stableadam.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from .foreach import ForEachOptimizer
 from ..imports import *
 
 # %% auto 0
 __all__ = ['StableAdam', 'stableadam']
 
 # %% ../../nbs/optimizer.stableadam.ipynb 6
+# simplified version of:
+#   beta = beta*(1-beta**(step-1))/(1-beta**step)
 def debias(beta:float, step:int):
     "Stable Adam debias calculation"
-    return beta*(1-beta**(step-1))/(1-beta**step)
+    return (beta**step - beta)/(beta**step - 1)
 
 # %% ../../nbs/optimizer.stableadam.ipynb 7
 def stable_adam_step(p:Tensor, lr:float, eps:float, wd:float, mom:float, sqr_mom:float,
                      step:int=0, grad_avg:Tensor|None=None, sqr_avg:Tensor|None=None,
                      decouple_wd:bool=True, do_wd:bool=True, eps_t=None, **kwargs):
     "Updates Stable Adam moving averages and performs the Stable Adam step with `lr` on `p`"
     if step == 0:
@@ -79,16 +81,16 @@
         else:
             # expiramental l2_reg. not in paper
             wd = np.where(do_wd, wd, 1.)
             torch._foreach_addcdiv_(g, p, ones, scalars=wd.tolist())
             # cannot use scalers with foreach_add & multiple tensors, so divide by one with foreach_addcdiv
 
     # calculate debiased momentum (beta) terms
-    db_mom     = mom*(1-mom**(steps-1))/(1-mom**steps)
-    db_sqr_mom = sqr_mom*(1-sqr_mom**(steps-1))/(1-sqr_mom**steps)
+    db_mom     = (mom**steps - mom)/(mom**steps - 1)
+    db_sqr_mom = (sqr_mom**steps - sqr_mom)/(sqr_mom**steps - 1)
 
     # update moving average
     torch._foreach_mul_(grad_avg, scalars=db_mom.tolist())
     torch._foreach_addcdiv_(grad_avg, g, ones, scalars=(1-db_mom).tolist())
 
     # update squared moving average
     torch._foreach_mul_(sqr_avg, scalars=db_sqr_mom.tolist())
```

### Comparing `fastxtend-0.1.3/fastxtend/optimizer/torchscript.py` & `fastxtend-0.1.4/fastxtend/optimizer/torchscript.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/patches.py` & `fastxtend-0.1.4/fastxtend/patches.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/schedulers.py` & `fastxtend-0.1.4/fastxtend/schedulers.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/test_utils.py` & `fastxtend-0.1.4/fastxtend/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/torch_core.py` & `fastxtend-0.1.4/fastxtend/torch_core.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/transform.py` & `fastxtend-0.1.4/fastxtend/transform.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/utils.py` & `fastxtend-0.1.4/fastxtend/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from fastcore.foundation import contextmanager
 
 from fastai.learner import Learner
 from fastai.data.core import DataLoaders
 from fastai.callback.core import set_random_states, get_random_states
 
 # %% auto 0
-__all__ = ['free_gpu_memory', 'less_random', 'scale_time', 'pil_to_numpy']
+__all__ = ['free_gpu_memory', 'less_random', 'scale_time', 'pil_to_numpy', 'convert_to_int']
 
 # %% ../nbs/utils.ipynb 4
 def clean_ipython_hist():
     # Code in this function mainly copied from IPython source
     if not 'get_ipython' in globals():
         return
     ip = get_ipython()
@@ -123,7 +123,14 @@
     while not s:
         l, s, d = enc.encode(bufsize)
         mem[offset:offset + len(d)] = d
         offset += len(d)
     if s < 0:
         raise RuntimeError("encoder error %d in tobytes" % s)
     return data
+
+# %% ../nbs/utils.ipynb 11
+def convert_to_int(s):
+    try:
+        return int(s.replace(",", ""))
+    except ValueError:
+        return s
```

### Comparing `fastxtend-0.1.3/fastxtend/vision/augment/batch.py` & `fastxtend-0.1.4/fastxtend/vision/augment/batch.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/vision/augment/itemtensor.py` & `fastxtend-0.1.4/fastxtend/vision/augment/itemtensor.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/vision/data.py` & `fastxtend-0.1.4/fastxtend/vision/data.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/vision/models/attention_modules.py` & `fastxtend-0.1.4/fastxtend/vision/models/attention_modules.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/vision/models/pooling.py` & `fastxtend-0.1.4/fastxtend/vision/models/pooling.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend/vision/models/xresnet.py` & `fastxtend-0.1.4/fastxtend/vision/models/xresnet.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/fastxtend.egg-info/PKG-INFO` & `fastxtend-0.1.4/fastxtend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastxtend
-Version: 0.1.3
+Version: 0.1.4
 Summary: Train fastai models faster (and other useful tools)
 Home-page: https://github.com/warner-benjamin/fastxtend
 Author: Benjamin Warner
 Author-email: me@benjaminwarner.dev
 License: MIT License
 Project-URL: Documentation, https://fastxtend.benjaminwarner.dev/
 Keywords: fastai pytorch extensions
```

### Comparing `fastxtend-0.1.3/fastxtend.egg-info/SOURCES.txt` & `fastxtend-0.1.4/fastxtend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,26 @@
 fastxtend/audio/augment.py
 fastxtend/audio/core.py
 fastxtend/audio/data.py
 fastxtend/audio/learner.py
 fastxtend/audio/mixup.py
 fastxtend/callback/__init__.py
 fastxtend/callback/all.py
+fastxtend/callback/amp.py
 fastxtend/callback/channelslast.py
 fastxtend/callback/compiler.py
 fastxtend/callback/cutmixup.py
 fastxtend/callback/ema.py
+fastxtend/callback/gradaccum.py
 fastxtend/callback/lr_finder.py
 fastxtend/callback/profiler.py
 fastxtend/callback/progresize.py
 fastxtend/callback/simpleprofiler.py
 fastxtend/callback/tracker.py
+fastxtend/callback/utils.py
 fastxtend/data/__init__.py
 fastxtend/data/all.py
 fastxtend/data/transforms.py
 fastxtend/ffcv/__init__.py
 fastxtend/ffcv/all.py
 fastxtend/ffcv/epoch_iterator.py
 fastxtend/ffcv/fields.py
```

### Comparing `fastxtend-0.1.3/fastxtend.egg-info/requires.txt` & `fastxtend-0.1.4/fastxtend.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.3/setup.py` & `fastxtend-0.1.4/setup.py`

 * *Files identical despite different names*

