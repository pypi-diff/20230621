# Comparing `tmp/autogluon.tabular-0.8.1b20230620.tar.gz` & `tmp/autogluon.tabular-0.8.1b20230621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.8.1b20230620.tar", last modified: Tue Jun 20 09:04:12 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.8.1b20230621.tar", last modified: Wed Jun 21 09:04:16 2023, max compression
```

## Comparing `autogluon.tabular-0.8.1b20230620.tar` & `autogluon.tabular-0.8.1b20230621.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.776333 autogluon.tabular-0.8.1b20230620/
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-20 09:04:12.776333 autogluon.tabular-0.8.1b20230620/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:04:12.776333 autogluon.tabular-0.8.1b20230620/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.752333 autogluon.tabular-0.8.1b20230620/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.752333 autogluon.tabular-0.8.1b20230620/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.756333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.760333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.764333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.764333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.764333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.764333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.764333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.764333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.764333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.768333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.768333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.768333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.768333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.768333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.768333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.768333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.772333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35982 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.772333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.772333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.772333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.772333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.772333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.772333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)   267286 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.776333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.776333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.776333 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-20 09:03:44.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:12.756333 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:04:12.000000 autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.764482 autogluon.tabular-0.8.1b20230621/
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-21 09:04:16.764482 autogluon.tabular-0.8.1b20230621/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:04:16.764482 autogluon.tabular-0.8.1b20230621/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.744481 autogluon.tabular-0.8.1b20230621/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.744481 autogluon.tabular-0.8.1b20230621/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.748481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.748481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.748481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.748481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.752481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.756482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35982 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267286 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.760481 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.764482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.764482 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-21 09:03:46.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:16.748481 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:04:16.000000 autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.8.1b20230620/PKG-INFO` & `autogluon.tabular-0.8.1b20230621/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.8.1b20230620
+Version: 0.8.1b20230621
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -20,14 +20,15 @@
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Continuous Integration](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml)
         [![Platform Tests](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml/badge.svg?event=schedule)](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/autogluon/)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
+        [![](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
         [![Twitter](https://img.shields.io/twitter/follow/autogluon?style=social)](https://twitter.com/autogluon)
         
         [Install Instructions](https://auto.gluon.ai/stable/install.html) | Documentation ([Stable](https://auto.gluon.ai/stable/index.html) | [Latest](https://auto.gluon.ai/dev/index.html))
         
         AutoGluon automates machine learning tasks enabling you to easily achieve strong predictive performance in your applications.  With just a few lines of code, you can train and deploy high-accuracy machine learning and deep learning models on image, text, time series, and tabular data.
         
         ## Example
```

### Comparing `autogluon.tabular-0.8.1b20230620/setup.py` & `autogluon.tabular-0.8.1b20230621/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/predictor/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -2376,15 +2376,15 @@
                     "XT": {"compiler": "onnx"},
                     "NN_TORCH": {"compiler": "onnx"},
                 }
             else:
                 raise ValueError(f'Unknown compiler_configs preset: "{compiler_configs}"')
         self._trainer.compile_models(model_names=models, with_ancestors=with_ancestors, compiler_configs=compiler_configs)
 
-    def persist_models(self, models='best', with_ancestors=True, max_memory=0.1) -> list:
+    def persist_models(self, models='best', with_ancestors=True, max_memory=0.4) -> list:
         """
         Persist models in memory for reduced inference latency. This is particularly important if the models are being used for online-inference where low latency is critical.
         If models are not persisted in memory, they are loaded from disk every time they are asked to make predictions.
 
         Parameters
         ----------
         models : list of str or str, default = 'best'
@@ -2392,15 +2392,15 @@
             If 'best' then the model with the highest validation score is persisted (this is the model used for prediction by default).
             If 'all' then all models are persisted.
             Valid models are listed in this `predictor` by calling `predictor.get_model_names()`.
         with_ancestors : bool, default = True
             If True, all ancestor models of the provided models will also be persisted.
             If False, stacker models will not have the models they depend on persisted unless those models were specified in `models`. This will slow down inference as the ancestor models will still need to be loaded from disk for each predict call.
             Only relevant for stacker models.
-        max_memory : float, default = 0.1
+        max_memory : float, default = 0.4
             Proportion of total available memory to allow for the persisted models to use.
             If the models' summed memory usage requires a larger proportion of memory than max_memory, they are not persisted. In this case, the output will be an empty list.
             If None, then models are persisted regardless of estimated memory usage. This can cause out-of-memory errors.
 
         Returns
         -------
         List of persisted model names.
```

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.8.1b20230621/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.8.1b20230620
+Version: 0.8.1b20230621
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -20,14 +20,15 @@
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Continuous Integration](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml)
         [![Platform Tests](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml/badge.svg?event=schedule)](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/autogluon/)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
+        [![](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
         [![Twitter](https://img.shields.io/twitter/follow/autogluon?style=social)](https://twitter.com/autogluon)
         
         [Install Instructions](https://auto.gluon.ai/stable/install.html) | Documentation ([Stable](https://auto.gluon.ai/stable/index.html) | [Latest](https://auto.gluon.ai/dev/index.html))
         
         AutoGluon automates machine learning tasks enabling you to easily achieve strong predictive performance in your applications.  With just a few lines of code, you can train and deploy high-accuracy machine learning and deep learning models on image, text, time series, and tabular data.
         
         ## Example
```

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230620/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-0.8.1b20230621/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 numpy<1.27,>=1.21
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 networkx<4,>=3.0
-autogluon.core==0.8.1b20230620
-autogluon.features==0.8.1b20230620
+autogluon.core==0.8.1b20230621
+autogluon.features==0.8.1b20230621
 
 [all]
-xgboost<1.8,>=1.6
 fastai<2.8,>=2.3.1
 catboost<1.3,>=1.1
-lightgbm<3.4,>=3.3
-autogluon.core[all]==0.8.1b20230620
+autogluon.core[all]==0.8.1b20230621
 torch<1.14,>=1.9
+lightgbm<3.4,>=3.3
+xgboost<1.8,>=1.6
 
 [all:sys_platform == "darwin"]
 catboost<1.2,>=1.1
 
 [catboost]
 catboost<1.3,>=1.1
 
@@ -30,15 +30,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<3.4,>=3.3
 
 [ray]
-autogluon.core[all]==0.8.1b20230620
+autogluon.core[all]==0.8.1b20230621
 
 [skex]
 scikit-learn-intelex<2023.2,>=2021.7
 
 [skl2onnx]
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
```

