# Comparing `tmp/DoubleML-0.6.1.tar.gz` & `tmp/DoubleML-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DoubleML-0.6.1.tar", last modified: Mon May  8 07:40:23 2023, max compression
+gzip compressed data, was "DoubleML-0.6.2.tar", last modified: Wed Jun 21 14:29:30 2023, max compression
```

## Comparing `DoubleML-0.6.1.tar` & `DoubleML-0.6.2.tar`

### file list

```diff
@@ -1,108 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.437108 DoubleML-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.425108 DoubleML-0.6.1/DoubleML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 07:40:23.000000 DoubleML-0.6.1/DoubleML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-08 07:39:55.000000 DoubleML-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 07:39:55.000000 DoubleML-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-08 07:40:23.437108 DoubleML-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-08 07:39:55.000000 DoubleML-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.429108 DoubleML-0.6.1/doubleml/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/_utils_resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    65216 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_blp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    37992 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_did.py
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_did_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_iivm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19981 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_irm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_lpq.py
--rw-r--r--   0 runner    (1001) docker     (123)    35461 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_pliv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_plr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16978 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_pq.py
--rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_qte.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/double_ml_score_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:40:23.437108 DoubleML-0.6.1/doubleml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_blp_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_boot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_cvar_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_did_cs_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_did_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_dml_cv_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_iivm_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_irm_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_lpq_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_x_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_xz_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_z_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_plr_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_pq_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/_utils_qte_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_blp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_cv_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_cvar_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did_cs_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_did_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_dml_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_evaluate_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    55575 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_model_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_return_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_set_ml_nuisance_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_doubleml_set_sample_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_iivm_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_irm_with_missings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_lpq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_lpq_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_multiway_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_nonlinear_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_nonlinear_score_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pliv_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_multi_treat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_reestimate_from_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_rep_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_set_ml_nuisance_pars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_set_smpls_externally.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_plr_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_pq_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-08 07:39:55.000000 DoubleML-0.6.1/doubleml/tests/test_qte.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 07:39:55.000000 DoubleML-0.6.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:40:23.437108 DoubleML-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 07:39:55.000000 DoubleML-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.087888 DoubleML-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.075888 DoubleML-0.6.2/DoubleML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-21 14:29:30.000000 DoubleML-0.6.2/DoubleML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 14:28:54.000000 DoubleML-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 14:28:54.000000 DoubleML-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-21 14:29:30.087888 DoubleML-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-21 14:28:54.000000 DoubleML-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.079888 DoubleML-0.6.2/doubleml/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47326 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83209 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_blp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37992 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26082 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_did_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22294 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_iivm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_irm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25935 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_lpq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32893 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_pliv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_plr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_pq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30882 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_qte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_score_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.087888 DoubleML-0.6.2/doubleml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_blp_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_boot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_cvar_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_did_cs_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_did_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_dml_cv_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_doubleml_sensitivtiy_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_iivm_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_irm_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_lpq_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_x_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_xz_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_z_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_plr_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pq_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_qte_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_blp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_cv_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_cvar_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did_cs_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29385 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_dml_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_evaluate_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65581 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_model_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_sensitivity_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_set_ml_nuisance_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_set_sample_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_with_missings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_lpq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_lpq_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_multiway_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_nonlinear_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_nonlinear_score_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_multi_treat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_reestimate_from_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_rep_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_set_ml_nuisance_pars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_set_smpls_externally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pq_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_qte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 14:28:54.000000 DoubleML-0.6.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:29:30.087888 DoubleML-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-21 14:28:54.000000 DoubleML-0.6.2/setup.py
```

### Comparing `DoubleML-0.6.1/DoubleML.egg-info/PKG-INFO` & `DoubleML-0.6.2/DoubleML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoubleML
-Version: 0.6.1
+Version: 0.6.2
 Summary: Double Machine Learning in Python
 Home-page: https://docs.doubleml.org
 Author: Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.
 Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Documentation, https://docs.doubleml.org
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DoubleML Version: 0.6.1 Summary: Double Machine
+Metadata-Version: 2.1 Name: DoubleML Version: 0.6.2 Summary: Double Machine
 Learning in Python Home-page: https://docs.doubleml.org Author: Bach, P.,
 Chernozhukov, V., Kurz, M. S., and Spindler, M. Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de License: UNKNOWN Project-URL:
 Documentation, https://docs.doubleml.org Project-URL: Source Code, https://
 github.com/DoubleML/doubleml-for-py Project-URL: Bug Tracker, https://
 github.com/DoubleML/doubleml-for-py/issues Description: # DoubleML - Double
 Machine Learning in Python [https://raw.githubusercontent.com/DoubleML/
```

### Comparing `DoubleML-0.6.1/DoubleML.egg-info/SOURCES.txt` & `DoubleML-0.6.2/DoubleML.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 DoubleML.egg-info/PKG-INFO
 DoubleML.egg-info/SOURCES.txt
 DoubleML.egg-info/dependency_links.txt
 DoubleML.egg-info/requires.txt
 DoubleML.egg-info/top_level.txt
 doubleml/__init__.py
 doubleml/_utils.py
+doubleml/_utils_checks.py
+doubleml/_utils_plots.py
 doubleml/_utils_resampling.py
 doubleml/datasets.py
 doubleml/double_ml.py
 doubleml/double_ml_blp.py
 doubleml/double_ml_cvar.py
 doubleml/double_ml_data.py
 doubleml/double_ml_did.py
@@ -31,14 +33,15 @@
 doubleml/tests/_utils_blp_manual.py
 doubleml/tests/_utils_boot.py
 doubleml/tests/_utils_cluster.py
 doubleml/tests/_utils_cvar_manual.py
 doubleml/tests/_utils_did_cs_manual.py
 doubleml/tests/_utils_did_manual.py
 doubleml/tests/_utils_dml_cv_predict.py
+doubleml/tests/_utils_doubleml_sensitivtiy_manual.py
 doubleml/tests/_utils_iivm_manual.py
 doubleml/tests/_utils_irm_manual.py
 doubleml/tests/_utils_lpq_manual.py
 doubleml/tests/_utils_pliv_manual.py
 doubleml/tests/_utils_pliv_partial_x_manual.py
 doubleml/tests/_utils_pliv_partial_xz_manual.py
 doubleml/tests/_utils_pliv_partial_z_manual.py
@@ -57,14 +60,16 @@
 doubleml/tests/test_did_tune.py
 doubleml/tests/test_dml_data.py
 doubleml/tests/test_doubleml_evaluate_learner.py
 doubleml/tests/test_doubleml_exceptions.py
 doubleml/tests/test_doubleml_model_defaults.py
 doubleml/tests/test_doubleml_return_types.py
 doubleml/tests/test_doubleml_scores.py
+doubleml/tests/test_doubleml_sensitivity.py
+doubleml/tests/test_doubleml_sensitivity_cluster.py
 doubleml/tests/test_doubleml_set_ml_nuisance_params.py
 doubleml/tests/test_doubleml_set_sample_splitting.py
 doubleml/tests/test_iivm.py
 doubleml/tests/test_iivm_classifier.py
 doubleml/tests/test_iivm_no_cross_fit.py
 doubleml/tests/test_iivm_subgroups.py
 doubleml/tests/test_iivm_tune.py
```

### Comparing `DoubleML-0.6.1/LICENSE` & `DoubleML-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/PKG-INFO` & `DoubleML-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoubleML
-Version: 0.6.1
+Version: 0.6.2
 Summary: Double Machine Learning in Python
 Home-page: https://docs.doubleml.org
 Author: Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.
 Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Documentation, https://docs.doubleml.org
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DoubleML Version: 0.6.1 Summary: Double Machine
+Metadata-Version: 2.1 Name: DoubleML Version: 0.6.2 Summary: Double Machine
 Learning in Python Home-page: https://docs.doubleml.org Author: Bach, P.,
 Chernozhukov, V., Kurz, M. S., and Spindler, M. Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de License: UNKNOWN Project-URL:
 Documentation, https://docs.doubleml.org Project-URL: Source Code, https://
 github.com/DoubleML/doubleml-for-py Project-URL: Bug Tracker, https://
 github.com/DoubleML/doubleml-for-py/issues Description: # DoubleML - Double
 Machine Learning in Python [https://raw.githubusercontent.com/DoubleML/
```

### Comparing `DoubleML-0.6.1/README.md` & `DoubleML-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/__init__.py` & `DoubleML-0.6.2/doubleml/__init__.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/_utils.py` & `DoubleML-0.6.2/doubleml/double_ml_cvar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,390 +1,382 @@
 import numpy as np
-import warnings
-from scipy.optimize import minimize_scalar
-
-from sklearn.model_selection import cross_val_predict
+import copy
 from sklearn.base import clone
-from sklearn.preprocessing import LabelEncoder
-from sklearn.model_selection import KFold, GridSearchCV, RandomizedSearchCV
-from sklearn.metrics import mean_squared_error
-from sklearn.utils.multiclass import type_of_target
-
-from statsmodels.nonparametric.kde import KDEUnivariate
-
-from joblib import Parallel, delayed
-
-
-def _assure_2d_array(x):
-    if x.ndim == 1:
-        x = x.reshape(-1, 1)
-    elif x.ndim > 2:
-        raise ValueError('Only one- or two-dimensional arrays are allowed')
-    return x
-
-
-def _get_cond_smpls(smpls, bin_var):
-    smpls_0 = [(np.intersect1d(np.where(bin_var == 0)[0], train), test) for train, test in smpls]
-    smpls_1 = [(np.intersect1d(np.where(bin_var == 1)[0], train), test) for train, test in smpls]
-    return smpls_0, smpls_1
-
-
-def _get_cond_smpls_2d(smpls, bin_var1, bin_var2):
-    subset_00 = (bin_var1 == 0) & (bin_var2 == 0)
-    smpls_00 = [(np.intersect1d(np.where(subset_00)[0], train), test) for train, test in smpls]
-    subset_01 = (bin_var1 == 0) & (bin_var2 == 1)
-    smpls_01 = [(np.intersect1d(np.where(subset_01)[0], train), test) for train, test in smpls]
-    subset_10 = (bin_var1 == 1) & (bin_var2 == 0)
-    smpls_10 = [(np.intersect1d(np.where(subset_10)[0], train), test) for train, test in smpls]
-    subset_11 = (bin_var1 == 1) & (bin_var2 == 1)
-    smpls_11 = [(np.intersect1d(np.where(subset_11)[0], train), test) for train, test in smpls]
-    return smpls_00, smpls_01, smpls_10, smpls_11
-
-
-def _check_is_partition(smpls, n_obs):
-    test_indices = np.concatenate([test_index for _, test_index in smpls])
-    if len(test_indices) != n_obs:
-        return False
-    hit = np.zeros(n_obs, dtype=bool)
-    hit[test_indices] = True
-    if not np.all(hit):
-        return False
-    return True
-
-
-def _check_all_smpls(all_smpls, n_obs, check_intersect=False):
-    all_smpls_checked = list()
-    for smpl in all_smpls:
-        all_smpls_checked.append(_check_smpl_split(smpl, n_obs, check_intersect))
-    return all_smpls_checked
-
-
-def _check_smpl_split(smpl, n_obs, check_intersect=False):
-    smpl_checked = list()
-    for tpl in smpl:
-        smpl_checked.append(_check_smpl_split_tpl(tpl, n_obs, check_intersect))
-    return smpl_checked
-
-
-def _check_smpl_split_tpl(tpl, n_obs, check_intersect=False):
-    train_index = np.sort(np.array(tpl[0]))
-    test_index = np.sort(np.array(tpl[1]))
-
-    if not issubclass(train_index.dtype.type, np.integer):
-        raise TypeError('Invalid sample split. Train indices must be of type integer.')
-    if not issubclass(test_index.dtype.type, np.integer):
-        raise TypeError('Invalid sample split. Test indices must be of type integer.')
-
-    if check_intersect:
-        if set(train_index) & set(test_index):
-            raise ValueError('Invalid sample split. Intersection of train and test indices is not empty.')
-
-    if len(np.unique(train_index)) != len(train_index):
-        raise ValueError('Invalid sample split. Train indices contain non-unique entries.')
-    if len(np.unique(test_index)) != len(test_index):
-        raise ValueError('Invalid sample split. Test indices contain non-unique entries.')
-
-    # we sort the indices above
-    # if not np.all(np.diff(train_index) > 0):
-    #     raise NotImplementedError('Invalid sample split. Only sorted train indices are supported.')
-    # if not np.all(np.diff(test_index) > 0):
-    #     raise NotImplementedError('Invalid sample split. Only sorted test indices are supported.')
-
-    if not set(train_index).issubset(range(n_obs)):
-        raise ValueError('Invalid sample split. Train indices must be in [0, n_obs).')
-    if not set(test_index).issubset(range(n_obs)):
-        raise ValueError('Invalid sample split. Test indices must be in [0, n_obs).')
-
-    return train_index, test_index
-
-
-def _fit(estimator, x, y, train_index, idx=None):
-    estimator.fit(x[train_index, :], y[train_index])
-    return estimator, idx
-
-
-def _dml_cv_predict(estimator, x, y, smpls=None,
-                    n_jobs=None, est_params=None, method='predict', return_train_preds=False, return_models=False):
-    n_obs = x.shape[0]
-
-    smpls_is_partition = _check_is_partition(smpls, n_obs)
-    fold_specific_params = (est_params is not None) & (not isinstance(est_params, dict))
-    fold_specific_target = isinstance(y, list)
-    manual_cv_predict = (not smpls_is_partition) | return_train_preds | fold_specific_params | fold_specific_target \
-        | return_models
-
-    res = {'models': None}
-    if not manual_cv_predict:
-        if est_params is None:
-            # if there are no parameters set we redirect to the standard method
-            preds = cross_val_predict(clone(estimator), x, y, cv=smpls, n_jobs=n_jobs, method=method)
-        else:
-            assert isinstance(est_params, dict)
-            # if no fold-specific parameters we redirect to the standard method
-            # warnings.warn("Using the same (hyper-)parameters for all folds")
-            preds = cross_val_predict(clone(estimator).set_params(**est_params), x, y, cv=smpls, n_jobs=n_jobs,
-                                      method=method)
-        if method == 'predict_proba':
-            res['preds'] = preds[:, 1]
-        else:
-            res['preds'] = preds
-        res['targets'] = np.copy(y)
-    else:
-        if not smpls_is_partition:
-            assert not fold_specific_target, 'combination of fold-specific y and no cross-fitting not implemented yet'
-            assert len(smpls) == 1
-
-        if method == 'predict_proba':
-            assert not fold_specific_target  # fold_specific_target only needed for PLIV.partialXZ
-            y = np.asarray(y)
-            le = LabelEncoder()
-            y = le.fit_transform(y)
-
-        parallel = Parallel(n_jobs=n_jobs, verbose=0, pre_dispatch='2*n_jobs')
-
-        if fold_specific_target:
-            y_list = list()
-            for idx, (train_index, _) in enumerate(smpls):
-                xx = np.full(n_obs, np.nan)
-                xx[train_index] = y[idx]
-                y_list.append(xx)
-        else:
-            # just replicate the y in a list
-            y_list = [y] * len(smpls)
-
-        if est_params is None:
-            fitted_models = parallel(delayed(_fit)(
-                clone(estimator), x, y_list[idx], train_index, idx)
-                                     for idx, (train_index, test_index) in enumerate(smpls))
-        elif isinstance(est_params, dict):
-            # warnings.warn("Using the same (hyper-)parameters for all folds")
-            fitted_models = parallel(delayed(_fit)(
-                clone(estimator).set_params(**est_params), x, y_list[idx], train_index, idx)
-                                     for idx, (train_index, test_index) in enumerate(smpls))
-        else:
-            assert len(est_params) == len(smpls), 'provide one parameter setting per fold'
-            fitted_models = parallel(delayed(_fit)(
-                clone(estimator).set_params(**est_params[idx]), x, y_list[idx], train_index, idx)
-                                     for idx, (train_index, test_index) in enumerate(smpls))
-
-        preds = np.full(n_obs, np.nan)
-        targets = np.full(n_obs, np.nan)
-        train_preds = list()
-        train_targets = list()
-        for idx, (train_index, test_index) in enumerate(smpls):
-            assert idx == fitted_models[idx][1]
-            pred_fun = getattr(fitted_models[idx][0], method)
-            if method == 'predict_proba':
-                preds[test_index] = pred_fun(x[test_index, :])[:, 1]
-            else:
-                preds[test_index] = pred_fun(x[test_index, :])
+from sklearn.utils import check_X_y
+from sklearn.model_selection import StratifiedKFold, train_test_split
 
-            if fold_specific_target:
-                # targets not available for fold specific target
-                targets = None
+from .double_ml import DoubleML
+from .double_ml_score_mixins import LinearScoreMixin
+from ._utils import _dml_cv_predict, _trimm, _predict_zero_one_propensity, \
+    _normalize_ipw, _dml_tune, _get_bracket_guess, _solve_ipw_score
+from .double_ml_data import DoubleMLData
+from ._utils_resampling import DoubleMLResampling
+from ._utils_checks import _check_score, _check_trimming, _check_zero_one_treatment, _check_treatment, \
+    _check_contains_iv, _check_quantile
+
+
+class DoubleMLCVAR(LinearScoreMixin, DoubleML):
+    """Double machine learning for conditional value at risk for potential outcomes
+
+    Parameters
+    ----------
+    obj_dml_data : :class:`DoubleMLData` object
+        The :class:`DoubleMLData` object providing the data and specifying the variables for the causal model.
+
+    ml_g : estimator implementing ``fit()`` and ``predict()``
+        A machine learner implementing ``fit()`` and ``predict()`` methods (e.g.
+        :py:class:`sklearn.ensemble.RandomForestRegressor`) for the nuisance element which depends on preliminary estimation.
+
+    ml_m : classifier implementing ``fit()`` and ``predict_proba()``
+        A machine learner implementing ``fit()`` and ``predict_proba()`` methods (e.g.
+        :py:class:`sklearn.ensemble.RandomForestClassifier`) for the nuisance function :math:`m_0(X) = E[D=d|X]`.
+
+    treatment : int
+        Binary treatment indicator. Has to be either ``0`` or ``1``. Determines the potential outcome to be considered.
+        Default is ``1``.
+
+    quantile : float
+        Quantile of the potential outcome. Has to be between ``0`` and ``1``.
+        Default is ``0.5``.
+
+    n_folds : int
+        Number of folds.
+        Default is ``5``.
+
+    n_rep : int
+        Number of repetitons for the sample splitting.
+        Default is ``1``.
+
+    score : str
+        A str (``'CVaR'`` is the only choice) specifying the score function
+        for conditional value at risk for potential outcomes.
+        Default is ``'CVaR'``.
+
+    dml_procedure : str
+        A str (``'dml1'`` or ``'dml2'``) specifying the double machine learning algorithm.
+        Default is ``'dml2'``.
+
+    normalize_ipw : bool
+        Indicates whether the inverse probability weights are normalized.
+        Default is ``True``.
+
+    trimming_rule : str
+        A str (``'truncate'`` is the only choice) specifying the trimming approach.
+        Default is ``'truncate'``.
+
+    trimming_threshold : float
+        The threshold used for trimming.
+        Default is ``1e-2``.
+
+    draw_sample_splitting : bool
+        Indicates whether the sample splitting should be drawn during initialization of the object.
+        Default is ``True``.
+
+    apply_cross_fitting : bool
+        Indicates whether cross-fitting should be applied(``True`` is the only choice).
+        Default is ``True``.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> import doubleml as dml
+    >>> from doubleml.datasets import make_irm_data
+    >>> from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+    >>> np.random.seed(3141)
+    >>> ml_g = RandomForestRegressor(n_estimators=100, max_features=20, max_depth=10, min_samples_leaf=2)
+    >>> ml_m = RandomForestClassifier(n_estimators=100, max_features=20, max_depth=10, min_samples_leaf=2)
+    >>> data = make_irm_data(theta=0.5, n_obs=500, dim_x=20, return_type='DataFrame')
+    >>> obj_dml_data = dml.DoubleMLData(data, 'y', 'd')
+    >>> dml_cvar_obj = dml.DoubleMLCVAR(obj_dml_data, ml_g, ml_m, treatment=1, quantile=0.5)
+    >>> dml_cvar_obj.fit().summary
+           coef   std err          t         P>|t|     2.5 %    97.5 %
+    d  1.591441  0.095781  16.615498  5.382582e-62  1.403715  1.779167
+    """
+
+    def __init__(self,
+                 obj_dml_data,
+                 ml_g,
+                 ml_m,
+                 treatment=1,
+                 quantile=0.5,
+                 n_folds=5,
+                 n_rep=1,
+                 score='CVaR',
+                 dml_procedure='dml2',
+                 normalize_ipw=True,
+                 trimming_rule='truncate',
+                 trimming_threshold=1e-2,
+                 draw_sample_splitting=True,
+                 apply_cross_fitting=True):
+        super().__init__(obj_dml_data,
+                         n_folds,
+                         n_rep,
+                         score,
+                         dml_procedure,
+                         draw_sample_splitting,
+                         apply_cross_fitting)
+
+        self._quantile = quantile
+        self._treatment = treatment
+        self._normalize_ipw = normalize_ipw
+
+        self._check_data(self._dml_data)
+        valid_score = ['CVaR']
+        _check_score(self.score, valid_score, allow_callable=False)
+        _check_quantile(self.quantile)
+        _check_treatment(self.treatment)
+
+        if not isinstance(self.normalize_ipw, bool):
+            raise TypeError('Normalization indicator has to be boolean. ' +
+                            f'Object of type {str(type(self.normalize_ipw))} passed.')
+
+        # initialize starting values and bounds
+        self._coef_bounds = (self._dml_data.y.min(), self._dml_data.y.max())
+        y_treat = self._dml_data.y[self._dml_data.d == self.treatment]
+        self._coef_start_val = np.mean(y_treat[y_treat >= np.quantile(y_treat, self.quantile)])
+
+        # initialize and check trimming
+        self._trimming_rule = trimming_rule
+        self._trimming_threshold = trimming_threshold
+        _check_trimming(self._trimming_rule, self._trimming_threshold)
+
+        _ = self._check_learner(ml_g, 'ml_g', regressor=True, classifier=False)
+        _ = self._check_learner(ml_m, 'ml_m', regressor=False, classifier=True)
+        self._learner = {'ml_g': clone(ml_g), 'ml_m': clone(ml_m)}
+        self._predict_method = {'ml_g': 'predict', 'ml_m': 'predict_proba'}
+
+        self._initialize_ml_nuisance_params()
+
+        if draw_sample_splitting:
+            obj_dml_resampling = DoubleMLResampling(n_folds=self.n_folds,
+                                                    n_rep=self.n_rep,
+                                                    n_obs=self._dml_data.n_obs,
+                                                    apply_cross_fitting=self.apply_cross_fitting,
+                                                    stratify=self._dml_data.d)
+            self._smpls = obj_dml_resampling.split_samples()
+
+    @property
+    def quantile(self):
+        """
+        Quantile for potential outcome.
+        """
+        return self._quantile
+
+    @property
+    def treatment(self):
+        """
+        Treatment indicator for potential outcome.
+        """
+        return self._treatment
+
+    @property
+    def normalize_ipw(self):
+        """
+        Indicates whether the inverse probability weights are normalized.
+        """
+        return self._normalize_ipw
+
+    @property
+    def trimming_rule(self):
+        """
+        Specifies the used trimming rule.
+        """
+        return self._trimming_rule
+
+    @property
+    def trimming_threshold(self):
+        """
+        Specifies the used trimming threshold.
+        """
+        return self._trimming_threshold
+
+    def _compute_ipw_score(self, theta, d, y, prop):
+        score = (d == self.treatment) / prop * (y <= theta) - self.quantile
+        return score
+
+    def _score_elements(self, y, d, g_hat, m_hat, pq_est):
+        # recalculate the target for g based on the pq_est
+        g_target_1 = np.ones_like(y) * pq_est
+        g_target_2 = (y - self.quantile * pq_est) / (1 - self.quantile)
+        g_target = np.max(np.column_stack((g_target_1, g_target_2)), 1)
+
+        psi_b = (d == self.treatment) * (g_target - g_hat) / m_hat + g_hat
+        psi_a = np.full_like(m_hat, -1.0)
+        return psi_a, psi_b
+
+    def _initialize_ml_nuisance_params(self):
+        self._params = {learner: {key: [None] * self.n_rep for key in self._dml_data.d_cols}
+                        for learner in ['ml_g', 'ml_m']}
+
+    def _nuisance_est(self, smpls, n_jobs_cv, return_models=False):
+        x, y = check_X_y(self._dml_data.x, self._dml_data.y,
+                         force_all_finite=False)
+        x, d = check_X_y(x, self._dml_data.d,
+                         force_all_finite=False)
+
+        # initialize nuisance predictions, targets and models
+        g_hat = {'models': None,
+                 'targets': np.full(shape=self._dml_data.n_obs, fill_value=np.nan),
+                 'preds': np.full(shape=self._dml_data.n_obs, fill_value=np.nan)
+                 }
+        m_hat = copy.deepcopy(g_hat)
+
+        # initialize models
+        fitted_models = {}
+        for learner in self.params_names:
+            # set nuisance model parameters
+            est_params = self._get_params(learner)
+            if est_params is not None:
+                fitted_models[learner] = [clone(self._learner[learner]).set_params(**est_params[i_fold])
+                                          for i_fold in range(self.n_folds)]
             else:
-                targets[test_index] = y[test_index]
+                fitted_models[learner] = [clone(self._learner[learner]) for i_fold in range(self.n_folds)]
+
+        ipw_vec = np.full(shape=self.n_folds, fill_value=np.nan)
+        # caculate nuisance functions over different folds
+        for i_fold in range(self.n_folds):
+            train_inds = smpls[i_fold][0]
+            test_inds = smpls[i_fold][1]
+
+            # start nested crossfitting
+            train_inds_1, train_inds_2 = train_test_split(train_inds, test_size=0.5,
+                                                          random_state=42, stratify=d[train_inds])
+            smpls_prelim = [(train, test) for train, test in
+                            StratifiedKFold(n_splits=self.n_folds).split(X=train_inds_1, y=d[train_inds_1])]
+
+            d_train_1 = d[train_inds_1]
+            y_train_1 = y[train_inds_1]
+            x_train_1 = x[train_inds_1, :]
+
+            # get a copy of ml_m as a preliminary learner
+            ml_m_prelim = clone(fitted_models['ml_m'][i_fold])
+            m_hat_prelim = _dml_cv_predict(ml_m_prelim, x_train_1, d_train_1,
+                                           method='predict_proba', smpls=smpls_prelim)['preds']
+
+            m_hat_prelim = _trimm(m_hat_prelim, self.trimming_rule, self.trimming_threshold)
+
+            if self._normalize_ipw:
+                m_hat_prelim = _normalize_ipw(m_hat_prelim, d_train_1)
+            if self.treatment == 0:
+                m_hat_prelim = 1 - m_hat_prelim
+
+            # preliminary ipw estimate
+            def ipw_score(theta):
+                res = np.mean(self._compute_ipw_score(theta, d_train_1, y_train_1, m_hat_prelim))
+                return res
+
+            _, bracket_guess = _get_bracket_guess(ipw_score, self._coef_start_val, self._coef_bounds)
+            ipw_est = _solve_ipw_score(ipw_score=ipw_score, bracket_guess=bracket_guess)
+            ipw_vec[i_fold] = ipw_est
+
+            # use the preliminary estimates to fit the nuisance parameters on train_2
+            d_train_2 = d[train_inds_2]
+            x_train_2 = x[train_inds_2, :]
+            x_test = x[test_inds, :]
+
+            # calculate the target for g
+            g_target_1 = np.ones_like(y) * ipw_est
+            g_target_2 = (y - self.quantile * ipw_est) / (1 - self.quantile)
+            g_target = np.max(np.column_stack((g_target_1, g_target_2)), 1)
+            g_target_train_2 = g_target[train_inds_2]
+
+            # only consider values with the right treatment status and fit the model
+            dx_treat_train_2 = x_train_2[d_train_2 == self.treatment, :]
+            g_target_train_2_d = g_target_train_2[d_train_2 == self.treatment]
+            fitted_models['ml_g'][i_fold].fit(dx_treat_train_2, g_target_train_2_d)
+
+            # predict nuisance values on the test data and the corresponding targets
+            g_hat['preds'][test_inds] = fitted_models['ml_g'][i_fold].predict(x_test)
+            g_hat['targets'][test_inds] = g_target[test_inds]
+
+            # refit the propensity score on the whole training set
+            fitted_models['ml_m'][i_fold].fit(x[train_inds, :], d[train_inds])
+            m_hat['preds'][test_inds] = _predict_zero_one_propensity(fitted_models['ml_m'][i_fold], x_test)
+
+        # set target for propensity score
+        m_hat['targets'] = d
+
+        # set the target for g to be a float and only relevant values
+        g_hat['targets'] = g_hat['targets'].astype(float)
+        g_hat['targets'][d != self.treatment] = np.nan
 
-            if return_train_preds:
-                train_preds.append(pred_fun(x[train_index, :]))
-                train_targets.append(y[train_index])
-
-        res['preds'] = preds
-        res['targets'] = targets
-        if return_train_preds:
-            res['train_preds'] = train_preds
-            res['train_targets'] = train_targets
         if return_models:
-            fold_ids = [xx[1] for xx in fitted_models]
-            if not np.alltrue(fold_ids == np.arange(len(smpls))):
-                raise RuntimeError('export of fitted models failed')
-            res['models'] = [xx[0] for xx in fitted_models]
-
-    return res
-
-
-def _dml_tune(y, x, train_inds,
-              learner, param_grid, scoring_method,
-              n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search):
-    tune_res = list()
-    for train_index in train_inds:
-        tune_resampling = KFold(n_splits=n_folds_tune, shuffle=True)
-        if search_mode == 'grid_search':
-            g_grid_search = GridSearchCV(learner, param_grid,
-                                         scoring=scoring_method,
-                                         cv=tune_resampling, n_jobs=n_jobs_cv)
-        else:
-            assert search_mode == 'randomized_search'
-            g_grid_search = RandomizedSearchCV(learner, param_grid,
-                                               scoring=scoring_method,
-                                               cv=tune_resampling, n_jobs=n_jobs_cv,
-                                               n_iter=n_iter_randomized_search)
-        tune_res.append(g_grid_search.fit(x[train_index, :], y[train_index]))
-
-    return tune_res
-
-
-def _draw_weights(method, n_rep_boot, n_obs):
-    if method == 'Bayes':
-        weights = np.random.exponential(scale=1.0, size=(n_rep_boot, n_obs)) - 1.
-    elif method == 'normal':
-        weights = np.random.normal(loc=0.0, scale=1.0, size=(n_rep_boot, n_obs))
-    elif method == 'wild':
-        xx = np.random.normal(loc=0.0, scale=1.0, size=(n_rep_boot, n_obs))
-        yy = np.random.normal(loc=0.0, scale=1.0, size=(n_rep_boot, n_obs))
-        weights = xx / np.sqrt(2) + (np.power(yy, 2) - 1) / 2
-    else:
-        raise ValueError('invalid boot method')
-
-    return weights
-
-
-def _check_finite_predictions(preds, learner, learner_name, smpls):
-    test_indices = np.concatenate([test_index for _, test_index in smpls])
-    if not np.all(np.isfinite(preds[test_indices])):
-        raise ValueError(f'Predictions from learner {str(learner)} for {learner_name} are not finite.')
-    return
-
-
-def _trimm(preds, trimming_rule, trimming_threshold):
-    if trimming_rule == 'truncate':
-        preds[preds < trimming_threshold] = trimming_threshold
-        preds[preds > 1 - trimming_threshold] = 1 - trimming_threshold
-    return preds
-
-
-def _normalize_ipw(propensity, treatment):
-    mean_treat1 = np.mean(np.divide(treatment, propensity))
-    mean_treat0 = np.mean(np.divide(1.0-treatment, 1.0-propensity))
-    normalized_weights = np.multiply(treatment, np.multiply(propensity, mean_treat1)) \
-        + np.multiply(1.0-treatment, 1.0 - np.multiply(1.0-propensity, mean_treat0))
-
-    return normalized_weights
-
-
-def _check_is_propensity(preds, learner, learner_name, smpls, eps=1e-12):
-    test_indices = np.concatenate([test_index for _, test_index in smpls])
-    if any((preds[test_indices] < eps) | (preds[test_indices] > 1 - eps)):
-        warnings.warn(f'Propensity predictions from learner {str(learner)} for'
-                      f' {learner_name} are close to zero or one (eps={eps}).')
-    return
-
-
-def _rmse(y_true, y_pred):
-    subset = np.logical_not(np.isnan(y_true))
-    rmse = mean_squared_error(y_true[subset], y_pred[subset], squared=False)
-    return rmse
-
-
-def _predict_zero_one_propensity(learner, X):
-    pred_proba = learner.predict_proba(X)
-    if pred_proba.shape[1] == 2:
-        res = pred_proba[:, 1]
-    else:
-        warnings.warn("Subsample has not common support. Results are based on adjusted propensities.")
-        res = learner.predict(X)
-    return res
-
-
-def _check_contains_iv(obj_dml_data):
-    if obj_dml_data.z_cols is not None:
-        raise ValueError('Incompatible data. ' +
-                         ' and '.join(obj_dml_data.z_cols) +
-                         ' have been set as instrumental variable(s). '
-                         'To fit an local model see the documentation.')
-
-
-def _check_zero_one_treatment(obj_dml):
-    one_treat = (obj_dml._dml_data.n_treat == 1)
-    binary_treat = (type_of_target(obj_dml._dml_data.d) == 'binary')
-    zero_one_treat = np.all((np.power(obj_dml._dml_data.d, 2) - obj_dml._dml_data.d) == 0)
-    if not (one_treat & binary_treat & zero_one_treat):
-        raise ValueError('Incompatible data. '
-                         f'To fit an {str(obj_dml.score)} model with DML '
-                         'exactly one binary variable with values 0 and 1 '
-                         'needs to be specified as treatment variable.')
-
-
-def _check_quantile(quantile):
-    if not isinstance(quantile, float):
-        raise TypeError('Quantile has to be a float. ' +
-                        f'Object of type {str(type(quantile))} passed.')
-
-    if (quantile <= 0) | (quantile >= 1):
-        raise ValueError('Quantile has be between 0 or 1. ' +
-                         f'Quantile {str(quantile)} passed.')
-    return
-
-
-def _check_treatment(treatment):
-    if not isinstance(treatment, int):
-        raise TypeError('Treatment indicator has to be an integer. ' +
-                        f'Object of type {str(type(treatment))} passed.')
-
-    if (treatment != 0) & (treatment != 1):
-        raise ValueError('Treatment indicator has be either 0 or 1. ' +
-                         f'Treatment indicator {str(treatment)} passed.')
-    return
-
-
-def _check_trimming(trimming_rule, trimming_threshold):
-    valid_trimming_rule = ['truncate']
-    if trimming_rule not in valid_trimming_rule:
-        raise ValueError('Invalid trimming_rule ' + str(trimming_rule) + '. ' +
-                         'Valid trimming_rule ' + ' or '.join(valid_trimming_rule) + '.')
-    if not isinstance(trimming_threshold, float):
-        raise TypeError('trimming_threshold has to be a float. ' +
-                        f'Object of type {str(type(trimming_threshold))} passed.')
-    if (trimming_threshold <= 0) | (trimming_threshold >= 0.5):
-        raise ValueError('Invalid trimming_threshold ' + str(trimming_threshold) + '. ' +
-                         'trimming_threshold has to be between 0 and 0.5.')
-    return
-
-
-def _check_score(score, valid_score, allow_callable=True):
-    if isinstance(score, str):
-        if score not in valid_score:
-            raise ValueError('Invalid score ' + score + '. ' +
-                             'Valid score ' + ' or '.join(valid_score) + '.')
-    else:
-        if allow_callable:
-            if not callable(score):
-                raise TypeError('score should be either a string or a callable. '
-                                '%r was passed.' % score)
-        else:
-            raise TypeError('score should be a string. '
-                            '%r was passed.' % score)
-    return
-
-
-def _get_bracket_guess(score, coef_start, coef_bounds):
-    max_bracket_length = coef_bounds[1] - coef_bounds[0]
-    b_guess = coef_bounds
-    delta = 0.1
-    s_different = False
-    while (not s_different) & (delta <= 1.0):
-        a = np.maximum(coef_start - delta * max_bracket_length / 2, coef_bounds[0])
-        b = np.minimum(coef_start + delta * max_bracket_length / 2, coef_bounds[1])
-        b_guess = (a, b)
-        f_a = score(b_guess[0])
-        f_b = score(b_guess[1])
-        s_different = (np.sign(f_a) != np.sign(f_b))
-        delta += 0.1
-    return s_different, b_guess
-
-
-def _default_kde(u, weights):
-    dens = KDEUnivariate(u)
-    dens.fit(kernel='gau', bw='silverman', weights=weights, fft=False)
-
-    return dens.evaluate(0)
-
-
-def _solve_ipw_score(ipw_score, bracket_guess):
-    def abs_ipw_score(theta):
-        return abs(ipw_score(theta))
-
-    res = minimize_scalar(abs_ipw_score,
-                          bracket=bracket_guess,
-                          method='brent')
-    ipw_est = res.x
-    return ipw_est
+            g_hat['models'] = fitted_models['ml_g']
+            m_hat['models'] = fitted_models['ml_m']
+
+        # clip propensities and normalize ipw weights
+        # this is not done in the score to be equivalent to PQ models
+        m_hat_adj = _trimm(m_hat['preds'], self.trimming_rule, self.trimming_threshold)
+        if self._normalize_ipw:
+            if self.dml_procedure == 'dml1':
+                for _, test_index in smpls:
+                    m_hat_adj[test_index] = _normalize_ipw(m_hat_adj[test_index], d[test_index])
+            else:
+                m_hat_adj = _normalize_ipw(m_hat_adj, d)
+
+        if self.treatment == 0:
+            m_hat_adj = 1 - m_hat_adj
+
+        # use the average of the ipw estimates to approximate the potential quantile for U (p.4 Kallus et. al)
+        pq_est = np.mean(ipw_vec)
+        psi_a, psi_b = self._score_elements(y, d, g_hat['preds'], m_hat_adj, pq_est)
+        psi_elements = {'psi_a': psi_a,
+                        'psi_b': psi_b}
+        preds = {'predictions': {'ml_g': g_hat['preds'],
+                                 'ml_m': m_hat['preds']},
+                 'targets': {'ml_g': g_hat['targets'],
+                             'ml_m': m_hat['targets']},
+                 'models': {'ml_g': g_hat['models'],
+                            'ml_m': m_hat['models']}
+                 }
+        return psi_elements, preds
+
+    def _nuisance_tuning(self, smpls, param_grids, scoring_methods, n_folds_tune, n_jobs_cv,
+                         search_mode, n_iter_randomized_search):
+        x, y = check_X_y(self._dml_data.x, self._dml_data.y,
+                         force_all_finite=False)
+        x, d = check_X_y(x, self._dml_data.d,
+                         force_all_finite=False)
+
+        if scoring_methods is None:
+            scoring_methods = {'ml_g': None,
+                               'ml_m': None}
+
+        train_inds = [train_index for (train_index, _) in smpls]
+        train_inds_treat = [np.intersect1d(np.where(d == self.treatment)[0], train) for train, _ in smpls]
+
+        # use self._coef_start_val as a very crude approximation of ipw_est
+        quantile_approx = np.quantile(y[d == self.treatment], self.quantile)
+        g_target_1 = np.ones_like(y) * quantile_approx
+        g_target_2 = (y - self.quantile * quantile_approx) / (1 - self.quantile)
+        g_target_approx = np.max(np.column_stack((g_target_1, g_target_2)), 1)
+        g_tune_res = _dml_tune(g_target_approx, x, train_inds_treat,
+                               self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
+                               n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
+
+        m_tune_res = _dml_tune(d, x, train_inds,
+                               self._learner['ml_m'], param_grids['ml_m'], scoring_methods['ml_m'],
+                               n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
+
+        g_best_params = [xx.best_params_ for xx in g_tune_res]
+        m_best_params = [xx.best_params_ for xx in m_tune_res]
+
+        params = {'ml_g': g_best_params,
+                  'ml_m': m_best_params}
+        tune_res = {'g_tune': g_tune_res,
+                    'm_tune': m_tune_res}
+
+        res = {'params': params,
+               'tune_res': tune_res}
+
+        return res
+
+    def _check_data(self, obj_dml_data):
+        if not isinstance(obj_dml_data, DoubleMLData):
+            raise TypeError('The data must be of DoubleMLData type. '
+                            f'{str(obj_dml_data)} of type {str(type(obj_dml_data))} was passed.')
+        _check_contains_iv(obj_dml_data)
+        _check_zero_one_treatment(self)
+        return
+
+    def _sensitivity_element_est(self, preds):
+        pass
```

### Comparing `DoubleML-0.6.1/doubleml/_utils_resampling.py` & `DoubleML-0.6.2/doubleml/_utils_resampling.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/datasets.py` & `DoubleML-0.6.2/doubleml/datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import numpy as np
 
 from scipy.linalg import toeplitz
+from scipy.optimize import minimize_scalar
 
 from sklearn.preprocessing import PolynomialFeatures, OneHotEncoder
 from sklearn.datasets import make_spd_matrix
 
 from .double_ml_data import DoubleMLData, DoubleMLClusterData
 
 _array_alias = ['array', 'np.ndarray', 'np.array', np.ndarray]
@@ -804,15 +805,14 @@
     def f_ps(w, xi):
         res = xi*(-w[:, 0] + 0.5*w[:, 1] - 0.25*w[:, 2] - 0.1*w[:, 3])
         return res
 
     dim_x = 4
     cov_mat = toeplitz([np.power(c, k) for k in range(dim_x)])
     x = np.random.multivariate_normal(np.zeros(dim_x), cov_mat, size=[n_obs, ])
-    # x = np.random.normal(loc=0, scale=1, size=[n_obs, 4])
 
     z_tilde_1 = np.exp(0.5*x[:, 0])
     z_tilde_2 = 10 + x[:, 1] / (1 + np.exp(x[:, 0]))
     z_tilde_3 = (0.6 + x[:, 0]*x[:, 2]/25)**3
     z_tilde_4 = (20 + x[:, 1] + x[:, 3])**2
 
     z_tilde = np.column_stack((z_tilde_1, z_tilde_2, z_tilde_3, z_tilde_4))
@@ -889,7 +889,342 @@
                                 columns=z_cols + ['y', 'd', 't'])
             if return_type in _data_frame_alias:
                 return data
             else:
                 return DoubleMLData(data, 'y', 'd', z_cols, t_col='t')
         else:
             raise ValueError('Invalid return_type.')
+
+
+def make_confounded_irm_data(n_obs=500, theta=5.0, cf_y=0.04, cf_d=0.04):
+    """
+    Generates counfounded data from an interactive regression model.
+
+    The data generating process is defined as follows (similar to the Monte Carlo simulation used
+    in Sant'Anna and Zhao (2020)).
+
+    Let :math:`X= (X_1, X_2, X_3, X_4, X_5)^T \\sim \\mathcal{N}(0, \\Sigma)`, where  :math:`\\Sigma` corresponds
+    to the identity matrix.
+    Further, define :math:`Z_j = (\\tilde{Z_j} - \\mathbb{E}[\\tilde{Z}_j]) / \\sqrt{\\text{Var}(\\tilde{Z}_j)}`,
+    where
+
+    .. math::
+
+        \\tilde{Z}_1 &= \\exp(0.5 \\cdot X_1)
+
+        \\tilde{Z}_2 &= 10 + X_2/(1 + \\exp(X_1))
+
+        \\tilde{Z}_3 &= (0.6 + X_1 \\cdot X_3 / 25)^3
+
+        \\tilde{Z}_4 &= (20 + X_2 + X_4)^2
+
+        \\tilde{Z}_5 &= X_5.
+
+    Additionally, generate a confounder :math:`A \\sim \\mathcal{U}[-1, 1]`.
+    At first, define the propensity score as
+
+    .. math::
+
+        m(X, A) = P(D=1|X,A) = 0.5 + \\gamma_A \\cdot A
+
+    and generate the treatment :math:`D = 1\\{m(X, A) \\ge U\\}` with :math:`U \\sim \\mathcal{U}[0, 1]`.
+    Since :math:`A` is independent of :math:`X`, the short form of the propensity score is given as
+
+    .. math::
+
+        P(D=1|X) = 0.5.
+
+    Further, generate the outcome of interest :math:`Y` as
+
+    .. math::
+
+        Y &= \\theta \\cdot D (Z_5 + 1) + g(Z) + \\beta_A \\cdot A + \\varepsilon
+
+        g(Z) &= 210 + 27.4 \\cdot Z_1 +13.7 \\cdot (Z_2 + Z_3 + Z_4)
+
+    where :math:`\\varepsilon \\sim \\mathcal{N}(0,5)`.
+    This implies an average treatment effect of :math:`\\theta`. Additionally, the long and short forms of
+    the conditional expectation take the following forms
+
+    .. math::
+
+        \\mathbb{E}[Y|D, X, A] &= \\theta \\cdot D (Z_5 + 1) + g(Z) + \\beta_A \\cdot A
+
+        \\mathbb{E}[Y|D, X] &= (\\theta + \\beta_A \\frac{\\mathrm{Cov}(A, D(Z_5 + 1))}{\\mathrm{Var}(D(Z_5 + 1))})
+            \\cdot D (Z_5 + 1) + g(Z).
+
+    Consequently, the strength of confounding is determined via :math:`\\gamma_A` and :math:`\\beta_A`.
+    Both are chosen to obtain the desired confounding of the outcome and Riesz Representer (in sample).
+
+    The observed data is given as :math:`W = (Y, D, X)`.
+    Further, orcale values of the confounder :math:`A`, the transformed covariated :math:`Z`,
+    the potential outcomes of :math:`Y`, the coefficients :math:`\\gamma_a`, :math:`\\beta_a`, the
+    long and short forms of the main regression and the propensity score
+    are returned in a dictionary.
+
+    Parameters
+    ----------
+    n_obs : int
+        The number of observations to simulate.
+        Default is ``500``.
+    theta : float or int
+        Average treatment effect.
+        Default is ``5.0``.
+    cf_y : float
+        Percentage of the residual variation of the outcome explained by latent/confounding variable.
+        Default is ``0.04``.
+    cf_d : float
+        Percentage gains in the variation of the Riesz Representer generated by latent/confounding variable.
+        Default is ``0.04``.
+
+    Returns
+    -------
+    res_dict : dictionary
+       Dictionary with entries ``x``, ``y``, ``d`` and ``oracle_values``.
+
+    References
+    ----------
+    Sant’Anna, P. H. and Zhao, J. (2020),
+    Doubly robust difference-in-differences estimators. Journal of Econometrics, 219(1), 101-122.
+    doi:`10.1016/j.jeconom.2020.06.003 <https://doi.org/10.1016/j.jeconom.2020.06.003>`_.
+    """
+    c = 0.0  # the confounding strength is only valid for c=0
+    dim_x = 5
+
+    # observed covariates
+    cov_mat = toeplitz([np.power(c, k) for k in range(dim_x)])
+    x = np.random.multivariate_normal(np.zeros(dim_x), cov_mat, size=[n_obs, ])
+
+    z_tilde_1 = np.exp(0.5*x[:, 0])
+    z_tilde_2 = 10 + x[:, 1] / (1 + np.exp(x[:, 0]))
+    z_tilde_3 = (0.6 + x[:, 0] * x[:, 2]/25)**3
+    z_tilde_4 = (20 + x[:, 1] + x[:, 3])**2
+
+    z_tilde = np.column_stack((z_tilde_1, z_tilde_2, z_tilde_3, z_tilde_4, x[:, 4:]))
+    z = (z_tilde - np.mean(z_tilde, axis=0)) / np.std(z_tilde, axis=0)
+
+    # error terms and unobserved confounder
+    var_eps_y = 5
+    eps_y = np.random.normal(loc=0, scale=np.sqrt(var_eps_y), size=n_obs)
+
+    # unobserved confounder
+    a_bounds = (-1, 1)
+    a = np.random.uniform(low=a_bounds[0], high=a_bounds[1], size=n_obs)
+
+    # get the required impact of the confounder on the propensity score
+    possible_coefs = np.arange(0.001, 0.4999, 0.001)
+    gamma_a = possible_coefs[(np.arctanh(2*possible_coefs) / (2*possible_coefs)) - 1 - cf_d/(1 - cf_d) >= 0][0]
+
+    # compute short and long form of riesz representer
+    m_long = 0.5 + gamma_a*a
+    m_short = 0.5 * np.ones_like(m_long)
+
+    u = np.random.uniform(low=0, high=1, size=n_obs)
+    d = 1.0 * (m_long >= u)
+
+    # short and long version of g
+    g_partial_reg = 210 + 27.4*z[:, 0] + 13.7*(z[:, 1] + z[:, 2] + z[:, 3])
+
+    dx = d * (x[:, 4] + 1)
+    d1x = x[:, 4] + 1
+    var_dx = np.var(dx)
+    cov_adx = np.cov(a, dx)[0, 1]
+
+    def f_g(beta_a):
+        g_diff = beta_a * (a - cov_adx / var_dx)
+        y_diff = eps_y + g_diff
+        return np.square(np.mean(np.square(g_diff)) / np.mean(np.square(y_diff)) - cf_y)
+    beta_a = minimize_scalar(f_g).x
+
+    g_short_d0 = g_partial_reg
+    g_short_d1 = (theta + beta_a * cov_adx / var_dx) * d1x + g_partial_reg
+    g_short = d * g_short_d1 + (1.0-d) * g_short_d0
+
+    g_long_d0 = g_partial_reg + beta_a * a
+    g_long_d1 = theta * d1x + g_partial_reg + beta_a * a
+    g_long = d * g_long_d1 + (1.0-d) * g_long_d0
+
+    y0 = g_long_d0 + eps_y
+    y1 = g_long_d1 + eps_y
+
+    y = d * y1 + (1.0-d) * y0
+
+    oracle_values = {'g_long': g_long,
+                     'g_short': g_short,
+                     'm_long': m_long,
+                     'm_short': m_short,
+                     'gamma_a': gamma_a,
+                     'beta_a': beta_a,
+                     'a': a,
+                     'y0': y0,
+                     'y1': y1,
+                     'z': z}
+
+    res_dict = {'x': x,
+                'y': y,
+                'd': d,
+                'oracle_values': oracle_values}
+
+    return res_dict
+
+
+def make_confounded_plr_data(n_obs=500, theta=5.0, cf_y=0.04, cf_d=0.04, **kwargs):
+    """
+    Generates counfounded data from an partially linear regression model.
+
+    The data generating process is defined as follows (similar to the Monte Carlo simulation used
+    in Sant'Anna and Zhao (2020)). Let :math:`X= (X_1, X_2, X_3, X_4, X_5)^T \\sim \\mathcal{N}(0, \\Sigma)`,
+    where  :math:`\\Sigma` is a matrix with entries
+    :math:`\\Sigma_{kj} = c^{|j-k|}`. The default value is  :math:`c = 0`, corresponding to the identity matrix.
+    Further, define :math:`Z_j = (\\tilde{Z_j} - \\mathbb{E}[\\tilde{Z}_j]) / \\sqrt{\\text{Var}(\\tilde{Z}_j)}`,
+    where
+
+    .. math::
+
+        \\tilde{Z}_1 &= \\exp(0.5 \\cdot X_1)
+
+        \\tilde{Z}_2 &= 10 + X_2/(1 + \\exp(X_1))
+
+        \\tilde{Z}_3 &= (0.6 + X_1 \\cdot X_3 / 25)^3
+
+        \\tilde{Z}_4 &= (20 + X_2 + X_4)^2.
+
+    Additionally, generate a confounder :math:`A \\sim \\mathcal{U}[-1, 1]`.
+    At first, define the treatment as
+
+    .. math::
+
+        D = -Z_1 + 0.5 \\cdot Z_2 - 0.25 \\cdot Z_3 - 0.1 \\cdot Z_4 + \\gamma_A \\cdot A + \\varepsilon_D
+
+    and with :math:`\\varepsilon \\sim \\mathcal{N}(0,1)`.
+    Since :math:`A` is independent of :math:`X`, the long and short form of the treatment regression are given as
+
+    .. math::
+
+        E[D|X,A] = -Z_1 + 0.5 \\cdot Z_2 - 0.25 \\cdot Z_3 - 0.1 \\cdot Z_4 + \\gamma_A \\cdot A
+
+        E[D|X] = -Z_1 + 0.5 \\cdot Z_2 - 0.25 \\cdot Z_3 - 0.1 \\cdot Z_4.
+
+    Further, generate the outcome of interest :math:`Y` as
+
+    .. math::
+
+        Y &= \\theta \\cdot D + g(Z) + \\beta_A \\cdot A + \\varepsilon
+
+        g(Z) &= 210 + 27.4 \\cdot Z_1 +13.7 \\cdot (Z_2 + Z_3 + Z_4)
+
+    where :math:`\\varepsilon \\sim \\mathcal{N}(0,5)`.
+    This implies an average treatment effect of :math:`\\theta`. Additionally, the long and short forms of
+    the conditional expectation take the following forms
+
+    .. math::
+
+        \\mathbb{E}[Y|D, X, A] &= \\theta \\cdot D + g(Z) + \\beta_A \\cdot A
+
+        \\mathbb{E}[Y|D, X] &= (\\theta + \\gamma_A\\beta_A \\frac{\\mathrm{Var}(A)}{\\mathrm{Var}(D)}) \\cdot D + g(Z).
+
+    Consequently, the strength of confounding is determined via :math:`\\gamma_A` and :math:`\\beta_A`.
+    Both are chosen to obtain the desired confounding of the outcome and Riesz Representer (in sample).
+
+    The observed data is given as :math:`W = (Y, D, X)`.
+    Further, orcale values of the confounder :math:`A`, the transformed covariated :math:`Z`, the effect :math:`\\theta`,
+    the coefficients :math:`\\gamma_a`, :math:`\\beta_a`, the long and short forms of the main regression and
+    the propensity score are returned in a dictionary.
+
+    Parameters
+    ----------
+    n_obs : int
+        The number of observations to simulate.
+        Default is ``500``.
+    theta : float or int
+        Average treatment effect.
+        Default is ``5.0``.
+    cf_y : float
+        Percentage of the residual variation of the outcome explained by latent/confounding variable.
+        Default is ``0.04``.
+    cf_d : float
+        Percentage gains in the variation of the Riesz Representer generated by latent/confounding variable.
+        Default is ``0.04``.
+
+    Returns
+    -------
+    res_dict : dictionary
+       Dictionary with entries ``x``, ``y``, ``d`` and ``oracle_values``.
+
+    References
+    ----------
+    Sant’Anna, P. H. and Zhao, J. (2020),
+    Doubly robust difference-in-differences estimators. Journal of Econometrics, 219(1), 101-122.
+    doi:`10.1016/j.jeconom.2020.06.003 <https://doi.org/10.1016/j.jeconom.2020.06.003>`_.
+    """
+    c = kwargs.get('c', 0.0)
+    dim_x = kwargs.get('dim_x', 4)
+
+    # observed covariates
+    cov_mat = toeplitz([np.power(c, k) for k in range(dim_x)])
+    x = np.random.multivariate_normal(np.zeros(dim_x), cov_mat, size=[n_obs, ])
+
+    z_tilde_1 = np.exp(0.5*x[:, 0])
+    z_tilde_2 = 10 + x[:, 1] / (1 + np.exp(x[:, 0]))
+    z_tilde_3 = (0.6 + x[:, 0] * x[:, 2]/25)**3
+    z_tilde_4 = (20 + x[:, 1] + x[:, 3])**2
+
+    z_tilde = np.column_stack((z_tilde_1, z_tilde_2, z_tilde_3, z_tilde_4, x[:, 4:]))
+    z = (z_tilde - np.mean(z_tilde, axis=0)) / np.std(z_tilde, axis=0)
+
+    # error terms
+    var_eps_y = 5
+    eps_y = np.random.normal(loc=0, scale=np.sqrt(var_eps_y), size=n_obs)
+    var_eps_d = 1
+    eps_d = np.random.normal(loc=0, scale=np.sqrt(var_eps_d), size=n_obs)
+
+    # unobserved confounder
+    a_bounds = (-1, 1)
+    a = np.random.uniform(low=a_bounds[0], high=a_bounds[1], size=n_obs)
+    var_a = np.square(a_bounds[1] - a_bounds[0]) / 12
+
+    # get the required impact of the confounder on the propensity score
+    m_short = -z[:, 0] + 0.5*z[:, 1] - 0.25*z[:, 2] - 0.1*z[:, 3]
+
+    def f_m(gamma_a):
+        rr_long = eps_d / var_eps_d
+        rr_short = (gamma_a * a + eps_d) / (gamma_a**2 * var_a + var_eps_d)
+        C2_D = (np.mean(np.square(rr_long)) - np.mean(np.square(rr_short))) / np.mean(np.square(rr_short))
+        return np.square(C2_D / (1 + C2_D) - cf_d)
+
+    gamma_a = minimize_scalar(f_m).x
+    m_long = m_short + gamma_a*a
+    d = m_long + eps_d
+
+    # short and long version of g
+    g_partial_reg = 210 + 27.4*z[:, 0] + 13.7*(z[:, 1] + z[:, 2] + z[:, 3])
+
+    var_d = np.var(d)
+
+    def f_g(beta_a):
+        g_diff = beta_a * (a - gamma_a * (var_a/var_d) * d)
+        y_diff = eps_y + g_diff
+        return np.square(np.mean(np.square(g_diff)) / np.mean(np.square(y_diff)) - cf_y)
+
+    beta_a = minimize_scalar(f_g).x
+
+    g_long = theta*d + g_partial_reg + beta_a*a
+    g_short = (theta + gamma_a*beta_a * var_a / var_d)*d + g_partial_reg
+
+    y = g_long + eps_y
+
+    oracle_values = {'g_long': g_long,
+                     'g_short': g_short,
+                     'm_long': m_long,
+                     'm_short': m_short,
+                     'theta': theta,
+                     'gamma_a': gamma_a,
+                     'beta_a': beta_a,
+                     'a': a,
+                     'z': z}
+
+    res_dict = {'x': x,
+                'y': y,
+                'd': d,
+                'oracle_values': oracle_values}
+
+    return res_dict
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml.py` & `DoubleML-0.6.2/doubleml/double_ml.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 from sklearn.base import is_regressor, is_classifier
 
 from scipy.stats import norm
 
 from statsmodels.stats.multitest import multipletests
 
 from abc import ABC, abstractmethod
+from scipy.optimize import minimize_scalar
 
 from .double_ml_data import DoubleMLBaseData, DoubleMLClusterData
+
 from ._utils_resampling import DoubleMLResampling, DoubleMLClusterResampling
-from ._utils import _check_is_partition, _check_all_smpls, _check_smpl_split, _check_smpl_split_tpl, _draw_weights, \
-    _rmse
+from ._utils import _draw_weights, _rmse, _aggregate_coefs_and_ses, _var_est
+from ._utils_checks import _check_in_zero_one, _check_integer, _check_float, _check_bool, _check_is_partition, \
+    _check_all_smpls, _check_smpl_split, _check_smpl_split_tpl
+from ._utils_plots import _sensitivity_contour_plot
 
 
 _implemented_data_backends = ['DoubleMLData', 'DoubleMLClusterData']
 
 
 class DoubleML(ABC):
     """Double Machine Learning.
@@ -50,14 +54,19 @@
         self._predictions = None
         self._nuisance_targets = None
         self._rmses = None
 
         # initialize models to None which are only stored if method fit is called with store_models=True
         self._models = None
 
+        # initialize sensitivity elements to None (only available if implemented for the class
+        self._sensitivity_implemented = False
+        self._sensitivity_elements = None
+        self._sensitivity_params = None
+
         # check resampling specifications
         if not isinstance(n_folds, int):
             raise TypeError('The number of folds must be of int type. '
                             f'{str(n_folds)} of type {str(type(n_folds))} was passed.')
         if n_folds < 1:
             raise ValueError('The number of folds must be positive. '
                              f'{str(n_folds)} was passed.')
@@ -74,15 +83,15 @@
                             f'Got {str(apply_cross_fitting)}.')
         if not isinstance(draw_sample_splitting, bool):
             raise TypeError('draw_sample_splitting must be True or False. '
                             f'Got {str(draw_sample_splitting)}.')
 
         # set resampling specifications
         if self._is_cluster_data:
-            if (n_folds == 1) | (not apply_cross_fitting):
+            if (n_folds == 1) or (not apply_cross_fitting):
                 raise NotImplementedError('No cross-fitting (`apply_cross_fitting = False`) '
                                           'is not yet implemented with clustering.')
             self._n_folds_per_cluster = n_folds
             self._n_folds = n_folds ** self._dml_data.n_cluster_vars
         else:
             self._n_folds = n_folds
         self._n_rep = n_rep
@@ -338,14 +347,32 @@
         Values of the score function components after calling :meth:`fit`;
         For models (e.g., PLR, IRM, PLIV, IIVM) with linear score (in the parameter) a dictionary with entries ``psi_a``
         and ``psi_b`` for :math:`\\psi_a(W; \\eta)` and :math:`\\psi_b(W; \\eta)`.
         """
         return self._psi_elements
 
     @property
+    def sensitivity_elements(self):
+        """
+        Values of the sensitivity components after calling :meth:`fit`;
+        If available (e.g., PLR, IRM) a dictionary with entries ``sigma2``, ``nu2``, ``psi_sigma2``
+        and ``psi_nu2``.
+        """
+        return self._sensitivity_elements
+
+    @property
+    def sensitivity_params(self):
+        """
+        Values of the sensitivity parameters after calling :meth:`sesitivity_analysis`;
+        If available (e.g., PLR, IRM) a dictionary with entries ``theta``, ``se``, ``ci``, ``rv``
+        and ``rva``.
+        """
+        return self._sensitivity_params
+
+    @property
     def coef(self):
         """
         Estimates for the causal parameter(s) after calling :meth:`fit`.
         """
         return self._coef
 
     @coef.setter
@@ -500,26 +527,30 @@
 
         if store_predictions:
             self._initialize_predictions_and_targets()
 
         if store_models:
             self._initialize_models()
 
+        if self._sensitivity_implemented:
+            self._sensitivity_elements = self._initialize_sensitivity_elements((self._dml_data.n_obs,
+                                                                                self.n_rep,
+                                                                                self._dml_data.n_coefs))
+
         for i_rep in range(self.n_rep):
             self._i_rep = i_rep
             for i_d in range(self._dml_data.n_treat):
                 self._i_treat = i_d
 
                 # this step could be skipped for the single treatment variable case
                 if self._dml_data.n_treat > 1:
                     self._dml_data.set_x_d(self._dml_data.d_cols[i_d])
 
                 # ml estimation of nuisance models and computation of score elements
                 score_elements, preds = self._nuisance_est(self.__smpls, n_jobs_cv, return_models=store_models)
-
                 self._set_score_elements(score_elements, self._i_rep, self._i_treat)
 
                 # calculate rmses and store predictions and targets of the nuisance models
                 self._calc_rmses(preds['predictions'], preds['targets'])
                 if store_predictions:
                     self._store_predictions_and_targets(preds['predictions'], preds['targets'])
                 if store_models:
@@ -540,16 +571,28 @@
                 self._psi_deriv[:, self._i_rep, self._i_treat] = self._compute_score_deriv(
                     self._get_score_elements(self._i_rep, self._i_treat),
                     self._all_coef[self._i_treat, self._i_rep])
 
                 # compute standard errors for causal parameter
                 self._all_se[self._i_treat, self._i_rep] = self._se_causal_pars()
 
+                if self._sensitivity_implemented:
+                    # not yet implemented
+                    if self._is_cluster_data or self.apply_cross_fitting:
+                        pass
+                    # check if callable score
+                    if callable(self.score):
+                        warnings.warn('Sensitivity analysis not implemented for callable scores.')
+                    else:
+                        # compute sensitivity analysis elements
+                        element_dict = self._sensitivity_element_est(preds)
+                        self._set_sensitivity_elements(element_dict, self._i_rep, self._i_treat)
+
         # aggregated parameter estimates and standard errors from repeated cross-fitting
-        self._agg_cross_fit()
+        self.coef, self.se = _aggregate_coefs_and_ses(self._all_coef, self._all_se, self._var_scaling_factor)
 
         return self
 
     def bootstrap(self, method='normal', n_rep_boot=500):
         """
         Multiplier bootstrap for DoubleML models.
 
@@ -990,18 +1033,20 @@
         else:
             if not hasattr(learner, 'predict'):
                 raise TypeError(err_msg_prefix + f'{str(learner)} has no method .predict().')
 
         return learner_is_classifier
 
     def _initialize_arrays(self):
+        # scores
         psi = np.full((self._dml_data.n_obs, self.n_rep, self._dml_data.n_coefs), np.nan)
         psi_deriv = np.full((self._dml_data.n_obs, self.n_rep, self._dml_data.n_coefs), np.nan)
         psi_elements = self._initialize_score_elements((self._dml_data.n_obs, self.n_rep, self._dml_data.n_coefs))
 
+        # coefficients and ses
         coef = np.full(self._dml_data.n_coefs, np.nan)
         se = np.full(self._dml_data.n_coefs, np.nan)
 
         all_coef = np.full((self._dml_data.n_coefs, self.n_rep), np.nan)
         all_se = np.full((self._dml_data.n_coefs, self.n_rep), np.nan)
 
         if self.dml_procedure == 'dml1':
@@ -1060,15 +1105,15 @@
             A list of strings which correspond to the nuisance functions of the model.
 
         metric : callable
             A callable function with inputs ``y_pred`` and ``y_true`` of shape ``(1, n)``,
             where ``n`` specifies the number of observations. Remark that some models like IRM are
             not able to provide all values for ``y_true`` for all learners and might contain
             some ``nan`` values in the target vector.
-            Default is the euclidean distance.
+            Default is the root-mean-square error.
 
         Returns
         -------
         dist : dict
             A dictionary containing the evaluated metric for each learner.
 
         Examples
@@ -1081,18 +1126,21 @@
         >>> np.random.seed(3141)
         >>> ml_g = RandomForestRegressor(n_estimators=100, max_features=20, max_depth=5, min_samples_leaf=2)
         >>> ml_m = RandomForestClassifier(n_estimators=100, max_features=20, max_depth=5, min_samples_leaf=2)
         >>> data = make_irm_data(theta=0.5, n_obs=500, dim_x=20, return_type='DataFrame')
         >>> obj_dml_data = dml.DoubleMLData(data, 'y', 'd')
         >>> dml_irm_obj = dml.DoubleMLIRM(obj_dml_data, ml_g, ml_m)
         >>> dml_irm_obj.fit()
-        >>> dml_irm_obj.evaluate_learners(metric=mean_absolute_error)
-        {'ml_g0': array([[1.13318973]]),
-         'ml_g1': array([[0.91659939]]),
-         'ml_m': array([[0.36350912]])}
+        >>> def mae(y_true, y_pred):
+        >>>     subset = np.logical_not(np.isnan(y_true))
+        >>>     return mean_absolute_error(y_true[subset], y_pred[subset])
+        >>> dml_irm_obj.evaluate_learners(metric=mae)
+        {'ml_g0': array([[0.85974356]]),
+         'ml_g1': array([[0.85280376]]),
+         'ml_m': array([[0.35365143]])}
         """
         # if no learners are provided try to evaluate all learners
         if learners is None:
             learners = self.params_names
 
         # check metric
         if not callable(metric):
@@ -1322,33 +1370,37 @@
                     scaling_factor[i_fold] = 1./np.prod(np.array([len(inds) for inds in test_cluster_inds]))
                 coef = self._est_coef(psi_elements, smpls=smpls, scaling_factor=scaling_factor)
 
         return coef, dml1_coefs
 
     def _se_causal_pars(self):
         if not self._is_cluster_data:
-            se = np.sqrt(self._var_est())
+            cluster_vars = None
+            smpls_cluster = None
+            n_folds_per_cluster = None
+
         else:
-            se = np.sqrt(self._var_est_cluster_data())
+            cluster_vars = self._dml_data.cluster_vars
+            smpls_cluster = self.__smpls_cluster
+            n_folds_per_cluster = self._n_folds_per_cluster
+
+        sigma2_hat, var_scaling_factor = _var_est(psi=self.__psi,
+                                                  psi_deriv=self.__psi_deriv,
+                                                  apply_cross_fitting=self.apply_cross_fitting,
+                                                  smpls=self.__smpls,
+                                                  is_cluster_data=self._is_cluster_data,
+                                                  cluster_vars=cluster_vars,
+                                                  smpls_cluster=smpls_cluster,
+                                                  n_folds_per_cluster=n_folds_per_cluster)
 
+        self._var_scaling_factor = var_scaling_factor
+        se = np.sqrt(sigma2_hat)
         return se
 
-    def _agg_cross_fit(self):
-        # aggregate parameters from the repeated cross-fitting
-        # don't use the getter (always for one treatment variable and one sample), but the private variable
-        self.coef = np.median(self._all_coef, 1)
-
-        # TODO: In the documentation of standard errors we need to cleary state what we return here, i.e.,
-        #  the asymptotic variance sigma_hat/N and not sigma_hat (which sometimes is also called the asympt var)!
-        # TODO: In the edge case of repeated no-cross-fitting, the test sets might have different size and therefore
-        #  it would note be valid to always use the same self._var_scaling_factor
-        xx = np.tile(self.coef.reshape(-1, 1), self.n_rep)
-        self.se = np.sqrt(np.divide(np.median(np.multiply(np.power(self._all_se, 2), self._var_scaling_factor) +
-                                              np.power(self._all_coef - xx, 2), 1), self._var_scaling_factor))
-
+    # to estimate causal parameters without predictions
     def _est_causal_pars_and_se(self):
         for i_rep in range(self.n_rep):
             self._i_rep = i_rep
             for i_d in range(self._dml_data.n_treat):
                 self._i_treat = i_d
 
                 # estimate the causal parameter
@@ -1366,16 +1418,16 @@
                 self._psi_deriv[:, self._i_rep, self._i_treat] = self._compute_score_deriv(
                     self._get_score_elements(self._i_rep, self._i_treat),
                     self._all_coef[self._i_treat, self._i_rep])
 
                 # compute standard errors for causal parameter
                 self._all_se[self._i_treat, self._i_rep] = self._se_causal_pars()
 
-            # aggregated parameter estimates and standard errors from repeated cross-fitting
-        self._agg_cross_fit()
+        # aggregated parameter estimates and standard errors from repeated cross-fitting
+        self.coef, self.se = _aggregate_coefs_and_ses(self._all_coef, self._all_se, self._var_scaling_factor)
 
     def _compute_bootstrap(self, weights):
         if self.apply_cross_fitting:
             J = np.mean(self.__psi_deriv)
             boot_coef = np.matmul(weights, self.__psi) / (self._dml_data.n_obs * J)
             boot_t_stat = np.matmul(weights, self.__psi) / (self._dml_data.n_obs * self.__all_se * J)
 
@@ -1385,87 +1437,15 @@
             test_index = smpls[0][1]
             J = np.mean(self.__psi_deriv[test_index])
             boot_coef = np.matmul(weights, self.__psi[test_index]) / (len(test_index) * J)
             boot_t_stat = np.matmul(weights, self.__psi[test_index]) / (len(test_index) * self.__all_se * J)
 
         return boot_coef, boot_t_stat
 
-    def _var_est(self):
-        """
-        Estimate the standard errors of the structural parameter
-        """
-        psi_deriv = self.__psi_deriv
-        psi = self.__psi
-
-        if self.apply_cross_fitting:
-            self._var_scaling_factor = self._dml_data.n_obs
-        else:
-            # In case of no-cross-fitting, the score function was only evaluated on the test data set
-            smpls = self.__smpls
-            test_index = smpls[0][1]
-            psi_deriv = psi_deriv[test_index]
-            psi = psi[test_index]
-            self._var_scaling_factor = len(test_index)
-
-        J = np.mean(psi_deriv)
-        sigma2_hat = 1 / self._var_scaling_factor * np.mean(np.power(psi, 2)) / np.power(J, 2)
-
-        return sigma2_hat
-
-    def _var_est_cluster_data(self):
-        psi_deriv = self.__psi_deriv
-        psi = self.__psi
-
-        if self._dml_data.n_cluster_vars == 1:
-            this_cluster_var = self._dml_data.cluster_vars[:, 0]
-            clusters = np.unique(this_cluster_var)
-            gamma_hat = 0
-            j_hat = 0
-            for i_fold in range(self.n_folds):
-                test_inds = self.__smpls[i_fold][1]
-                test_cluster_inds = self.__smpls_cluster[i_fold][1]
-                I_k = test_cluster_inds[0]
-                const = 1 / len(I_k)
-                for cluster_value in I_k:
-                    ind_cluster = (this_cluster_var == cluster_value)
-                    gamma_hat += const * np.sum(np.outer(psi[ind_cluster], psi[ind_cluster]))
-                j_hat += np.sum(psi_deriv[test_inds]) / len(I_k)
-
-            gamma_hat = gamma_hat / self._n_folds_per_cluster
-            j_hat = j_hat / self._n_folds_per_cluster
-            self._var_scaling_factor = len(clusters)
-            sigma2_hat = gamma_hat / (j_hat ** 2) / self._var_scaling_factor
-        else:
-            assert self._dml_data.n_cluster_vars == 2
-            first_cluster_var = self._dml_data.cluster_vars[:, 0]
-            second_cluster_var = self._dml_data.cluster_vars[:, 1]
-            gamma_hat = 0
-            j_hat = 0
-            for i_fold in range(self.n_folds):
-                test_inds = self.__smpls[i_fold][1]
-                test_cluster_inds = self.__smpls_cluster[i_fold][1]
-                I_k = test_cluster_inds[0]
-                J_l = test_cluster_inds[1]
-                const = min(len(I_k), len(J_l)) / ((len(I_k) * len(J_l)) ** 2)
-                for cluster_value in I_k:
-                    ind_cluster = (first_cluster_var == cluster_value) & np.in1d(second_cluster_var, J_l)
-                    gamma_hat += const * np.sum(np.outer(psi[ind_cluster], psi[ind_cluster]))
-                for cluster_value in J_l:
-                    ind_cluster = (second_cluster_var == cluster_value) & np.in1d(first_cluster_var, I_k)
-                    gamma_hat += const * np.sum(np.outer(psi[ind_cluster], psi[ind_cluster]))
-                j_hat += np.sum(psi_deriv[test_inds]) / (len(I_k) * len(J_l))
-            gamma_hat = gamma_hat / (self._n_folds_per_cluster ** 2)
-            j_hat = j_hat / (self._n_folds_per_cluster ** 2)
-            n_first_clusters = len(np.unique(first_cluster_var))
-            n_second_clusters = len(np.unique(second_cluster_var))
-            self._var_scaling_factor = min(n_first_clusters, n_second_clusters)
-            sigma2_hat = gamma_hat / (j_hat ** 2) / self._var_scaling_factor
-
-        return sigma2_hat
-
+    # Score estimation and elements
     @abstractmethod
     def _est_coef(self, psi_elements, smpls=None, scaling_factor=None, inds=None):
         pass
 
     @property
     @abstractmethod
     def _score_element_names(self):
@@ -1494,7 +1474,378 @@
         for key in self._score_element_names:
             self.psi_elements[key][:, i_rep, i_treat] = psi_elements[key]
         return
 
     def _initialize_score_elements(self, score_dim):
         psi_elements = {key: np.full(score_dim, np.nan) for key in self._score_element_names}
         return psi_elements
+
+    # Sensitivity estimation and elements
+    @abstractmethod
+    def _sensitivity_element_est(self, preds):
+        pass
+
+    @property
+    def _sensitivity_element_names(self):
+        return ['sigma2', 'nu2', 'psi_sigma2', 'psi_nu2']
+
+    # the dimensions will usually be (n_obs, n_rep, n_coefs) to be equal to the score dimensions psi
+    def _initialize_sensitivity_elements(self, score_dim):
+        sensitivity_elements = {'sigma2': np.full((1, score_dim[1], score_dim[2]), np.nan),
+                                'nu2': np.full((1, score_dim[1], score_dim[2]), np.nan),
+                                'psi_sigma2': np.full(score_dim, np.nan),
+                                'psi_nu2': np.full(score_dim, np.nan)}
+        return sensitivity_elements
+
+    def _get_sensitivity_elements(self, i_rep, i_treat):
+        sensitivity_elements = {key: value[:, i_rep, i_treat] for key, value in self.sensitivity_elements.items()}
+        return sensitivity_elements
+
+    def _set_sensitivity_elements(self, sensitivity_elements, i_rep, i_treat):
+        if not isinstance(sensitivity_elements, dict):
+            raise TypeError('_sensitivity_element_est must return sensitivity elements in a dict. '
+                            f'Got type {str(type(sensitivity_elements))}.')
+        if not (set(self._sensitivity_element_names) == set(sensitivity_elements.keys())):
+            raise ValueError('_sensitivity_element_est returned incomplete sensitivity elements. '
+                             'Expected dict with keys: ' + ' and '.join(set(self._sensitivity_element_names)) + '. '
+                             'Got dict with keys: ' + ' and '.join(set(sensitivity_elements.keys())) + '.')
+        for key in self._sensitivity_element_names:
+            self.sensitivity_elements[key][:, i_rep, i_treat] = sensitivity_elements[key]
+        return
+
+    def _calc_sensitivity_analysis(self, cf_y, cf_d, rho, level):
+        if not self.apply_cross_fitting:
+            raise NotImplementedError('Sensitivity analysis not yet implemented without cross-fitting.')
+        if self._sensitivity_elements is None:
+            raise NotImplementedError(f'Sensitivity analysis not yet implemented for {str(type(self))}.')
+
+        # checks
+        _check_in_zero_one(cf_y, 'cf_y', include_one=False)
+        _check_in_zero_one(cf_d, 'cf_d', include_one=False)
+        if not isinstance(rho, float):
+            raise TypeError(f'rho must be of float type. '
+                            f'{str(rho)} of type {str(type(rho))} was passed.')
+        _check_in_zero_one(abs(rho), 'The absolute value of rho')
+        _check_in_zero_one(level, 'The confidence level', include_zero=False, include_one=False)
+
+        # set elements for readability
+        sigma2 = self.sensitivity_elements['sigma2']
+        nu2 = self.sensitivity_elements['nu2']
+        psi_sigma = self.sensitivity_elements['psi_sigma2']
+        psi_nu = self.sensitivity_elements['psi_nu2']
+        psi_scaled = np.divide(self.psi, np.mean(self.psi_deriv, axis=0))
+
+        if (np.any(sigma2 < 0)) | (np.any(nu2 < 0)):
+            raise ValueError('sensitivity_elements sigma2 and nu2 have to be positive. '
+                             f"Got sigma2 {str(sigma2)} and nu2 {str(nu2)}. "
+                             'Most likely this is due to low quality learners (especially propensity scores).')
+
+        # elementwise operations
+        confounding_strength = np.multiply(np.abs(rho), np.sqrt(np.multiply(cf_y, np.divide(cf_d, 1.0-cf_d))))
+        S = np.sqrt(np.multiply(sigma2, nu2))
+
+        # sigma2 and nu2 are of shape (1, n_rep, n_coefs), whereas the all_coefs is of shape (n_coefs, n_reps)
+        all_theta_lower = self.all_coef - np.multiply(np.transpose(np.squeeze(S, axis=0)), confounding_strength)
+        all_theta_upper = self.all_coef + np.multiply(np.transpose(np.squeeze(S, axis=0)), confounding_strength)
+
+        psi_S2 = np.multiply(sigma2, psi_nu) + np.multiply(nu2, psi_sigma)
+        psi_bias = np.multiply(np.divide(confounding_strength, np.multiply(2.0, S)), psi_S2)
+        psi_lower = psi_scaled - psi_bias
+        psi_upper = psi_scaled + psi_bias
+
+        # transpose to obtain shape (n_coefs, n_reps); includes scaling with n^{-1/2}
+        all_sigma_lower = np.full_like(all_theta_lower, fill_value=np.nan)
+        all_sigma_upper = np.full_like(all_theta_upper, fill_value=np.nan)
+        for i_rep in range(self.n_rep):
+            self._i_rep = i_rep
+            for i_d in range(self._dml_data.n_treat):
+                self._i_treat = i_d
+
+                if not self._is_cluster_data:
+                    cluster_vars = None
+                    smpls_cluster = None
+                    n_folds_per_cluster = None
+                else:
+                    cluster_vars = self._dml_data.cluster_vars
+                    smpls_cluster = self.__smpls_cluster
+                    n_folds_per_cluster = self._n_folds_per_cluster
+
+                sigma2_lower_hat, _ = _var_est(psi=psi_lower[:, i_rep, i_d],
+                                               psi_deriv=np.ones_like(psi_lower[:, i_rep, i_d]),
+                                               apply_cross_fitting=self.apply_cross_fitting,
+                                               smpls=self.__smpls,
+                                               is_cluster_data=self._is_cluster_data,
+                                               cluster_vars=cluster_vars,
+                                               smpls_cluster=smpls_cluster,
+                                               n_folds_per_cluster=n_folds_per_cluster)
+                sigma2_upper_hat, _ = _var_est(psi=psi_upper[:, i_rep, i_d],
+                                               psi_deriv=np.ones_like(psi_upper[:, i_rep, i_d]),
+                                               apply_cross_fitting=self.apply_cross_fitting,
+                                               smpls=self.__smpls,
+                                               is_cluster_data=self._is_cluster_data,
+                                               cluster_vars=cluster_vars,
+                                               smpls_cluster=smpls_cluster,
+                                               n_folds_per_cluster=n_folds_per_cluster)
+
+                all_sigma_lower[self._i_treat, self._i_rep] = np.sqrt(sigma2_lower_hat)
+                all_sigma_upper[self._i_treat, self._i_rep] = np.sqrt(sigma2_upper_hat)
+
+        # aggregate coefs and ses over n_rep
+        theta_lower, sigma_lower = _aggregate_coefs_and_ses(all_theta_lower, all_sigma_lower, self._var_scaling_factor)
+        theta_upper, sigma_upper = _aggregate_coefs_and_ses(all_theta_upper, all_sigma_upper, self._var_scaling_factor)
+
+        quant = norm.ppf(level)
+        ci_lower = theta_lower - np.multiply(quant, sigma_lower)
+        ci_upper = theta_upper + np.multiply(quant, sigma_upper)
+
+        theta_dict = {'lower': theta_lower,
+                      'upper': theta_upper}
+
+        se_dict = {'lower': sigma_lower,
+                   'upper': sigma_upper}
+
+        ci_dict = {'lower': ci_lower,
+                   'upper': ci_upper}
+
+        res_dict = {'theta': theta_dict,
+                    'se': se_dict,
+                    'ci': ci_dict}
+
+        return res_dict
+
+    def _calc_robustness_value(self, null_hypothesis, level, rho, idx_treatment):
+        _check_float(null_hypothesis, "null_hypothesis")
+        _check_integer(idx_treatment, "idx_treatment", lower_bound=0, upper_bound=self._dml_data.n_treat-1)
+
+        # check which side is relvant
+        bound = 'upper' if (null_hypothesis > self.coef[idx_treatment]) else 'lower'
+
+        # minimize the square to find boundary solutions
+        def rv_fct(value, param):
+            res = self._calc_sensitivity_analysis(cf_y=value,
+                                                  cf_d=value,
+                                                  rho=rho,
+                                                  level=level)[param][bound][idx_treatment] - null_hypothesis
+            return np.square(res)
+
+        rv = minimize_scalar(rv_fct, bounds=(0, 0.9999), method='bounded', args=('theta', )).x
+        rva = minimize_scalar(rv_fct, bounds=(0, 0.9999), method='bounded', args=('ci', )).x
+
+        return rv, rva
+
+    def sensitivity_analysis(self, cf_y=0.03, cf_d=0.03, rho=1.0, level=0.95, null_hypothesis=0.0):
+        """
+        Performs a sensitivity analysis to account for unobserved confounders.
+
+        The evaluated scenario is stored as a dictionary in the property ``sensitivity_params``.
+
+        Parameters
+        ----------
+        cf_y : float
+            Percentage of the residual variation of the outcome explained by latent/confounding variables.
+            Default is ``0.03``.
+
+        cf_d : float
+            Percentage gains in the variation of the Riesz representer generated by latent/confounding variables.
+            Default is ``0.03``.
+
+        rho : float
+            The correlation between the differences in short and long representations in the main regression and
+            Riesz representer. Has to be in [-1,1]. The absolute value determines the adversarial strength of the
+            confounding (maximizes at 1.0).
+            Default is ``1.0``.
+
+        level : float
+            The confidence level.
+            Default is ``0.95``.
+
+        null_hypothesis : float or numpy.ndarray
+            Null hypothesis for the effect. Determines the robustness values.
+            If it is a single float uses the same null hypothesis for all estimated parameters.
+            Else the array has to be of shape (n_coefs,).
+            Default is ``0.0``.
+
+        Returns
+        -------
+        self : object
+        """
+        # compute sensitivity analysis
+        sensitivity_dict = self._calc_sensitivity_analysis(cf_y=cf_y, cf_d=cf_d, rho=rho, level=level)
+
+        if isinstance(null_hypothesis, float):
+            null_hypothesis_vec = np.full(shape=self._dml_data.n_treat, fill_value=null_hypothesis)
+        elif isinstance(null_hypothesis, np.ndarray):
+            if null_hypothesis.shape == (self._dml_data.n_treat,):
+                null_hypothesis_vec = null_hypothesis
+            else:
+                raise ValueError("null_hypothesis is numpy.ndarray but does not have the required "
+                                 f"shape ({self._dml_data.n_treat},). "
+                                 f'Array of shape {str(null_hypothesis.shape)} was passed.')
+        else:
+            raise TypeError("null_hypothesis has to be of type float or np.ndarry. "
+                            f"{str(null_hypothesis)} of type {str(type(null_hypothesis))} was passed.")
+
+        # compute robustess values with respect to null_hypothesis
+        rv = np.full(shape=self._dml_data.n_treat, fill_value=np.nan)
+        rva = np.full(shape=self._dml_data.n_treat, fill_value=np.nan)
+
+        for i_treat in range(self._dml_data.n_treat):
+            rv[i_treat], rva[i_treat] = self._calc_robustness_value(null_hypothesis=null_hypothesis_vec[i_treat],
+                                                                    level=level, rho=rho, idx_treatment=i_treat)
+
+        sensitivity_dict['rv'] = rv
+        sensitivity_dict['rva'] = rva
+
+        # add all input parameters
+        input_params = {'cf_y': cf_y,
+                        'cf_d': cf_d,
+                        'rho': rho,
+                        'level': level,
+                        'null_hypothesis': null_hypothesis_vec}
+        sensitivity_dict['input'] = input_params
+
+        self._sensitivity_params = sensitivity_dict
+        return self
+
+    @property
+    def sensitivity_summary(self):
+        """
+        Returns a summary for the sensitivity analysis after calling :meth:`sensitivity_analysis`.
+
+        Returns
+        -------
+        res : str
+            Summary for the sensitivity analysis.
+        """
+        header = '================== Sensitivity Analysis ==================\n'
+        if self.sensitivity_params is None:
+            res = header + 'Apply sensitivity_analysis() to generate sensitivity_summary.'
+        else:
+            sig_level = f'Significance Level: level={self.sensitivity_params["input"]["level"]}\n'
+            scenario_params = f'Sensitivity parameters: cf_y={self.sensitivity_params["input"]["cf_y"]}; ' \
+                              f'cf_d={self.sensitivity_params["input"]["cf_d"]}, ' \
+                              f'rho={self.sensitivity_params["input"]["rho"]}'
+
+            theta_and_ci_col_names = ['CI lower', 'theta lower', ' theta', 'theta upper', 'CI upper']
+            theta_and_ci = np.transpose(np.vstack((self._sensitivity_params['ci']['lower'],
+                                                   self._sensitivity_params['theta']['lower'],
+                                                   self.coef,
+                                                   self._sensitivity_params['theta']['upper'],
+                                                   self._sensitivity_params['ci']['upper'])))
+            df_theta_and_ci = pd.DataFrame(theta_and_ci,
+                                           columns=theta_and_ci_col_names,
+                                           index=self._dml_data.d_cols)
+            theta_and_ci_summary = str(df_theta_and_ci)
+
+            rvs_col_names = ['H_0', 'RV (%)', 'RVa (%)']
+            rvs = np.transpose(np.vstack((self._sensitivity_params['rv'],
+                                          self._sensitivity_params['rva']))) * 100
+
+            df_rvs = pd.DataFrame(np.column_stack((self.sensitivity_params["input"]["null_hypothesis"], rvs)),
+                                  columns=rvs_col_names,
+                                  index=self._dml_data.d_cols)
+            rvs_summary = str(df_rvs)
+
+            res = header + \
+                '\n------------------ Scenario          ------------------\n' + \
+                sig_level + scenario_params + '\n' + \
+                '\n------------------ Bounds with CI    ------------------\n' + \
+                theta_and_ci_summary + '\n' + \
+                '\n------------------ Robustness Values ------------------\n' + \
+                rvs_summary
+
+        return res
+
+    def sensitivity_plot(self, idx_treatment=0, value='theta', include_scenario=True,
+                         fill=True, grid_bounds=(0.15, 0.15), grid_size=100):
+        """
+        Contour plot of the sensivity with respect to latent/confounding variables.
+
+        Parameters
+        ----------
+        idx_treatment : int
+            Index of the treatment to perform the sensitivity analysis.
+            Default is ``0``.
+
+        value : str
+            Determines which contours to plot. Valid values are ``'theta'`` (refers to the bounds)
+            and ``'ci'`` (refers to the bounds including statistical uncertainty).
+            Default is ``'theta'``.
+
+        include_scenario : bool
+            Indicates whether to highlight the scenario from the call of :meth:`sensitivity_analysis`.
+            Default is ``True``.
+
+        fill : bool
+            Indicates whether to use a heatmap style or only contour lines.
+            Default is ``True``.
+
+        grid_bounds : tuple
+            Determines the evaluation bounds of the grid for ``cf_d`` and ``cf_y``. Has to contain two floats in [0, 1).
+            Default is ``(0.15, 0.15)``.
+
+        grid_size : int
+            Determines the number of evaluation points of the grid.
+            Default is ``100``.
+
+        Returns
+        -------
+        fig : object
+            Plotly figure of the sensitivity contours.
+        """
+        if self.sensitivity_params is None:
+            raise ValueError('Apply sensitivity_analysis() to include senario in sensitivity_plot. '
+                             'The values of rho and the level are used for the scenario.')
+        _check_integer(idx_treatment, "idx_treatment", lower_bound=0, upper_bound=self._dml_data.n_treat-1)
+        if not isinstance(value, str):
+            raise TypeError('value must be a string. '
+                            f'{str(value)} of type {type(value)} was passed.')
+        valid_values = ['theta', 'ci']
+        if value not in valid_values:
+            raise ValueError('Invalid value ' + value + '. ' +
+                             'Valid values ' + ' or '.join(valid_values) + '.')
+        _check_bool(include_scenario, 'include_scenario')
+        _check_bool(fill, 'fill')
+        _check_in_zero_one(grid_bounds[0], "grid_bounds", include_zero=False, include_one=False)
+        _check_in_zero_one(grid_bounds[1], "grid_bounds", include_zero=False, include_one=False)
+        _check_integer(grid_size, "grid_size", lower_bound=10)
+
+        null_hypothesis = self.sensitivity_params['input']['null_hypothesis'][idx_treatment]
+        unadjusted_theta = self.coef[idx_treatment]
+        # check which side is relvant
+        bound = 'upper' if (null_hypothesis > unadjusted_theta) else 'lower'
+
+        # create evaluation grid
+        cf_d_vec = np.linspace(0, grid_bounds[0], grid_size)
+        cf_y_vec = np.linspace(0, grid_bounds[1], grid_size)
+
+        # compute contour values
+        contour_values = np.full(shape=(grid_size, grid_size), fill_value=np.nan)
+        for i_cf_d_grid, cf_d_grid in enumerate(cf_d_vec):
+            for i_cf_y_grid, cf_y_grid in enumerate(cf_y_vec):
+                sens_dict = self._calc_sensitivity_analysis(cf_y=cf_y_grid,
+                                                            cf_d=cf_d_grid,
+                                                            rho=self.sensitivity_params['input']['rho'],
+                                                            level=self.sensitivity_params['input']['level'])
+                contour_values[i_cf_d_grid, i_cf_y_grid] = sens_dict[value][bound][idx_treatment]
+
+        # get the correct unadjusted value for confidence bands
+        if value == 'theta':
+            unadjusted_value = unadjusted_theta
+        else:
+            assert value == 'ci'
+            ci = self.confint(level=self.sensitivity_params['input']['level'])
+            if bound == 'upper':
+                unadjusted_value = ci.iloc[idx_treatment, 1]
+            else:
+                unadjusted_value = ci.iloc[idx_treatment, 0]
+
+        fig = _sensitivity_contour_plot(x=cf_d_vec,
+                                        y=cf_y_vec,
+                                        contour_values=contour_values,
+                                        unadjusted_value=unadjusted_value,
+                                        scenario_x=self.sensitivity_params['input']['cf_d'],
+                                        scenario_y=self.sensitivity_params['input']['cf_y'],
+                                        scenario_value=self.sensitivity_params[value][bound][idx_treatment],
+                                        include_scenario=include_scenario,
+                                        fill=fill)
+        return fig
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_blp.py` & `DoubleML-0.6.2/doubleml/double_ml_blp.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/double_ml_cvar.py` & `DoubleML-0.6.2/doubleml/double_ml_pq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import numpy as np
 import copy
 from sklearn.base import clone
 from sklearn.utils import check_X_y
 from sklearn.model_selection import StratifiedKFold, train_test_split
 
 from .double_ml import DoubleML
-from .double_ml_score_mixins import LinearScoreMixin
-from ._utils import _dml_cv_predict, _trimm, _predict_zero_one_propensity, _check_contains_iv, \
-    _check_zero_one_treatment, _check_quantile, _check_treatment, _check_trimming, _check_score, \
-    _normalize_ipw, _dml_tune, _get_bracket_guess, _solve_ipw_score
+from .double_ml_score_mixins import NonLinearScoreMixin
 from .double_ml_data import DoubleMLData
+
+from ._utils import _dml_cv_predict, _trimm, _predict_zero_one_propensity, _get_bracket_guess, \
+    _default_kde, _normalize_ipw, _dml_tune, _solve_ipw_score
 from ._utils_resampling import DoubleMLResampling
+from ._utils_checks import _check_score, _check_trimming, _check_zero_one_treatment, _check_treatment, \
+    _check_contains_iv, _check_quantile
 
 
-class DoubleMLCVAR(LinearScoreMixin, DoubleML):
-    """Double machine learning for conditional value at risk for potential outcomes
+class DoubleMLPQ(NonLinearScoreMixin, DoubleML):
+    """Double machine learning for potential quantiles
 
     Parameters
     ----------
     obj_dml_data : :class:`DoubleMLData` object
         The :class:`DoubleMLData` object providing the data and specifying the variables for the causal model.
 
-    ml_g : estimator implementing ``fit()`` and ``predict()``
-        A machine learner implementing ``fit()`` and ``predict()`` methods (e.g.
-        :py:class:`sklearn.ensemble.RandomForestRegressor`) for the nuisance element which depends on preliminary estimation.
+    ml_g : classifier implementing ``fit()`` and ``predict()``
+        A machine learner implementing ``fit()`` and ``predict_proba()`` methods (e.g.
+        :py:class:`sklearn.ensemble.RandomForestClassifier`) for the nuisance function
+        :math:`g_0(X) = E[Y <= \\theta | X, D=d]` .
 
     ml_m : classifier implementing ``fit()`` and ``predict_proba()``
         A machine learner implementing ``fit()`` and ``predict_proba()`` methods (e.g.
         :py:class:`sklearn.ensemble.RandomForestClassifier`) for the nuisance function :math:`m_0(X) = E[D=d|X]`.
 
     treatment : int
         Binary treatment indicator. Has to be either ``0`` or ``1``. Determines the potential outcome to be considered.
@@ -42,26 +45,32 @@
         Default is ``5``.
 
     n_rep : int
         Number of repetitons for the sample splitting.
         Default is ``1``.
 
     score : str
-        A str (``'CVaR'`` is the only choice) specifying the score function
-        for conditional value at risk for potential outcomes.
-        Default is ``'CVaR'``.
+        A str (``'PQ'`` is the only choice) specifying the score function
+        for potential quantiles.
+        Default is ``'PQ'``.
 
     dml_procedure : str
         A str (``'dml1'`` or ``'dml2'``) specifying the double machine learning algorithm.
         Default is ``'dml2'``.
 
     normalize_ipw : bool
         Indicates whether the inverse probability weights are normalized.
         Default is ``True``.
 
+    kde : callable or None
+        A callable object / function with signature ``deriv = kde(u, weights)`` for weighted kernel density estimation.
+        Here ``deriv`` should evaluate the density in ``0``.
+        Default is ``'None'``, which uses :py:class:`statsmodels.nonparametric.kde.KDEUnivariate` with a
+        gaussian kernel and silverman for bandwidth determination.
+
     trimming_rule : str
         A str (``'truncate'`` is the only choice) specifying the trimming approach.
         Default is ``'truncate'``.
 
     trimming_threshold : float
         The threshold used for trimming.
         Default is ``1e-2``.
@@ -75,77 +84,85 @@
         Default is ``True``.
 
     Examples
     --------
     >>> import numpy as np
     >>> import doubleml as dml
     >>> from doubleml.datasets import make_irm_data
-    >>> from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+    >>> from sklearn.ensemble import RandomForestClassifier
     >>> np.random.seed(3141)
-    >>> ml_g = RandomForestRegressor(n_estimators=100, max_features=20, max_depth=10, min_samples_leaf=2)
+    >>> ml_g = RandomForestClassifier(n_estimators=100, max_features=20, max_depth=10, min_samples_leaf=2)
     >>> ml_m = RandomForestClassifier(n_estimators=100, max_features=20, max_depth=10, min_samples_leaf=2)
     >>> data = make_irm_data(theta=0.5, n_obs=500, dim_x=20, return_type='DataFrame')
     >>> obj_dml_data = dml.DoubleMLData(data, 'y', 'd')
-    >>> dml_cvar_obj = dml.DoubleMLCVAR(obj_dml_data, ml_g, ml_m, treatment=1, quantile=0.5)
-    >>> dml_cvar_obj.fit().summary
-           coef   std err          t         P>|t|     2.5 %    97.5 %
-    d  1.591441  0.095781  16.615498  5.382582e-62  1.403715  1.779167
+    >>> dml_pq_obj = dml.DoubleMLPQ(obj_dml_data, ml_g, ml_m, treatment=1, quantile=0.5)
+    >>> dml_pq_obj.fit().summary
+           coef   std err         t     P>|t|     2.5 %    97.5 %
+    d  0.553878  0.149858  3.696011  0.000219  0.260161  0.847595
     """
 
     def __init__(self,
                  obj_dml_data,
                  ml_g,
                  ml_m,
                  treatment=1,
                  quantile=0.5,
                  n_folds=5,
                  n_rep=1,
-                 score='CVaR',
+                 score='PQ',
                  dml_procedure='dml2',
                  normalize_ipw=True,
+                 kde=None,
                  trimming_rule='truncate',
                  trimming_threshold=1e-2,
                  draw_sample_splitting=True,
                  apply_cross_fitting=True):
         super().__init__(obj_dml_data,
                          n_folds,
                          n_rep,
                          score,
                          dml_procedure,
                          draw_sample_splitting,
                          apply_cross_fitting)
 
         self._quantile = quantile
         self._treatment = treatment
-        self._normalize_ipw = normalize_ipw
+        if kde is None:
+            self._kde = _default_kde
+        else:
+            if not callable(kde):
+                raise TypeError('kde should be either a callable or None. '
+                                '%r was passed.' % kde)
+            self._kde = kde
 
+        self._normalize_ipw = normalize_ipw
         self._check_data(self._dml_data)
-        valid_score = ['CVaR']
+
+        valid_score = ['PQ']
         _check_score(self.score, valid_score, allow_callable=False)
         _check_quantile(self.quantile)
         _check_treatment(self.treatment)
 
         if not isinstance(self.normalize_ipw, bool):
             raise TypeError('Normalization indicator has to be boolean. ' +
                             f'Object of type {str(type(self.normalize_ipw))} passed.')
 
         # initialize starting values and bounds
         self._coef_bounds = (self._dml_data.y.min(), self._dml_data.y.max())
-        y_treat = self._dml_data.y[self._dml_data.d == self.treatment]
-        self._coef_start_val = np.mean(y_treat[y_treat >= np.quantile(y_treat, self.quantile)])
+        self._coef_start_val = np.quantile(self._dml_data.y[self._dml_data.d == self.treatment], self.quantile)
 
         # initialize and check trimming
         self._trimming_rule = trimming_rule
         self._trimming_threshold = trimming_threshold
         _check_trimming(self._trimming_rule, self._trimming_threshold)
 
-        _ = self._check_learner(ml_g, 'ml_g', regressor=True, classifier=False)
+        _ = self._check_learner(ml_g, 'ml_g', regressor=False, classifier=True)
         _ = self._check_learner(ml_m, 'ml_m', regressor=False, classifier=True)
-        self._learner = {'ml_g': clone(ml_g), 'ml_m': clone(ml_m)}
-        self._predict_method = {'ml_g': 'predict', 'ml_m': 'predict_proba'}
+        self._learner = {'ml_g': ml_g, 'ml_m': ml_m}
+        self._predict_method = {'ml_g': 'predict_proba', 'ml_m': 'predict_proba'}
 
         self._initialize_ml_nuisance_params()
 
         if draw_sample_splitting:
             obj_dml_resampling = DoubleMLResampling(n_folds=self.n_folds,
                                                     n_rep=self.n_rep,
                                                     n_obs=self._dml_data.n_obs,
@@ -164,14 +181,21 @@
     def treatment(self):
         """
         Treatment indicator for potential outcome.
         """
         return self._treatment
 
     @property
+    def kde(self):
+        """
+        The kernel density estimation of the derivative.
+        """
+        return self._kde
+
+    @property
     def normalize_ipw(self):
         """
         Indicates whether the inverse probability weights are normalized.
         """
         return self._normalize_ipw
 
     @property
@@ -184,27 +208,53 @@
     @property
     def trimming_threshold(self):
         """
         Specifies the used trimming threshold.
         """
         return self._trimming_threshold
 
+    @property
+    def _score_element_names(self):
+        return ['ind_d', 'g', 'm', 'y']
+
     def _compute_ipw_score(self, theta, d, y, prop):
         score = (d == self.treatment) / prop * (y <= theta) - self.quantile
         return score
 
-    def _score_elements(self, y, d, g_hat, m_hat, pq_est):
-        # recalculate the target for g based on the pq_est
-        g_target_1 = np.ones_like(y) * pq_est
-        g_target_2 = (y - self.quantile * pq_est) / (1 - self.quantile)
-        g_target = np.max(np.column_stack((g_target_1, g_target_2)), 1)
-
-        psi_b = (d == self.treatment) * (g_target - g_hat) / m_hat + g_hat
-        psi_a = np.full_like(m_hat, -1.0)
-        return psi_a, psi_b
+    def _compute_score(self, psi_elements, coef, inds=None):
+        ind_d = psi_elements['ind_d']
+        g = psi_elements['g']
+        m = psi_elements['m']
+        y = psi_elements['y']
+
+        if inds is not None:
+            ind_d = psi_elements['ind_d'][inds]
+            g = psi_elements['g'][inds]
+            m = psi_elements['m'][inds]
+            y = psi_elements['y'][inds]
+
+        score = ind_d * ((y <= coef) - g) / m + g - self.quantile
+        return score
+
+    def _compute_score_deriv(self, psi_elements, coef, inds=None):
+        ind_d = psi_elements['ind_d']
+        m = psi_elements['m']
+        y = psi_elements['y']
+
+        if inds is not None:
+            ind_d = psi_elements['ind_d'][inds]
+            m = psi_elements['m'][inds]
+            y = psi_elements['y'][inds]
+
+        score_weights = ind_d / m
+
+        u = (y - coef).reshape(-1, 1)
+        deriv = self.kde(u, score_weights)
+
+        return deriv
 
     def _initialize_ml_nuisance_params(self):
         self._params = {learner: {key: [None] * self.n_rep for key in self._dml_data.d_cols}
                         for learner in ['ml_g', 'ml_m']}
 
     def _nuisance_est(self, smpls, n_jobs_cv, return_models=False):
         x, y = check_X_y(self._dml_data.x, self._dml_data.y,
@@ -215,26 +265,26 @@
         # initialize nuisance predictions, targets and models
         g_hat = {'models': None,
                  'targets': np.full(shape=self._dml_data.n_obs, fill_value=np.nan),
                  'preds': np.full(shape=self._dml_data.n_obs, fill_value=np.nan)
                  }
         m_hat = copy.deepcopy(g_hat)
 
+        ipw_vec = np.full(shape=self.n_folds, fill_value=np.nan)
         # initialize models
         fitted_models = {}
         for learner in self.params_names:
             # set nuisance model parameters
             est_params = self._get_params(learner)
             if est_params is not None:
                 fitted_models[learner] = [clone(self._learner[learner]).set_params(**est_params[i_fold])
                                           for i_fold in range(self.n_folds)]
             else:
                 fitted_models[learner] = [clone(self._learner[learner]) for i_fold in range(self.n_folds)]
 
-        ipw_vec = np.full(shape=self.n_folds, fill_value=np.nan)
         # caculate nuisance functions over different folds
         for i_fold in range(self.n_folds):
             train_inds = smpls[i_fold][0]
             test_inds = smpls[i_fold][1]
 
             # start nested crossfitting
             train_inds_1, train_inds_2 = train_test_split(train_inds, test_size=0.5,
@@ -265,65 +315,61 @@
 
             _, bracket_guess = _get_bracket_guess(ipw_score, self._coef_start_val, self._coef_bounds)
             ipw_est = _solve_ipw_score(ipw_score=ipw_score, bracket_guess=bracket_guess)
             ipw_vec[i_fold] = ipw_est
 
             # use the preliminary estimates to fit the nuisance parameters on train_2
             d_train_2 = d[train_inds_2]
+            y_train_2 = y[train_inds_2]
             x_train_2 = x[train_inds_2, :]
-            x_test = x[test_inds, :]
-
-            # calculate the target for g
-            g_target_1 = np.ones_like(y) * ipw_est
-            g_target_2 = (y - self.quantile * ipw_est) / (1 - self.quantile)
-            g_target = np.max(np.column_stack((g_target_1, g_target_2)), 1)
-            g_target_train_2 = g_target[train_inds_2]
 
-            # only consider values with the right treatment status and fit the model
             dx_treat_train_2 = x_train_2[d_train_2 == self.treatment, :]
-            g_target_train_2_d = g_target_train_2[d_train_2 == self.treatment]
-            fitted_models['ml_g'][i_fold].fit(dx_treat_train_2, g_target_train_2_d)
+            y_treat_train_2 = y_train_2[d_train_2 == self.treatment]
+
+            fitted_models['ml_g'][i_fold].fit(dx_treat_train_2, y_treat_train_2 <= ipw_est)
 
             # predict nuisance values on the test data and the corresponding targets
-            g_hat['preds'][test_inds] = fitted_models['ml_g'][i_fold].predict(x_test)
-            g_hat['targets'][test_inds] = g_target[test_inds]
+            g_hat['preds'][test_inds] = _predict_zero_one_propensity(fitted_models['ml_g'][i_fold], x[test_inds, :])
+            g_hat['targets'][test_inds] = y[test_inds] <= ipw_est
 
             # refit the propensity score on the whole training set
             fitted_models['ml_m'][i_fold].fit(x[train_inds, :], d[train_inds])
-            m_hat['preds'][test_inds] = _predict_zero_one_propensity(fitted_models['ml_m'][i_fold], x_test)
+            m_hat['preds'][test_inds] = _predict_zero_one_propensity(fitted_models['ml_m'][i_fold], x[test_inds, :])
 
         # set target for propensity score
         m_hat['targets'] = d
 
         # set the target for g to be a float and only relevant values
         g_hat['targets'] = g_hat['targets'].astype(float)
         g_hat['targets'][d != self.treatment] = np.nan
 
         if return_models:
             g_hat['models'] = fitted_models['ml_g']
             m_hat['models'] = fitted_models['ml_m']
 
         # clip propensities and normalize ipw weights
-        # this is not done in the score to be equivalent to PQ models
+        # this is not done in the score to save computation due to multiple score evaluations
+        # to be able to evaluate the raw models the m_hat['preds'] are not changed
         m_hat_adj = _trimm(m_hat['preds'], self.trimming_rule, self.trimming_threshold)
         if self._normalize_ipw:
             if self.dml_procedure == 'dml1':
                 for _, test_index in smpls:
                     m_hat_adj[test_index] = _normalize_ipw(m_hat_adj[test_index], d[test_index])
             else:
                 m_hat_adj = _normalize_ipw(m_hat_adj, d)
 
         if self.treatment == 0:
             m_hat_adj = 1 - m_hat_adj
 
-        # use the average of the ipw estimates to approximate the potential quantile for U (p.4 Kallus et. al)
-        pq_est = np.mean(ipw_vec)
-        psi_a, psi_b = self._score_elements(y, d, g_hat['preds'], m_hat_adj, pq_est)
-        psi_elements = {'psi_a': psi_a,
-                        'psi_b': psi_b}
+        # readjust start value for minimization
+        self._coef_start_val = np.mean(ipw_vec)
+
+        psi_elements = {'ind_d': d == self.treatment, 'g': g_hat['preds'],
+                        'm': m_hat_adj, 'y': y}
+
         preds = {'predictions': {'ml_g': g_hat['preds'],
                                  'ml_m': m_hat['preds']},
                  'targets': {'ml_g': g_hat['targets'],
                              'ml_m': m_hat['targets']},
                  'models': {'ml_g': g_hat['models'],
                             'ml_m': m_hat['models']}
                  }
@@ -340,19 +386,16 @@
             scoring_methods = {'ml_g': None,
                                'ml_m': None}
 
         train_inds = [train_index for (train_index, _) in smpls]
         train_inds_treat = [np.intersect1d(np.where(d == self.treatment)[0], train) for train, _ in smpls]
 
         # use self._coef_start_val as a very crude approximation of ipw_est
-        quantile_approx = np.quantile(y[d == self.treatment], self.quantile)
-        g_target_1 = np.ones_like(y) * quantile_approx
-        g_target_2 = (y - self.quantile * quantile_approx) / (1 - self.quantile)
-        g_target_approx = np.max(np.column_stack((g_target_1, g_target_2)), 1)
-        g_tune_res = _dml_tune(g_target_approx, x, train_inds_treat,
+        approx_goal = y <= np.quantile(y[d == self.treatment], self.quantile)
+        g_tune_res = _dml_tune(approx_goal, x, train_inds_treat,
                                self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
                                n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
 
         m_tune_res = _dml_tune(d, x, train_inds,
                                self._learner['ml_m'], param_grids['ml_m'], scoring_methods['ml_m'],
                                n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
 
@@ -372,7 +415,10 @@
     def _check_data(self, obj_dml_data):
         if not isinstance(obj_dml_data, DoubleMLData):
             raise TypeError('The data must be of DoubleMLData type. '
                             f'{str(obj_dml_data)} of type {str(type(obj_dml_data))} was passed.')
         _check_contains_iv(obj_dml_data)
         _check_zero_one_treatment(self)
         return
+
+    def _sensitivity_element_est(self, preds):
+        pass
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_data.py` & `DoubleML-0.6.2/doubleml/double_ml_data.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/double_ml_did.py` & `DoubleML-0.6.2/doubleml/double_ml_did.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from sklearn.utils.multiclass import type_of_target
 import warnings
 
 from .double_ml import DoubleML
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
 
-from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _check_finite_predictions, _check_is_propensity, \
-    _trimm, _check_score, _check_trimming
+from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _trimm
+from ._utils_checks import _check_score, _check_trimming, _check_finite_predictions, _check_is_propensity
 
 
 class DoubleMLDID(LinearScoreMixin, DoubleML):
     """Double machine learning for difference-in-differences models with panel data (two time periods).
 
     Parameters
     ----------
@@ -143,14 +143,16 @@
             self._predict_method['ml_m'] = 'predict_proba'
         self._initialize_ml_nuisance_params()
 
         self._trimming_rule = trimming_rule
         self._trimming_threshold = trimming_threshold
         _check_trimming(self._trimming_rule, self._trimming_threshold)
 
+        self._sensitivity_implemented = True
+
     @property
     def in_sample_normalization(self):
         """
         Indicates whether the in sample normalization of weights are used.
         """
         return self._in_sample_normalization
 
@@ -206,36 +208,34 @@
                                  return_models=return_models)
 
         _check_finite_predictions(g_hat0['preds'], self._learner['ml_g'], 'ml_g', smpls)
         # adjust target values to consider only compatible subsamples
         g_hat0['targets'] = g_hat0['targets'].astype(float)
         g_hat0['targets'][d == 1] = np.nan
 
-        # only relevant for observational or experimental setting
+        g_hat1 = _dml_cv_predict(self._learner['ml_g'], x, y, smpls=smpls_d1, n_jobs=n_jobs_cv,
+                                 est_params=self._get_params('ml_g1'), method=self._predict_method['ml_g'],
+                                 return_models=return_models)
+
+        _check_finite_predictions(g_hat0['preds'], self._learner['ml_g'], 'ml_g', smpls)
+        # adjust target values to consider only compatible subsamples
+        g_hat1['targets'] = g_hat1['targets'].astype(float)
+        g_hat1['targets'][d == 0] = np.nan
+
+        # only relevant for observational setting
         m_hat = {'preds': None, 'targets': None, 'models': None}
-        g_hat1 = {'preds': None, 'targets': None, 'models': None}
         if self.score == 'observational':
             # nuisance m
             m_hat = _dml_cv_predict(self._learner['ml_m'], x, d, smpls=smpls, n_jobs=n_jobs_cv,
                                     est_params=self._get_params('ml_m'), method=self._predict_method['ml_m'],
                                     return_models=return_models)
             _check_finite_predictions(m_hat['preds'], self._learner['ml_m'], 'ml_m', smpls)
             _check_is_propensity(m_hat['preds'], self._learner['ml_m'], 'ml_m', smpls, eps=1e-12)
             m_hat['preds'] = _trimm(m_hat['preds'], self.trimming_rule, self.trimming_threshold)
 
-        if self.score == 'experimental':
-            g_hat1 = _dml_cv_predict(self._learner['ml_g'], x, y, smpls=smpls_d1, n_jobs=n_jobs_cv,
-                                     est_params=self._get_params('ml_g1'), method=self._predict_method['ml_g'],
-                                     return_models=return_models)
-
-            _check_finite_predictions(g_hat0['preds'], self._learner['ml_g'], 'ml_g', smpls)
-            # adjust target values to consider only compatible subsamples
-            g_hat1['targets'] = g_hat1['targets'].astype(float)
-            g_hat1['targets'][d == 0] = np.nan
-
         # nuisance estimates of the uncond. treatment prob.
         p_hat = np.full_like(d, np.nan, dtype='float64')
         for train_index, test_index in smpls:
             p_hat[test_index] = np.mean(d[train_index])
 
         psi_a, psi_b = self._score_elements(y, d, g_hat0['preds'], g_hat1['preds'], m_hat['preds'], p_hat)
 
@@ -287,14 +287,57 @@
 
         # set score elements
         psi_a = -1.0 * weight_psi_a
         psi_b = psi_b_1 + np.multiply(weight_resid_d0,  resid_d0)
 
         return psi_a, psi_b
 
+    def _sensitivity_element_est(self, preds):
+        y = self._dml_data.y
+        d = self._dml_data.d
+
+        m_hat = preds['predictions']['ml_m']
+        g_hat0 = preds['predictions']['ml_g0']
+        g_hat1 = preds['predictions']['ml_g1']
+
+        g_hat = np.multiply(d, g_hat1) + np.multiply(1.0-d, g_hat0)
+        sigma2_score_element = np.square(y - g_hat)
+        sigma2 = np.mean(sigma2_score_element)
+        psi_sigma2 = sigma2_score_element - sigma2
+
+        # calc m(W,alpha) and Riesz representer
+        p_hat = np.mean(d)
+        if self.score == 'observational':
+            propensity_weight_d0 = np.divide(m_hat, 1.0-m_hat)
+            if self.in_sample_normalization:
+                weight_d0 = np.multiply(1.0-d, propensity_weight_d0)
+                mean_weight_d0 = np.mean(weight_d0)
+
+                m_alpha = np.multiply(np.divide(d, p_hat),
+                                      np.divide(1.0, p_hat) + np.divide(propensity_weight_d0, mean_weight_d0))
+                rr = np.divide(d, p_hat) - np.divide(weight_d0, mean_weight_d0)
+            else:
+                m_alpha = np.multiply(np.divide(d, np.square(p_hat)), (1.0 + propensity_weight_d0))
+                rr = np.divide(d, p_hat) - np.multiply(np.divide(1.0-d, p_hat), propensity_weight_d0)
+        else:
+            assert self.score == 'experimental'
+            # the same with or without self-normalization
+            m_alpha = np.divide(1.0, p_hat) + np.divide(1.0, 1.0-p_hat)
+            rr = np.divide(d, p_hat) - np.divide(1.0-d, 1.0-p_hat)
+
+        nu2_score_element = np.multiply(2.0, m_alpha) - np.square(rr)
+        nu2 = np.mean(nu2_score_element)
+        psi_nu2 = nu2_score_element - nu2
+
+        element_dict = {'sigma2': sigma2,
+                        'nu2': nu2,
+                        'psi_sigma2': psi_sigma2,
+                        'psi_nu2': psi_nu2}
+        return element_dict
+
     def _nuisance_tuning(self, smpls, param_grids, scoring_methods, n_folds_tune, n_jobs_cv,
                          search_mode, n_iter_randomized_search):
         x, y = check_X_y(self._dml_data.x, self._dml_data.y,
                          force_all_finite=False)
         x, d = check_X_y(x, self._dml_data.d,
                          force_all_finite=False)
         # get train indices for d == 0 and d == 1
@@ -306,34 +349,34 @@
 
         train_inds = [train_index for (train_index, _) in smpls]
         train_inds_d0 = [train_index for (train_index, _) in smpls_d0]
         train_inds_d1 = [train_index for (train_index, _) in smpls_d1]
         g0_tune_res = _dml_tune(y, x, train_inds_d0,
                                 self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
                                 n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
+        g1_tune_res = _dml_tune(y, x, train_inds_d1,
+                                self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
+                                n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
+
+        g0_best_params = [xx.best_params_ for xx in g0_tune_res]
+        g1_best_params = [xx.best_params_ for xx in g1_tune_res]
+
         m_tune_res = list()
         if self.score == 'observational':
             m_tune_res = _dml_tune(d, x, train_inds,
                                    self._learner['ml_m'], param_grids['ml_m'], scoring_methods['ml_m'],
                                    n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
-        g1_tune_res = list()
-        if self.score == 'experimental':
-            g1_tune_res = _dml_tune(y, x, train_inds_d1,
-                                    self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
-                                    n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
-
-        g0_best_params = [xx.best_params_ for xx in g0_tune_res]
-        if self.score == 'observational':
             m_best_params = [xx.best_params_ for xx in m_tune_res]
             params = {'ml_g0': g0_best_params,
+                      'ml_g1': g1_best_params,
                       'ml_m': m_best_params}
             tune_res = {'g0_tune': g0_tune_res,
+                        'g1_tune': g1_tune_res,
                         'm_tune': m_tune_res}
         else:
-            g1_best_params = [xx.best_params_ for xx in g1_tune_res]
             params = {'ml_g0': g0_best_params,
                       'ml_g1': g1_best_params}
             tune_res = {'g0_tune': g0_tune_res,
                         'g1_tune': g1_tune_res}
 
         res = {'params': params,
                'tune_res': tune_res}
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_did_cs.py` & `DoubleML-0.6.2/doubleml/double_ml_did_cs.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from sklearn.utils.multiclass import type_of_target
 import warnings
 
 from .double_ml import DoubleML
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
 
-from ._utils import _dml_cv_predict, _check_finite_predictions, _check_is_propensity, \
-    _trimm, _get_cond_smpls_2d, _dml_tune, _check_score, _check_trimming
+from ._utils import _dml_cv_predict, _trimm, _get_cond_smpls_2d, _dml_tune
+from ._utils_checks import _check_score, _check_trimming, _check_finite_predictions, _check_is_propensity
 
 
 class DoubleMLDIDCS(LinearScoreMixin, DoubleML):
     """Double machine learning for difference-in-difference with repeated cross-sections.
 
     Parameters
     ----------
@@ -143,14 +143,16 @@
             self._predict_method['ml_m'] = 'predict_proba'
         self._initialize_ml_nuisance_params()
 
         self._trimming_rule = trimming_rule
         self._trimming_threshold = trimming_threshold
         _check_trimming(self._trimming_rule, self._trimming_threshold)
 
+        self._sensitivity_implemented = True
+
     @property
     def in_sample_normalization(self):
         """
         Indicates whether the in sample normalization of weights are used.
         """
         return self._in_sample_normalization
 
@@ -295,84 +297,75 @@
 
         # calculate residuals
         resid_d0_t0 = y - g_hat_d0_t0
         resid_d0_t1 = y - g_hat_d0_t1
         resid_d1_t0 = y - g_hat_d1_t0
         resid_d1_t1 = y - g_hat_d1_t1
 
+        d1t1 = np.multiply(d, t)
+        d1t0 = np.multiply(d, 1.0-t)
+        d0t1 = np.multiply(1.0-d, t)
+        d0t0 = np.multiply(1.0-d, 1.0-t)
+
         if self.score == 'observational':
             if self.in_sample_normalization:
                 weight_psi_a = np.divide(d, np.mean(d))
                 weight_g_d1_t1 = weight_psi_a
                 weight_g_d1_t0 = -1.0 * weight_psi_a
                 weight_g_d0_t1 = -1.0 * weight_psi_a
                 weight_g_d0_t0 = weight_psi_a
 
-                weight_resid_d1_t1 = np.divide(np.multiply(d, t),
-                                               np.mean(np.multiply(d, t)))
-                weight_resid_d1_t0 = -1.0 * np.divide(np.multiply(d, 1.0-t),
-                                                      np.mean(np.multiply(d, 1.0-t)))
+                weight_resid_d1_t1 = np.divide(d1t1, np.mean(d1t1))
+                weight_resid_d1_t0 = -1.0 * np.divide(d1t0, np.mean(d1t0))
 
                 prop_weighting = np.divide(m_hat, 1.0-m_hat)
-                unscaled_d0_t1 = np.multiply(np.multiply(1.0-d, t), prop_weighting)
+                unscaled_d0_t1 = np.multiply(d0t1, prop_weighting)
                 weight_resid_d0_t1 = -1.0 * np.divide(unscaled_d0_t1, np.mean(unscaled_d0_t1))
 
-                unscaled_d0_t0 = np.multiply(np.multiply(1.0-d, 1.0-t), prop_weighting)
+                unscaled_d0_t0 = np.multiply(d0t0, prop_weighting)
                 weight_resid_d0_t0 = np.divide(unscaled_d0_t0, np.mean(unscaled_d0_t0))
             else:
                 weight_psi_a = np.divide(d, p_hat)
                 weight_g_d1_t1 = weight_psi_a
                 weight_g_d1_t0 = -1.0 * weight_psi_a
                 weight_g_d0_t1 = -1.0 * weight_psi_a
                 weight_g_d0_t0 = weight_psi_a
 
-                weight_resid_d1_t1 = np.divide(np.multiply(d, t),
-                                               np.multiply(p_hat, lambda_hat))
-                weight_resid_d1_t0 = -1.0 * np.divide(np.multiply(d, 1.0-t),
-                                                      np.multiply(p_hat, 1.0-lambda_hat))
+                weight_resid_d1_t1 = np.divide(d1t1, np.multiply(p_hat, lambda_hat))
+                weight_resid_d1_t0 = -1.0 * np.divide(d1t0, np.multiply(p_hat, 1.0-lambda_hat))
 
                 prop_weighting = np.divide(m_hat, 1.0-m_hat)
-                weight_resid_d0_t1 = -1.0 * np.multiply(np.divide(np.multiply(1.0-d, t),
-                                                                  np.multiply(p_hat, lambda_hat)),
+                weight_resid_d0_t1 = -1.0 * np.multiply(np.divide(d0t1, np.multiply(p_hat, lambda_hat)),
                                                         prop_weighting)
-                weight_resid_d0_t0 = np.multiply(np.divide(np.multiply(1.0-d, 1.0-t),
-                                                           np.multiply(p_hat, 1.0-lambda_hat)),
+                weight_resid_d0_t0 = np.multiply(np.divide(d0t0, np.multiply(p_hat, 1.0-lambda_hat)),
                                                  prop_weighting)
         else:
             assert self.score == 'experimental'
             if self.in_sample_normalization:
                 weight_psi_a = np.ones_like(y)
                 weight_g_d1_t1 = weight_psi_a
                 weight_g_d1_t0 = -1.0 * weight_psi_a
                 weight_g_d0_t1 = -1.0 * weight_psi_a
                 weight_g_d0_t0 = weight_psi_a
 
-                weight_resid_d1_t1 = np.divide(np.multiply(d, t),
-                                               np.mean(np.multiply(d, t)))
-                weight_resid_d1_t0 = -1.0 * np.divide(np.multiply(d, 1.0-t),
-                                                      np.mean(np.multiply(d, 1.0-t)))
-                weight_resid_d0_t1 = -1.0 * np.divide(np.multiply(1.0-d, t),
-                                                      np.mean(np.multiply(1.0-d, t)))
-                weight_resid_d0_t0 = np.divide(np.multiply(1.0-d, 1.0-t),
-                                               np.mean(np.multiply(1.0-d, 1.0-t)))
+                weight_resid_d1_t1 = np.divide(d1t1, np.mean(d1t1))
+                weight_resid_d1_t0 = -1.0 * np.divide(d1t0, np.mean(d1t0))
+                weight_resid_d0_t1 = -1.0 * np.divide(d0t1, np.mean(d0t1))
+                weight_resid_d0_t0 = np.divide(d0t0, np.mean(d0t0))
             else:
                 weight_psi_a = np.ones_like(y)
                 weight_g_d1_t1 = weight_psi_a
                 weight_g_d1_t0 = -1.0 * weight_psi_a
                 weight_g_d0_t1 = -1.0 * weight_psi_a
                 weight_g_d0_t0 = weight_psi_a
 
-                weight_resid_d1_t1 = np.divide(np.multiply(d, t),
-                                               np.multiply(p_hat, lambda_hat))
-                weight_resid_d1_t0 = -1.0 * np.divide(np.multiply(d, 1.0-t),
-                                                      np.multiply(p_hat, 1.0-lambda_hat))
-                weight_resid_d0_t1 = -1.0 * np.divide(np.multiply(1.0-d, t),
-                                                      np.multiply(1.0-p_hat, lambda_hat))
-                weight_resid_d0_t0 = np.divide(np.multiply(1.0-d, 1.0-t),
-                                               np.multiply(1.0-p_hat, 1.0-lambda_hat))
+                weight_resid_d1_t1 = np.divide(d1t1, np.multiply(p_hat, lambda_hat))
+                weight_resid_d1_t0 = -1.0 * np.divide(d1t0, np.multiply(p_hat, 1.0-lambda_hat))
+                weight_resid_d0_t1 = -1.0 * np.divide(d0t1, np.multiply(1.0-p_hat, lambda_hat))
+                weight_resid_d0_t0 = np.divide(d0t0, np.multiply(1.0-p_hat, 1.0-lambda_hat))
 
         # set score elements
         psi_a = -1.0 * weight_psi_a
 
         # psi_b
         psi_b_1 = np.multiply(weight_g_d1_t1,  g_hat_d1_t1) + \
             np.multiply(weight_g_d1_t0,  g_hat_d1_t0) + \
@@ -383,14 +376,95 @@
             np.multiply(weight_resid_d0_t0,  resid_d0_t0) + \
             np.multiply(weight_resid_d0_t1,  resid_d0_t1)
 
         psi_b = psi_b_1 + psi_b_2
 
         return psi_a, psi_b
 
+    def _sensitivity_element_est(self, preds):
+        y = self._dml_data.y
+        d = self._dml_data.d
+        t = self._dml_data.t
+
+        m_hat = preds['predictions']['ml_m']
+        g_hat_d0_t0 = preds['predictions']['ml_g_d0_t0']
+        g_hat_d0_t1 = preds['predictions']['ml_g_d0_t1']
+        g_hat_d1_t0 = preds['predictions']['ml_g_d1_t0']
+        g_hat_d1_t1 = preds['predictions']['ml_g_d1_t1']
+
+        d0t0 = np.multiply(1.0-d, 1.0-t)
+        d0t1 = np.multiply(1.0-d, t)
+        d1t0 = np.multiply(d, 1.0-t)
+        d1t1 = np.multiply(d, t)
+
+        g_hat = np.multiply(d0t0, g_hat_d0_t0) + np.multiply(d0t1, g_hat_d0_t1) + \
+            np.multiply(d1t0, g_hat_d1_t0) + np.multiply(d1t1, g_hat_d1_t1)
+        sigma2_score_element = np.square(y - g_hat)
+        sigma2 = np.mean(sigma2_score_element)
+        psi_sigma2 = sigma2_score_element - sigma2
+
+        # calc m(W,alpha) and Riesz representer
+        p_hat = np.mean(d)
+        lambda_hat = np.mean(t)
+        if self.score == 'observational':
+            propensity_weight_d0 = np.divide(m_hat, 1.0-m_hat)
+            if self.in_sample_normalization:
+                weight_d0t1 = np.multiply(d0t1, propensity_weight_d0)
+                weight_d0t0 = np.multiply(d0t0, propensity_weight_d0)
+                mean_weight_d0t1 = np.mean(weight_d0t1)
+                mean_weight_d0t0 = np.mean(weight_d0t0)
+
+                m_alpha = np.multiply(np.divide(d, p_hat),
+                                      np.divide(1.0, np.mean(d1t1)) +
+                                      np.divide(1.0, np.mean(d1t0)) +
+                                      np.divide(propensity_weight_d0, mean_weight_d0t1) +
+                                      np.divide(propensity_weight_d0, mean_weight_d0t0))
+
+                rr = np.divide(d1t1, np.mean(d1t1)) - \
+                    np.divide(d1t0, np.mean(d1t0)) - \
+                    np.divide(weight_d0t1, mean_weight_d0t1) + \
+                    np.divide(weight_d0t0, mean_weight_d0t0)
+            else:
+                m_alpha_1 = np.divide(1.0, lambda_hat) + np.divide(1.0, 1.0-lambda_hat)
+                m_alpha = np.multiply(np.divide(d, np.square(p_hat)), np.multiply(m_alpha_1, 1.0 + propensity_weight_d0))
+
+                rr_1 = np.divide(t, np.multiply(p_hat, lambda_hat)) + np.divide(1.0-t, np.multiply(p_hat, 1.0-lambda_hat))
+                rr_2 = d + np.multiply(1.0-d, propensity_weight_d0)
+                rr = np.multiply(rr_1, rr_2)
+        else:
+            assert self.score == 'experimental'
+            if self.in_sample_normalization:
+                m_alpha = np.divide(1.0, np.mean(d1t1)) + \
+                    np.divide(1.0, np.mean(d1t0)) + \
+                    np.divide(1.0, np.mean(d0t1)) + \
+                    np.divide(1.0, np.mean(d0t0))
+                rr = np.divide(d1t1, np.mean(d1t1)) - \
+                    np.divide(d1t0, np.mean(d1t0)) - \
+                    np.divide(d0t1, np.mean(d0t1)) + \
+                    np.divide(d0t0, np.mean(d0t0))
+            else:
+                m_alpha = np.divide(1.0, np.multiply(p_hat, lambda_hat)) + \
+                    np.divide(1.0, np.multiply(p_hat, 1.0-lambda_hat)) + \
+                    np.divide(1.0, np.multiply(1.0-p_hat, lambda_hat)) + \
+                    np.divide(1.0, np.multiply(1.0-p_hat, 1.0-lambda_hat))
+                rr = np.divide(d1t1, np.multiply(p_hat, lambda_hat)) - \
+                    np.divide(d1t0, np.multiply(p_hat, 1.0-lambda_hat)) - \
+                    np.divide(d0t1, np.multiply(1.0-p_hat, lambda_hat)) + \
+                    np.divide(d0t0, np.multiply(1.0-p_hat, 1.0-lambda_hat))
+
+        nu2_score_element = np.multiply(2.0, m_alpha) - np.square(rr)
+        nu2 = np.mean(nu2_score_element)
+        psi_nu2 = nu2_score_element - nu2
+
+        element_dict = {'sigma2': sigma2,
+                        'nu2': nu2,
+                        'psi_sigma2': psi_sigma2,
+                        'psi_nu2': psi_nu2}
+        return element_dict
+
     def _nuisance_tuning(self, smpls, param_grids, scoring_methods, n_folds_tune, n_jobs_cv,
                          search_mode, n_iter_randomized_search):
         x, y = check_X_y(self._dml_data.x, self._dml_data.y,
                          force_all_finite=False)
         x, d = check_X_y(x, self._dml_data.d,
                          force_all_finite=False)
         x, t = check_X_y(x, self._dml_data.t,
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_iivm.py` & `DoubleML-0.6.2/doubleml/double_ml_iivm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 from sklearn.utils import check_X_y
 from sklearn.utils.multiclass import type_of_target
 
 from .double_ml import DoubleML
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
-from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _check_finite_predictions, _check_is_propensity, \
-    _trimm, _normalize_ipw, _check_score, _check_trimming
+
+from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _trimm, _normalize_ipw
+from ._utils_checks import _check_score, _check_trimming, _check_finite_predictions, _check_is_propensity
 
 
 class DoubleMLIIVM(LinearScoreMixin, DoubleML):
     """Double machine learning for interactive IV regression models
 
     Parameters
     ----------
@@ -445,7 +446,10 @@
                     'r0_tune': r0_tune_res,
                     'r1_tune': r1_tune_res}
 
         res = {'params': params,
                'tune_res': tune_res}
 
         return res
+
+    def _sensitivity_element_est(self, preds):
+        pass
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_irm.py` & `DoubleML-0.6.2/doubleml/double_ml_irm.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from .double_ml import DoubleML
 
 from .double_ml_blp import DoubleMLBLP
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
 
-from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _check_finite_predictions, _check_is_propensity, \
-    _trimm, _normalize_ipw, _check_score, _check_trimming
+from ._utils import _dml_cv_predict, _get_cond_smpls, _dml_tune, _trimm, _normalize_ipw
+from ._utils_checks import _check_score, _check_trimming, _check_finite_predictions, _check_is_propensity
 
 
 class DoubleMLIRM(LinearScoreMixin, DoubleML):
     """Double machine learning for interactive regression models
 
     Parameters
     ----------
@@ -154,14 +154,16 @@
         if not isinstance(self.normalize_ipw, bool):
             raise TypeError('Normalization indicator has to be boolean. ' +
                             f'Object of type {str(type(self.normalize_ipw))} passed.')
         self._trimming_rule = trimming_rule
         self._trimming_threshold = trimming_threshold
         _check_trimming(self._trimming_rule, self._trimming_threshold)
 
+        self._sensitivity_implemented = True
+
     @property
     def normalize_ipw(self):
         """
         Indicates whether the inverse probability weights are normalized.
         """
         return self._normalize_ipw
 
@@ -225,39 +227,38 @@
             zero_one_preds = np.all((np.power(g_hat0['preds'], 2) - g_hat0['preds']) == 0)
             if binary_preds & zero_one_preds:
                 raise ValueError(f'For the binary outcome variable {self._dml_data.y_col}, '
                                  f'predictions obtained with the ml_g learner {str(self._learner["ml_g"])} are also '
                                  'observed to be binary with values 0 and 1. Make sure that for classifiers '
                                  'probabilities and not labels are predicted.')
 
-        g_hat1 = {'preds': None, 'targets': None, 'models': None}
-        if (self.score == 'ATE') | callable(self.score):
-            g_hat1 = _dml_cv_predict(self._learner['ml_g'], x, y, smpls=smpls_d1, n_jobs=n_jobs_cv,
-                                     est_params=self._get_params('ml_g1'), method=self._predict_method['ml_g'],
-                                     return_models=return_models)
-            _check_finite_predictions(g_hat1['preds'], self._learner['ml_g'], 'ml_g', smpls)
-            # adjust target values to consider only compatible subsamples
-            g_hat1['targets'] = g_hat1['targets'].astype(float)
-            g_hat1['targets'][d == 0] = np.nan
-
-            if self._dml_data.binary_outcome:
-                binary_preds = (type_of_target(g_hat1['preds']) == 'binary')
-                zero_one_preds = np.all((np.power(g_hat1['preds'], 2) - g_hat1['preds']) == 0)
-                if binary_preds & zero_one_preds:
-                    raise ValueError(f'For the binary outcome variable {self._dml_data.y_col}, '
-                                     f'predictions obtained with the ml_g learner {str(self._learner["ml_g"])} are also '
-                                     'observed to be binary with values 0 and 1. Make sure that for classifiers '
-                                     'probabilities and not labels are predicted.')
+        g_hat1 = _dml_cv_predict(self._learner['ml_g'], x, y, smpls=smpls_d1, n_jobs=n_jobs_cv,
+                                 est_params=self._get_params('ml_g1'), method=self._predict_method['ml_g'],
+                                 return_models=return_models)
+        _check_finite_predictions(g_hat1['preds'], self._learner['ml_g'], 'ml_g', smpls)
+        # adjust target values to consider only compatible subsamples
+        g_hat1['targets'] = g_hat1['targets'].astype(float)
+        g_hat1['targets'][d == 0] = np.nan
+
+        if self._dml_data.binary_outcome:
+            binary_preds = (type_of_target(g_hat1['preds']) == 'binary')
+            zero_one_preds = np.all((np.power(g_hat1['preds'], 2) - g_hat1['preds']) == 0)
+            if binary_preds & zero_one_preds:
+                raise ValueError(f'For the binary outcome variable {self._dml_data.y_col}, '
+                                 f'predictions obtained with the ml_g learner {str(self._learner["ml_g"])} are also '
+                                 'observed to be binary with values 0 and 1. Make sure that for classifiers '
+                                 'probabilities and not labels are predicted.')
 
         # nuisance m
         m_hat = _dml_cv_predict(self._learner['ml_m'], x, d, smpls=smpls, n_jobs=n_jobs_cv,
                                 est_params=self._get_params('ml_m'), method=self._predict_method['ml_m'],
                                 return_models=return_models)
         _check_finite_predictions(m_hat['preds'], self._learner['ml_m'], 'ml_m', smpls)
         _check_is_propensity(m_hat['preds'], self._learner['ml_m'], 'ml_m', smpls, eps=1e-12)
+        m_hat['preds'] = _trimm(m_hat['preds'], self.trimming_rule, self.trimming_threshold)
 
         psi_a, psi_b = self._score_elements(y, d,
                                             g_hat0['preds'], g_hat1['preds'], m_hat['preds'],
                                             smpls)
         psi_elements = {'psi_a': psi_a,
                         'psi_b': psi_b}
         preds = {'predictions': {'ml_g0': g_hat0['preds'],
@@ -270,23 +271,22 @@
                             'ml_g1': g_hat1['models'],
                             'ml_m': m_hat['models']}
                  }
 
         return psi_elements, preds
 
     def _score_elements(self, y, d, g_hat0, g_hat1, m_hat, smpls):
+
         # fraction of treated for ATTE
         p_hat = None
         if self.score == 'ATTE':
             p_hat = np.full_like(d, np.nan, dtype='float64')
             for _, test_index in smpls:
                 p_hat[test_index] = np.mean(d[test_index])
 
-        m_hat = _trimm(m_hat, self.trimming_rule, self.trimming_threshold)
-
         if self.normalize_ipw:
             if self.dml_procedure == 'dml1':
                 for _, test_index in smpls:
                     m_hat[test_index] = _normalize_ipw(m_hat[test_index], d[test_index])
             else:
                 m_hat = _normalize_ipw(m_hat, d)
 
@@ -312,14 +312,50 @@
             assert callable(self.score)
             psi_a, psi_b = self.score(y=y, d=d,
                                       g_hat0=g_hat0, g_hat1=g_hat1, m_hat=m_hat,
                                       smpls=smpls)
 
         return psi_a, psi_b
 
+    def _sensitivity_element_est(self, preds):
+        # set elments for readability
+        y = self._dml_data.y
+        d = self._dml_data.d
+
+        m_hat = preds['predictions']['ml_m']
+        g_hat0 = preds['predictions']['ml_g0']
+        g_hat1 = preds['predictions']['ml_g1']
+
+        # use weights make this extendable
+        if self.score == 'ATE':
+            weights = np.ones_like(d)
+            weights_bar = np.ones_like(d)
+        else:
+            assert self.score == 'ATTE'
+            weights = np.divide(d, np.mean(d))
+            weights_bar = np.divide(m_hat, np.mean(d))
+
+        sigma2_score_element = np.square(y - np.multiply(d, g_hat1) - np.multiply(1.0-d, g_hat0))
+        sigma2 = np.mean(sigma2_score_element)
+        psi_sigma2 = sigma2_score_element - sigma2
+
+        # calc m(W,alpha) and Riesz representer
+        m_alpha = np.multiply(weights, np.multiply(weights_bar, (np.divide(1.0, m_hat) + np.divide(1.0, 1.0-m_hat))))
+        rr = np.multiply(weights_bar, (np.divide(d, m_hat) - np.divide(1.0-d, 1.0-m_hat)))
+
+        nu2_score_element = np.multiply(2.0, m_alpha) - np.square(rr)
+        nu2 = np.mean(nu2_score_element)
+        psi_nu2 = nu2_score_element - nu2
+
+        element_dict = {'sigma2': sigma2,
+                        'nu2': nu2,
+                        'psi_sigma2': psi_sigma2,
+                        'psi_nu2': psi_nu2}
+        return element_dict
+
     def _nuisance_tuning(self, smpls, param_grids, scoring_methods, n_folds_tune, n_jobs_cv,
                          search_mode, n_iter_randomized_search):
         x, y = check_X_y(self._dml_data.x, self._dml_data.y,
                          force_all_finite=False)
         x, d = check_X_y(x, self._dml_data.d,
                          force_all_finite=False)
         # get train indices for d == 0 and d == 1
@@ -332,38 +368,32 @@
         train_inds = [train_index for (train_index, _) in smpls]
         train_inds_d0 = [train_index for (train_index, _) in smpls_d0]
         train_inds_d1 = [train_index for (train_index, _) in smpls_d1]
         g0_tune_res = _dml_tune(y, x, train_inds_d0,
                                 self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
                                 n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
         g1_tune_res = list()
-        if self.score == 'ATE':
-            g1_tune_res = _dml_tune(y, x, train_inds_d1,
-                                    self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
-                                    n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
+        g1_tune_res = _dml_tune(y, x, train_inds_d1,
+                                self._learner['ml_g'], param_grids['ml_g'], scoring_methods['ml_g'],
+                                n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
 
         m_tune_res = _dml_tune(d, x, train_inds,
                                self._learner['ml_m'], param_grids['ml_m'], scoring_methods['ml_m'],
                                n_folds_tune, n_jobs_cv, search_mode, n_iter_randomized_search)
 
         g0_best_params = [xx.best_params_ for xx in g0_tune_res]
+        g1_best_params = [xx.best_params_ for xx in g1_tune_res]
         m_best_params = [xx.best_params_ for xx in m_tune_res]
-        if self.score == 'ATTE':
-            params = {'ml_g0': g0_best_params,
-                      'ml_m': m_best_params}
-            tune_res = {'g0_tune': g0_tune_res,
-                        'm_tune': m_tune_res}
-        else:
-            g1_best_params = [xx.best_params_ for xx in g1_tune_res]
-            params = {'ml_g0': g0_best_params,
-                      'ml_g1': g1_best_params,
-                      'ml_m': m_best_params}
-            tune_res = {'g0_tune': g0_tune_res,
-                        'g1_tune': g1_tune_res,
-                        'm_tune': m_tune_res}
+
+        params = {'ml_g0': g0_best_params,
+                  'ml_g1': g1_best_params,
+                  'ml_m': m_best_params}
+        tune_res = {'g0_tune': g0_tune_res,
+                    'g1_tune': g1_tune_res,
+                    'm_tune': m_tune_res}
 
         res = {'params': params,
                'tune_res': tune_res}
 
         return res
 
     def cate(self, basis):
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_lpq.py` & `DoubleML-0.6.2/doubleml/double_ml_lpq.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from sklearn.utils.multiclass import type_of_target
 from sklearn.base import clone
 from sklearn.utils import check_X_y
 from sklearn.model_selection import StratifiedKFold, train_test_split
 
 from .double_ml import DoubleML
 from .double_ml_score_mixins import NonLinearScoreMixin
-from ._utils import _dml_cv_predict, _trimm, _predict_zero_one_propensity, _check_zero_one_treatment, _check_score,\
-    _check_trimming, _check_quantile, _check_treatment, _get_bracket_guess, _default_kde, _normalize_ipw, _dml_tune, \
-    _solve_ipw_score
 from .double_ml_data import DoubleMLData
+
+from ._utils import _dml_cv_predict, _trimm, _predict_zero_one_propensity, \
+    _get_bracket_guess, _default_kde, _normalize_ipw, _dml_tune, _solve_ipw_score
 from ._utils_resampling import DoubleMLResampling
+from ._utils_checks import _check_score, _check_trimming, _check_zero_one_treatment, _check_treatment, \
+    _check_quantile
 
 
 class DoubleMLLPQ(NonLinearScoreMixin, DoubleML):
     """Double machine learning for local potential quantiles
 
     Parameters
     ----------
@@ -555,7 +557,10 @@
             binary_instr = (type_of_target(obj_dml_data.z) == 'binary')
             zero_one_instr = np.all((np.power(obj_dml_data.z, 2) - obj_dml_data.z) == 0)
             if not (one_instr & binary_instr & zero_one_instr):
                 raise ValueError(err_msg)
         else:
             raise ValueError(err_msg)
         return
+
+    def _sensitivity_element_est(self, preds):
+        pass
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_pliv.py` & `DoubleML-0.6.2/doubleml/double_ml_pliv.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from sklearn.dummy import DummyRegressor
 
 import warnings
 
 from .double_ml import DoubleML
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
-from ._utils import _dml_cv_predict, _dml_tune, _check_finite_predictions
+
+from ._utils import _dml_cv_predict, _dml_tune
+from ._utils_checks import _check_finite_predictions
 
 
 class DoubleMLPLIV(LinearScoreMixin, DoubleML):
     """Double machine learning for partially linear IV regression models
 
     Parameters
     ----------
@@ -277,25 +279,14 @@
         if obj_dml_data.n_instr == 0:
             raise ValueError('Incompatible data. ' +
                              'At least one variable must be set as instrumental variable. '
                              'To fit a partially linear regression model without instrumental variable(s) '
                              'use DoubleMLPLR instead of DoubleMLPLIV.')
         return
 
-    # To be removed in version 0.6.0
-    def set_ml_nuisance_params(self, learner, treat_var, params):
-        if isinstance(self.score, str) & (self.score == 'partialling out') & (learner == 'ml_g'):
-            warnings.warn(("Learner ml_g was renamed to ml_l. "
-                           "Please adapt the argument learner accordingly. "
-                           "The provided parameters are set for ml_l. "
-                           "The redirection will be removed in a future version."),
-                          DeprecationWarning, stacklevel=2)
-            learner = 'ml_l'
-        super(DoubleMLPLIV, self).set_ml_nuisance_params(learner, treat_var, params)
-
     def _nuisance_est(self, smpls, n_jobs_cv, return_models=False):
         if self.partialX & (not self.partialZ):
             psi_elements, preds = self._nuisance_est_partial_x(smpls, n_jobs_cv, return_models)
         elif (not self.partialX) & self.partialZ:
             psi_elements, preds = self._nuisance_est_partial_z(smpls, n_jobs_cv, return_models)
         else:
             assert (self.partialX & self.partialZ)
@@ -519,49 +510,14 @@
                  'models': {'ml_l': l_hat['models'],
                             'ml_m': m_hat['models'],
                             'ml_r': m_hat_tilde['models']}
                  }
 
         return psi_elements, preds
 
-    # To be removed in version 0.6.0
-    def tune(self,
-             param_grids,
-             tune_on_folds=False,
-             scoring_methods=None,  # if None the estimator's score method is used
-             n_folds_tune=5,
-             search_mode='grid_search',
-             n_iter_randomized_search=100,
-             n_jobs_cv=None,
-             set_as_params=True,
-             return_tune_res=False):
-
-        if isinstance(self.score, str) and (self.score == 'partialling out') and (param_grids is not None) and \
-                ('ml_g' in param_grids) and ('ml_l' not in param_grids):
-            warnings.warn(("Learner ml_g was renamed to ml_l. "
-                           "Please adapt the key of param_grids accordingly. "
-                           "The provided param_grids for ml_g are set for ml_l. "
-                           "The redirection will be removed in a future version."),
-                          DeprecationWarning, stacklevel=2)
-            param_grids['ml_l'] = param_grids.pop('ml_g')
-
-        if isinstance(self.score, str) and (self.score == 'partialling out') and (scoring_methods is not None) and \
-                ('ml_g' in scoring_methods) and ('ml_l' not in scoring_methods):
-            warnings.warn(("Learner ml_g was renamed to ml_l. "
-                           "Please adapt the key of scoring_methods accordingly. "
-                           "The provided scoring_methods for ml_g are set for ml_l. "
-                           "The redirection will be removed in a future version."),
-                          DeprecationWarning, stacklevel=2)
-            scoring_methods['ml_l'] = scoring_methods.pop('ml_g')
-
-        tune_res = super(DoubleMLPLIV, self).tune(param_grids, tune_on_folds, scoring_methods, n_folds_tune,
-                                                  search_mode, n_iter_randomized_search, n_jobs_cv, set_as_params,
-                                                  return_tune_res)
-        return tune_res
-
     def _nuisance_tuning_partial_x(self, smpls, param_grids, scoring_methods, n_folds_tune, n_jobs_cv,
                                    search_mode, n_iter_randomized_search):
         x, y = check_X_y(self._dml_data.x, self._dml_data.y,
                          force_all_finite=False)
         x, d = check_X_y(x, self._dml_data.d,
                          force_all_finite=False)
 
@@ -727,7 +683,10 @@
                     'm_tune': m_tune_res,
                     'r_tune': r_tune_res}
 
         res = {'params': params,
                'tune_res': tune_res}
 
         return res
+
+    def _sensitivity_element_est(self, preds):
+        pass
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_plr.py` & `DoubleML-0.6.2/doubleml/double_ml_plr.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from sklearn.base import clone
 
 import warnings
 
 from .double_ml import DoubleML
 from .double_ml_data import DoubleMLData
 from .double_ml_score_mixins import LinearScoreMixin
-from ._utils import _dml_cv_predict, _dml_tune, _check_finite_predictions, _check_is_propensity, _check_score
+
+from ._utils import _dml_cv_predict, _dml_tune
+from ._utils_checks import _check_score, _check_finite_predictions, _check_is_propensity
 
 
 class DoubleMLPLR(LinearScoreMixin, DoubleML):
     """Double machine learning for partially linear regression models
 
     Parameters
     ----------
@@ -143,14 +145,15 @@
             else:
                 raise ValueError(f'The ml_m learner {str(ml_m)} was identified as classifier '
                                  'but at least one treatment variable is not binary with values 0 and 1.')
         else:
             self._predict_method['ml_m'] = 'predict'
 
         self._initialize_ml_nuisance_params()
+        self._sensitivity_implemented = True
 
     def _initialize_ml_nuisance_params(self):
         self._params = {learner: {key: [None] * self.n_rep for key in self._dml_data.d_cols}
                         for learner in self._learner}
 
     def _check_data(self, obj_dml_data):
         if not isinstance(obj_dml_data, DoubleMLData):
@@ -159,25 +162,14 @@
         if obj_dml_data.z_cols is not None:
             raise ValueError('Incompatible data. ' +
                              ' and '.join(obj_dml_data.z_cols) +
                              ' have been set as instrumental variable(s). '
                              'To fit a partially linear IV regression model use DoubleMLPLIV instead of DoubleMLPLR.')
         return
 
-    # To be removed in version 0.6.0
-    def set_ml_nuisance_params(self, learner, treat_var, params):
-        if isinstance(self.score, str) & (self.score == 'partialling out') & (learner == 'ml_g'):
-            warnings.warn(("Learner ml_g was renamed to ml_l. "
-                           "Please adapt the argument learner accordingly. "
-                           "The provided parameters are set for ml_l. "
-                           "The redirection will be removed in a future version."),
-                          DeprecationWarning, stacklevel=2)
-            learner = 'ml_l'
-        super(DoubleMLPLR, self).set_ml_nuisance_params(learner, treat_var, params)
-
     def _nuisance_est(self, smpls, n_jobs_cv, return_models=False):
         x, y = check_X_y(self._dml_data.x, self._dml_data.y,
                          force_all_finite=False)
         x, d = check_X_y(x, self._dml_data.d,
                          force_all_finite=False)
 
         # nuisance l
@@ -248,47 +240,41 @@
             assert callable(self.score)
             psi_a, psi_b = self.score(y=y, d=d,
                                       l_hat=l_hat, m_hat=m_hat, g_hat=g_hat,
                                       smpls=smpls)
 
         return psi_a, psi_b
 
-    # To be removed in version 0.6.0
-    def tune(self,
-             param_grids,
-             tune_on_folds=False,
-             scoring_methods=None,  # if None the estimator's score method is used
-             n_folds_tune=5,
-             search_mode='grid_search',
-             n_iter_randomized_search=100,
-             n_jobs_cv=None,
-             set_as_params=True,
-             return_tune_res=False):
-
-        if isinstance(self.score, str) and (self.score == 'partialling out') and (param_grids is not None) and \
-                ('ml_g' in param_grids) and ('ml_l' not in param_grids):
-            warnings.warn(("Learner ml_g was renamed to ml_l. "
-                           "Please adapt the key of param_grids accordingly. "
-                           "The provided param_grids for ml_g are set for ml_l. "
-                           "The redirection will be removed in a future version."),
-                          DeprecationWarning, stacklevel=2)
-            param_grids['ml_l'] = param_grids.pop('ml_g')
-
-        if isinstance(self.score, str) and (self.score == 'partialling out') and (scoring_methods is not None) and \
-                ('ml_g' in scoring_methods) and ('ml_l' not in scoring_methods):
-            warnings.warn(("Learner ml_g was renamed to ml_l. "
-                           "Please adapt the key of scoring_methods accordingly. "
-                           "The provided scoring_methods for ml_g are set for ml_l. "
-                           "The redirection will be removed in a future version."),
-                          DeprecationWarning, stacklevel=2)
-            scoring_methods['ml_l'] = scoring_methods.pop('ml_g')
-
-        tune_res = super(DoubleMLPLR, self).tune(param_grids, tune_on_folds, scoring_methods, n_folds_tune, search_mode,
-                                                 n_iter_randomized_search, n_jobs_cv, set_as_params, return_tune_res)
-        return tune_res
+    def _sensitivity_element_est(self, preds):
+        # set elments for readability
+        y = self._dml_data.y
+        d = self._dml_data.d
+
+        m_hat = preds['predictions']['ml_m']
+        theta = self.all_coef[self._i_treat, self._i_rep]
+
+        if self.score == 'partialling out':
+            l_hat = preds['predictions']['ml_l']
+            sigma2_score_element = np.square(y - l_hat - np.multiply(theta, d-m_hat))
+        else:
+            assert self.score == 'IV-type'
+            g_hat = preds['predictions']['ml_g']
+            sigma2_score_element = np.square(y - g_hat - np.multiply(theta, d))
+
+        sigma2 = np.mean(sigma2_score_element)
+        psi_sigma2 = sigma2_score_element - sigma2
+
+        nu2 = np.divide(1.0, np.mean(np.square(d - m_hat)))
+        psi_nu2 = nu2 - np.multiply(np.square(d-m_hat), np.square(nu2))
+
+        element_dict = {'sigma2': sigma2,
+                        'nu2': nu2,
+                        'psi_sigma2': psi_sigma2,
+                        'psi_nu2': psi_nu2}
+        return element_dict
 
     def _nuisance_tuning(self, smpls, param_grids, scoring_methods, n_folds_tune, n_jobs_cv,
                          search_mode, n_iter_randomized_search):
         x, y = check_X_y(self._dml_data.x, self._dml_data.y,
                          force_all_finite=False)
         x, d = check_X_y(x, self._dml_data.d,
                          force_all_finite=False)
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_qte.py` & `DoubleML-0.6.2/doubleml/double_ml_qte.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 import pandas as pd
 from scipy.stats import norm
 
 from sklearn.base import clone
 
 from joblib import Parallel, delayed
 
-from ._utils import _draw_weights, _check_zero_one_treatment, _check_score, _check_trimming, _default_kde
-from ._utils_resampling import DoubleMLResampling
 from .double_ml_data import DoubleMLData, DoubleMLClusterData
 from .double_ml_pq import DoubleMLPQ
 from .double_ml_lpq import DoubleMLLPQ
 from .double_ml_cvar import DoubleMLCVAR
 
+from ._utils import _draw_weights, _default_kde
+from ._utils_resampling import DoubleMLResampling
+from ._utils_checks import _check_score, _check_trimming, _check_zero_one_treatment
+
 
 class DoubleMLQTE:
     """Double machine learning for quantile treatment effects
 
     Parameters
     ----------
     obj_dml_data : :class:`DoubleMLData` object
```

### Comparing `DoubleML-0.6.1/doubleml/double_ml_score_mixins.py` & `DoubleML-0.6.2/doubleml/double_ml_score_mixins.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils.py` & `DoubleML-0.6.2/doubleml/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_blp_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_blp_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_boot.py` & `DoubleML-0.6.2/doubleml/tests/_utils_boot.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_cluster.py` & `DoubleML-0.6.2/doubleml/tests/_utils_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_cvar_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_cvar_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_did_cs_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_did_cs_manual.py`

 * *Files 16% similar despite different names*

```diff
@@ -272,7 +272,93 @@
         m_best_params = [xx.best_params_ for xx in m_tune_res]
     else:
         assert score == 'experimental'
         m_best_params = None
 
     return g_d0_t0_best_params, g_d0_t1_best_params, \
         g_d1_t0_best_params, g_d1_t1_best_params, m_best_params
+
+
+def fit_sensitivity_elements_did_cs(y, d, t, all_coef, predictions, score, in_sample_normalization, n_rep):
+    n_treat = 1
+    n_obs = len(y)
+
+    sigma2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    nu2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    psi_sigma2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+    psi_nu2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+
+    for i_rep in range(n_rep):
+
+        m_hat = predictions['ml_m'][:, i_rep, 0]
+        g_hat_d0_t0 = predictions['ml_g_d0_t0'][:, i_rep, 0]
+        g_hat_d0_t1 = predictions['ml_g_d0_t1'][:, i_rep, 0]
+        g_hat_d1_t0 = predictions['ml_g_d1_t0'][:, i_rep, 0]
+        g_hat_d1_t1 = predictions['ml_g_d1_t1'][:, i_rep, 0]
+
+        d0t0 = np.multiply(1.0-d, 1.0-t)
+        d0t1 = np.multiply(1.0-d, t)
+        d1t0 = np.multiply(d, 1.0-t)
+        d1t1 = np.multiply(d, t)
+
+        g_hat = np.multiply(d0t0, g_hat_d0_t0) + np.multiply(d0t1, g_hat_d0_t1) + \
+            np.multiply(d1t0, g_hat_d1_t0) + np.multiply(d1t1, g_hat_d1_t1)
+        sigma2_score_element = np.square(y - g_hat)
+        sigma2[0, i_rep, 0] = np.mean(sigma2_score_element)
+        psi_sigma2[:, i_rep, 0] = sigma2_score_element - sigma2[0, i_rep, 0]
+
+        p_hat = np.mean(d)
+        lambda_hat = np.mean(t)
+        if score == 'observational':
+            propensity_weight_d0 = np.divide(m_hat, 1.0-m_hat)
+            if in_sample_normalization:
+                weight_d0t1 = np.multiply(d0t1, propensity_weight_d0)
+                weight_d0t0 = np.multiply(d0t0, propensity_weight_d0)
+                m_alpha_1 = np.divide(1.0, np.mean(d1t1)) + \
+                    np.divide(1.0, np.mean(d1t0)) + \
+                    np.divide(propensity_weight_d0, np.mean(weight_d0t1)) + \
+                    np.divide(propensity_weight_d0, np.mean(weight_d0t0))
+                m_alpha = np.multiply(np.divide(d, p_hat), m_alpha_1)
+                rr = np.divide(d1t1, np.mean(d1t1)) - \
+                    np.divide(d1t0, np.mean(d1t0)) - \
+                    np.divide(weight_d0t1, np.mean(weight_d0t1)) + \
+                    np.divide(weight_d0t0, np.mean(weight_d0t0))
+            else:
+                m_alpha_1 = np.divide(1.0, np.multiply(p_hat, lambda_hat)) + \
+                    np.divide(1.0, np.multiply(p_hat, 1.0-lambda_hat)) + \
+                    np.divide(propensity_weight_d0, np.multiply(p_hat, lambda_hat)) + \
+                    np.divide(propensity_weight_d0, np.multiply(p_hat, 1.0-lambda_hat))
+                m_alpha = np.multiply(np.divide(d, p_hat), m_alpha_1)
+                rr = np.divide(d1t1, np.multiply(p_hat, lambda_hat)) - \
+                    np.divide(d1t0, np.multiply(p_hat, 1.0-lambda_hat)) - \
+                    np.multiply(np.divide(d0t1, np.multiply(p_hat, lambda_hat)), propensity_weight_d0) + \
+                    np.multiply(np.divide(d0t0, np.multiply(p_hat, 1.0-lambda_hat)), propensity_weight_d0)
+        else:
+            assert score == 'experimental'
+            if in_sample_normalization:
+                m_alpha = np.divide(1.0, np.mean(d1t1)) + \
+                    np.divide(1.0, np.mean(d1t0)) + \
+                    np.divide(1.0, np.mean(d0t1)) + \
+                    np.divide(1.0, np.mean(d0t0))
+                rr = np.divide(d1t1, np.mean(d1t1)) - \
+                    np.divide(d1t0, np.mean(d1t0)) - \
+                    np.divide(d0t1, np.mean(d0t1)) + \
+                    np.divide(d0t0, np.mean(d0t0))
+            else:
+                m_alpha = np.divide(1.0, np.multiply(p_hat, lambda_hat)) + \
+                    np.divide(1.0, np.multiply(p_hat, 1.0-lambda_hat)) + \
+                    np.divide(1.0, np.multiply(1.0-p_hat, lambda_hat)) + \
+                    np.divide(1.0, np.multiply(1.0-p_hat, 1.0-lambda_hat))
+                rr = np.divide(d1t1, np.multiply(p_hat, lambda_hat)) - \
+                    np.divide(d1t0, np.multiply(p_hat, 1.0-lambda_hat)) - \
+                    np.divide(d0t1, np.multiply(1.0-p_hat, lambda_hat)) + \
+                    np.divide(d0t0, np.multiply(1.0-p_hat, 1.0-lambda_hat))
+
+        nu2_score_element = np.multiply(2.0, m_alpha) - np.square(rr)
+        nu2[0, i_rep, 0] = np.mean(nu2_score_element)
+        psi_nu2[:, i_rep, 0] = nu2_score_element - nu2[0, i_rep, 0]
+
+    element_dict = {'sigma2': sigma2,
+                    'nu2': nu2,
+                    'psi_sigma2': psi_sigma2,
+                    'psi_nu2': psi_nu2}
+    return element_dict
```

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_did_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_did_manual.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,30 +65,25 @@
                      trimming_threshold=1e-12):
     ml_g0 = clone(learner_g)
     ml_g1 = clone(learner_g)
     train_cond0 = np.where(d == 0)[0]
     g_hat0_list = fit_predict(y, x, ml_g0, g0_params, smpls,
                               train_cond=train_cond0)
 
+    train_cond1 = np.where(d == 1)[0]
+    g_hat1_list = fit_predict(y, x, ml_g1, g1_params, smpls,
+                              train_cond=train_cond1)
     if score == 'experimental':
-        train_cond1 = np.where(d == 1)[0]
-        g_hat1_list = fit_predict(y, x, ml_g1, g1_params, smpls,
-                                  train_cond=train_cond1)
         m_hat_list = list()
         for idx, _ in enumerate(smpls):
             # fill it up, but its not further used
             m_hat_list.append(np.zeros_like(g_hat0_list[idx], dtype='float64'))
 
     else:
         assert score == 'observational'
-        g_hat1_list = list()
-        for idx, _ in enumerate(smpls):
-            # fill it up, but its not further used
-            g_hat1_list.append(np.zeros_like(g_hat0_list[idx], dtype='float64'))
-
         ml_m = clone(learner_m)
         m_hat_list = fit_predict_proba(d, x, ml_m, m_params, smpls,
                                        trimming_threshold=trimming_threshold)
 
     p_hat_list = []
     for (train_index, _) in smpls:
         p_hat_list.append(np.mean(d[train_index]))
@@ -220,21 +215,69 @@
 
 def tune_nuisance_did(y, x, d, ml_g, ml_m, smpls, score, n_folds_tune,
                       param_grid_g, param_grid_m):
     train_cond0 = np.where(d == 0)[0]
     g0_tune_res = tune_grid_search(y, x, ml_g, smpls, param_grid_g, n_folds_tune,
                                    train_cond=train_cond0)
     g0_best_params = [xx.best_params_ for xx in g0_tune_res]
+
+    train_cond1 = np.where(d == 1)[0]
+    g1_tune_res = tune_grid_search(y, x, ml_g, smpls, param_grid_g, n_folds_tune,
+                                   train_cond=train_cond1)
+    g1_best_params = [xx.best_params_ for xx in g1_tune_res]
+
     if score == 'experimental':
-        train_cond1 = np.where(d == 1)[0]
-        g1_tune_res = tune_grid_search(y, x, ml_g, smpls, param_grid_g, n_folds_tune,
-                                       train_cond=train_cond1)
-        g1_best_params = [xx.best_params_ for xx in g1_tune_res]
         m_best_params = None
     else:
         assert score == 'observational'
-        g1_best_params = None
-
         m_tune_res = tune_grid_search(d, x, ml_m, smpls, param_grid_m, n_folds_tune)
         m_best_params = [xx.best_params_ for xx in m_tune_res]
 
     return g0_best_params, g1_best_params, m_best_params
+
+
+def fit_sensitivity_elements_did(y, d, all_coef, predictions, score, in_sample_normalization, n_rep):
+    n_treat = 1
+    n_obs = len(y)
+
+    sigma2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    nu2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    psi_sigma2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+    psi_nu2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+
+    for i_rep in range(n_rep):
+
+        m_hat = predictions['ml_m'][:, i_rep, 0]
+        g_hat0 = predictions['ml_g0'][:, i_rep, 0]
+        g_hat1 = predictions['ml_g1'][:, i_rep, 0]
+
+        sigma2_score_element = np.square(y - np.multiply(d, g_hat1) - np.multiply(1.0-d, g_hat0))
+        sigma2[0, i_rep, 0] = np.mean(sigma2_score_element)
+        psi_sigma2[:, i_rep, 0] = sigma2_score_element - sigma2[0, i_rep, 0]
+
+        if score == 'observational':
+            propensity_weight_d0 = np.divide(m_hat, 1.0-m_hat)
+            if in_sample_normalization:
+                m_alpha_1 = np.divide(d, np.mean(d))
+                m_alpha_2 = np.divide(1, np.mean(d)) + \
+                    np.divide(propensity_weight_d0, np.mean(np.multiply(1.0-d, propensity_weight_d0)))
+                m_alpha = np.multiply(m_alpha_1, m_alpha_2)
+                rr_1 = np.multiply(1.0-d, propensity_weight_d0)
+                rr = np.divide(d, np.mean(d)) - np.divide(rr_1, np.mean(rr_1))
+            else:
+                m_alpha_1 = np.divide(d, np.square(np.mean(d)))
+                m_alpha = np.multiply(m_alpha_1, 1.0+propensity_weight_d0)
+                rr = np.divide(d, np.mean(d)) - np.multiply(np.divide(1.0-d, np.mean(d)), propensity_weight_d0)
+        else:
+            assert score == 'experimental'
+            m_alpha = np.divide(1.0, np.mean(d)) + np.divide(1.0, 1.0-np.mean(d))
+            rr = np.divide(d, np.mean(d)) - np.divide(1.0-d, 1.0-np.mean(d))
+
+        nu2_score_element = np.multiply(2.0, m_alpha) - np.square(rr)
+        nu2[0, i_rep, 0] = np.mean(nu2_score_element)
+        psi_nu2[:, i_rep, 0] = nu2_score_element - nu2[0, i_rep, 0]
+
+    element_dict = {'sigma2': sigma2,
+                    'nu2': nu2,
+                    'psi_sigma2': psi_sigma2,
+                    'psi_nu2': psi_nu2}
+    return element_dict
```

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_dml_cv_predict.py` & `DoubleML-0.6.2/doubleml/tests/_utils_dml_cv_predict.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_iivm_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_iivm_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_irm_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_irm_manual.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from sklearn.base import clone, is_classifier
 
 from ._utils_boot import boot_manual, draw_weights
 from ._utils import fit_predict, fit_predict_proba, tune_grid_search
 
-from .._utils import _check_is_propensity, _normalize_ipw
+from .._utils import _normalize_ipw
+from .._utils_checks import _check_is_propensity
 
 
 def fit_irm(y, x, d,
             learner_g, learner_m, all_smpls, dml_procedure, score,
             n_rep=1, g0_params=None, g1_params=None, m_params=None,
             normalize_ipw=True, trimming_threshold=1e-2):
     n_obs = len(y)
@@ -62,28 +63,21 @@
     if is_classifier(learner_g):
         g_hat0_list = fit_predict_proba(y, x, ml_g0, g0_params, smpls,
                                         train_cond=train_cond0)
     else:
         g_hat0_list = fit_predict(y, x, ml_g0, g0_params, smpls,
                                   train_cond=train_cond0)
 
-    if score == 'ATE':
-        train_cond1 = np.where(d == 1)[0]
-        if is_classifier(learner_g):
-            g_hat1_list = fit_predict_proba(y, x, ml_g1, g1_params, smpls,
-                                            train_cond=train_cond1)
-        else:
-            g_hat1_list = fit_predict(y, x, ml_g1, g1_params, smpls,
-                                      train_cond=train_cond1)
+    train_cond1 = np.where(d == 1)[0]
+    if is_classifier(learner_g):
+        g_hat1_list = fit_predict_proba(y, x, ml_g1, g1_params, smpls,
+                                        train_cond=train_cond1)
     else:
-        assert score == 'ATTE'
-        g_hat1_list = list()
-        for idx, _ in enumerate(smpls):
-            # fill it up, but its not further used
-            g_hat1_list.append(np.zeros_like(g_hat0_list[idx], dtype='float64'))
+        g_hat1_list = fit_predict(y, x, ml_g1, g1_params, smpls,
+                                  train_cond=train_cond1)
 
     ml_m = clone(learner_m)
     m_hat_list = fit_predict_proba(d, x, ml_m, m_params, smpls,
                                    trimming_threshold=trimming_threshold)
 
     p_hat_list = []
     for (_, test_index) in smpls:
@@ -94,25 +88,22 @@
 
 def tune_nuisance_irm(y, x, d, ml_g, ml_m, smpls, score, n_folds_tune,
                       param_grid_g, param_grid_m):
     train_cond0 = np.where(d == 0)[0]
     g0_tune_res = tune_grid_search(y, x, ml_g, smpls, param_grid_g, n_folds_tune,
                                    train_cond=train_cond0)
 
-    if score == 'ATE':
-        train_cond1 = np.where(d == 1)[0]
-        g1_tune_res = tune_grid_search(y, x, ml_g, smpls, param_grid_g, n_folds_tune,
-                                       train_cond=train_cond1)
-        g1_best_params = [xx.best_params_ for xx in g1_tune_res]
-    else:
-        g1_best_params = None
+    train_cond1 = np.where(d == 1)[0]
+    g1_tune_res = tune_grid_search(y, x, ml_g, smpls, param_grid_g, n_folds_tune,
+                                   train_cond=train_cond1)
 
     m_tune_res = tune_grid_search(d, x, ml_m, smpls, param_grid_m, n_folds_tune)
 
     g0_best_params = [xx.best_params_ for xx in g0_tune_res]
+    g1_best_params = [xx.best_params_ for xx in g1_tune_res]
     m_best_params = [xx.best_params_ for xx in m_tune_res]
 
     return g0_best_params, g1_best_params, m_best_params
 
 
 def compute_iivm_residuals(y, g_hat0_list, g_hat1_list, m_hat_list, p_hat_list, smpls):
     u_hat0 = np.full_like(y, np.nan, dtype='float64')
@@ -280,7 +271,49 @@
             - np.divide(np.multiply(m_hat, np.multiply(1.-d, u_hat0)),
                         np.multiply(p_hat, (1.-m_hat))) \
             - theta * np.divide(d, p_hat)
 
     boot_theta, boot_t_stat = boot_manual(psi, J, smpls, se, weights, n_rep_boot, apply_cross_fitting)
 
     return boot_theta, boot_t_stat
+
+
+def fit_sensitivity_elements_irm(y, d, all_coef, predictions, score, n_rep):
+    n_treat = 1
+    n_obs = len(y)
+
+    sigma2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    nu2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    psi_sigma2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+    psi_nu2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+
+    for i_rep in range(n_rep):
+
+        m_hat = predictions['ml_m'][:, i_rep, 0]
+        g_hat0 = predictions['ml_g0'][:, i_rep, 0]
+        g_hat1 = predictions['ml_g1'][:, i_rep, 0]
+
+        if score == 'ATE':
+            weights = np.ones_like(d)
+            weights_bar = np.ones_like(d)
+        else:
+            assert score == 'ATTE'
+            weights = np.divide(d, np.mean(d))
+            weights_bar = np.divide(m_hat, np.mean(d))
+
+        sigma2_score_element = np.square(y - np.multiply(d, g_hat1) - np.multiply(1.0-d, g_hat0))
+        sigma2[0, i_rep, 0] = np.mean(sigma2_score_element)
+        psi_sigma2[:, i_rep, 0] = sigma2_score_element - sigma2[0, i_rep, 0]
+
+        # calc m(W,alpha) and Riesz representer
+        m_alpha = np.multiply(weights, np.multiply(weights_bar, (np.divide(1.0, m_hat) + np.divide(1.0, 1.0-m_hat))))
+        rr = np.multiply(weights_bar, (np.divide(d, m_hat) - np.divide(1.0-d, 1.0-m_hat)))
+
+        nu2_score_element = np.multiply(2.0, m_alpha) - np.square(rr)
+        nu2[0, i_rep, 0] = np.mean(nu2_score_element)
+        psi_nu2[:, i_rep, 0] = nu2_score_element - nu2[0, i_rep, 0]
+
+    element_dict = {'sigma2': sigma2,
+                    'nu2': nu2,
+                    'psi_sigma2': psi_sigma2,
+                    'psi_nu2': psi_nu2}
+    return element_dict
```

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_lpq_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_lpq_manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .._utils import _dml_cv_predict, _trimm, _default_kde, _normalize_ipw, _get_bracket_guess, _solve_ipw_score
 
 
 def fit_lpq(y, x, d, z, quantile,
             learner_g, learner_m, all_smpls, treatment, dml_procedure, n_rep=1,
             trimming_rule='truncate',
             trimming_threshold=1e-2,
+            kde=_default_kde,
             normalize_ipw=True, m_z_params=None,
             m_d_z0_params=None, m_d_z1_params=None,
             g_du_z0_params=None, g_du_z1_params=None):
     n_obs = len(y)
 
     lpqs = np.zeros(n_rep)
     ses = np.zeros(n_rep)
@@ -33,18 +34,18 @@
                                                                    m_z_params=m_z_params,
                                                                    m_d_z0_params=m_d_z0_params,
                                                                    m_d_z1_params=m_d_z1_params,
                                                                    g_du_z0_params=g_du_z0_params,
                                                                    g_du_z1_params=g_du_z1_params)
         if dml_procedure == 'dml1':
             lpqs[i_rep], ses[i_rep] = lpq_dml1(y, d, z, m_z_hat, g_du_z0_hat, g_du_z1_hat, comp_prob_hat,
-                                               treatment, quantile, ipw_vec, coef_bounds, smpls)
+                                               treatment, quantile, ipw_vec, coef_bounds, smpls, kde)
         else:
             lpqs[i_rep], ses[i_rep] = lpq_dml2(y, d, z, m_z_hat, g_du_z0_hat, g_du_z1_hat, comp_prob_hat,
-                                               treatment, quantile, ipw_vec, coef_bounds)
+                                               treatment, quantile, ipw_vec, coef_bounds, kde)
 
     lpq = np.median(lpqs)
     se = np.sqrt(np.median(np.power(ses, 2) * n_obs + np.power(lpqs - lpq, 2)) / n_obs)
 
     res = {'lpq': lpq, 'se': se,
            'lpqs': lpqs, 'ses': ses}
 
@@ -196,36 +197,36 @@
     # estimate final nuisance parameter
     comp_prob_hat = np.mean(m_d_z1_hat - m_d_z0_hat
                             + z / m_z_hat * (d - m_d_z1_hat)
                             - (1 - z) / (1 - m_z_hat) * (d - m_d_z0_hat))
     return m_z_hat, g_du_z0_hat, g_du_z1_hat, comp_prob_hat, ipw_vec, coef_bounds
 
 
-def lpq_dml1(y, d, z, m_z, g_du_z0, g_du_z1, comp_prob, treatment, quantile, ipw_vec, coef_bounds, smpls):
+def lpq_dml1(y, d, z, m_z, g_du_z0, g_du_z1, comp_prob, treatment, quantile, ipw_vec, coef_bounds, smpls, kde):
     thetas = np.zeros(len(smpls))
     n_obs = len(y)
     ipw_est = ipw_vec.mean()
     for idx, (_, test_index) in enumerate(smpls):
         thetas[idx] = lpq_est(m_z[test_index], g_du_z0[test_index], g_du_z1[test_index],
                               comp_prob, d[test_index], y[test_index], z[test_index], treatment, quantile,
                               ipw_est, coef_bounds)
 
     theta_hat = np.mean(thetas)
 
-    se = np.sqrt(lpq_var_est(theta_hat, m_z, g_du_z0, g_du_z1, comp_prob, d, y, z, treatment, quantile, n_obs))
+    se = np.sqrt(lpq_var_est(theta_hat, m_z, g_du_z0, g_du_z1, comp_prob, d, y, z, treatment, quantile, n_obs, kde))
 
     return theta_hat, se
 
 
-def lpq_dml2(y, d, z, m_z, g_du_z0, g_du_z1, comp_prob, treatment, quantile, ipw_vec, coef_bounds):
+def lpq_dml2(y, d, z, m_z, g_du_z0, g_du_z1, comp_prob, treatment, quantile, ipw_vec, coef_bounds, kde):
     n_obs = len(y)
     ipw_est = ipw_vec.mean()
     theta_hat = lpq_est(m_z, g_du_z0, g_du_z1, comp_prob, d, y, z, treatment, quantile, ipw_est, coef_bounds)
 
-    se = np.sqrt(lpq_var_est(theta_hat, m_z, g_du_z0, g_du_z1, comp_prob, d, y, z, treatment, quantile, n_obs))
+    se = np.sqrt(lpq_var_est(theta_hat, m_z, g_du_z0, g_du_z1, comp_prob, d, y, z, treatment, quantile, n_obs, kde))
 
     return theta_hat, se
 
 
 def lpq_est(m_z, g_du_z0, g_du_z1, comp_prob, d, y, z, treatment, quantile, ipw_est, coef_bounds):
 
     def compute_score(coef):
```

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_pliv_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_pliv_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_x_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_x_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_xz_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_xz_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_pliv_partial_z_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_z_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_plr_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_plr_manual.py`

 * *Files 11% similar despite different names*

```diff
@@ -336,7 +336,43 @@
     else:
         assert score == 'IV-type'
         psi = np.multiply(y_minus_g_hat - d * theta, d_minus_m_hat)
 
     boot_theta, boot_t_stat = boot_manual(psi, J, smpls, se, weights, n_rep, apply_cross_fitting)
 
     return boot_theta, boot_t_stat
+
+
+def fit_sensitivity_elements_plr(y, d, all_coef, predictions, score, n_rep):
+    n_treat = d.shape[1]
+    n_obs = len(y)
+
+    sigma2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    nu2 = np.full(shape=(1, n_rep, n_treat), fill_value=np.nan)
+    psi_sigma2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+    psi_nu2 = np.full(shape=(n_obs, n_rep, n_treat), fill_value=np.nan)
+
+    for i_rep in range(n_rep):
+        for i_treat in range(n_treat):
+            d_tilde = d[:, i_treat]
+            m_hat = predictions['ml_m'][:, i_rep, i_treat]
+            theta = all_coef[i_treat, i_rep]
+            if score == 'partialling out':
+                l_hat = predictions['ml_l'][:, i_rep, i_treat]
+                sigma2_score_element = np.square(y - l_hat - np.multiply(theta, d_tilde-m_hat))
+            else:
+                assert score == 'IV-type'
+                g_hat = predictions['ml_g'][:, i_rep, i_treat]
+                sigma2_score_element = np.square(y - g_hat - np.multiply(theta, d_tilde))
+
+            sigma2[0, i_rep, i_treat] = np.mean(sigma2_score_element)
+            psi_sigma2[:, i_rep, i_treat] = sigma2_score_element - sigma2[0, i_rep, i_treat]
+
+            nu2[0, i_rep, i_treat] = np.divide(1.0, np.mean(np.square(d_tilde-m_hat)))
+            psi_nu2[:, i_rep, i_treat] = nu2[0, i_rep, i_treat] - \
+                np.multiply(np.square(d_tilde-m_hat), np.square(nu2[0, i_rep, i_treat]))
+
+    element_dict = {'sigma2': sigma2,
+                    'nu2': nu2,
+                    'psi_sigma2': psi_sigma2,
+                    'psi_nu2': psi_nu2}
+    return element_dict
```

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_pq_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_pq_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/_utils_qte_manual.py` & `DoubleML-0.6.2/doubleml/tests/_utils_qte_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/conftest.py` & `DoubleML-0.6.2/doubleml/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_blp.py` & `DoubleML-0.6.2/doubleml/tests/test_blp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import pytest
+import copy
 
 import doubleml as dml
 
 from ._utils_blp_manual import fit_blp, blp_confint
 
 
 @pytest.fixture(scope='module',
@@ -22,15 +23,18 @@
 @pytest.fixture(scope='module')
 def dml_blp_fixture(ci_joint, ci_level):
     n = 50
     np.random.seed(42)
     random_basis = pd.DataFrame(np.random.normal(0, 1, size=(n, 3)))
     random_signal = np.random.normal(0, 1, size=(n, ))
 
-    blp = dml.DoubleMLBLP(random_signal, random_basis).fit()
+    blp = dml.DoubleMLBLP(random_signal, random_basis)
+
+    blp_obj = copy.copy(blp)
+    blp.fit()
     blp_manual = fit_blp(random_signal, random_basis)
 
     np.random.seed(42)
     ci_1 = blp.confint(random_basis, joint=ci_joint, level=ci_level, n_rep_boot=1000)
     np.random.seed(42)
     ci_2 = blp.confint(joint=ci_joint, level=ci_level, n_rep_boot=1000)
     np.random.seed(42)
@@ -43,15 +47,16 @@
                 'omega': blp.blp_omega,
                 'omega_manual': blp_manual.cov_HC0,
                 'basis': blp.basis,
                 'signal': blp.orth_signal,
                 'ci_1': ci_1,
                 'ci_2': ci_2,
                 'ci_manual': ci_manual,
-                'blp_model': blp}
+                'blp_model': blp,
+                'unfitted_blp_model': blp_obj}
 
     return res_dict
 
 
 @pytest.mark.ci
 def test_dml_blp_coef(dml_blp_fixture):
     assert np.allclose(dml_blp_fixture['coef'],
@@ -87,14 +92,15 @@
                        rtol=1e-9, atol=1e-4)
 
 
 @pytest.mark.ci
 def test_dml_blp_return_types(dml_blp_fixture):
     assert isinstance(dml_blp_fixture['blp_model'].__str__(), str)
     assert isinstance(dml_blp_fixture['blp_model'].summary, pd.DataFrame)
+    assert isinstance(dml_blp_fixture['unfitted_blp_model'].summary, pd.DataFrame)
 
 
 @pytest.mark.ci
 def test_doubleml_exception_blp():
     random_basis = pd.DataFrame(np.random.normal(0, 1, size=(2, 3)))
     signal = np.array([1, 2])
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_cv_predict.py` & `DoubleML-0.6.2/doubleml/tests/test_cv_predict.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_cvar.py` & `DoubleML-0.6.2/doubleml/tests/test_cvar.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_cvar_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_cvar_tune.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import numpy as np
 import pytest
 import math
 
 from sklearn.base import clone
-
-from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 
 import doubleml as dml
 
 from ._utils import draw_smpls
 from ._utils_cvar_manual import fit_cvar, tune_nuisance_cvar
 
@@ -54,17 +52,14 @@
 def tune_on_folds(request):
     return request.param
 
 
 def get_par_grid(learner):
     if learner.__class__ in [RandomForestRegressor, RandomForestClassifier]:
         par_grid = {'n_estimators': [5, 10, 15, 20]}
-    else:
-        assert learner.__class__ in [LogisticRegression]
-        par_grid = {'C': np.logspace(-4, 2, 10)}
     return par_grid
 
 
 @pytest.fixture(scope='module')
 def dml_cvar_fixture(generate_data_quantiles, treatment, quantile, learner_g, learner_m, dml_procedure,
                      normalize_ipw, tune_on_folds):
     par_grid = {'ml_g': get_par_grid(learner_g),
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_datasets.py` & `DoubleML-0.6.2/doubleml/tests/test_datasets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import pandas as pd
 import numpy as np
 
 from doubleml import DoubleMLData, DoubleMLClusterData
 from doubleml.datasets import fetch_401K, fetch_bonus, make_plr_CCDDHNR2018, make_plr_turrell2018, \
     make_irm_data, make_iivm_data, _make_pliv_data, make_pliv_CHS2015, make_pliv_multiway_cluster_CKMS2021, \
-    make_did_SZ2020
+    make_did_SZ2020, make_confounded_irm_data, make_confounded_plr_data
 
 msg_inv_return_type = 'Invalid return_type.'
 
 
 def test_fetch_401K_return_types():
     res = fetch_401K('DoubleMLData')
     assert isinstance(res, DoubleMLData)
@@ -180,7 +180,50 @@
     assert isinstance(y, np.ndarray)
     assert isinstance(d, np.ndarray)
     with pytest.raises(ValueError, match=msg_inv_return_type):
         _ = make_did_SZ2020(n_obs=100, dgp_type=dgp_type, cross_sectional_data=cross_sectional, return_type='matrix')
     msg = 'The dgp_type is not valid.'
     with pytest.raises(ValueError, match=msg):
         _ = make_did_SZ2020(n_obs=100, dgp_type="5", cross_sectional_data=cross_sectional, return_type='matrix')
+
+
+@pytest.mark.ci
+def test_make_confounded_irm_data_return_types():
+    np.random.seed(3141)
+    res = make_confounded_irm_data()
+    assert isinstance(res, dict)
+    assert isinstance(res['x'], np.ndarray)
+    assert isinstance(res['y'], np.ndarray)
+    assert isinstance(res['d'], np.ndarray)
+
+    assert isinstance(res['oracle_values'], dict)
+    assert isinstance(res['oracle_values']['g_long'], np.ndarray)
+    assert isinstance(res['oracle_values']['g_short'], np.ndarray)
+    assert isinstance(res['oracle_values']['m_long'], np.ndarray)
+    assert isinstance(res['oracle_values']['m_short'], np.ndarray)
+    assert isinstance(res['oracle_values']['gamma_a'], float)
+    assert isinstance(res['oracle_values']['beta_a'], float)
+    assert isinstance(res['oracle_values']['a'], np.ndarray)
+    assert isinstance(res['oracle_values']['y0'], np.ndarray)
+    assert isinstance(res['oracle_values']['y1'], np.ndarray)
+    assert isinstance(res['oracle_values']['z'], np.ndarray)
+
+
+@pytest.mark.ci
+def test_make_confounded_plr_data_return_types():
+    np.random.seed(3141)
+    res = make_confounded_plr_data(theta=5.0)
+    assert isinstance(res, dict)
+    assert isinstance(res['x'], np.ndarray)
+    assert isinstance(res['y'], np.ndarray)
+    assert isinstance(res['d'], np.ndarray)
+
+    assert isinstance(res['oracle_values'], dict)
+    assert isinstance(res['oracle_values']['g_long'], np.ndarray)
+    assert isinstance(res['oracle_values']['g_short'], np.ndarray)
+    assert isinstance(res['oracle_values']['m_long'], np.ndarray)
+    assert isinstance(res['oracle_values']['m_short'], np.ndarray)
+    assert isinstance(res['oracle_values']['theta'], float)
+    assert isinstance(res['oracle_values']['gamma_a'], float)
+    assert isinstance(res['oracle_values']['beta_a'], float)
+    assert isinstance(res['oracle_values']['a'], np.ndarray)
+    assert isinstance(res['oracle_values']['z'], np.ndarray)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_did.py` & `DoubleML-0.6.2/doubleml/tests/test_iivm_subgroups.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,169 +1,156 @@
 import numpy as np
 import pytest
 import math
 
 from sklearn.base import clone
 
-from sklearn.linear_model import LogisticRegression, LinearRegression
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 
 import doubleml as dml
 
 from ._utils import draw_smpls
-from ._utils_did_manual import fit_did, boot_did
+from ._utils_iivm_manual import fit_iivm, boot_iivm
 
 
 @pytest.fixture(scope='module',
-                params=[[LinearRegression(),
-                         LogisticRegression(solver='lbfgs', max_iter=250)],
-                        [RandomForestRegressor(max_depth=5, n_estimators=10, random_state=42),
-                         RandomForestClassifier(max_depth=5, n_estimators=10, random_state=42)]])
+                params=[[RandomForestRegressor(max_depth=2, n_estimators=10),
+                         RandomForestClassifier(max_depth=2, n_estimators=10)]])
 def learner(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['observational', 'experimental'])
+                params=['LATE'])
 def score(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[True, False])
-def in_sample_normalization(request):
+                params=['dml1', 'dml2'])
+def dml_procedure(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['dml1', 'dml2'])
-def dml_procedure(request):
+                params=[True, False])
+def normalize_ipw(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[0.01, 0.05])
+                params=[0.01])
 def trimming_threshold(request):
     return request.param
 
 
-@pytest.fixture(scope='module')
-def dml_did_fixture(generate_data_did, learner, score, in_sample_normalization,
-                    dml_procedure, trimming_threshold):
+@pytest.fixture(scope='module',
+                params=[{'always_takers': True, 'never_takers': True},
+                        {'always_takers': False, 'never_takers': True},
+                        {'always_takers': True, 'never_takers': False}])
+def subgroups(request):
+    return request.param
+
+
+@pytest.fixture(scope="module")
+def dml_iivm_subgroups_fixture(generate_data_iivm, learner, score, dml_procedure, normalize_ipw,
+                               trimming_threshold, subgroups):
     boot_methods = ['normal']
     n_folds = 2
-    n_rep_boot = 499
+    n_rep_boot = 491
 
     # collect data
-    (x, y, d) = generate_data_did
+    data = generate_data_iivm
+    x_cols = data.columns[data.columns.str.startswith('X')].tolist()
 
     # Set machine learning methods for m & g
     ml_g = clone(learner[0])
     ml_m = clone(learner[1])
+    ml_r = clone(learner[1])
 
     np.random.seed(3141)
-    n_obs = len(y)
-    all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=d)
-    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
+    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'], x_cols, 'z')
+    dml_iivm_obj = dml.DoubleMLIIVM(obj_dml_data,
+                                    ml_g, ml_m, ml_r,
+                                    n_folds,
+                                    subgroups=subgroups,
+                                    dml_procedure=dml_procedure,
+                                    normalize_ipw=normalize_ipw,
+                                    trimming_threshold=trimming_threshold)
 
-    np.random.seed(3141)
-    dml_did_obj = dml.DoubleMLDID(obj_dml_data,
-                                  ml_g, ml_m,
-                                  n_folds,
-                                  score=score,
-                                  in_sample_normalization=in_sample_normalization,
-                                  dml_procedure=dml_procedure,
-                                  draw_sample_splitting=False,
-                                  trimming_threshold=trimming_threshold)
-
-    # synchronize the sample splitting
-    dml_did_obj.set_sample_splitting(all_smpls=all_smpls)
-    dml_did_obj.fit()
+    dml_iivm_obj.fit(store_predictions=True)
 
     np.random.seed(3141)
-    res_manual = fit_did(y, x, d,
-                         clone(learner[0]), clone(learner[1]),
-                         all_smpls, dml_procedure, score, in_sample_normalization,
-                         trimming_threshold=trimming_threshold)
+    y = data['y'].values
+    x = data.loc[:, x_cols].values
+    d = data['d'].values
+    z = data['z'].values
+    n_obs = len(y)
+    all_smpls = draw_smpls(n_obs, n_folds)
+
+    res_manual = fit_iivm(y, x, d, z,
+                          clone(learner[0]), clone(learner[1]), clone(learner[1]),
+                          all_smpls, dml_procedure, score,
+                          normalize_ipw=normalize_ipw, trimming_threshold=trimming_threshold,
+                          always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
 
-    res_dict = {'coef': dml_did_obj.coef,
+    res_dict = {'coef': dml_iivm_obj.coef,
                 'coef_manual': res_manual['theta'],
-                'se': dml_did_obj.se,
+                'se': dml_iivm_obj.se,
                 'se_manual': res_manual['se'],
-                'boot_methods': boot_methods}
+                'boot_methods': boot_methods,
+                'always_takers': subgroups['always_takers'],
+                'never_takers': subgroups['never_takers'],
+                'rhat0': dml_iivm_obj.predictions['ml_r0'],
+                'rhat1': dml_iivm_obj.predictions['ml_r1'],
+                'z': z
+                }
 
     for bootstrap in boot_methods:
         np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_did(y, res_manual['thetas'], res_manual['ses'],
-                                           res_manual['all_psi_a'], res_manual['all_psi_b'],
-                                           all_smpls, bootstrap, n_rep_boot)
+        boot_theta, boot_t_stat = boot_iivm(y, d, z, res_manual['thetas'], res_manual['ses'],
+                                            res_manual['all_g_hat0'], res_manual['all_g_hat1'],
+                                            res_manual['all_m_hat'], res_manual['all_r_hat0'], res_manual['all_r_hat1'],
+                                            all_smpls, score, bootstrap, n_rep_boot, dml_procedure,
+                                            normalize_ipw=normalize_ipw)
 
         np.random.seed(3141)
-        dml_did_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
-        res_dict['boot_coef' + bootstrap] = dml_did_obj.boot_coef
-        res_dict['boot_t_stat' + bootstrap] = dml_did_obj.boot_t_stat
+        dml_iivm_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
+        res_dict['boot_coef' + bootstrap] = dml_iivm_obj.boot_coef
+        res_dict['boot_t_stat' + bootstrap] = dml_iivm_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_did_coef(dml_did_fixture):
-    assert math.isclose(dml_did_fixture['coef'],
-                        dml_did_fixture['coef_manual'],
+def test_dml_iivm_subgroups_coef(dml_iivm_subgroups_fixture):
+    assert math.isclose(dml_iivm_subgroups_fixture['coef'],
+                        dml_iivm_subgroups_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_did_se(dml_did_fixture):
-    assert math.isclose(dml_did_fixture['se'],
-                        dml_did_fixture['se_manual'],
+def test_dml_iivm_subgroups_se(dml_iivm_subgroups_fixture):
+    assert math.isclose(dml_iivm_subgroups_fixture['se'],
+                        dml_iivm_subgroups_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_did_boot(dml_did_fixture):
-    for bootstrap in dml_did_fixture['boot_methods']:
-        assert np.allclose(dml_did_fixture['boot_coef' + bootstrap],
-                           dml_did_fixture['boot_coef' + bootstrap + '_manual'],
+def test_dml_iivm_subgroups_boot(dml_iivm_subgroups_fixture):
+    for bootstrap in dml_iivm_subgroups_fixture['boot_methods']:
+        assert np.allclose(dml_iivm_subgroups_fixture['boot_coef' + bootstrap],
+                           dml_iivm_subgroups_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-        assert np.allclose(dml_did_fixture['boot_t_stat' + bootstrap],
-                           dml_did_fixture['boot_t_stat' + bootstrap + '_manual'],
+        assert np.allclose(dml_iivm_subgroups_fixture['boot_t_stat' + bootstrap],
+                           dml_iivm_subgroups_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_did_experimental(generate_data_did, in_sample_normalization, learner):
-    # collect data
-    (x, y, d) = generate_data_did
-
-    # Set machine learning methods for m & g
-    ml_g = clone(learner[0])
-    ml_m = clone(learner[1])
-
-    np.random.seed(3141)
-    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
-
-    np.random.seed(3141)
-    dml_did_obj_without_ml_m = dml.DoubleMLDID(obj_dml_data,
-                                               ml_g,
-                                               score='experimental',
-                                               in_sample_normalization=in_sample_normalization)
-    dml_did_obj_without_ml_m.fit()
-
-    np.random.seed(3141)
-    dml_did_obj_with_ml_m = dml.DoubleMLDID(obj_dml_data,
-                                            ml_g, ml_m,
-                                            score='experimental',
-                                            in_sample_normalization=in_sample_normalization)
-    dml_did_obj_with_ml_m.fit()
-    assert math.isclose(dml_did_obj_with_ml_m.coef,
-                        dml_did_obj_without_ml_m.coef,
-                        rel_tol=1e-9, abs_tol=1e-4)
-
-    msg = ('A learner ml_m has been provided for score = "experimental" but will be ignored. '
-           'A learner ml_m is not required for estimation.')
-    with pytest.warns(UserWarning, match=msg):
-        dml.DoubleMLDID(obj_dml_data, ml_g, ml_m,
-                        score='experimental',
-                        in_sample_normalization=in_sample_normalization)
+def test_dml_iivm_subgroups(dml_iivm_subgroups_fixture):
+    if not dml_iivm_subgroups_fixture['always_takers']:
+        assert np.all(dml_iivm_subgroups_fixture['rhat0'] == 0)
+    if not dml_iivm_subgroups_fixture['never_takers']:
+        assert np.all(dml_iivm_subgroups_fixture['rhat1'] == 1)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_did_cs.py` & `DoubleML-0.6.2/doubleml/tests/test_iivm_tune.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,170 +1,200 @@
 import numpy as np
 import pytest
 import math
 
 from sklearn.base import clone
 
-from sklearn.linear_model import LogisticRegression, LinearRegression
+from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 
 import doubleml as dml
 
 from ._utils import draw_smpls
-from ._utils_did_cs_manual import fit_did_cs
-from ._utils_did_manual import boot_did
+from ._utils_iivm_manual import fit_iivm, boot_iivm, tune_nuisance_iivm
 
 
 @pytest.fixture(scope='module',
-                params=[[LinearRegression(),
-                         LogisticRegression(solver='lbfgs', max_iter=250)],
-                        [RandomForestRegressor(max_depth=5, n_estimators=10, random_state=42),
-                         RandomForestClassifier(max_depth=5, n_estimators=10, random_state=42)]])
-def learner(request):
+                params=[RandomForestRegressor()])
+def learner_g(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['observational', 'experimental'])
+                params=[RandomForestClassifier()])
+def learner_m(request):
+    return request.param
+
+
+@pytest.fixture(scope='module',
+                params=[LogisticRegression()])
+def learner_r(request):
+    return request.param
+
+
+@pytest.fixture(scope='module',
+                params=['LATE'])
 def score(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
+                params=['dml2'])
+def dml_procedure(request):
+    return request.param
+
+
+@pytest.fixture(scope='module',
                 params=[True, False])
-def in_sample_normalization(request):
+def normalize_ipw(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['dml1', 'dml2'])
-def dml_procedure(request):
+                params=[{'always_takers': True, 'never_takers': True},
+                        {'always_takers': False, 'never_takers': False}])
+def subgroups(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[0.01, 0.05])
-def trimming_threshold(request):
+                params=[True, False])
+def tune_on_folds(request):
     return request.param
 
 
-@pytest.fixture(scope='module')
-def dml_did_cs_fixture(generate_data_did_cs, learner, score, in_sample_normalization,
-                       dml_procedure, trimming_threshold):
+def get_par_grid(learner):
+    if learner.__class__ in [RandomForestRegressor, RandomForestClassifier]:
+        par_grid = {'n_estimators': [5, 10, 20]}
+    else:
+        assert learner.__class__ in [LogisticRegression]
+        par_grid = {'C': np.logspace(-4, 2, 10)}
+    return par_grid
+
+
+@pytest.fixture(scope="module")
+def dml_iivm_fixture(generate_data_iivm, learner_g, learner_m, learner_r, score, dml_procedure, normalize_ipw, subgroups,
+                     tune_on_folds):
+    par_grid = {'ml_g': get_par_grid(learner_g),
+                'ml_m': get_par_grid(learner_m),
+                'ml_r': get_par_grid(learner_r)}
+    n_folds_tune = 4
+
     boot_methods = ['normal']
     n_folds = 2
-    n_rep_boot = 499
+    n_rep_boot = 491
 
     # collect data
-    (x, y, d, t) = generate_data_did_cs
-
-    # Set machine learning methods for m & g
-    ml_g = clone(learner[0])
-    ml_m = clone(learner[1])
+    data = generate_data_iivm
+    x_cols = data.columns[data.columns.str.startswith('X')].tolist()
 
-    np.random.seed(3141)
+    # Set machine learning methods for m, g & r
+    ml_g = clone(learner_g)
+    ml_m = clone(learner_m)
+    ml_r = clone(learner_r)
+
+    np.random.seed(3141)
+    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'], x_cols, 'z')
+    dml_iivm_obj = dml.DoubleMLIIVM(obj_dml_data,
+                                    ml_g, ml_m, ml_r,
+                                    n_folds,
+                                    subgroups=subgroups,
+                                    dml_procedure=dml_procedure,
+                                    normalize_ipw=normalize_ipw)
+    # tune hyperparameters
+    tune_res = dml_iivm_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune,
+                                 return_tune_res=True)
+    assert isinstance(tune_res, list)
+
+    dml_iivm_obj.fit()
+
+    np.random.seed(3141)
+    y = data['y'].values
+    x = data.loc[:, x_cols].values
+    d = data['d'].values
+    z = data['z'].values
     n_obs = len(y)
-    all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=d)
-    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d, t=t)
+    all_smpls = draw_smpls(n_obs, n_folds)
+    smpls = all_smpls[0]
 
-    np.random.seed(3141)
-    dml_did_cs_obj = dml.DoubleMLDIDCS(obj_dml_data,
-                                       ml_g, ml_m,
-                                       n_folds,
-                                       score=score,
-                                       in_sample_normalization=in_sample_normalization,
-                                       dml_procedure=dml_procedure,
-                                       draw_sample_splitting=False,
-                                       trimming_threshold=trimming_threshold)
-
-    # synchronize the sample splitting
-    dml_did_cs_obj.set_sample_splitting(all_smpls=all_smpls)
-    dml_did_cs_obj.fit()
+    if tune_on_folds:
+        g0_params, g1_params, m_params,  r0_params, r1_params = \
+            tune_nuisance_iivm(y, x, d, z,
+                               clone(learner_g), clone(learner_m), clone(learner_r), smpls,
+                               n_folds_tune,
+                               par_grid['ml_g'], par_grid['ml_m'], par_grid['ml_r'],
+                               always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
+    else:
+        xx = [(np.arange(data.shape[0]), np.array([]))]
+        g0_params, g1_params, m_params,  r0_params, r1_params = \
+            tune_nuisance_iivm(y, x, d, z,
+                               clone(learner_g), clone(learner_m), clone(learner_r), xx,
+                               n_folds_tune,
+                               par_grid['ml_g'], par_grid['ml_m'], par_grid['ml_r'],
+                               always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
+        g0_params = g0_params * n_folds
+        g1_params = g1_params * n_folds
+        m_params = m_params * n_folds
+        if subgroups['always_takers']:
+            r0_params = r0_params * n_folds
+        else:
+            r0_params = r0_params
+        if subgroups['never_takers']:
+            r1_params = r1_params * n_folds
+        else:
+            r1_params = r1_params
+
+    res_manual = fit_iivm(y, x, d, z,
+                          clone(learner_g), clone(learner_m), clone(learner_r),
+                          all_smpls, dml_procedure, score,
+                          g0_params=g0_params, g1_params=g1_params,
+                          m_params=m_params, r0_params=r0_params, r1_params=r1_params,
+                          normalize_ipw=normalize_ipw,
+                          always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
 
-    np.random.seed(3141)
-    res_manual = fit_did_cs(y, x, d, t,
-                            clone(learner[0]), clone(learner[1]),
-                            all_smpls, dml_procedure, score, in_sample_normalization,
-                            trimming_threshold=trimming_threshold)
-
-    res_dict = {'coef': dml_did_cs_obj.coef,
+    res_dict = {'coef': dml_iivm_obj.coef,
                 'coef_manual': res_manual['theta'],
-                'se': dml_did_cs_obj.se,
+                'se': dml_iivm_obj.se,
                 'se_manual': res_manual['se'],
                 'boot_methods': boot_methods}
 
     for bootstrap in boot_methods:
         np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_did(y, res_manual['thetas'], res_manual['ses'],
-                                           res_manual['all_psi_a'], res_manual['all_psi_b'],
-                                           all_smpls, bootstrap, n_rep_boot)
+        boot_theta, boot_t_stat = boot_iivm(y, d, z, res_manual['thetas'], res_manual['ses'],
+                                            res_manual['all_g_hat0'], res_manual['all_g_hat1'],
+                                            res_manual['all_m_hat'], res_manual['all_r_hat0'], res_manual['all_r_hat1'],
+                                            all_smpls, score, bootstrap, n_rep_boot, dml_procedure,
+                                            normalize_ipw=normalize_ipw)
 
         np.random.seed(3141)
-        dml_did_cs_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
-        res_dict['boot_coef' + bootstrap] = dml_did_cs_obj.boot_coef
-        res_dict['boot_t_stat' + bootstrap] = dml_did_cs_obj.boot_t_stat
+        dml_iivm_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
+        res_dict['boot_coef' + bootstrap] = dml_iivm_obj.boot_coef
+        res_dict['boot_t_stat' + bootstrap] = dml_iivm_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_did_cs_coef(dml_did_cs_fixture):
-    assert math.isclose(dml_did_cs_fixture['coef'],
-                        dml_did_cs_fixture['coef_manual'],
+def test_dml_iivm_coef(dml_iivm_fixture):
+    assert math.isclose(dml_iivm_fixture['coef'],
+                        dml_iivm_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_did_cs_se(dml_did_cs_fixture):
-    assert math.isclose(dml_did_cs_fixture['se'],
-                        dml_did_cs_fixture['se_manual'],
+def test_dml_iivm_se(dml_iivm_fixture):
+    assert math.isclose(dml_iivm_fixture['se'],
+                        dml_iivm_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_did_cs_boot(dml_did_cs_fixture):
-    for bootstrap in dml_did_cs_fixture['boot_methods']:
-        assert np.allclose(dml_did_cs_fixture['boot_coef' + bootstrap],
-                           dml_did_cs_fixture['boot_coef' + bootstrap + '_manual'],
+def test_dml_iivm_boot(dml_iivm_fixture):
+    for bootstrap in dml_iivm_fixture['boot_methods']:
+        assert np.allclose(dml_iivm_fixture['boot_coef' + bootstrap],
+                           dml_iivm_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-        assert np.allclose(dml_did_cs_fixture['boot_t_stat' + bootstrap],
-                           dml_did_cs_fixture['boot_t_stat' + bootstrap + '_manual'],
+        assert np.allclose(dml_iivm_fixture['boot_t_stat' + bootstrap],
+                           dml_iivm_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-
-
-@pytest.mark.ci
-def test_dml_did_cs_experimental(generate_data_did_cs, in_sample_normalization, learner):
-    # collect data
-    (x, y, d, t) = generate_data_did_cs
-
-    # Set machine learning methods for m & g
-    ml_g = clone(learner[0])
-    ml_m = clone(learner[1])
-
-    np.random.seed(3141)
-    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d, t=t)
-
-    np.random.seed(3141)
-    dml_did_obj_without_ml_m = dml.DoubleMLDIDCS(obj_dml_data,
-                                                 ml_g,
-                                                 score='experimental',
-                                                 in_sample_normalization=in_sample_normalization)
-    dml_did_obj_without_ml_m.fit()
-
-    np.random.seed(3141)
-    dml_did_obj_with_ml_m = dml.DoubleMLDIDCS(obj_dml_data,
-                                              ml_g, ml_m,
-                                              score='experimental',
-                                              in_sample_normalization=in_sample_normalization)
-    dml_did_obj_with_ml_m.fit()
-    assert math.isclose(dml_did_obj_with_ml_m.coef,
-                        dml_did_obj_without_ml_m.coef,
-                        rel_tol=1e-9, abs_tol=1e-4)
-
-    msg = ('A learner ml_m has been provided for score = "experimental" but will be ignored. '
-           'A learner ml_m is not required for estimation.')
-    with pytest.warns(UserWarning, match=msg):
-        dml.DoubleMLDIDCS(obj_dml_data, ml_g, ml_m,
-                          score='experimental',
-                          in_sample_normalization=in_sample_normalization)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_did_cs_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_did_cs_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_did_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_did_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_dml_data.py` & `DoubleML-0.6.2/doubleml/tests/test_dml_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 import pytest
 import numpy as np
 import pandas as pd
 
 from doubleml import DoubleMLData, DoubleMLPLR, DoubleMLClusterData, DoubleMLDIDCS
 from doubleml.datasets import make_plr_CCDDHNR2018, _make_pliv_data, make_pliv_CHS2015,\
     make_pliv_multiway_cluster_CKMS2021, make_did_SZ2020
+from doubleml.double_ml_data import DoubleMLBaseData
+
 from sklearn.linear_model import Lasso, LogisticRegression
 
 
+class DummyDataClass(DoubleMLBaseData):
+    def __init__(self, data):
+        DoubleMLBaseData.__init__(self, data)
+
+    @property
+    def n_coefs(self):
+        return 1
+
+
+@pytest.mark.ci
+def test_doubleml_basedata():
+    dummy_dml_data = DummyDataClass(pd.DataFrame(np.zeros((100, 10))))
+    assert dummy_dml_data.d_cols[0] == 'theta'
+    assert dummy_dml_data.n_treat == 1
+    assert dummy_dml_data.n_coefs == 1
+
 @pytest.fixture(scope="module")
 def dml_data_fixture(generate_data1):
     data = generate_data1
     np.random.seed(3141)
     x_cols = data.columns[data.columns.str.startswith('X')].tolist()
 
     obj_from_np = DoubleMLData.from_arrays(data.loc[:, x_cols].values,
@@ -153,20 +171,30 @@
     dml_data = DoubleMLData.from_arrays(x, y, d)
     assert dml_data.z is None
     assert dml_data.n_instr == 0
     assert dml_data.t is None
 
 
 @pytest.mark.ci
-def test_dml_cluster_summary_with_time():
+def test_dml_summary_with_time():
     dml_data_did_cs = make_did_SZ2020(n_obs=200, cross_sectional_data=True)
     dml_did_cs = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression())
     assert isinstance(dml_did_cs.__str__(), str)
     assert isinstance(dml_did_cs.summary, pd.DataFrame)
 
+    dml_data = make_plr_CCDDHNR2018(n_obs=100)
+    df = dml_data.data.copy().iloc[:, :11]
+    df.columns = [f'X{i + 1}' for i in np.arange(8)] + ['y', 'd1', 'd2']
+    print(df)
+    dml_data = DoubleMLClusterData(df, 'y', ['d1', 'd2'],
+                                   cluster_cols=[f'X{i + 1}' for i in [5, 6]],
+                                   x_cols=[f'X{i + 1}' for i in np.arange(5)],
+                                   t_col='X8')
+    assert isinstance(dml_data._data_summary_str(), str)
+
 
 @pytest.mark.ci
 def test_x_cols_setter_defaults():
     df = pd.DataFrame(np.tile(np.arange(4), (4, 1)),
                       columns=['yy', 'dd', 'xx1', 'xx2'])
     dml_data = DoubleMLData(df, y_col='yy', d_cols='dd')
     assert dml_data.x_cols == ['xx1', 'xx2']
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_doubleml_evaluate_learner.py` & `DoubleML-0.6.2/doubleml/tests/test_doubleml_evaluate_learner.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_doubleml_exceptions.py` & `DoubleML-0.6.2/doubleml/tests/test_doubleml_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,16 +174,20 @@
         _ = DoubleMLLPQ(DoubleMLData(df_iivm, 'y', ['d', 'X1'], 'z'),
                         LogisticRegression(), LogisticRegression(), treatment=1)
     msg = ('Incompatible data. To fit an LPQ model with DML exactly one binary variable with values 0 and 1 '
            'needs to be specified as instrumental variable.')
     df_iivm = dml_data_iivm.data.copy()
     df_iivm['z'] = df_iivm['z'] * 2
     with pytest.raises(ValueError, match=msg):
+        # no instrument Z for LPQ
+        _ = DoubleMLLPQ(DoubleMLData(df_iivm, 'y', 'd', x_cols=['z']),
+                        LogisticRegression(), LogisticRegression(), treatment=1)
+    with pytest.raises(ValueError, match=msg):
         # non-binary Z for LPQ
-        _ = DoubleMLLPQ(DoubleMLData(df_iivm, 'y', 'd', 'z'),
+        _ = DoubleMLLPQ(DoubleMLData(df_iivm, 'y', 'd', z_cols=['z']),
                         LogisticRegression(), LogisticRegression(), treatment=1)
 
     # CVAR with IV
     msg = r'Incompatible data. z have been set as instrumental variable\(s\).'
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLCVAR(dml_data_iivm, Lasso(), LogisticRegression(), treatment=1)
     msg = ('Incompatible data. To fit an CVaR model with DML exactly one binary variable with values 0 and 1 '
@@ -466,29 +470,33 @@
 @pytest.mark.ci
 def test_doubleml_exception_kde():
     msg = "kde should be either a callable or None. '0.1' was passed."
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, ml_g, ml_m, treatment=1, kde="0.1")
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLLPQ(dml_data_iivm, ml_g, ml_m, treatment=1, kde="0.1")
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLQTE(dml_data_irm, ml_g, ml_m, kde="0.1")
 
 
 @pytest.mark.ci
-def test_doubleml_exception_normalization():
+def test_doubleml_exception_ipw_normalization():
     msg = "Normalization indicator has to be boolean. Object of type <class 'int'> passed."
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLIRM(dml_data_irm, ml_g, LogisticRegression(), normalize_ipw=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLIIVM(dml_data_iivm, ml_g, LogisticRegression(), LogisticRegression(), normalize_ipw=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLPQ(dml_data_irm, ml_g, ml_m, treatment=1, normalize_ipw=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLQTE(dml_data_irm, ml_g, ml_m, normalize_ipw=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLLPQ(dml_data_iivm, ml_g, ml_m, treatment=1, normalize_ipw=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = DoubleMLCVAR(dml_data_irm, Lasso(), LogisticRegression(), treatment=1, normalize_ipw=1)
 
     # DID models in_sample_normalization
     msg = "in_sample_normalization indicator has to be boolean. Object of type <class 'int'> passed."
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLDID(dml_data_did, ml_g, ml_m, in_sample_normalization=1)
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLDIDCS(dml_data_did_cs, ml_g, ml_m, in_sample_normalization=1)
@@ -722,37 +730,14 @@
         dml_plr_iv_type.tune([0.05, 0.5])
     msg = (r"Invalid param_grids {'ml_g': {'alpha': \[0.05, 0.5\]}, 'ml_m': {'alpha': \[0.05, 0.5\]}}. "
            "param_grids must be a dictionary with keys ml_l and ml_m and ml_g.")
     with pytest.raises(ValueError, match=msg):
         dml_plr_iv_type.tune({'ml_g': {'alpha': [0.05, 0.5]},
                               'ml_m': {'alpha': [0.05, 0.5]}})
 
-    msg = 'Learner ml_g was renamed to ml_l. '
-    with pytest.warns(DeprecationWarning, match=msg):
-        dml_plr.tune({'ml_g': {'alpha': [0.05, 0.5]},
-                      'ml_m': {'alpha': [0.05, 0.5]}})
-    with pytest.warns(DeprecationWarning, match=msg):
-        dml_plr.tune({'ml_l': {'alpha': [0.05, 0.5]},
-                      'ml_m': {'alpha': [0.05, 0.5]}},
-                     scoring_methods={'ml_g': 'explained_variance',
-                                      'ml_m': 'explained_variance'})
-
-    msg = 'Learner ml_g was renamed to ml_l. '
-    with pytest.warns(DeprecationWarning, match=msg):
-        dml_pliv.tune({'ml_g': {'alpha': [0.05, 0.5]},
-                       'ml_m': {'alpha': [0.05, 0.5]},
-                       'ml_r': {'alpha': [0.05, 0.5]}})
-    with pytest.warns(DeprecationWarning, match=msg):
-        dml_pliv.tune({'ml_l': {'alpha': [0.05, 0.5]},
-                       'ml_m': {'alpha': [0.05, 0.5]},
-                       'ml_r': {'alpha': [0.05, 0.5]}},
-                      scoring_methods={'ml_g': 'explained_variance',
-                                       'ml_m': 'explained_variance',
-                                       'ml_r': 'explained_variance'})
-
     param_grids = {'ml_l': {'alpha': [0.05, 0.5]}, 'ml_m': {'alpha': [0.05, 0.5]}}
     msg = ('Invalid scoring_methods neg_mean_absolute_error. '
            'scoring_methods must be a dictionary. '
            'Valid keys are ml_l and ml_m.')
     with pytest.raises(ValueError, match=msg):
         dml_plr.tune(param_grids, scoring_methods='neg_mean_absolute_error')
 
@@ -888,14 +873,26 @@
 
     # we allow classifiers for ml_g for binary treatment variables in IRM
     msg = (r'The ml_g learner LogisticRegression\(\) was identified as classifier '
            'but the outcome variable is not binary with values 0 and 1.')
     with pytest.raises(ValueError, match=msg):
         _ = DoubleMLIIVM(dml_data_iivm, LogisticRegression(), LogisticRegression(), LogisticRegression())
 
+    # we allow classifiers for ml_g for binary treatment variables in DID
+    msg = (r'The ml_g learner LogisticRegression\(\) was identified as classifier '
+           'but the outcome variable is not binary with values 0 and 1.')
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDID(dml_data_did, LogisticRegression(), LogisticRegression())
+
+    # we allow classifiers for ml_g for binary treatment variables in DIDCS
+    msg = (r'The ml_g learner LogisticRegression\(\) was identified as classifier '
+           'but the outcome variable is not binary with values 0 and 1.')
+    with pytest.raises(ValueError, match=msg):
+        _ = DoubleMLDIDCS(dml_data_did_cs, LogisticRegression(), LogisticRegression())
+
     # construct a classifier which is not identifiable as classifier via is_classifier by sklearn
     # it then predicts labels and therefore an exception will be thrown
     log_reg = LogisticRegression()
     log_reg._estimator_type = None
     msg = (r'Learner provided for ml_m is probably invalid: LogisticRegression\(\) is \(probably\) neither a regressor '
            'nor a classifier. Method predict is used for prediction.')
     with pytest.warns(UserWarning, match=msg):
@@ -935,35 +932,225 @@
            'that for classifiers probabilities and not labels are predicted.')
     with pytest.raises(ValueError, match=msg):
         dml_iivm_hidden_classifier.fit()
     with pytest.raises(ValueError, match=msg):
         dml_iivm_hidden_classifier.set_ml_nuisance_params('ml_g0', 'd', {'max_iter': 314})
         dml_iivm_hidden_classifier.fit()
 
-    msg = 'Learner ml_g was renamed to ml_l. '
-    with pytest.warns(DeprecationWarning, match=msg):
-        dml_plr.set_ml_nuisance_params('ml_g', 'd', {'max_iter': 314})
-
-    msg = 'Learner ml_g was renamed to ml_l. '
-    with pytest.warns(DeprecationWarning, match=msg):
-        dml_pliv.set_ml_nuisance_params('ml_g', 'd', {'max_iter': 314})
-
 
 @pytest.mark.ci
 @pytest.mark.filterwarnings("ignore:Learner provided for")
 def test_doubleml_exception_and_warning_learner():
     # msg = err_msg_prefix + r'_DummyNoClassifier\(\) has no method .predict\(\).'
     with pytest.raises(TypeError):
         _ = DoubleMLPLR(dml_data, _DummyNoClassifier(), Lasso())
     msg = 'Invalid learner provided for ml_m: ' + r'Lasso\(\) has no method .predict_proba\(\).'
     with pytest.raises(TypeError, match=msg):
         _ = DoubleMLIRM(dml_data_irm, Lasso(), Lasso())
 
 
 @pytest.mark.ci
+def test_doubleml_sensitivity_not_yet_implemented():
+    dml_pliv = DoubleMLPLIV(dml_data_pliv, ml_g, ml_m, ml_r, n_folds=1, apply_cross_fitting=False)
+    dml_pliv.fit()
+    msg = ("Sensitivity analysis not yet implemented without cross-fitting.")
+    with pytest.raises(NotImplementedError, match=msg):
+        _ = dml_pliv.sensitivity_analysis()
+
+    dml_pliv = DoubleMLPLIV(dml_data_pliv, ml_g, ml_m, ml_r)
+    dml_pliv.fit()
+    msg = ("Sensitivity analysis not yet implemented for <class 'doubleml.double_ml_pliv.DoubleMLPLIV'>.")
+    with pytest.raises(NotImplementedError, match=msg):
+        _ = dml_pliv.sensitivity_analysis()
+
+
+def test_doubleml_sensitivity_inputs():
+    dml_irm = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression(), trimming_threshold=0.1)
+    dml_irm.fit()
+
+    # test cf_y
+    msg = "cf_y must be of float type. 1 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=1, cf_d=0.03, rho=1.0, level=0.95)
+
+    msg = r'cf_y must be in \[0,1\). 1.0 was passed.'
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=1.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=1.0, cf_d=0.03, rho=1.0, level=0.95)
+
+    # test cf_d
+    msg = "cf_d must be of float type. 1 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=1, rho=1.0, level=0.95)
+
+    msg = r'cf_d must be in \[0,1\). 1.0 was passed.'
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=1.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=1.0, rho=1.0, level=0.95)
+
+    # test rho
+    msg = "rho must be of float type. 1 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1, level=0.95)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_robustness_value(rho=1, null_hypothesis=0.0, level=0.95, idx_treatment=0)
+
+    msg = "rho must be of float type. 1 of type <class 'str'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho="1")
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho="1", level=0.95)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_robustness_value(rho="1", null_hypothesis=0.0, level=0.95, idx_treatment=0)
+
+    msg = r'The absolute value of rho must be in \[0,1\]. 1.1 was passed.'
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.1)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.1, level=0.95)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_robustness_value(rho=1.1, null_hypothesis=0.0, level=0.95, idx_treatment=0)
+
+    # test level
+    msg = "The confidence level must be of float type. 1 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.0, level=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.0, level=1)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_robustness_value(rho=1.0, level=1, null_hypothesis=0.0, idx_treatment=0)
+
+    msg = r'The confidence level must be in \(0,1\). 1.0 was passed.'
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.0, level=1.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.0, level=1.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_robustness_value(rho=1.0, level=1.0, null_hypothesis=0.0, idx_treatment=0)
+
+    msg = r'The confidence level must be in \(0,1\). 0.0 was passed.'
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.0, level=0.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_sensitivity_analysis(cf_y=0.1, cf_d=0.15, rho=1.0, level=0.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_robustness_value(rho=1.0, level=0.0, null_hypothesis=0.0, idx_treatment=0)
+
+    # test null_hypothesis
+    msg = "null_hypothesis has to be of type float or np.ndarry. 1 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_analysis(null_hypothesis=1)
+    msg = r"null_hypothesis is numpy.ndarray but does not have the required shape \(1,\). Array of shape \(2,\) was passed."
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_analysis(null_hypothesis=np.array([1, 2]))
+    msg = "null_hypothesis must be of float type. 1 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_robustness_value(null_hypothesis=1, level=0.95, rho=1.0, idx_treatment=0)
+    msg = r"null_hypothesis must be of float type. \[1\] of type <class 'numpy.ndarray'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_robustness_value(null_hypothesis=np.array([1]), level=0.95, rho=1.0, idx_treatment=0)
+
+    # test idx_treatment
+    dml_irm.sensitivity_analysis()
+    msg = "idx_treatment must be an integer. 0.0 of type <class 'float'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._calc_robustness_value(idx_treatment=0.0, null_hypothesis=0.0, level=0.95, rho=1.0)
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_plot(idx_treatment=0.0)
+
+    msg = "idx_treatment must be larger or equal to 0. -1 was passed."
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_robustness_value(idx_treatment=-1, null_hypothesis=0.0, level=0.95, rho=1.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(idx_treatment=-1)
+
+    msg = "idx_treatment must be smaller or equal to 0. 1 was passed."
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm._calc_robustness_value(idx_treatment=1, null_hypothesis=0.0, level=0.95, rho=1.0)
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(idx_treatment=1)
+
+    # test setter
+    msg = ("_sensitivity_element_est must return sensitivity elements in a dict. "
+           "Got type <class 'int'>.")
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm._set_sensitivity_elements(sensitivity_elements=1, i_rep=0, i_treat=0)
+
+    sensitivity_elements = dict({'sigma2': 1})
+    with pytest.raises(ValueError):
+        _ = dml_irm._set_sensitivity_elements(sensitivity_elements=sensitivity_elements, i_rep=0, i_treat=0)
+
+    # test variances
+    sensitivity_elements = dict({'sigma2': 1.0, 'nu2': -2.4, 'psi_sigma2': 1.0, 'psi_nu2': 1.0})
+    _ = dml_irm._set_sensitivity_elements(sensitivity_elements=sensitivity_elements, i_rep=0, i_treat=0)
+    msg = ('sensitivity_elements sigma2 and nu2 have to be positive. '
+           r'Got sigma2 \[\[\[1.\]\]\] and nu2 \[\[\[-2.4\]\]\]. '
+           r'Most likely this is due to low quality learners \(especially propensity scores\).')
+    with pytest.raises(ValueError, match=msg):
+        dml_irm.sensitivity_analysis()
+
+
+def test_doubleml_sensitivity_plot_input():
+    dml_irm = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression(), trimming_threshold=0.1)
+    dml_irm.fit()
+
+    msg = (r'Apply sensitivity_analysis\(\) to include senario in sensitivity_plot. '
+           'The values of rho and the level are used for the scenario.')
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot()
+
+    dml_irm.sensitivity_analysis()
+    msg = "include_scenario has to be boolean. True of type <class 'str'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_plot(include_scenario="True")
+
+    msg = "value must be a string. 2 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_plot(value=2)
+    msg = "Invalid value test. Valid values theta or ci."
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(value='test')
+
+    msg = "fill has to be boolean. True of type <class 'str'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_plot(fill="True")
+
+    msg = "grid_size must be an integer. 0.0 of type <class 'float'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_size=0.0)
+    msg = "grid_size must be larger or equal to 10. 9 was passed."
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_size=9)
+
+    msg = "grid_bounds must be of float type. 1 of type <class 'int'> was passed."
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_bounds=(0.15, 1))
+    with pytest.raises(TypeError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_bounds=(1, 0.15))
+    msg = r'grid_bounds must be in \(0,1\). 1.0 was passed.'
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_bounds=(1.0, 0.15))
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_bounds=(0.15, 1.0))
+    msg = r'grid_bounds must be in \(0,1\). 0.0 was passed.'
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_bounds=(0.0, 0.15))
+    with pytest.raises(ValueError, match=msg):
+        _ = dml_irm.sensitivity_plot(grid_bounds=(0.15, 0.0))
+
+
+@pytest.mark.ci
 def test_doubleml_cluster_not_yet_implemented():
     dml_pliv_cluster = DoubleMLPLIV(dml_cluster_data_pliv, ml_g, ml_m, ml_r)
     dml_pliv_cluster.fit()
     msg = 'bootstrap not yet implemented with clustering.'
     with pytest.raises(NotImplementedError, match=msg):
         _ = dml_pliv_cluster.bootstrap()
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_doubleml_model_defaults.py` & `DoubleML-0.6.2/doubleml/tests/test_doubleml_model_defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,7 +172,19 @@
 def test_did_cs_defaults():
     _assert_resampling_default_settings(dml_did_cs)
     assert dml_did.score == 'observational'
     assert dml_did_cs.in_sample_normalization
     assert dml_did_cs.dml_procedure == 'dml2'
     assert dml_did_cs.trimming_rule == 'truncate'
     assert dml_did_cs.trimming_threshold == 1e-2
+
+
+@pytest.mark.ci
+def test_sensitivity_defaults():
+    input_dict = {'cf_y': 0.03,
+                  'cf_d': 0.03,
+                  'rho': 1.0,
+                  'level': 0.95,
+                  'null_hypothesis': np.array([0.])}
+
+    dml_plr.sensitivity_analysis()
+    assert dml_plr._sensitivity_params['input'] == input_dict
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_doubleml_return_types.py` & `DoubleML-0.6.2/doubleml/tests/test_doubleml_return_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 import pytest
 import pandas as pd
 import numpy as np
+import plotly
 
-from doubleml import DoubleMLPLR, DoubleMLIRM, DoubleMLIIVM, DoubleMLPLIV, DoubleMLClusterData, \
+from doubleml import DoubleMLPLR, DoubleMLIRM, DoubleMLIIVM, DoubleMLPLIV, DoubleMLData, DoubleMLClusterData, \
     DoubleMLCVAR, DoubleMLPQ, DoubleMLLPQ, DoubleMLDID, DoubleMLDIDCS
 from doubleml.datasets import make_plr_CCDDHNR2018, make_irm_data, make_pliv_CHS2015, make_iivm_data,\
     make_pliv_multiway_cluster_CKMS2021, make_did_SZ2020
 
 from sklearn.linear_model import Lasso, LogisticRegression
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 from sklearn.svm import LinearSVR
 
 np.random.seed(3141)
-dml_data_plr = make_plr_CCDDHNR2018(n_obs=200)
-dml_data_pliv = make_pliv_CHS2015(n_obs=200, dim_z=1)
-dml_data_irm = make_irm_data(n_obs=200)
-dml_data_iivm = make_iivm_data(n_obs=200)
+n_obs = 200
+dml_data_plr = make_plr_CCDDHNR2018(n_obs=n_obs)
+dml_data_pliv = make_pliv_CHS2015(n_obs=n_obs, dim_z=1)
+dml_data_irm = make_irm_data(n_obs=n_obs)
+dml_data_iivm = make_iivm_data(n_obs=n_obs)
 dml_cluster_data_pliv = make_pliv_multiway_cluster_CKMS2021(N=10, M=10)
-dml_data_did = make_did_SZ2020(n_obs=200)
-dml_data_did_cs = make_did_SZ2020(n_obs=200, cross_sectional_data=True)
+dml_data_did = make_did_SZ2020(n_obs=n_obs)
+dml_data_did_cs = make_did_SZ2020(n_obs=n_obs, cross_sectional_data=True)
+(x, y, d, t) = make_did_SZ2020(n_obs=n_obs, cross_sectional_data=True, return_type='array')
+binary_outcome = np.random.binomial(n=1, p=0.5, size=n_obs)
+dml_data_did_binary_outcome = DoubleMLData.from_arrays(x, binary_outcome, d)
+dml_data_did_cs_binary_outcome = DoubleMLData.from_arrays(x, binary_outcome, d, t=t)
 
 dml_plr = DoubleMLPLR(dml_data_plr, Lasso(), Lasso())
 dml_pliv = DoubleMLPLIV(dml_data_pliv, Lasso(), Lasso(), Lasso())
 dml_irm = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression())
 dml_iivm = DoubleMLIIVM(dml_data_iivm, Lasso(), LogisticRegression(), LogisticRegression())
 dml_pliv_cluster = DoubleMLPLIV(dml_cluster_data_pliv, Lasso(), Lasso(), Lasso())
 dml_cvar = DoubleMLCVAR(dml_data_irm, ml_g=RandomForestRegressor(), ml_m=RandomForestClassifier())
 dml_pq = DoubleMLPQ(dml_data_irm, ml_g=RandomForestClassifier(), ml_m=RandomForestClassifier())
 dml_lpq = DoubleMLLPQ(dml_data_iivm, ml_g=RandomForestClassifier(), ml_m=RandomForestClassifier())
 dml_did = DoubleMLDID(dml_data_did, Lasso(), LogisticRegression())
+dml_did_binary_outcome = DoubleMLDID(dml_data_did_binary_outcome, LogisticRegression(), LogisticRegression())
 dml_did_cs = DoubleMLDIDCS(dml_data_did_cs, Lasso(), LogisticRegression())
+dml_did_cs_binary_outcome = DoubleMLDIDCS(dml_data_did_cs_binary_outcome, LogisticRegression(), LogisticRegression())
 
 
 @pytest.mark.ci
 @pytest.mark.parametrize('dml_obj, cls',
                          [(dml_plr, DoubleMLPLR),
                           (dml_pliv, DoubleMLPLIV),
                           (dml_irm, DoubleMLIRM),
                           (dml_iivm, DoubleMLIIVM),
                           (dml_pliv_cluster, DoubleMLPLIV),
                           (dml_cvar, DoubleMLCVAR),
                           (dml_pq, DoubleMLPQ),
                           (dml_lpq, DoubleMLLPQ),
                           (dml_did, DoubleMLDID),
-                          (dml_did_cs, DoubleMLDIDCS)])
+                          (dml_did_binary_outcome, DoubleMLDID),
+                          (dml_did_cs, DoubleMLDIDCS),
+                          (dml_did_cs_binary_outcome, DoubleMLDIDCS)])
 def test_return_types(dml_obj, cls):
     # ToDo: A second test case with multiple treatment variables would be helpful
     assert isinstance(dml_obj.__str__(), str)
     assert isinstance(dml_obj.summary, pd.DataFrame)
     assert isinstance(dml_obj.draw_sample_splitting(), cls)
     if not dml_obj._is_cluster_data:
         assert isinstance(dml_obj.set_sample_splitting(dml_obj.smpls), cls)
@@ -89,15 +99,15 @@
 
 pliv_dml1 = DoubleMLPLIV(dml_data_pliv, Lasso(), Lasso(), Lasso(),
                          dml_procedure='dml1', n_rep=n_rep, n_folds=n_folds)
 pliv_dml1.fit()
 pliv_dml1.bootstrap(n_rep_boot=n_rep_boot)
 
 irm_dml1 = DoubleMLIRM(dml_data_irm, Lasso(), LogisticRegression(),
-                       dml_procedure='dml1', n_rep=n_rep, n_folds=n_folds)
+                       dml_procedure='dml1', n_rep=n_rep, n_folds=n_folds, trimming_threshold=0.1)
 irm_dml1.fit()
 irm_dml1.bootstrap(n_rep_boot=n_rep_boot)
 
 iivm_dml1 = DoubleMLIIVM(dml_data_iivm, Lasso(), LogisticRegression(), LogisticRegression(),
                          dml_procedure='dml1', n_rep=n_rep, n_folds=n_folds)
 iivm_dml1.fit()
 iivm_dml1.bootstrap(n_rep_boot=n_rep_boot)
@@ -126,15 +136,16 @@
                             dml_procedure='dml1', n_rep=n_rep, n_folds=n_folds)
 did_cs_dml1.fit()
 did_cs_dml1.bootstrap(n_rep_boot=n_rep_boot)
 
 
 @pytest.mark.ci
 @pytest.mark.parametrize('dml_obj',
-                         [plr_dml1, pliv_dml1,  irm_dml1,  iivm_dml1, cvar_dml1, pq_dml1, lpq_dml1, did_dml1, did_cs_dml1])
+                         [plr_dml1, pliv_dml1,  irm_dml1,  iivm_dml1, cvar_dml1, pq_dml1, lpq_dml1,
+                          did_dml1, did_cs_dml1])
 def test_property_types_and_shapes(dml_obj):
     # not checked: apply_cross_fitting, dml_procedure, learner, learner_names, params, params_names, score
     # already checked: summary
 
     # check that the setting is still in line with the hard-coded values
     assert dml_obj._dml_data.n_treat == n_treat
     assert dml_obj.n_rep == n_rep
@@ -336,7 +347,26 @@
     assert did_dml1.rmses['ml_m'].shape == (n_rep, n_treat)
 
     assert did_cs_dml1.rmses['ml_g_d0_t0'].shape == (n_rep, n_treat)
     assert did_cs_dml1.rmses['ml_g_d0_t1'].shape == (n_rep, n_treat)
     assert did_cs_dml1.rmses['ml_g_d1_t0'].shape == (n_rep, n_treat)
     assert did_cs_dml1.rmses['ml_g_d1_t1'].shape == (n_rep, n_treat)
     assert did_cs_dml1.rmses['ml_m'].shape == (n_rep, n_treat)
+
+
+@pytest.mark.ci
+def test_sensitivity():
+    assert isinstance(plr_dml1.sensitivity_summary, str)
+    plr_dml1.sensitivity_analysis()
+    assert isinstance(plr_dml1.sensitivity_summary, str)
+    assert isinstance(plr_dml1.sensitivity_plot(), plotly.graph_objs._figure.Figure)
+    assert isinstance(plr_dml1.sensitivity_plot(value='ci'), plotly.graph_objs._figure.Figure)
+    assert isinstance(plr_dml1._calc_sensitivity_analysis(cf_y=0.03, cf_d=0.03, rho=1.0, level=0.95), dict)
+    assert isinstance(plr_dml1._calc_robustness_value(null_hypothesis=0.0, level=0.95, rho=1.0, idx_treatment=0), tuple)
+
+    assert isinstance(irm_dml1.sensitivity_summary, str)
+    irm_dml1.sensitivity_analysis()
+    assert isinstance(irm_dml1.sensitivity_summary, str)
+    assert isinstance(irm_dml1.sensitivity_plot(), plotly.graph_objs._figure.Figure)
+    assert isinstance(irm_dml1.sensitivity_plot(value='ci'), plotly.graph_objs._figure.Figure)
+    assert isinstance(irm_dml1._calc_sensitivity_analysis(cf_y=0.03, cf_d=0.03, rho=1.0, level=0.95), dict)
+    assert isinstance(irm_dml1._calc_robustness_value(null_hypothesis=0.0, level=0.95, rho=1.0, idx_treatment=0), tuple)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_doubleml_scores.py` & `DoubleML-0.6.2/doubleml/tests/test_doubleml_scores.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_doubleml_set_ml_nuisance_params.py` & `DoubleML-0.6.2/doubleml/tests/test_doubleml_set_ml_nuisance_params.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_doubleml_set_sample_splitting.py` & `DoubleML-0.6.2/doubleml/tests/test_doubleml_set_sample_splitting.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_iivm.py` & `DoubleML-0.6.2/doubleml/tests/test_iivm.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_iivm_classifier.py` & `DoubleML-0.6.2/doubleml/tests/test_iivm_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_iivm_no_cross_fit.py` & `DoubleML-0.6.2/doubleml/tests/test_iivm_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_iivm_subgroups.py` & `DoubleML-0.6.2/doubleml/tests/test_irm_tune.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,156 +1,170 @@
 import numpy as np
 import pytest
 import math
 
 from sklearn.base import clone
 
-from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+from sklearn.linear_model import LogisticRegression
+from sklearn.ensemble import RandomForestRegressor
 
 import doubleml as dml
 
 from ._utils import draw_smpls
-from ._utils_iivm_manual import fit_iivm, boot_iivm
+from ._utils_irm_manual import fit_irm, boot_irm, tune_nuisance_irm
 
 
 @pytest.fixture(scope='module',
-                params=[[RandomForestRegressor(max_depth=2, n_estimators=10),
-                         RandomForestClassifier(max_depth=2, n_estimators=10)]])
-def learner(request):
+                params=[RandomForestRegressor(random_state=42)])
+def learner_g(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['LATE'])
+                params=[LogisticRegression()])
+def learner_m(request):
+    return request.param
+
+
+@pytest.fixture(scope='module',
+                params=['ATE', 'ATTE'])
 def score(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['dml1', 'dml2'])
+                params=['dml2'])
 def dml_procedure(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=[True, False])
 def normalize_ipw(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[0.01])
-def trimming_threshold(request):
+                params=[True, False])
+def tune_on_folds(request):
     return request.param
 
 
-@pytest.fixture(scope='module',
-                params=[{'always_takers': True, 'never_takers': True},
-                        {'always_takers': False, 'never_takers': True},
-                        {'always_takers': True, 'never_takers': False}])
-def subgroups(request):
-    return request.param
+def get_par_grid(learner):
+    if learner.__class__ in [RandomForestRegressor]:
+        par_grid = {'n_estimators': [5, 10, 20]}
+    else:
+        assert learner.__class__ in [LogisticRegression]
+        par_grid = {'C': np.logspace(-4, 2, 10)}
+    return par_grid
+
 
+@pytest.fixture(scope='module')
+def dml_irm_fixture(generate_data_irm, learner_g, learner_m, score, dml_procedure, normalize_ipw, tune_on_folds):
+    par_grid = {'ml_g': get_par_grid(learner_g),
+                'ml_m': get_par_grid(learner_m)}
+    n_folds_tune = 4
 
-@pytest.fixture(scope="module")
-def dml_iivm_subgroups_fixture(generate_data_iivm, learner, score, dml_procedure, normalize_ipw,
-                               trimming_threshold, subgroups):
     boot_methods = ['normal']
     n_folds = 2
-    n_rep_boot = 491
+    n_rep_boot = 499
 
     # collect data
-    data = generate_data_iivm
-    x_cols = data.columns[data.columns.str.startswith('X')].tolist()
+    (x, y, d) = generate_data_irm
 
     # Set machine learning methods for m & g
-    ml_g = clone(learner[0])
-    ml_m = clone(learner[1])
-    ml_r = clone(learner[1])
+    ml_g = clone(learner_g)
+    ml_m = clone(learner_m)
 
     np.random.seed(3141)
-    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'], x_cols, 'z')
-    dml_iivm_obj = dml.DoubleMLIIVM(obj_dml_data,
-                                    ml_g, ml_m, ml_r,
-                                    n_folds,
-                                    subgroups=subgroups,
-                                    dml_procedure=dml_procedure,
-                                    normalize_ipw=normalize_ipw,
-                                    trimming_threshold=trimming_threshold)
+    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
+    dml_irm_obj = dml.DoubleMLIRM(obj_dml_data,
+                                  ml_g, ml_m,
+                                  n_folds,
+                                  score=score,
+                                  dml_procedure=dml_procedure,
+                                  normalize_ipw=normalize_ipw)
+
+    # tune hyperparameters
+    tune_res = dml_irm_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune,
+                                return_tune_res=False)
+    assert isinstance(tune_res, dml.DoubleMLIRM)
 
-    dml_iivm_obj.fit(store_predictions=True)
+    dml_irm_obj.fit()
 
     np.random.seed(3141)
-    y = data['y'].values
-    x = data.loc[:, x_cols].values
-    d = data['d'].values
-    z = data['z'].values
     n_obs = len(y)
     all_smpls = draw_smpls(n_obs, n_folds)
+    smpls = all_smpls[0]
 
-    res_manual = fit_iivm(y, x, d, z,
-                          clone(learner[0]), clone(learner[1]), clone(learner[1]),
-                          all_smpls, dml_procedure, score,
-                          normalize_ipw=normalize_ipw, trimming_threshold=trimming_threshold,
-                          always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
+    if tune_on_folds:
+        g0_params, g1_params, m_params = tune_nuisance_irm(y, x, d,
+                                                           clone(learner_g), clone(learner_m), smpls, score,
+                                                           n_folds_tune,
+                                                           par_grid['ml_g'], par_grid['ml_m'])
+    else:
+        xx = [(np.arange(len(y)), np.array([]))]
+        g0_params, g1_params, m_params = tune_nuisance_irm(y, x, d,
+                                                           clone(learner_g), clone(learner_m), xx, score,
+                                                           n_folds_tune,
+                                                           par_grid['ml_g'], par_grid['ml_m'])
+        g0_params = g0_params * n_folds
+        m_params = m_params * n_folds
+        if score == 'ATE':
+            g1_params = g1_params * n_folds
+        else:
+            assert score == 'ATTE'
+            g1_params = None
+
+    res_manual = fit_irm(y, x, d, clone(learner_g), clone(learner_m),
+                         all_smpls, dml_procedure, score,
+                         normalize_ipw=normalize_ipw,
+                         g0_params=g0_params, g1_params=g1_params, m_params=m_params)
 
-    res_dict = {'coef': dml_iivm_obj.coef,
+    res_dict = {'coef': dml_irm_obj.coef,
                 'coef_manual': res_manual['theta'],
-                'se': dml_iivm_obj.se,
+                'se': dml_irm_obj.se,
                 'se_manual': res_manual['se'],
-                'boot_methods': boot_methods,
-                'always_takers': subgroups['always_takers'],
-                'never_takers': subgroups['never_takers'],
-                'rhat0': dml_iivm_obj.predictions['ml_r0'],
-                'rhat1': dml_iivm_obj.predictions['ml_r1'],
-                'z': z
-                }
+                'boot_methods': boot_methods}
 
     for bootstrap in boot_methods:
         np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_iivm(y, d, z, res_manual['thetas'], res_manual['ses'],
-                                            res_manual['all_g_hat0'], res_manual['all_g_hat1'],
-                                            res_manual['all_m_hat'], res_manual['all_r_hat0'], res_manual['all_r_hat1'],
-                                            all_smpls, score, bootstrap, n_rep_boot, dml_procedure,
-                                            normalize_ipw=normalize_ipw)
+        boot_theta, boot_t_stat = boot_irm(y, d, res_manual['thetas'], res_manual['ses'],
+                                           res_manual['all_g_hat0'], res_manual['all_g_hat1'],
+                                           res_manual['all_m_hat'], res_manual['all_p_hat'],
+                                           all_smpls, score, bootstrap, n_rep_boot,
+                                           normalize_ipw=normalize_ipw,
+                                           dml_procedure=dml_procedure)
 
         np.random.seed(3141)
-        dml_iivm_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
-        res_dict['boot_coef' + bootstrap] = dml_iivm_obj.boot_coef
-        res_dict['boot_t_stat' + bootstrap] = dml_iivm_obj.boot_t_stat
+        dml_irm_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
+        res_dict['boot_coef' + bootstrap] = dml_irm_obj.boot_coef
+        res_dict['boot_t_stat' + bootstrap] = dml_irm_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_iivm_subgroups_coef(dml_iivm_subgroups_fixture):
-    assert math.isclose(dml_iivm_subgroups_fixture['coef'],
-                        dml_iivm_subgroups_fixture['coef_manual'],
+def test_dml_irm_coef(dml_irm_fixture):
+    assert math.isclose(dml_irm_fixture['coef'],
+                        dml_irm_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_iivm_subgroups_se(dml_iivm_subgroups_fixture):
-    assert math.isclose(dml_iivm_subgroups_fixture['se'],
-                        dml_iivm_subgroups_fixture['se_manual'],
+def test_dml_irm_se(dml_irm_fixture):
+    assert math.isclose(dml_irm_fixture['se'],
+                        dml_irm_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_iivm_subgroups_boot(dml_iivm_subgroups_fixture):
-    for bootstrap in dml_iivm_subgroups_fixture['boot_methods']:
-        assert np.allclose(dml_iivm_subgroups_fixture['boot_coef' + bootstrap],
-                           dml_iivm_subgroups_fixture['boot_coef' + bootstrap + '_manual'],
+def test_dml_irm_boot(dml_irm_fixture):
+    for bootstrap in dml_irm_fixture['boot_methods']:
+        assert np.allclose(dml_irm_fixture['boot_coef' + bootstrap],
+                           dml_irm_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-        assert np.allclose(dml_iivm_subgroups_fixture['boot_t_stat' + bootstrap],
-                           dml_iivm_subgroups_fixture['boot_t_stat' + bootstrap + '_manual'],
+        assert np.allclose(dml_irm_fixture['boot_t_stat' + bootstrap],
+                           dml_irm_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-
-
-@pytest.mark.ci
-def test_dml_iivm_subgroups(dml_iivm_subgroups_fixture):
-    if not dml_iivm_subgroups_fixture['always_takers']:
-        assert np.all(dml_iivm_subgroups_fixture['rhat0'] == 0)
-    if not dml_iivm_subgroups_fixture['never_takers']:
-        assert np.all(dml_iivm_subgroups_fixture['rhat1'] == 1)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_iivm_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_tune.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,200 +1,185 @@
 import numpy as np
 import pytest
 import math
 
-from sklearn.base import clone
-
-from sklearn.linear_model import LogisticRegression
-from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+from sklearn.linear_model import Lasso, ElasticNet
 
 import doubleml as dml
 
-from ._utils import draw_smpls
-from ._utils_iivm_manual import fit_iivm, boot_iivm, tune_nuisance_iivm
+from ._utils import draw_smpls, _clone
+from ._utils_pliv_manual import fit_pliv, boot_pliv, tune_nuisance_pliv
 
 
 @pytest.fixture(scope='module',
-                params=[RandomForestRegressor()])
-def learner_g(request):
+                params=[Lasso(),
+                        ElasticNet()])
+def learner_l(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[RandomForestClassifier()])
+                params=[ElasticNet()])
 def learner_m(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[LogisticRegression()])
+                params=[ElasticNet()])
 def learner_r(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['LATE'])
-def score(request):
-    return request.param
-
-
-@pytest.fixture(scope='module',
-                params=['dml2'])
-def dml_procedure(request):
+                params=[ElasticNet()])
+def learner_g(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[True, False])
-def normalize_ipw(request):
+                params=['partialling out', 'IV-type'])
+def score(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[{'always_takers': True, 'never_takers': True},
-                        {'always_takers': False, 'never_takers': False}])
-def subgroups(request):
+                params=['dml2'])
+def dml_procedure(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=[True, False])
 def tune_on_folds(request):
     return request.param
 
 
 def get_par_grid(learner):
-    if learner.__class__ in [RandomForestRegressor, RandomForestClassifier]:
-        par_grid = {'n_estimators': [5, 10, 20]}
+    if learner.__class__ == Lasso:
+        par_grid = {'alpha': np.linspace(0.05, .95, 7)}
     else:
-        assert learner.__class__ in [LogisticRegression]
-        par_grid = {'C': np.logspace(-4, 2, 10)}
+        assert learner.__class__ == ElasticNet
+        par_grid = {'l1_ratio': [.1, .5, .7, .9, .95, .99, 1], 'alpha': np.linspace(0.05, 1., 7)}
     return par_grid
 
 
-@pytest.fixture(scope="module")
-def dml_iivm_fixture(generate_data_iivm, learner_g, learner_m, learner_r, score, dml_procedure, normalize_ipw, subgroups,
-                     tune_on_folds):
-    par_grid = {'ml_g': get_par_grid(learner_g),
+@pytest.fixture(scope='module')
+def dml_pliv_fixture(generate_data_iv, learner_l, learner_m, learner_r, learner_g, score, dml_procedure, tune_on_folds):
+    par_grid = {'ml_l': get_par_grid(learner_l),
                 'ml_m': get_par_grid(learner_m),
-                'ml_r': get_par_grid(learner_r)}
+                'ml_r': get_par_grid(learner_r),
+                'ml_g': get_par_grid(learner_g)}
     n_folds_tune = 4
 
-    boot_methods = ['normal']
+    boot_methods = ['Bayes', 'normal', 'wild']
     n_folds = 2
-    n_rep_boot = 491
+    n_rep_boot = 503
 
     # collect data
-    data = generate_data_iivm
+    data = generate_data_iv
     x_cols = data.columns[data.columns.str.startswith('X')].tolist()
 
-    # Set machine learning methods for m, g & r
-    ml_g = clone(learner_g)
-    ml_m = clone(learner_m)
-    ml_r = clone(learner_r)
+    # Set machine learning methods for l, m, r & g
+    ml_l = _clone(learner_l)
+    ml_m = _clone(learner_m)
+    ml_r = _clone(learner_r)
+    if score == 'IV-type':
+        ml_g = _clone(learner_g)
+    else:
+        ml_g = None
 
     np.random.seed(3141)
-    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'], x_cols, 'z')
-    dml_iivm_obj = dml.DoubleMLIIVM(obj_dml_data,
-                                    ml_g, ml_m, ml_r,
-                                    n_folds,
-                                    subgroups=subgroups,
-                                    dml_procedure=dml_procedure,
-                                    normalize_ipw=normalize_ipw)
+    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'], x_cols, 'Z1')
+    dml_pliv_obj = dml.DoubleMLPLIV(obj_dml_data,
+                                    ml_l, ml_m, ml_r, ml_g,
+                                    n_folds=n_folds,
+                                    score=score,
+                                    dml_procedure=dml_procedure)
+
     # tune hyperparameters
-    tune_res = dml_iivm_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune,
-                                 return_tune_res=True)
-    assert isinstance(tune_res, list)
+    tune_res = dml_pliv_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune,
+                                 return_tune_res=False)
+    assert isinstance(tune_res, dml.DoubleMLPLIV)
 
-    dml_iivm_obj.fit()
+    dml_pliv_obj.fit()
 
     np.random.seed(3141)
     y = data['y'].values
     x = data.loc[:, x_cols].values
     d = data['d'].values
-    z = data['z'].values
+    z = data['Z1'].values
     n_obs = len(y)
     all_smpls = draw_smpls(n_obs, n_folds)
     smpls = all_smpls[0]
 
+    tune_g = (score == 'IV-type') | callable(score)
     if tune_on_folds:
-        g0_params, g1_params, m_params,  r0_params, r1_params = \
-            tune_nuisance_iivm(y, x, d, z,
-                               clone(learner_g), clone(learner_m), clone(learner_r), smpls,
-                               n_folds_tune,
-                               par_grid['ml_g'], par_grid['ml_m'], par_grid['ml_r'],
-                               always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
+        l_params, m_params, r_params, g_params = tune_nuisance_pliv(
+            y, x, d, z,
+            _clone(learner_l), _clone(learner_m), _clone(learner_r), _clone(learner_g),
+            smpls, n_folds_tune,
+            par_grid['ml_l'], par_grid['ml_m'], par_grid['ml_r'], par_grid['ml_g'],
+            tune_g)
     else:
-        xx = [(np.arange(data.shape[0]), np.array([]))]
-        g0_params, g1_params, m_params,  r0_params, r1_params = \
-            tune_nuisance_iivm(y, x, d, z,
-                               clone(learner_g), clone(learner_m), clone(learner_r), xx,
-                               n_folds_tune,
-                               par_grid['ml_g'], par_grid['ml_m'], par_grid['ml_r'],
-                               always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
-        g0_params = g0_params * n_folds
-        g1_params = g1_params * n_folds
+        xx = [(np.arange(len(y)), np.array([]))]
+        l_params, m_params, r_params, g_params = tune_nuisance_pliv(
+            y, x, d, z,
+            _clone(learner_l), _clone(learner_m), _clone(learner_r), _clone(learner_g),
+            xx, n_folds_tune,
+            par_grid['ml_l'], par_grid['ml_m'], par_grid['ml_r'], par_grid['ml_g'],
+            tune_g)
+
+        l_params = l_params * n_folds
         m_params = m_params * n_folds
-        if subgroups['always_takers']:
-            r0_params = r0_params * n_folds
-        else:
-            r0_params = r0_params
-        if subgroups['never_takers']:
-            r1_params = r1_params * n_folds
-        else:
-            r1_params = r1_params
+        r_params = r_params * n_folds
+        g_params = g_params * n_folds
 
-    res_manual = fit_iivm(y, x, d, z,
-                          clone(learner_g), clone(learner_m), clone(learner_r),
+    res_manual = fit_pliv(y, x, d, z, _clone(learner_l), _clone(learner_m), _clone(learner_r), _clone(learner_g),
                           all_smpls, dml_procedure, score,
-                          g0_params=g0_params, g1_params=g1_params,
-                          m_params=m_params, r0_params=r0_params, r1_params=r1_params,
-                          normalize_ipw=normalize_ipw,
-                          always_takers=subgroups['always_takers'], never_takers=subgroups['never_takers'])
+                          l_params=l_params, m_params=m_params, r_params=r_params, g_params=g_params)
 
-    res_dict = {'coef': dml_iivm_obj.coef,
+    res_dict = {'coef': dml_pliv_obj.coef,
                 'coef_manual': res_manual['theta'],
-                'se': dml_iivm_obj.se,
+                'se': dml_pliv_obj.se,
                 'se_manual': res_manual['se'],
                 'boot_methods': boot_methods}
 
     for bootstrap in boot_methods:
         np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_iivm(y, d, z, res_manual['thetas'], res_manual['ses'],
-                                            res_manual['all_g_hat0'], res_manual['all_g_hat1'],
-                                            res_manual['all_m_hat'], res_manual['all_r_hat0'], res_manual['all_r_hat1'],
-                                            all_smpls, score, bootstrap, n_rep_boot, dml_procedure,
-                                            normalize_ipw=normalize_ipw)
+        boot_theta, boot_t_stat = boot_pliv(y, d, z, res_manual['thetas'], res_manual['ses'],
+                                            res_manual['all_l_hat'], res_manual['all_m_hat'],
+                                            res_manual['all_r_hat'], res_manual['all_g_hat'],
+                                            all_smpls, score, bootstrap, n_rep_boot)
 
         np.random.seed(3141)
-        dml_iivm_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
-        res_dict['boot_coef' + bootstrap] = dml_iivm_obj.boot_coef
-        res_dict['boot_t_stat' + bootstrap] = dml_iivm_obj.boot_t_stat
+        dml_pliv_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
+        res_dict['boot_coef' + bootstrap] = dml_pliv_obj.boot_coef
+        res_dict['boot_t_stat' + bootstrap] = dml_pliv_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_iivm_coef(dml_iivm_fixture):
-    assert math.isclose(dml_iivm_fixture['coef'],
-                        dml_iivm_fixture['coef_manual'],
+def test_dml_pliv_coef(dml_pliv_fixture):
+    assert math.isclose(dml_pliv_fixture['coef'],
+                        dml_pliv_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_iivm_se(dml_iivm_fixture):
-    assert math.isclose(dml_iivm_fixture['se'],
-                        dml_iivm_fixture['se_manual'],
+def test_dml_pliv_se(dml_pliv_fixture):
+    assert math.isclose(dml_pliv_fixture['se'],
+                        dml_pliv_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_iivm_boot(dml_iivm_fixture):
-    for bootstrap in dml_iivm_fixture['boot_methods']:
-        assert np.allclose(dml_iivm_fixture['boot_coef' + bootstrap],
-                           dml_iivm_fixture['boot_coef' + bootstrap + '_manual'],
+def test_dml_pliv_boot(dml_pliv_fixture):
+    for bootstrap in dml_pliv_fixture['boot_methods']:
+        assert np.allclose(dml_pliv_fixture['boot_coef' + bootstrap],
+                           dml_pliv_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-        assert np.allclose(dml_iivm_fixture['boot_t_stat' + bootstrap],
-                           dml_iivm_fixture['boot_t_stat' + bootstrap + '_manual'],
+        assert np.allclose(dml_pliv_fixture['boot_t_stat' + bootstrap],
+                           dml_pliv_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_irm.py` & `DoubleML-0.6.2/doubleml/tests/test_irm.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from sklearn.linear_model import LogisticRegression, LinearRegression
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 
 import doubleml as dml
 from doubleml.datasets import make_irm_data
 
 from ._utils import draw_smpls
-from ._utils_irm_manual import fit_irm, boot_irm
+from ._utils_irm_manual import fit_irm, boot_irm, fit_sensitivity_elements_irm
 
 
 @pytest.fixture(scope='module',
                 params=[[LinearRegression(),
                          LogisticRegression(solver='lbfgs', max_iter=250)],
-                        [RandomForestRegressor(max_depth=5, n_estimators=10),
-                         RandomForestClassifier(max_depth=5, n_estimators=10)]])
+                        [RandomForestRegressor(max_depth=5, n_estimators=10, random_state=42),
+                         RandomForestClassifier(max_depth=5, n_estimators=10, random_state=42)]])
 def learner(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=['ATE', 'ATTE'])
 def score(request):
@@ -33,21 +33,21 @@
 @pytest.fixture(scope='module',
                 params=['dml1', 'dml2'])
 def dml_procedure(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[True, False])
+                params=[False, True])
 def normalize_ipw(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[0.01, 0.05])
+                params=[0.2, 0.15])
 def trimming_threshold(request):
     return request.param
 
 
 @pytest.fixture(scope='module')
 def dml_irm_fixture(generate_data_irm, learner, score, dml_procedure, normalize_ipw, trimming_threshold):
     boot_methods = ['normal']
@@ -105,14 +105,25 @@
         np.random.seed(3141)
         dml_irm_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
         res_dict['boot_coef' + bootstrap] = dml_irm_obj.boot_coef
         res_dict['boot_t_stat' + bootstrap] = dml_irm_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
+    # sensitivity tests
+    res_dict['sensitivity_elements'] = dml_irm_obj.sensitivity_elements
+    res_dict['sensitivity_elements_manual'] = fit_sensitivity_elements_irm(y, d,
+                                                                           all_coef=dml_irm_obj.all_coef,
+                                                                           predictions=dml_irm_obj.predictions,
+                                                                           score=score,
+                                                                           n_rep=1)
+
+    # check if sensitivity score with rho=0 gives equal asymptotic standard deviation
+    dml_irm_obj.sensitivity_analysis(rho=0.0)
+    res_dict['sensitivity_ses'] = dml_irm_obj.sensitivity_params['se']
     return res_dict
 
 
 @pytest.mark.ci
 def test_dml_irm_coef(dml_irm_fixture):
     assert math.isclose(dml_irm_fixture['coef'],
                         dml_irm_fixture['coef_manual'],
@@ -134,14 +145,33 @@
                            rtol=1e-9, atol=1e-4)
         assert np.allclose(dml_irm_fixture['boot_t_stat' + bootstrap],
                            dml_irm_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
 
 
 @pytest.mark.ci
+def test_dml_irm_sensitivity(dml_irm_fixture):
+    sensitivity_element_names = ['sigma2', 'nu2', 'psi_sigma2', 'psi_nu2']
+    for sensitivity_element in sensitivity_element_names:
+        assert np.allclose(dml_irm_fixture['sensitivity_elements'][sensitivity_element],
+                           dml_irm_fixture['sensitivity_elements_manual'][sensitivity_element],
+                           rtol=1e-9, atol=1e-4)
+
+
+@pytest.mark.ci
+def test_dml_irm_sensitivity_rho0(dml_irm_fixture):
+    assert np.allclose(dml_irm_fixture['se'],
+                       dml_irm_fixture['sensitivity_ses']['lower'],
+                       rtol=1e-9, atol=1e-4)
+    assert np.allclose(dml_irm_fixture['se'],
+                       dml_irm_fixture['sensitivity_ses']['upper'],
+                       rtol=1e-9, atol=1e-4)
+
+
+@pytest.mark.ci
 def test_dml_irm_cate_gate():
     n = 9
     # collect data
     np.random.seed(42)
     obj_dml_data = make_irm_data(n_obs=n, dim_x=2)
 
     # First stage estimation
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_irm_classifier.py` & `DoubleML-0.6.2/doubleml/tests/test_irm_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from ._utils import draw_smpls
 from ._utils_irm_manual import fit_irm, boot_irm
 
 
 @pytest.fixture(scope='module',
                 params=[[LogisticRegression(solver='lbfgs', max_iter=250),
                          LogisticRegression(solver='lbfgs', max_iter=250)],
-                        [RandomForestClassifier(max_depth=2, n_estimators=10),
-                         RandomForestClassifier(max_depth=2, n_estimators=10)]])
+                        [RandomForestClassifier(max_depth=2, n_estimators=10, random_state=42),
+                         RandomForestClassifier(max_depth=2, n_estimators=10, random_state=42)]])
 def learner(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=['ATE', 'ATTE'])
 def score(request):
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_irm_no_cross_fit.py` & `DoubleML-0.6.2/doubleml/tests/test_irm_no_cross_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import doubleml as dml
 
 from ._utils import draw_smpls
 from ._utils_irm_manual import fit_irm, boot_irm
 
 
 @pytest.fixture(scope='module',
-                params=[[RandomForestRegressor(max_depth=2, n_estimators=10),
-                         RandomForestClassifier(max_depth=2, n_estimators=10)]])
+                params=[[RandomForestRegressor(max_depth=2, n_estimators=10, random_state=42),
+                         RandomForestClassifier(max_depth=2, n_estimators=10, random_state=42)]])
 def learner(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=['ATE', 'ATTE'])
 def score(request):
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_irm_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_plr_tune.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,170 +1,170 @@
 import numpy as np
 import pytest
 import math
 
-from sklearn.base import clone
-
-from sklearn.linear_model import LogisticRegression
-from sklearn.ensemble import RandomForestRegressor
+from sklearn.linear_model import Lasso, ElasticNet
 
 import doubleml as dml
 
-from ._utils import draw_smpls
-from ._utils_irm_manual import fit_irm, boot_irm, tune_nuisance_irm
+from ._utils import draw_smpls, _clone
+from ._utils_plr_manual import fit_plr, boot_plr, tune_nuisance_plr
 
 
 @pytest.fixture(scope='module',
-                params=[RandomForestRegressor()])
-def learner_g(request):
+                params=[Lasso(),
+                        ElasticNet()])
+def learner_l(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[LogisticRegression()])
+                params=[Lasso(),
+                        ElasticNet()])
 def learner_m(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['ATE', 'ATTE'])
-def score(request):
+                params=[Lasso(),
+                        ElasticNet()])
+def learner_g(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['dml2'])
-def dml_procedure(request):
+                params=['partialling out', 'IV-type'])
+def score(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[True, False])
-def normalize_ipw(request):
+                params=['dml2'])
+def dml_procedure(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=[True, False])
 def tune_on_folds(request):
     return request.param
 
 
 def get_par_grid(learner):
-    if learner.__class__ in [RandomForestRegressor]:
-        par_grid = {'n_estimators': [5, 10, 20]}
+    if learner.__class__ == Lasso:
+        par_grid = {'alpha': np.linspace(0.05, .95, 7)}
     else:
-        assert learner.__class__ in [LogisticRegression]
-        par_grid = {'C': np.logspace(-4, 2, 10)}
+        assert learner.__class__ == ElasticNet
+        par_grid = {'l1_ratio': [.1, .5, .7, .9, .95, .99, 1], 'alpha': np.linspace(0.05, 1., 7)}
     return par_grid
 
 
-@pytest.fixture(scope='module')
-def dml_irm_fixture(generate_data_irm, learner_g, learner_m, score, dml_procedure, normalize_ipw, tune_on_folds):
-    par_grid = {'ml_g': get_par_grid(learner_g),
-                'ml_m': get_par_grid(learner_m)}
+@pytest.fixture(scope="module")
+def dml_plr_fixture(generate_data2, learner_l, learner_m, learner_g, score, dml_procedure, tune_on_folds):
+    par_grid = {'ml_l': get_par_grid(learner_l),
+                'ml_m': get_par_grid(learner_m),
+                'ml_g': get_par_grid(learner_g)}
     n_folds_tune = 4
 
     boot_methods = ['normal']
     n_folds = 2
-    n_rep_boot = 499
+    n_rep_boot = 502
 
     # collect data
-    (x, y, d) = generate_data_irm
+    obj_dml_data = generate_data2
 
     # Set machine learning methods for m & g
-    ml_g = clone(learner_g)
-    ml_m = clone(learner_m)
+    ml_l = _clone(learner_l)
+    ml_m = _clone(learner_m)
+    if score == 'IV-type':
+        ml_g = _clone(learner_g)
+    else:
+        ml_g = None
 
     np.random.seed(3141)
-    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
-    dml_irm_obj = dml.DoubleMLIRM(obj_dml_data,
-                                  ml_g, ml_m,
+    dml_plr_obj = dml.DoubleMLPLR(obj_dml_data,
+                                  ml_l, ml_m, ml_g,
                                   n_folds,
                                   score=score,
-                                  dml_procedure=dml_procedure,
-                                  normalize_ipw=normalize_ipw)
+                                  dml_procedure=dml_procedure)
 
     # tune hyperparameters
-    tune_res = dml_irm_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune,
-                                return_tune_res=False)
-    assert isinstance(tune_res, dml.DoubleMLIRM)
+    tune_res = dml_plr_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune,
+                                return_tune_res=True)
+    assert isinstance(tune_res, list)
 
-    dml_irm_obj.fit()
+    # fit with tuned parameters
+    dml_plr_obj.fit()
 
     np.random.seed(3141)
+    y = obj_dml_data.y
+    x = obj_dml_data.x
+    d = obj_dml_data.d
     n_obs = len(y)
     all_smpls = draw_smpls(n_obs, n_folds)
     smpls = all_smpls[0]
 
+    tune_g = (score == 'IV-type')
     if tune_on_folds:
-        g0_params, g1_params, m_params = tune_nuisance_irm(y, x, d,
-                                                           clone(learner_g), clone(learner_m), smpls, score,
-                                                           n_folds_tune,
-                                                           par_grid['ml_g'], par_grid['ml_m'])
+        l_params, m_params, g_params = tune_nuisance_plr(y, x, d,
+                                                         _clone(learner_l), _clone(learner_m), _clone(learner_g),
+                                                         smpls, n_folds_tune,
+                                                         par_grid['ml_l'], par_grid['ml_m'], par_grid['ml_g'], tune_g)
     else:
         xx = [(np.arange(len(y)), np.array([]))]
-        g0_params, g1_params, m_params = tune_nuisance_irm(y, x, d,
-                                                           clone(learner_g), clone(learner_m), xx, score,
-                                                           n_folds_tune,
-                                                           par_grid['ml_g'], par_grid['ml_m'])
-        g0_params = g0_params * n_folds
+        l_params, m_params, g_params = tune_nuisance_plr(y, x, d,
+                                                         _clone(learner_l), _clone(learner_m), _clone(learner_g),
+                                                         xx, n_folds_tune,
+                                                         par_grid['ml_l'], par_grid['ml_m'], par_grid['ml_g'], tune_g)
+        l_params = l_params * n_folds
+        g_params = g_params * n_folds
         m_params = m_params * n_folds
-        if score == 'ATE':
-            g1_params = g1_params * n_folds
-        else:
-            assert score == 'ATTE'
-            g1_params = None
 
-    res_manual = fit_irm(y, x, d, clone(learner_g), clone(learner_m),
+    res_manual = fit_plr(y, x, d, _clone(learner_l), _clone(learner_m), _clone(learner_g),
                          all_smpls, dml_procedure, score,
-                         normalize_ipw=normalize_ipw,
-                         g0_params=g0_params, g1_params=g1_params, m_params=m_params)
+                         l_params=l_params, m_params=m_params, g_params=g_params)
 
-    res_dict = {'coef': dml_irm_obj.coef,
+    res_dict = {'coef': dml_plr_obj.coef,
                 'coef_manual': res_manual['theta'],
-                'se': dml_irm_obj.se,
+                'se': dml_plr_obj.se,
                 'se_manual': res_manual['se'],
                 'boot_methods': boot_methods}
 
     for bootstrap in boot_methods:
         np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_irm(y, d, res_manual['thetas'], res_manual['ses'],
-                                           res_manual['all_g_hat0'], res_manual['all_g_hat1'],
-                                           res_manual['all_m_hat'], res_manual['all_p_hat'],
-                                           all_smpls, score, bootstrap, n_rep_boot,
-                                           normalize_ipw=normalize_ipw,
-                                           dml_procedure=dml_procedure)
+        boot_theta, boot_t_stat = boot_plr(y, d, res_manual['thetas'], res_manual['ses'],
+                                           res_manual['all_l_hat'], res_manual['all_m_hat'], res_manual['all_g_hat'],
+                                           all_smpls, score, bootstrap, n_rep_boot)
 
         np.random.seed(3141)
-        dml_irm_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
-        res_dict['boot_coef' + bootstrap] = dml_irm_obj.boot_coef
-        res_dict['boot_t_stat' + bootstrap] = dml_irm_obj.boot_t_stat
+        dml_plr_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
+        res_dict['boot_coef' + bootstrap] = dml_plr_obj.boot_coef
+        res_dict['boot_t_stat' + bootstrap] = dml_plr_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_irm_coef(dml_irm_fixture):
-    assert math.isclose(dml_irm_fixture['coef'],
-                        dml_irm_fixture['coef_manual'],
+def test_dml_plr_coef(dml_plr_fixture):
+    assert math.isclose(dml_plr_fixture['coef'],
+                        dml_plr_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_irm_se(dml_irm_fixture):
-    assert math.isclose(dml_irm_fixture['se'],
-                        dml_irm_fixture['se_manual'],
+def test_dml_plr_se(dml_plr_fixture):
+    assert math.isclose(dml_plr_fixture['se'],
+                        dml_plr_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_irm_boot(dml_irm_fixture):
-    for bootstrap in dml_irm_fixture['boot_methods']:
-        assert np.allclose(dml_irm_fixture['boot_coef' + bootstrap],
-                           dml_irm_fixture['boot_coef' + bootstrap + '_manual'],
+def test_dml_plr_boot(dml_plr_fixture):
+    for bootstrap in dml_plr_fixture['boot_methods']:
+        assert np.allclose(dml_plr_fixture['boot_coef' + bootstrap],
+                           dml_plr_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-        assert np.allclose(dml_irm_fixture['boot_t_stat' + bootstrap],
-                           dml_irm_fixture['boot_t_stat' + bootstrap + '_manual'],
+        assert np.allclose(dml_plr_fixture['boot_t_stat' + bootstrap],
+                           dml_plr_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_irm_with_missings.py` & `DoubleML-0.6.2/doubleml/tests/test_irm_with_missings.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_lpq.py` & `DoubleML-0.6.2/doubleml/tests/test_pq.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import doubleml as dml
 
 from sklearn.base import clone
 from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
 
 from ._utils import draw_smpls
-from ._utils_lpq_manual import fit_lpq
+from ._utils_pq_manual import fit_pq
 
 
 @pytest.fixture(scope='module',
                 params=[0, 1])
 def treatment(request):
     return request.param
 
@@ -21,15 +21,15 @@
 @pytest.fixture(scope='module',
                 params=[0.25, 0.5, 0.75])
 def quantile(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[RandomForestClassifier(max_depth=2, n_estimators=5, random_state=42),
+                params=[RandomForestClassifier(max_depth=2, n_estimators=10, random_state=42),
                         LogisticRegression()])
 def learner(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=['dml1', 'dml2'])
@@ -46,61 +46,61 @@
 @pytest.fixture(scope='module',
                 params=[0.01, 0.05])
 def trimming_threshold(request):
     return request.param
 
 
 @pytest.fixture(scope="module")
-def dml_lpq_fixture(generate_data_local_quantiles, treatment, quantile, learner,
-                    dml_procedure, normalize_ipw, trimming_threshold):
+def dml_pq_fixture(generate_data_quantiles, treatment, quantile, learner,
+                   dml_procedure, normalize_ipw, trimming_threshold):
     n_folds = 3
 
     # collect data
-    (x, y, d, z) = generate_data_local_quantiles
-    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d, z)
+    (x, y, d) = generate_data_quantiles
+    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
     np.random.seed(42)
     n_obs = len(y)
-    strata = d + 2 * z
-    all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=strata)
+    all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=d)
 
     np.random.seed(42)
-    dml_lpq_obj = dml.DoubleMLLPQ(obj_dml_data,
-                                  clone(learner), clone(learner),
-                                  treatment=treatment,
-                                  quantile=quantile,
-                                  n_folds=n_folds,
-                                  n_rep=1,
-                                  dml_procedure=dml_procedure,
-                                  normalize_ipw=normalize_ipw,
-                                  trimming_threshold=trimming_threshold,
-                                  draw_sample_splitting=False)
+    dml_pq_obj = dml.DoubleMLPQ(obj_dml_data,
+                                clone(learner), clone(learner),
+                                treatment=treatment,
+                                quantile=quantile,
+                                n_folds=n_folds,
+                                n_rep=1,
+                                dml_procedure=dml_procedure,
+                                trimming_threshold=trimming_threshold,
+                                normalize_ipw=normalize_ipw,
+                                draw_sample_splitting=False)
 
     # synchronize the sample splitting
-    dml_lpq_obj.set_sample_splitting(all_smpls=all_smpls)
-    dml_lpq_obj.fit()
+    dml_pq_obj.set_sample_splitting(all_smpls=all_smpls)
+    np.random.seed(42)
+    dml_pq_obj.fit()
 
     np.random.seed(42)
-    res_manual = fit_lpq(y, x, d, z, quantile, clone(learner), clone(learner),
-                         all_smpls, treatment, dml_procedure,
-                         normalize_ipw=normalize_ipw,
-                         n_rep=1, trimming_threshold=trimming_threshold)
-
-    res_dict = {'coef': dml_lpq_obj.coef,
-                'coef_manual': res_manual['lpq'],
-                'se': dml_lpq_obj.se,
+    res_manual = fit_pq(y, x, d, quantile,
+                        clone(learner), clone(learner),
+                        all_smpls, treatment, dml_procedure,
+                        n_rep=1, trimming_threshold=trimming_threshold, normalize_ipw=normalize_ipw)
+
+    res_dict = {'coef': dml_pq_obj.coef,
+                'coef_manual': res_manual['pq'],
+                'se': dml_pq_obj.se,
                 'se_manual': res_manual['se']}
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_lpq_coef(dml_lpq_fixture):
-    assert math.isclose(dml_lpq_fixture['coef'],
-                        dml_lpq_fixture['coef_manual'],
+def test_dml_pq_coef(dml_pq_fixture):
+    assert math.isclose(dml_pq_fixture['coef'],
+                        dml_pq_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_lpq_se(dml_lpq_fixture):
-    assert math.isclose(dml_lpq_fixture['se'],
-                        dml_lpq_fixture['se_manual'],
+def test_dml_pq_se(dml_pq_fixture):
+    assert math.isclose(dml_pq_fixture['se'],
+                        dml_pq_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_lpq_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_lpq_tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import numpy as np
 import pytest
 import math
 
 from sklearn.base import clone
-
-from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
 
 import doubleml as dml
 
 from ._utils import draw_smpls
 from ._utils_lpq_manual import fit_lpq, tune_nuisance_lpq
 
@@ -48,17 +46,14 @@
 def tune_on_folds(request):
     return request.param
 
 
 def get_par_grid(learner):
     if learner.__class__ in [RandomForestClassifier]:
         par_grid = {'n_estimators': [5, 10, 20]}
-    else:
-        assert learner.__class__ in [LogisticRegression]
-        par_grid = {'C': np.logspace(-4, 2, 10)}
     return par_grid
 
 
 @pytest.fixture(scope='module')
 def dml_lpq_fixture(generate_data_local_quantiles, treatment, quantile, learner, dml_procedure, normalize_ipw,
                     tune_on_folds):
     par_grid = {'ml_m_z': get_par_grid(learner),
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_multiway_cluster.py` & `DoubleML-0.6.2/doubleml/tests/test_multiway_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_nonlinear_cluster.py` & `DoubleML-0.6.2/doubleml/tests/test_nonlinear_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_nonlinear_score_mixin.py` & `DoubleML-0.6.2/doubleml/tests/test_nonlinear_score_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from sklearn.base import clone
 from sklearn.linear_model import LinearRegression
 from sklearn.utils import check_X_y
 
 import doubleml as dml
 from doubleml.double_ml import DoubleML
-from doubleml._utils import _dml_cv_predict, _check_finite_predictions
+from doubleml._utils import _dml_cv_predict
+from doubleml._utils_checks import _check_finite_predictions
 from doubleml.double_ml_score_mixins import NonLinearScoreMixin
 
 
 class DoubleMLPLRWithNonLinearScoreMixin(NonLinearScoreMixin, DoubleML):
     _coef_bounds = (-np.inf, np.inf)
     _coef_start_val = 3.0
 
@@ -160,14 +161,17 @@
 
         return psi_a, psi_b
 
     def _nuisance_tuning(self, smpls, param_grids, scoring_methods, n_folds_tune, n_jobs_cv,
                          search_mode, n_iter_randomized_search):
         pass
 
+    def _sensitivity_element_est(self, preds):
+        pass
+
 
 @pytest.fixture(scope='module',
                 params=[LinearRegression()])
 def learner(request):
     return request.param
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv_no_cross_fit.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_x_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_xz_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pliv_partial_z_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr.py` & `DoubleML-0.6.2/doubleml/tests/test_plr.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from sklearn.linear_model import LinearRegression, Lasso
 from sklearn.ensemble import RandomForestRegressor
 
 import doubleml as dml
 
 from ._utils import draw_smpls
-from ._utils_plr_manual import fit_plr, plr_dml1, plr_dml2, boot_plr
+from ._utils_plr_manual import fit_plr, plr_dml1, plr_dml2, boot_plr, fit_sensitivity_elements_plr
 
 
 @pytest.fixture(scope='module',
                 params=[RandomForestRegressor(max_depth=2, n_estimators=10),
                         LinearRegression(),
                         Lasso(alpha=0.1)])
 def learner(request):
@@ -92,14 +92,24 @@
         np.random.seed(3141)
         dml_plr_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
         res_dict['boot_coef' + bootstrap] = dml_plr_obj.boot_coef
         res_dict['boot_t_stat' + bootstrap] = dml_plr_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
+    # sensitivity tests
+    res_dict['sensitivity_elements'] = dml_plr_obj.sensitivity_elements
+    res_dict['sensitivity_elements_manual'] = fit_sensitivity_elements_plr(y, d.reshape(-1, 1),
+                                                                           all_coef=dml_plr_obj.all_coef,
+                                                                           predictions=dml_plr_obj.predictions,
+                                                                           score=score,
+                                                                           n_rep=1)
+    # check if sensitivity score with rho=0 gives equal asymptotic standard deviation
+    dml_plr_obj.sensitivity_analysis(rho=0.0)
+    res_dict['sensitivity_ses'] = dml_plr_obj.sensitivity_params['se']
     return res_dict
 
 
 @pytest.mark.ci
 def test_dml_plr_coef(dml_plr_fixture):
     assert math.isclose(dml_plr_fixture['coef'],
                         dml_plr_fixture['coef_manual'],
@@ -120,14 +130,32 @@
                            dml_plr_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
         assert np.allclose(dml_plr_fixture['boot_t_stat' + bootstrap],
                            dml_plr_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
 
 
+@pytest.mark.ci
+def test_dml_plr_sensitivity(dml_plr_fixture):
+    sensitivity_element_names = ['sigma2', 'nu2', 'psi_sigma2', 'psi_nu2']
+    for sensitivity_element in sensitivity_element_names:
+        assert np.allclose(dml_plr_fixture['sensitivity_elements'][sensitivity_element],
+                           dml_plr_fixture['sensitivity_elements_manual'][sensitivity_element])
+
+
+@pytest.mark.ci
+def test_dml_plr_sensitivity_rho0(dml_plr_fixture):
+    assert np.allclose(dml_plr_fixture['se'],
+                       dml_plr_fixture['sensitivity_ses']['lower'],
+                       rtol=1e-9, atol=1e-4)
+    assert np.allclose(dml_plr_fixture['se'],
+                       dml_plr_fixture['sensitivity_ses']['upper'],
+                       rtol=1e-9, atol=1e-4)
+
+
 @pytest.fixture(scope="module")
 def dml_plr_ols_manual_fixture(generate_data1, score, dml_procedure):
     learner = LinearRegression()
     boot_methods = ['Bayes', 'normal', 'wild']
     n_folds = 2
     n_rep_boot = 501
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr_classifier.py` & `DoubleML-0.6.2/doubleml/tests/test_plr_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr_multi_treat.py` & `DoubleML-0.6.2/doubleml/tests/test_plr_rep_cross.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import numpy as np
 import pytest
+import math
 
-from sklearn.linear_model import Lasso
+from sklearn.linear_model import LinearRegression
 from sklearn.ensemble import RandomForestRegressor
 
 import doubleml as dml
 
 from ._utils import draw_smpls, _clone
-from ._utils_plr_manual import fit_plr_multitreat, boot_plr_multitreat
+from ._utils_plr_manual import fit_plr, boot_plr
 
 
 @pytest.fixture(scope='module',
-                params=range(2))
-def idx(request):
-    return request.param
-
-
-@pytest.fixture(scope='module',
-                params=[Lasso(alpha=0.1),
-                        RandomForestRegressor(max_depth=2, n_estimators=10)])
+                params=[RandomForestRegressor(max_depth=2, n_estimators=10),
+                        LinearRegression()])
 def learner(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=['IV-type', 'partialling out'])
 def score(request):
@@ -32,106 +27,97 @@
 @pytest.fixture(scope='module',
                 params=['dml1', 'dml2'])
 def dml_procedure(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[1, 3])
+                params=[3])
 def n_rep(request):
     return request.param
 
 
-@pytest.fixture(scope='module')
-def dml_plr_multitreat_fixture(generate_data_bivariate, generate_data_toeplitz, idx, learner,
-                               score, dml_procedure, n_rep):
+@pytest.fixture(scope="module")
+def dml_plr_fixture(generate_data1, learner, score, dml_procedure, n_rep):
     boot_methods = ['normal']
     n_folds = 2
-    n_rep_boot = 483
+    n_rep_boot = 498
 
     # collect data
-    if idx == 0:
-        data = generate_data_bivariate
-    else:
-        assert idx == 1
-        data = generate_data_toeplitz
+    data = generate_data1
     x_cols = data.columns[data.columns.str.startswith('X')].tolist()
-    d_cols = data.columns[data.columns.str.startswith('d')].tolist()
 
     # Set machine learning methods for l, m & g
     ml_l = _clone(learner)
     ml_m = _clone(learner)
     if score == 'IV-type':
         ml_g = _clone(learner)
     else:
         ml_g = None
 
     np.random.seed(3141)
-    obj_dml_data = dml.DoubleMLData(data, 'y', d_cols, x_cols)
+    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'], x_cols)
     dml_plr_obj = dml.DoubleMLPLR(obj_dml_data,
                                   ml_l, ml_m, ml_g,
-                                  n_folds, n_rep,
-                                  score=score,
-                                  dml_procedure=dml_procedure)
+                                  n_folds,
+                                  n_rep,
+                                  score,
+                                  dml_procedure)
 
     dml_plr_obj.fit()
 
     np.random.seed(3141)
     y = data['y'].values
     x = data.loc[:, x_cols].values
-    d = data.loc[:, d_cols].values
+    d = data['d'].values
     n_obs = len(y)
     all_smpls = draw_smpls(n_obs, n_folds, n_rep)
 
-    res_manual = fit_plr_multitreat(y, x, d,
-                                    _clone(learner), _clone(learner), _clone(learner),
-                                    all_smpls, dml_procedure, score,
-                                    n_rep=n_rep)
+    res_manual = fit_plr(y, x, d, _clone(learner), _clone(learner), _clone(learner),
+                         all_smpls, dml_procedure, score, n_rep)
 
     res_dict = {'coef': dml_plr_obj.coef,
                 'coef_manual': res_manual['theta'],
                 'se': dml_plr_obj.se,
                 'se_manual': res_manual['se'],
-                'boot_methods': boot_methods}
+                'boot_methods': boot_methods
+                }
 
     for bootstrap in boot_methods:
         np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_plr_multitreat(
-            y, d,
-            res_manual['thetas'], res_manual['ses'],
-            res_manual['all_l_hat'], res_manual['all_m_hat'], res_manual['all_g_hat'],
-            all_smpls, score,
-            bootstrap, n_rep_boot, n_rep)
+        boot_theta, boot_t_stat = boot_plr(y, d, res_manual['thetas'], res_manual['ses'],
+                                           res_manual['all_l_hat'], res_manual['all_m_hat'], res_manual['all_g_hat'],
+                                           all_smpls, score, bootstrap, n_rep_boot, n_rep)
 
         np.random.seed(3141)
         dml_plr_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
         res_dict['boot_coef' + bootstrap] = dml_plr_obj.boot_coef
         res_dict['boot_t_stat' + bootstrap] = dml_plr_obj.boot_t_stat
         res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
         res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_plr_multitreat_coef(dml_plr_multitreat_fixture):
-    assert np.allclose(dml_plr_multitreat_fixture['coef'],
-                       dml_plr_multitreat_fixture['coef_manual'],
-                       rtol=1e-9, atol=1e-4)
+def test_dml_plr_coef(dml_plr_fixture):
+    assert math.isclose(dml_plr_fixture['coef'],
+                        dml_plr_fixture['coef_manual'],
+                        rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_plr_multitreat_se(dml_plr_multitreat_fixture):
-    assert np.allclose(dml_plr_multitreat_fixture['se'],
-                       dml_plr_multitreat_fixture['se_manual'],
-                       rtol=1e-9, atol=1e-4)
+def test_dml_plr_se(dml_plr_fixture):
+    assert math.isclose(dml_plr_fixture['se'],
+                        dml_plr_fixture['se_manual'],
+                        rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_plr_multitreat_boot(dml_plr_multitreat_fixture):
-    for bootstrap in dml_plr_multitreat_fixture['boot_methods']:
-        assert np.allclose(dml_plr_multitreat_fixture['boot_coef' + bootstrap],
-                           dml_plr_multitreat_fixture['boot_coef' + bootstrap + '_manual'],
+def test_dml_plr_boot(dml_plr_fixture):
+    for bootstrap in dml_plr_fixture['boot_methods']:
+        assert np.allclose(dml_plr_fixture['boot_coef' + bootstrap],
+                           dml_plr_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
-        assert np.allclose(dml_plr_multitreat_fixture['boot_t_stat' + bootstrap],
-                           dml_plr_multitreat_fixture['boot_t_stat' + bootstrap + '_manual'],
+        assert np.allclose(dml_plr_fixture['boot_t_stat' + bootstrap],
+                           dml_plr_fixture['boot_t_stat' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr_no_cross_fit.py` & `DoubleML-0.6.2/doubleml/tests/test_plr_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr_reestimate_from_scores.py` & `DoubleML-0.6.2/doubleml/tests/test_plr_reestimate_from_scores.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr_rep_cross.py` & `DoubleML-0.6.2/doubleml/tests/test_plr_set_ml_nuisance_pars.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,119 @@
 import numpy as np
 import pytest
 import math
 
-from sklearn.linear_model import LinearRegression
-from sklearn.ensemble import RandomForestRegressor
+from sklearn.linear_model import Lasso
 
 import doubleml as dml
 
-from ._utils import draw_smpls, _clone
-from ._utils_plr_manual import fit_plr, boot_plr
-
-
-@pytest.fixture(scope='module',
-                params=[RandomForestRegressor(max_depth=2, n_estimators=10),
-                        LinearRegression()])
-def learner(request):
-    return request.param
+from ._utils import _clone
 
 
 @pytest.fixture(scope='module',
                 params=['IV-type', 'partialling out'])
 def score(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=['dml1', 'dml2'])
 def dml_procedure(request):
     return request.param
 
 
-@pytest.fixture(scope='module',
-                params=[3])
-def n_rep(request):
-    return request.param
-
-
 @pytest.fixture(scope="module")
-def dml_plr_fixture(generate_data1, learner, score, dml_procedure, n_rep):
+def dml_plr_fixture(generate_data1, score, dml_procedure):
     boot_methods = ['normal']
     n_folds = 2
-    n_rep_boot = 498
+    n_rep_boot = 502
 
     # collect data
     data = generate_data1
-    x_cols = data.columns[data.columns.str.startswith('X')].tolist()
 
+    alpha = 0.05
+    learner = Lasso(alpha=alpha)
     # Set machine learning methods for l, m & g
     ml_l = _clone(learner)
     ml_m = _clone(learner)
     if score == 'IV-type':
         ml_g = _clone(learner)
     else:
         ml_g = None
 
     np.random.seed(3141)
-    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'], x_cols)
+    obj_dml_data = dml.DoubleMLData(data, 'y', ['d'])
     dml_plr_obj = dml.DoubleMLPLR(obj_dml_data,
                                   ml_l, ml_m, ml_g,
                                   n_folds,
-                                  n_rep,
-                                  score,
-                                  dml_procedure)
+                                  score=score,
+                                  dml_procedure=dml_procedure)
 
     dml_plr_obj.fit()
 
     np.random.seed(3141)
-    y = data['y'].values
-    x = data.loc[:, x_cols].values
-    d = data['d'].values
-    n_obs = len(y)
-    all_smpls = draw_smpls(n_obs, n_folds, n_rep)
+    learner = Lasso()
+    # Set machine learning methods for l, m & g
+    ml_l = _clone(learner)
+    ml_m = _clone(learner)
+    if score == 'IV-type':
+        ml_g = _clone(learner)
+    else:
+        ml_g = None
 
-    res_manual = fit_plr(y, x, d, _clone(learner), _clone(learner), _clone(learner),
-                         all_smpls, dml_procedure, score, n_rep)
+    dml_plr_obj_ext_set_par = dml.DoubleMLPLR(obj_dml_data,
+                                              ml_l, ml_m, ml_g,
+                                              n_folds,
+                                              score=score,
+                                              dml_procedure=dml_procedure)
+    dml_plr_obj_ext_set_par.set_ml_nuisance_params('ml_l', 'd', {'alpha': alpha})
+    dml_plr_obj_ext_set_par.set_ml_nuisance_params('ml_m', 'd', {'alpha': alpha})
+    if score == 'IV-type':
+        dml_plr_obj_ext_set_par.set_ml_nuisance_params('ml_g', 'd', {'alpha': alpha})
+
+    dml_plr_obj_ext_set_par.fit()
 
     res_dict = {'coef': dml_plr_obj.coef,
-                'coef_manual': res_manual['theta'],
+                'coef_manual': dml_plr_obj_ext_set_par.coef,
                 'se': dml_plr_obj.se,
-                'se_manual': res_manual['se'],
-                'boot_methods': boot_methods
-                }
+                'se_manual': dml_plr_obj_ext_set_par.se,
+                'boot_methods': boot_methods}
 
     for bootstrap in boot_methods:
-        np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_plr(y, d, res_manual['thetas'], res_manual['ses'],
-                                           res_manual['all_l_hat'], res_manual['all_m_hat'], res_manual['all_g_hat'],
-                                           all_smpls, score, bootstrap, n_rep_boot, n_rep)
-
-        np.random.seed(3141)
+        np.random.seed(314122)
         dml_plr_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
         res_dict['boot_coef' + bootstrap] = dml_plr_obj.boot_coef
         res_dict['boot_t_stat' + bootstrap] = dml_plr_obj.boot_t_stat
-        res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
-        res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
+
+        np.random.seed(314122)
+        dml_plr_obj_ext_set_par.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
+        res_dict['boot_coef' + bootstrap + '_manual'] = dml_plr_obj_ext_set_par.boot_coef
+        res_dict['boot_t_stat' + bootstrap + '_manual'] = dml_plr_obj_ext_set_par.boot_t_stat
 
     return res_dict
 
 
 @pytest.mark.ci
+@pytest.mark.filterwarnings("ignore:Using the same")
 def test_dml_plr_coef(dml_plr_fixture):
     assert math.isclose(dml_plr_fixture['coef'],
                         dml_plr_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
+@pytest.mark.filterwarnings("ignore:Using the same")
 def test_dml_plr_se(dml_plr_fixture):
     assert math.isclose(dml_plr_fixture['se'],
                         dml_plr_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
+@pytest.mark.filterwarnings("ignore:Using the same")
 def test_dml_plr_boot(dml_plr_fixture):
     for bootstrap in dml_plr_fixture['boot_methods']:
         assert np.allclose(dml_plr_fixture['boot_coef' + bootstrap],
                            dml_plr_fixture['boot_coef' + bootstrap + '_manual'],
                            rtol=1e-9, atol=1e-4)
         assert np.allclose(dml_plr_fixture['boot_t_stat' + bootstrap],
                            dml_plr_fixture['boot_t_stat' + bootstrap + '_manual'],
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr_set_smpls_externally.py` & `DoubleML-0.6.2/doubleml/tests/test_plr_set_smpls_externally.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.1/doubleml/tests/test_plr_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_pq_tune.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,146 @@
 import numpy as np
 import pytest
 import math
 
-from sklearn.linear_model import Lasso, ElasticNet
+from sklearn.base import clone
+from sklearn.ensemble import RandomForestClassifier
 
 import doubleml as dml
 
-from ._utils import draw_smpls, _clone
-from ._utils_plr_manual import fit_plr, boot_plr, tune_nuisance_plr
+from ._utils import draw_smpls
+from ._utils_pq_manual import fit_pq, tune_nuisance_pq
 
 
 @pytest.fixture(scope='module',
-                params=[Lasso(),
-                        ElasticNet()])
-def learner_l(request):
+                params=[0, 1])
+def treatment(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[Lasso(),
-                        ElasticNet()])
-def learner_m(request):
+                params=[0.25, 0.5, 0.75])
+def quantile(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[Lasso(),
-                        ElasticNet()])
+                params=[RandomForestClassifier(max_depth=5, random_state=42)])
 def learner_g(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['partialling out', 'IV-type'])
-def score(request):
+                params=[RandomForestClassifier(max_depth=5, random_state=42)])
+def learner_m(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=['dml2'])
+                params=['dml1', 'dml2'])
 def dml_procedure(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=[True, False])
+def normalize_ipw(request):
+    return request.param
+
+
+@pytest.fixture(scope='module',
+                params=[True, False])
 def tune_on_folds(request):
     return request.param
 
 
 def get_par_grid(learner):
-    if learner.__class__ == Lasso:
-        par_grid = {'alpha': np.linspace(0.05, .95, 7)}
-    else:
-        assert learner.__class__ == ElasticNet
-        par_grid = {'l1_ratio': [.1, .5, .7, .9, .95, .99, 1], 'alpha': np.linspace(0.05, 1., 7)}
+    if learner.__class__ in [RandomForestClassifier]:
+        par_grid = {'n_estimators': [5, 10, 15, 20]}
     return par_grid
 
 
-@pytest.fixture(scope="module")
-def dml_plr_fixture(generate_data2, learner_l, learner_m, learner_g, score, dml_procedure, tune_on_folds):
-    par_grid = {'ml_l': get_par_grid(learner_l),
-                'ml_m': get_par_grid(learner_m),
-                'ml_g': get_par_grid(learner_g)}
+@pytest.fixture(scope='module')
+def dml_pq_fixture(generate_data_quantiles, treatment, quantile, learner_g, learner_m, dml_procedure, normalize_ipw,
+                   tune_on_folds):
+    par_grid = {'ml_g': get_par_grid(learner_g),
+                'ml_m': get_par_grid(learner_m)}
     n_folds_tune = 4
-
-    boot_methods = ['normal']
     n_folds = 2
-    n_rep_boot = 502
 
     # collect data
-    obj_dml_data = generate_data2
-
-    # Set machine learning methods for m & g
-    ml_l = _clone(learner_l)
-    ml_m = _clone(learner_m)
-    if score == 'IV-type':
-        ml_g = _clone(learner_g)
-    else:
-        ml_g = None
+    (x, y, d) = generate_data_quantiles
+    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
+    np.random.seed(42)
+    n_obs = len(y)
+    all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=d)
+    smpls = all_smpls[0]
 
-    np.random.seed(3141)
-    dml_plr_obj = dml.DoubleMLPLR(obj_dml_data,
-                                  ml_l, ml_m, ml_g,
-                                  n_folds,
-                                  score=score,
-                                  dml_procedure=dml_procedure)
+    np.random.seed(42)
+    dml_pq_obj = dml.DoubleMLPQ(obj_dml_data,
+                                clone(learner_g), clone(learner_m),
+                                treatment=treatment,
+                                quantile=quantile,
+                                n_folds=n_folds,
+                                n_rep=1,
+                                dml_procedure=dml_procedure,
+                                normalize_ipw=normalize_ipw,
+                                trimming_threshold=0.01,
+                                draw_sample_splitting=False)
 
+    # synchronize the sample splitting
+    dml_pq_obj.set_sample_splitting(all_smpls=all_smpls)
     # tune hyperparameters
-    tune_res = dml_plr_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune,
-                                return_tune_res=True)
-    assert isinstance(tune_res, list)
-
-    # fit with tuned parameters
-    dml_plr_obj.fit()
-
-    np.random.seed(3141)
-    y = obj_dml_data.y
-    x = obj_dml_data.x
-    d = obj_dml_data.d
-    n_obs = len(y)
-    all_smpls = draw_smpls(n_obs, n_folds)
-    smpls = all_smpls[0]
+    np.random.seed(42)
+    tune_res = dml_pq_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune, return_tune_res=False)
+    assert isinstance(tune_res, dml.DoubleMLPQ)
 
-    tune_g = (score == 'IV-type')
+    np.random.seed(42)
+    dml_pq_obj.fit()
+
+    np.random.seed(42)
     if tune_on_folds:
-        l_params, m_params, g_params = tune_nuisance_plr(y, x, d,
-                                                         _clone(learner_l), _clone(learner_m), _clone(learner_g),
-                                                         smpls, n_folds_tune,
-                                                         par_grid['ml_l'], par_grid['ml_m'], par_grid['ml_g'], tune_g)
+        g_params, m_params = tune_nuisance_pq(y, x, d,
+                                              clone(learner_g), clone(learner_m),
+                                              smpls, treatment, quantile,
+                                              n_folds_tune, par_grid['ml_g'], par_grid['ml_m'])
     else:
         xx = [(np.arange(len(y)), np.array([]))]
-        l_params, m_params, g_params = tune_nuisance_plr(y, x, d,
-                                                         _clone(learner_l), _clone(learner_m), _clone(learner_g),
-                                                         xx, n_folds_tune,
-                                                         par_grid['ml_l'], par_grid['ml_m'], par_grid['ml_g'], tune_g)
-        l_params = l_params * n_folds
+        g_params, m_params = tune_nuisance_pq(y, x, d,
+                                              clone(learner_g), clone(learner_m),
+                                              xx, treatment, quantile,
+                                              n_folds_tune, par_grid['ml_g'], par_grid['ml_m'])
+
         g_params = g_params * n_folds
         m_params = m_params * n_folds
 
-    res_manual = fit_plr(y, x, d, _clone(learner_l), _clone(learner_m), _clone(learner_g),
-                         all_smpls, dml_procedure, score,
-                         l_params=l_params, m_params=m_params, g_params=g_params)
-
-    res_dict = {'coef': dml_plr_obj.coef,
-                'coef_manual': res_manual['theta'],
-                'se': dml_plr_obj.se,
-                'se_manual': res_manual['se'],
-                'boot_methods': boot_methods}
-
-    for bootstrap in boot_methods:
-        np.random.seed(3141)
-        boot_theta, boot_t_stat = boot_plr(y, d, res_manual['thetas'], res_manual['ses'],
-                                           res_manual['all_l_hat'], res_manual['all_m_hat'], res_manual['all_g_hat'],
-                                           all_smpls, score, bootstrap, n_rep_boot)
-
-        np.random.seed(3141)
-        dml_plr_obj.bootstrap(method=bootstrap, n_rep_boot=n_rep_boot)
-        res_dict['boot_coef' + bootstrap] = dml_plr_obj.boot_coef
-        res_dict['boot_t_stat' + bootstrap] = dml_plr_obj.boot_t_stat
-        res_dict['boot_coef' + bootstrap + '_manual'] = boot_theta
-        res_dict['boot_t_stat' + bootstrap + '_manual'] = boot_t_stat
+    np.random.seed(42)
+    res_manual = fit_pq(y, x, d, quantile,
+                        learner_g=clone(learner_g),
+                        learner_m=clone(learner_m),
+                        all_smpls=all_smpls,
+                        treatment=treatment,
+                        dml_procedure=dml_procedure,
+                        n_rep=1, trimming_threshold=0.01,
+                        normalize_ipw=normalize_ipw,
+                        g_params=g_params, m_params=m_params)
+
+    res_dict = {'coef': dml_pq_obj.coef,
+                'coef_manual': res_manual['pq'],
+                'se': dml_pq_obj.se,
+                'se_manual': res_manual['se']}
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_plr_coef(dml_plr_fixture):
-    assert math.isclose(dml_plr_fixture['coef'],
-                        dml_plr_fixture['coef_manual'],
+def test_dml_pq_coef(dml_pq_fixture):
+    assert math.isclose(dml_pq_fixture['coef'],
+                        dml_pq_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_plr_se(dml_plr_fixture):
-    assert math.isclose(dml_plr_fixture['se'],
-                        dml_plr_fixture['se_manual'],
+def test_dml_pq_se(dml_pq_fixture):
+    assert math.isclose(dml_pq_fixture['se'],
+                        dml_pq_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
-
-
-@pytest.mark.ci
-def test_dml_plr_boot(dml_plr_fixture):
-    for bootstrap in dml_plr_fixture['boot_methods']:
-        assert np.allclose(dml_plr_fixture['boot_coef' + bootstrap],
-                           dml_plr_fixture['boot_coef' + bootstrap + '_manual'],
-                           rtol=1e-9, atol=1e-4)
-        assert np.allclose(dml_plr_fixture['boot_t_stat' + bootstrap],
-                           dml_plr_fixture['boot_t_stat' + bootstrap + '_manual'],
-                           rtol=1e-9, atol=1e-4)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_pq_tune.py` & `DoubleML-0.6.2/doubleml/tests/test_lpq.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import numpy as np
 import pytest
 import math
 
-from sklearn.base import clone
+import doubleml as dml
 
+from sklearn.base import clone
 from sklearn.linear_model import LogisticRegression
-from sklearn.ensemble import RandomForestClassifier
-
-import doubleml as dml
+from statsmodels.nonparametric.kde import KDEUnivariate
 
 from ._utils import draw_smpls
-from ._utils_pq_manual import fit_pq, tune_nuisance_pq
+from ._utils_lpq_manual import fit_lpq
+from .._utils import _default_kde
+
+
+def custom_kde(u, weights):
+    dens = KDEUnivariate(u)
+    dens.fit(kernel='epa', bw='silverman', weights=weights, fft=False)
+
+    return dens.evaluate(0)
 
 
 @pytest.fixture(scope='module',
                 params=[0, 1])
 def treatment(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[0.25, 0.5, 0.75])
+                params=[0.25, 0.75])
 def quantile(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[RandomForestClassifier(max_depth=5, random_state=42)])
-def learner_g(request):
-    return request.param
-
-
-@pytest.fixture(scope='module',
-                params=[RandomForestClassifier(max_depth=5, random_state=42)])
-def learner_m(request):
+                params=[LogisticRegression()])
+def learner(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
                 params=['dml1', 'dml2'])
 def dml_procedure(request):
     return request.param
@@ -46,106 +47,95 @@
 @pytest.fixture(scope='module',
                 params=[True, False])
 def normalize_ipw(request):
     return request.param
 
 
 @pytest.fixture(scope='module',
-                params=[True, False])
-def tune_on_folds(request):
+                params=[0.05])
+def trimming_threshold(request):
     return request.param
 
 
-def get_par_grid(learner):
-    if learner.__class__ in [RandomForestClassifier]:
-        par_grid = {'n_estimators': [5, 10, 15, 20]}
-    else:
-        assert learner.__class__ in [LogisticRegression]
-        par_grid = {'C': np.logspace(-4, 2, 10)}
-    return par_grid
+@pytest.fixture(scope='module',
+                params=['default', custom_kde])
+def kde(request):
+    return request.param
 
 
-@pytest.fixture(scope='module')
-def dml_pq_fixture(generate_data_quantiles, treatment, quantile, learner_g, learner_m, dml_procedure, normalize_ipw,
-                   tune_on_folds):
-    par_grid = {'ml_g': get_par_grid(learner_g),
-                'ml_m': get_par_grid(learner_m)}
-    n_folds_tune = 4
-    n_folds = 2
+@pytest.fixture(scope="module")
+def dml_lpq_fixture(generate_data_local_quantiles, treatment, quantile, learner,
+                    dml_procedure, normalize_ipw, trimming_threshold, kde):
+    n_folds = 3
 
     # collect data
-    (x, y, d) = generate_data_quantiles
-    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
+    (x, y, d, z) = generate_data_local_quantiles
+    obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d, z)
     np.random.seed(42)
     n_obs = len(y)
-    all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=d)
-    smpls = all_smpls[0]
-
-    np.random.seed(42)
-    dml_pq_obj = dml.DoubleMLPQ(obj_dml_data,
-                                clone(learner_g), clone(learner_m),
-                                treatment=treatment,
-                                quantile=quantile,
-                                n_folds=n_folds,
-                                n_rep=1,
-                                dml_procedure=dml_procedure,
-                                normalize_ipw=normalize_ipw,
-                                trimming_threshold=0.01,
-                                draw_sample_splitting=False)
-
-    # synchronize the sample splitting
-    dml_pq_obj.set_sample_splitting(all_smpls=all_smpls)
-    # tune hyperparameters
-    np.random.seed(42)
-    tune_res = dml_pq_obj.tune(par_grid, tune_on_folds=tune_on_folds, n_folds_tune=n_folds_tune, return_tune_res=False)
-    assert isinstance(tune_res, dml.DoubleMLPQ)
-
-    np.random.seed(42)
-    dml_pq_obj.fit()
+    strata = d + 2 * z
+    all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=strata)
 
     np.random.seed(42)
-    if tune_on_folds:
-        g_params, m_params = tune_nuisance_pq(y, x, d,
-                                              clone(learner_g), clone(learner_m),
-                                              smpls, treatment, quantile,
-                                              n_folds_tune, par_grid['ml_g'], par_grid['ml_m'])
+    if kde == 'default':
+        dml_lpq_obj = dml.DoubleMLLPQ(obj_dml_data,
+                                    clone(learner), clone(learner),
+                                    treatment=treatment,
+                                    quantile=quantile,
+                                    n_folds=n_folds,
+                                    n_rep=1,
+                                    dml_procedure=dml_procedure,
+                                    normalize_ipw=normalize_ipw,
+                                    trimming_threshold=trimming_threshold,
+                                    draw_sample_splitting=False)
+        # synchronize the sample splitting
+        dml_lpq_obj.set_sample_splitting(all_smpls=all_smpls)
+        dml_lpq_obj.fit()
+
+        np.random.seed(42)
+        res_manual = fit_lpq(y, x, d, z, quantile, clone(learner), clone(learner),
+                             all_smpls, treatment, dml_procedure,
+                             normalize_ipw=normalize_ipw, kde=_default_kde,
+                             n_rep=1, trimming_threshold=trimming_threshold)
     else:
-        xx = [(np.arange(len(y)), np.array([]))]
-        g_params, m_params = tune_nuisance_pq(y, x, d,
-                                              clone(learner_g), clone(learner_m),
-                                              xx, treatment, quantile,
-                                              n_folds_tune, par_grid['ml_g'], par_grid['ml_m'])
-
-        g_params = g_params * n_folds
-        m_params = m_params * n_folds
-
-    np.random.seed(42)
-    res_manual = fit_pq(y, x, d, quantile,
-                        learner_g=clone(learner_g),
-                        learner_m=clone(learner_m),
-                        all_smpls=all_smpls,
-                        treatment=treatment,
-                        dml_procedure=dml_procedure,
-                        n_rep=1, trimming_threshold=0.01,
-                        normalize_ipw=normalize_ipw,
-                        g_params=g_params, m_params=m_params)
-
-    res_dict = {'coef': dml_pq_obj.coef,
-                'coef_manual': res_manual['pq'],
-                'se': dml_pq_obj.se,
+        dml_lpq_obj = dml.DoubleMLLPQ(obj_dml_data,
+                                      clone(learner), clone(learner),
+                                      treatment=treatment,
+                                      quantile=quantile,
+                                      n_folds=n_folds,
+                                      n_rep=1,
+                                      dml_procedure=dml_procedure,
+                                      normalize_ipw=normalize_ipw,
+                                      kde=kde,
+                                      trimming_threshold=trimming_threshold,
+                                      draw_sample_splitting=False)
+
+        # synchronize the sample splitting
+        dml_lpq_obj.set_sample_splitting(all_smpls=all_smpls)
+        dml_lpq_obj.fit()
+
+        np.random.seed(42)
+        res_manual = fit_lpq(y, x, d, z, quantile, clone(learner), clone(learner),
+                             all_smpls, treatment, dml_procedure,
+                             normalize_ipw=normalize_ipw, kde=kde,
+                             n_rep=1, trimming_threshold=trimming_threshold)
+
+    res_dict = {'coef': dml_lpq_obj.coef,
+                'coef_manual': res_manual['lpq'],
+                'se': dml_lpq_obj.se,
                 'se_manual': res_manual['se']}
 
     return res_dict
 
 
 @pytest.mark.ci
-def test_dml_pq_coef(dml_pq_fixture):
-    assert math.isclose(dml_pq_fixture['coef'],
-                        dml_pq_fixture['coef_manual'],
+def test_dml_lpq_coef(dml_lpq_fixture):
+    assert math.isclose(dml_lpq_fixture['coef'],
+                        dml_lpq_fixture['coef_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
 
 
 @pytest.mark.ci
-def test_dml_pq_se(dml_pq_fixture):
-    assert math.isclose(dml_pq_fixture['se'],
-                        dml_pq_fixture['se_manual'],
+def test_dml_lpq_se(dml_lpq_fixture):
+    assert math.isclose(dml_lpq_fixture['se'],
+                        dml_lpq_fixture['se_manual'],
                         rel_tol=1e-9, abs_tol=1e-4)
```

### Comparing `DoubleML-0.6.1/doubleml/tests/test_qte.py` & `DoubleML-0.6.2/doubleml/tests/test_qte.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import numpy as np
 import pandas as pd
 import pytest
+import copy
 
 import doubleml as dml
 
 from sklearn.base import clone
 from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
 
 from ._utils import draw_smpls
 from ._utils_qte_manual import fit_qte, boot_qte, confint_qte
 
 from doubleml.datasets import make_irm_data
 from .._utils import _default_kde
 
 
+quantiles = [0.25, 0.5, 0.75]
+n_quantiles = len(quantiles)
+n_rep = 1
+
 @pytest.fixture(scope='module',
                 params=[RandomForestClassifier(max_depth=2, n_estimators=10, random_state=42),
                         LogisticRegression()])
 def learner(request):
     return request.param
 
 
@@ -39,38 +44,36 @@
 def kde(request):
     return request.param
 
 
 @pytest.fixture(scope="module")
 def dml_qte_fixture(generate_data_quantiles, learner, dml_procedure, normalize_ipw, kde):
     n_folds = 3
-    n_rep = 1
     boot_methods = ['normal']
     n_rep_boot = 2
 
     # collect data
     (x, y, d) = generate_data_quantiles
     obj_dml_data = dml.DoubleMLData.from_arrays(x, y, d)
 
     # Set machine learning methods for g & m
     ml_g = clone(learner)
     ml_m = clone(learner)
 
     np.random.seed(42)
-    quantiles = [0.25, 0.5, 0.75]
     dml_qte_obj = dml.DoubleMLQTE(obj_dml_data,
                                   ml_g, ml_m,
                                   quantiles=quantiles,
                                   n_folds=n_folds,
                                   n_rep=n_rep,
                                   dml_procedure=dml_procedure,
                                   normalize_ipw=normalize_ipw,
                                   trimming_threshold=1e-12,
                                   kde=kde)
-
+    unfitted_qte_model = copy.copy(dml_qte_obj)
     dml_qte_obj.fit()
 
     np.random.seed(42)
     n_obs = len(y)
     all_smpls = draw_smpls(n_obs, n_folds, n_rep=1, groups=d)
     res_manual = fit_qte(y, x, d, quantiles, ml_g, ml_g, all_smpls,
                          n_rep=n_rep, dml_procedure=dml_procedure,
@@ -84,15 +87,16 @@
     res_dict = {'coef': dml_qte_obj.coef,
                 'coef_manual': res_manual['qte'],
                 'se': dml_qte_obj.se,
                 'se_manual': res_manual['se'],
                 'boot_methods': boot_methods,
                 'ci': ci.to_numpy(),
                 'ci_manual': ci_manual.to_numpy(),
-                'qte_model': dml_qte_obj}
+                'qte_model': dml_qte_obj,
+                'unfitted_qte_model': unfitted_qte_model}
 
     for bootstrap in boot_methods:
         np.random.seed(42)
         boot_qte_coef, boot_t_stat = boot_qte(res_manual['scaled_scores'], res_manual['ses'], quantiles,
                                               all_smpls, n_rep, bootstrap, n_rep_boot, apply_cross_fitting=True)
 
         np.random.seed(42)
@@ -161,7 +165,10 @@
         dml_obj = dml.DoubleMLQTE(obj_dml_data, ml_g, ml_m, draw_sample_splitting=False)
         _ = dml_obj.smpls
 
 
 def test_doubleml_qte_return_types(dml_qte_fixture):
     assert isinstance(dml_qte_fixture['qte_model'].__str__(), str)
     assert isinstance(dml_qte_fixture['qte_model'].summary, pd.DataFrame)
+
+    assert dml_qte_fixture['qte_model'].all_coef.shape == (n_quantiles, n_rep)
+    assert isinstance(dml_qte_fixture['unfitted_qte_model'].summary, pd.DataFrame)
```

### Comparing `DoubleML-0.6.1/setup.py` & `DoubleML-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'Documentation': 'https://docs.doubleml.org',
     'Source Code': 'https://github.com/DoubleML/doubleml-for-py',
     'Bug Tracker': 'https://github.com/DoubleML/doubleml-for-py/issues',
 }
 
 setup(
     name='DoubleML',
-    version='0.6.1',
+    version='0.6.2',
     author='Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.',
     maintainer='Malte S. Kurz',
     maintainer_email='malte.simon.kurz@uni-hamburg.de',
     description='Double Machine Learning in Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://docs.doubleml.org',
```

