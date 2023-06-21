# Comparing `tmp/rl4co-0.0.3.dev1.tar.gz` & `tmp/rl4co-0.0.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.0.3.dev1.tar", last modified: Wed Jun 21 19:04:03 2023, max compression
+gzip compressed data, was "rl4co-0.0.3.dev3.tar", last modified: Wed Jun 21 19:57:20 2023, max compression
```

## Comparing `rl4co-0.0.3.dev1.tar` & `rl4co-0.0.3.dev3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.034426 rl4co-0.0.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-06-21 19:04:03.034426 rl4co-0.0.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.014426 rl4co-0.0.3.dev1/rl4co/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.018426 rl4co-0.0.3.dev1/rl4co/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/data/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.018426 rl4co-0.0.3.dev1/rl4co/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/atsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/dpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/ffsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/mdpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/mtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/op.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/pctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/sdvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/envs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.018426 rl4co-0.0.3.dev1/rl4co/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.022426 rl4co-0.0.3.dev1/rl4co/models/nn/
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/env_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/env_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.022426 rl4co-0.0.3.dev1/rl4co/models/nn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/graph/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/graph/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/graph/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.014426 rl4co-0.0.3.dev1/rl4co/models/rl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.022426 rl4co-0.0.3.dev1/rl4co/models/rl/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/rl/ppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/rl/ppo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.022426 rl4co-0.0.3.dev1/rl4co/models/rl/reinforce/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/rl/reinforce/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/rl/reinforce/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/rl/reinforce/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.014426 rl4co-0.0.3.dev1/rl4co/models/zoo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.022426 rl4co-0.0.3.dev1/rl4co/models/zoo/am/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/am/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/am/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/am/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/am/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.026426 rl4co-0.0.3.dev1/rl4co/models/zoo/amppo/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/amppo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/amppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/amppo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.026426 rl4co-0.0.3.dev1/rl4co/models/zoo/ham/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ham/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ham/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ham/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ham/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.026426 rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.026426 rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.030426 rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.030426 rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.030426 rl4co-0.0.3.dev1/rl4co/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/tasks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/tasks/rl4co.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.034426 rl4co-0.0.3.dev1/rl4co/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.034426 rl4co-0.0.3.dev1/rl4co/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/callbacks/speed_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.034426 rl4co-0.0.3.dev1/rl4co/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/download/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/download/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/download/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/param_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/rl4co/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.018426 rl4co-0.0.3.dev1/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-06-21 19:04:02.000000 rl4co-0.0.3.dev1/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-21 19:04:03.000000 rl4co-0.0.3.dev1/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:04:02.000000 rl4co-0.0.3.dev1/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 19:04:02.000000 rl4co-0.0.3.dev1/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 19:04:02.000000 rl4co-0.0.3.dev1/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:04:03.034426 rl4co-0.0.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:04:03.034426 rl4co-0.0.3.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 19:03:50.000000 rl4co-0.0.3.dev1/tests/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.060481 rl4co-0.0.3.dev3/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.064481 rl4co-0.0.3.dev3/rl4co/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/atsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/cvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/dpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/ffsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/mdpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/mtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/pctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/sdvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/env_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/env_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/nn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/graph/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/graph/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/graph/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.060481 rl4co-0.0.3.dev3/rl4co/models/rl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/rl/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/ppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/ppo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.060481 rl4co-0.0.3.dev3/rl4co/models/zoo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/am/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.076481 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.076481 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.076481 rl4co-0.0.3.dev3/rl4co/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/tasks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/tasks/rl4co.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/rl4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/rl4co/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/callbacks/speed_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/rl4co/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/param_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.064481 rl4co-0.0.3.dev3/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/tests/test_ops.py
```

### Comparing `rl4co-0.0.3.dev1/LICENSE` & `rl4co-0.0.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/PKG-INFO` & `rl4co-0.0.3.dev3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.3.dev1
+Version: 0.0.3.dev3
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,22 +220,23 @@
 Provides-Extra: testing
 Provides-Extra: linting
 License-File: LICENSE
 
 <div align="center">
 
 # RL4CO
-    
-An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering. 
-        
+
+An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
+
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
 <a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+[![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
 </div>
 
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
@@ -243,14 +244,15 @@
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
 ![image](https://github.com/kaist-silab/rl4co/assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60)
 
 
 ## Getting started
+<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 
 RL4CO is now available for installation on `pip`!
 ```bash
 pip install rl4co
 ```
 
 ### Local install and development
@@ -279,32 +281,32 @@
 To get started, we recommend checking out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 
 ## Usage
 
 
 Train model with default configuration (AM on TSP environment):
 ```bash
-python run.py  
+python run.py
 ```
 
 
 
 <details>
     <summary>Change experiment</summary>
 
 Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
 ```bash
-python run.py experiment=tsp/am env.num_loc=42 
+python run.py experiment=tsp/am env.num_loc=42
 ```
 </details>
 
 
 <details>
     <summary>Disable logging</summary>
-    
+
 ```bash
 python run.py experiment=test/am logger=none '~callbacks.learning_rate_monitor'
 ```
 Note that `~` is used to disable a callback that would need a logger.
 
 </details>
 
@@ -329,15 +331,15 @@
 from rl4co.envs import TSPEnv
 from rl4co.models.zoo.am import AttentionModel
 from rl4co.tasks.rl4co import RL4COLitModule
 
 config = DictConfig(
     {"data": {
             "train_size": 100000,
-            "val_size": 10000, 
+            "val_size": 10000,
             "batch_size": 512,
         },
     "optimizer": {"lr": 1e-4}}
 )
 
 # Environment, Model, and Lightning Module
 env = TSPEnv(num_loc=20)
@@ -364,13 +366,13 @@
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
 
 ## Contributing
-Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO! 
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO!
 
 ### Contributors
 <a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
 </a>
```

### Comparing `rl4co-0.0.3.dev1/README.md` & `rl4co-0.0.3.dev3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 <div align="center">
 
 # RL4CO
-    
-An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering. 
-        
+
+An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
+
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
 <a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+[![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
 </div>
 
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
@@ -20,14 +21,15 @@
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
 ![image](https://github.com/kaist-silab/rl4co/assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60)
 
 
 ## Getting started
+<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 
 RL4CO is now available for installation on `pip`!
 ```bash
 pip install rl4co
 ```
 
 ### Local install and development
@@ -56,32 +58,32 @@
 To get started, we recommend checking out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 
 ## Usage
 
 
 Train model with default configuration (AM on TSP environment):
 ```bash
-python run.py  
+python run.py
 ```
 
 
 
 <details>
     <summary>Change experiment</summary>
 
 Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
 ```bash
-python run.py experiment=tsp/am env.num_loc=42 
+python run.py experiment=tsp/am env.num_loc=42
 ```
 </details>
 
 
 <details>
     <summary>Disable logging</summary>
-    
+
 ```bash
 python run.py experiment=test/am logger=none '~callbacks.learning_rate_monitor'
 ```
 Note that `~` is used to disable a callback that would need a logger.
 
 </details>
 
@@ -106,15 +108,15 @@
 from rl4co.envs import TSPEnv
 from rl4co.models.zoo.am import AttentionModel
 from rl4co.tasks.rl4co import RL4COLitModule
 
 config = DictConfig(
     {"data": {
             "train_size": 100000,
-            "val_size": 10000, 
+            "val_size": 10000,
             "batch_size": 512,
         },
     "optimizer": {"lr": 1e-4}}
 )
 
 # Environment, Model, and Lightning Module
 env = TSPEnv(num_loc=20)
@@ -141,13 +143,13 @@
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
 
 ## Contributing
-Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO! 
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO!
 
 ### Contributors
 <a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
 </a>
```

#### html2text {}

```diff
@@ -1,47 +1,51 @@
 # RL4CO An extensive Reinforcement Learning (RL) for Combinatorial Optimization
   (CO) benchmark. Our goal is to provide a unified framework for RL-based CO
  algorithms, and to facilitate reproducible research in this field, decoupling
    the science from the engineering. [PyTorch] [Lightning] [base:_TorchRL]_
       [config:_Hydra]_[![Code_style:_black](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black)_![license](https:
-           //img.shields.io/badge/license-Apache%202.0-green.svg?)_
+   //img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://
+  img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)_[!
+   [Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/
+badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)_
 RL4CO is built upon: - [TorchRL](https://github.com/pytorch/rl): official
 PyTorch framework for RL algorithms and vectorized environments on GPUs -
 [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily
 handle heterogeneous data such as states, actions and rewards - [PyTorch
 Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch
 wrapper for high-performance AI research - [Hydra](https://github.com/
 facebookresearch/hydra): a framework for elegantly configuring complex
 applications ![image](https://github.com/kaist-silab/rl4co/assets/48984123/
-0db4efdd-1c93-4991-8f09-f3c6c1f35d60) ## Getting started RL4CO is now available
-for installation on `pip`! ```bash pip install rl4co ``` ### Local install and
-development If you want to develop RL4CO or access the latest builds, we
-recommend you to install it locally with `pip` in editable mode: ```bash git
-clone https://github.com/kaist-silab/rl4co && cd rl4co pip install -e . ```
-[Optional] Automatically install PyTorch with correct CUDA version These
-commands will [automatically install](https://github.com/pmeier/light-the-
-torch) PyTorch with the right GPU version for your system: ```bash pip install
-light-the-torch python3 -m light_the_torch install -r --upgrade torch ``` >
-Note: `conda` is also a good candidate for hassle-free installation of PyTorch:
-check out the [PyTorch website](https://pytorch.org/get-started/locally/) for
-more details.  To get started, we recommend checking out our [quickstart
-notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example]
-(#minimalistic-example) below. ## Usage Train model with default configuration
-(AM on TSP environment): ```bash python run.py ```  Change experiment Train
-model with chosen experiment configuration from [configs/experiment/](configs/
-experiment/) (e.g. tsp/am, and environment with 42 cities) ```bash python
-run.py experiment=tsp/am env.num_loc=42 ```   Disable logging ```bash python
-run.py experiment=test/am logger=none '~callbacks.learning_rate_monitor' ```
-Note that `~` is used to disable a callback that would need a logger.   Create
-a sweep over hyperparameters (-m for multirun) ```bash python run.py -
-m experiment=tsp/am train.optimizer.lr=1e-3,1e-4,1e-5 ```  ### Minimalistic
-Example Here is a minimalistic example training the Attention Model with greedy
-rollout baseline on TSP in less than 50 lines of code: ```python from omegaconf
-import DictConfig import lightning as L from rl4co.envs import TSPEnv from
+0db4efdd-1c93-4991-8f09-f3c6c1f35d60) ## Getting started [Open_In_Colab] RL4CO
+is now available for installation on `pip`! ```bash pip install rl4co ``` ###
+Local install and development If you want to develop RL4CO or access the latest
+builds, we recommend you to install it locally with `pip` in editable mode:
+```bash git clone https://github.com/kaist-silab/rl4co && cd rl4co pip install
+-e . ```  [Optional] Automatically install PyTorch with correct CUDA version
+These commands will [automatically install](https://github.com/pmeier/light-
+the-torch) PyTorch with the right GPU version for your system: ```bash pip
+install light-the-torch python3 -m light_the_torch install -r --upgrade torch
+``` > Note: `conda` is also a good candidate for hassle-free installation of
+PyTorch: check out the [PyTorch website](https://pytorch.org/get-started/
+locally/) for more details.  To get started, we recommend checking out our
+[quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic
+example](#minimalistic-example) below. ## Usage Train model with default
+configuration (AM on TSP environment): ```bash python run.py ```  Change
+experiment Train model with chosen experiment configuration from [configs/
+experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
+```bash python run.py experiment=tsp/am env.num_loc=42 ```   Disable logging
+```bash python run.py experiment=test/am logger=none
+'~callbacks.learning_rate_monitor' ``` Note that `~` is used to disable a
+callback that would need a logger.   Create a sweep over hyperparameters (-
+m for multirun) ```bash python run.py -m experiment=tsp/am
+train.optimizer.lr=1e-3,1e-4,1e-5 ```  ### Minimalistic Example Here is a
+minimalistic example training the Attention Model with greedy rollout baseline
+on TSP in less than 50 lines of code: ```python from omegaconf import
+DictConfig import lightning as L from rl4co.envs import TSPEnv from
 rl4co.models.zoo.am import AttentionModel from rl4co.tasks.rl4co import
 RL4COLitModule config = DictConfig( {"data": { "train_size": 100000,
 "val_size": 10000, "batch_size": 512, }, "optimizer": {"lr": 1e-4}} ) #
 Environment, Model, and Lightning Module env = TSPEnv(num_loc=20) model =
 AttentionModel(env) lit_module = RL4COLitModule(config, env, model) # Trainer
 trainer = L.Trainer( max_epochs=3, # only few epochs accelerator="gpu", # use
 GPU if available, else you can use others as "cpu" logger=None, # can replace
```

### Comparing `rl4co-0.0.3.dev1/pyproject.toml` & `rl4co-0.0.3.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/data/dataset.py` & `rl4co-0.0.3.dev3/rl4co/data/dataset.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/data/generate_data.py` & `rl4co-0.0.3.dev3/rl4co/data/generate_data.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/data/utils.py` & `rl4co-0.0.3.dev3/rl4co/data/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/atsp.py` & `rl4co-0.0.3.dev3/rl4co/envs/atsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/base.py` & `rl4co-0.0.3.dev3/rl4co/envs/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/cvrp.py` & `rl4co-0.0.3.dev3/rl4co/envs/cvrp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/dpp.py` & `rl4co-0.0.3.dev3/rl4co/envs/dpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/ffsp.py` & `rl4co-0.0.3.dev3/rl4co/envs/ffsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/mdpp.py` & `rl4co-0.0.3.dev3/rl4co/envs/mdpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/mtsp.py` & `rl4co-0.0.3.dev3/rl4co/envs/mtsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/op.py` & `rl4co-0.0.3.dev3/rl4co/envs/op.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/pctsp.py` & `rl4co-0.0.3.dev3/rl4co/envs/pctsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/pdp.py` & `rl4co-0.0.3.dev3/rl4co/envs/pdp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/sdvrp.py` & `rl4co-0.0.3.dev3/rl4co/envs/sdvrp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/tsp.py` & `rl4co-0.0.3.dev3/rl4co/envs/tsp.py`

 * *Files 16% similar despite different names*

```diff
@@ -169,16 +169,15 @@
             + self.min_loc
         )
         return TensorDict({"locs": locs}, batch_size=batch_size)
 
     @staticmethod
     def render(td, actions=None, ax=None):
         import matplotlib.pyplot as plt
-
-        from matplotlib import cm
+        import numpy as np
 
         if ax is None:
             # Create a plot of the nodes
             _, ax = plt.subplots()
 
         td = td.detach().cpu()
         # if batch_size greater than 0 , we need to select the first batch element
@@ -193,55 +192,24 @@
         # gather locs in order of action if available
         if actions is None:
             log.warning("No action in TensorDict, rendering unsorted locs")
         else:
             locs = gather_by_index(locs, actions, dim=0)
 
         # Cat the first node to the end to complete the tour
+        locs = torch.cat((locs, locs[0:1]))
         x, y = locs[:, 0], locs[:, 1]
 
-        # SECTION: new
-        # plot visited nodes
-        ax.scatter(
-            x,
-            y,
-            edgecolors=cm.Set2(0),
-            facecolors="none",
-            s=100,
-            linewidths=2,
-            marker="o",
-            alpha=1,
-        )
-
-        # plot actions
-        for action_idx in range(len(actions) - 1):
-            from_loc = locs[actions[action_idx]]
-            to_loc = locs[actions[action_idx + 1]]
-            ax.plot(
-                [from_loc[0], to_loc[0]],
-                [from_loc[1], to_loc[1]],
-                color=cm.tab20c(5),
-            )
-            ax.annotate(
-                "",
-                xy=(to_loc[0], to_loc[1]),
-                xytext=(from_loc[0], from_loc[1]),
-                arrowprops=dict(arrowstyle="->", color=cm.tab20c(5)),
-                annotation_clip=False,
-            )
-
-        # setup
-        ax.set_xlim(-0.05, 1.05)
-        ax.set_ylim(-0.05, 1.05)
-        ax.grid(axis="both", color="black", ls="--", alpha=0.1)
+        # Plot the visited nodes
+        ax.scatter(x, y, color="tab:blue")
 
-        # plt.tick_params(axis='both', which='both', bottom=False, top=False, labelbottom=False, right=False, left=False, labelleft=False)
+        # Add arrows between visited nodes as a quiver plot
+        dx, dy = np.diff(x), np.diff(y)
+        ax.quiver(
+            x[:-1], y[:-1], dx, dy, scale_units="xy", angles="xy", scale=1, color="k"
+        )
 
         # Set plot title and axis labels
-        title_font = {"fontsize": 14}
-        label_font = {"fontsize": 12}
-        ax.set_title("TSP Solution", fontdict=title_font)
-        ax.set_xlabel("X Coordinate", fontdict=label_font)
-        ax.set_ylabel("Y Coordinate", fontdict=label_font)
-
-        # plt.tight_layout()
+        ax.set_title("TSP Solution")
+        ax.set_xlabel("x-coordinate")
+        ax.set_ylabel("y-coordinate")
         plt.show()
```

### Comparing `rl4co-0.0.3.dev1/rl4co/envs/utils.py` & `rl4co-0.0.3.dev3/rl4co/envs/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/attention.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/env_context.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/env_context.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/env_embedding.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/env_embedding.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/flash_attention.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/graph/gat.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/graph/gat.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/graph/gcn.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/graph/gcn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/graph/mpnn.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/graph/mpnn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/mlp.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/ops.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/nn/utils.py` & `rl4co-0.0.3.dev3/rl4co/models/nn/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/rl/ppo/model.py` & `rl4co-0.0.3.dev3/rl4co/models/rl/ppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/rl/ppo/task.py` & `rl4co-0.0.3.dev3/rl4co/models/rl/ppo/task.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/rl/reinforce/base.py` & `rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/rl/reinforce/baselines.py` & `rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/baselines.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/rl/reinforce/critic.py` & `rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/am/decoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/am/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/am/model.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/am/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/am/policy.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/am/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/amppo/decoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/amppo/model.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/amppo/policy.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ham/attention.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ham/encoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ham/model.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ham/policy.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/decoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/encoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/model.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/mdam/policy.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/augmentations.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/decoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/model.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/pomo/policy.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/critic.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/decoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/encoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/model.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/ptrnet/policy.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/augmentations.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/decoder.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/losses.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/losses.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/model.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/models/zoo/symnco/policy.py` & `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/tasks/eval.py` & `rl4co-0.0.3.dev3/rl4co/tasks/eval.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/tasks/rl4co.py` & `rl4co-0.0.3.dev3/rl4co/tasks/rl4co.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/callbacks/speed_monitor.py` & `rl4co-0.0.3.dev3/rl4co/utils/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/download/downloader.py` & `rl4co-0.0.3.dev3/rl4co/utils/download/downloader.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/download/gdrive.py` & `rl4co-0.0.3.dev3/rl4co/utils/download/gdrive.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/download/s3.py` & `rl4co-0.0.3.dev3/rl4co/utils/download/s3.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/helpers.py` & `rl4co-0.0.3.dev3/rl4co/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/instantiators.py` & `rl4co-0.0.3.dev3/rl4co/utils/instantiators.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/lightning.py` & `rl4co-0.0.3.dev3/rl4co/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/logging_utils.py` & `rl4co-0.0.3.dev3/rl4co/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/ops.py` & `rl4co-0.0.3.dev3/rl4co/utils/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/param_grouping.py` & `rl4co-0.0.3.dev3/rl4co/utils/param_grouping.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/pylogger.py` & `rl4co-0.0.3.dev3/rl4co/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/rich_utils.py` & `rl4co-0.0.3.dev3/rl4co/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/test_utils.py` & `rl4co-0.0.3.dev3/rl4co/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/transfer.py` & `rl4co-0.0.3.dev3/rl4co/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co/utils/utils.py` & `rl4co-0.0.3.dev3/rl4co/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/rl4co.egg-info/PKG-INFO` & `rl4co-0.0.3.dev3/rl4co.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.3.dev1
+Version: 0.0.3.dev3
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,22 +220,23 @@
 Provides-Extra: testing
 Provides-Extra: linting
 License-File: LICENSE
 
 <div align="center">
 
 # RL4CO
-    
-An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering. 
-        
+
+An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
+
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
 <a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+[![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
 </div>
 
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
@@ -243,14 +244,15 @@
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
 ![image](https://github.com/kaist-silab/rl4co/assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60)
 
 
 ## Getting started
+<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 
 RL4CO is now available for installation on `pip`!
 ```bash
 pip install rl4co
 ```
 
 ### Local install and development
@@ -279,32 +281,32 @@
 To get started, we recommend checking out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 
 ## Usage
 
 
 Train model with default configuration (AM on TSP environment):
 ```bash
-python run.py  
+python run.py
 ```
 
 
 
 <details>
     <summary>Change experiment</summary>
 
 Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
 ```bash
-python run.py experiment=tsp/am env.num_loc=42 
+python run.py experiment=tsp/am env.num_loc=42
 ```
 </details>
 
 
 <details>
     <summary>Disable logging</summary>
-    
+
 ```bash
 python run.py experiment=test/am logger=none '~callbacks.learning_rate_monitor'
 ```
 Note that `~` is used to disable a callback that would need a logger.
 
 </details>
 
@@ -329,15 +331,15 @@
 from rl4co.envs import TSPEnv
 from rl4co.models.zoo.am import AttentionModel
 from rl4co.tasks.rl4co import RL4COLitModule
 
 config = DictConfig(
     {"data": {
             "train_size": 100000,
-            "val_size": 10000, 
+            "val_size": 10000,
             "batch_size": 512,
         },
     "optimizer": {"lr": 1e-4}}
 )
 
 # Environment, Model, and Lightning Module
 env = TSPEnv(num_loc=20)
@@ -364,13 +366,13 @@
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
 
 ## Contributing
-Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO! 
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO!
 
 ### Contributors
 <a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
 </a>
```

### Comparing `rl4co-0.0.3.dev1/rl4co.egg-info/SOURCES.txt` & `rl4co-0.0.3.dev3/rl4co.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/tests/test_envs.py` & `rl4co-0.0.3.dev3/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/tests/test_models.py` & `rl4co-0.0.3.dev3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev1/tests/test_ops.py` & `rl4co-0.0.3.dev3/tests/test_ops.py`

 * *Files identical despite different names*

