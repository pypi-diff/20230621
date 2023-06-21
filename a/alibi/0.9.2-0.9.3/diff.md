# Comparing `tmp/alibi-0.9.2.tar.gz` & `tmp/alibi-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alibi-0.9.2.tar", last modified: Fri Apr 28 13:44:02 2023, max compression
+gzip compressed data, was "alibi-0.9.3.tar", last modified: Wed Jun 21 13:28:31 2023, max compression
```

## Comparing `alibi-0.9.2.tar` & `alibi-0.9.3.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.075916 alibi-0.9.2/
--rw-r--r--   0 janis     (1000) janis     (1000)    11354 2023-04-28 13:41:02.000000 alibi-0.9.2/LICENSE
--rw-r--r--   0 janis     (1000) janis     (1000)       58 2023-04-28 13:41:02.000000 alibi-0.9.2/MANIFEST.in
--rw-r--r--   0 janis     (1000) janis     (1000)    20875 2023-04-28 13:44:02.079249 alibi-0.9.2/PKG-INFO
--rw-r--r--   0 janis     (1000) janis     (1000)    19975 2023-04-28 13:41:02.000000 alibi-0.9.2/README.md
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.045915 alibi-0.9.2/alibi/
--rw-r--r--   0 janis     (1000) janis     (1000)      187 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/api/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7096 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/defaults.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6960 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/interfaces.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/api/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2793 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/tests/test_interfaces.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/confidence/
--rw-r--r--   0 janis     (1000) janis     (1000)      251 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18571 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/model_linearity.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/confidence/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8326 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/tests/test_model_linearity.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2174 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/tests/test_trustscore.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8214 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/trustscore.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/data/
--rw-r--r--   0 janis     (1000) janis     (1000)   116015 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/data/cats.tar.gz
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/datasets/
--rw-r--r--   0 janis     (1000) janis     (1000)      451 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12968 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/default.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1037 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/tensorflow.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/datasets/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4559 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/tests/test_datasets.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1813 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/exceptions.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.052582 alibi-0.9.2/alibi/explainers/
--rw-r--r--   0 janis     (1000) janis     (1000)     2230 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    29966 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/ale.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/anchors/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    35805 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4371 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_explanation.py
--rw-r--r--   0 janis     (1000) janis     (1000)    28092 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_image.py
--rw-r--r--   0 janis     (1000) janis     (1000)    49286 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12848 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_tabular_distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)    24277 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_text.py
--rw-r--r--   0 janis     (1000) janis     (1000)    27223 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/language_model_text_sampler.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16961 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/text_samplers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/backends/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4211 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    39363 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/cfrl_tabular.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/backends/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17765 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6141 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_tabular.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/backends/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    19783 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6379 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    35265 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cem.py
--rw-r--r--   0 janis     (1000) janis     (1000)    66499 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cfproto.py
--rw-r--r--   0 janis     (1000) janis     (1000)    44884 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    23850 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cfrl_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    27167 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/counterfactual.py
--rw-r--r--   0 janis     (1000) janis     (1000)    56445 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/integrated_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)    73613 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/partial_dependence.py
--rw-r--r--   0 janis     (1000) janis     (1000)    39164 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/pd_variance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    45135 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/permutation_importance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    80284 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/shap_wrappers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/similarity/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/similarity/backends/
--rw-r--r--   0 janis     (1000) janis     (1000)     1321 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4753 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/base.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.059249 alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4341 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8837 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    13302 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/grad.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2654 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/metrics.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/explainers/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    11006 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17481 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_ale.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2582 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7874 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_image.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16247 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18774 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_text.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1572 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_cem.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6681 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_cfproto.py
--rw-r--r--   0 janis     (1000) janis     (1000)    20718 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_cfrl.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4900 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_counterfactual.py
--rw-r--r--   0 janis     (1000) janis     (1000)    37074 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_integrated_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)    42674 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_partial_dependence.py
--rw-r--r--   0 janis     (1000) janis     (1000)    28620 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_pd_variance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    23539 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_permutation_importance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    65433 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_shap_wrappers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5894 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5864 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_backends.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17977 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
--rw-r--r--   0 janis     (1000) janis     (1000)     9302 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3086 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/utils.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/models/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/models/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)      477 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2748 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3094 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8134 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/cfrl_models.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4952 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/metrics.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12988 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/model.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.065916 alibi-0.9.2/alibi/models/pytorch/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1767 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)      647 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3778 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_cfrl_models.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1847 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_metrics.py
--rw-r--r--   0 janis     (1000) janis     (1000)    21220 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_model.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.065916 alibi-0.9.2/alibi/models/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)      486 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2913 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3378 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8692 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/cfrl_models.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.065916 alibi-0.9.2/alibi/models/tensorflow/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1655 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/test_actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)      643 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/test_autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3708 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/test_cfrl_models.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.069249 alibi-0.9.2/alibi/prototypes/
--rw-r--r--   0 janis     (1000) janis     (1000)      250 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    32709 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/protoselect.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.069249 alibi-0.9.2/alibi/prototypes/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    11674 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/tests/test_protoselect.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3195 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/tests/test_utils.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16242 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/saving.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.072583 alibi-0.9.2/alibi/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)      622 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7261 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/test_dep_management.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18797 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/test_saving.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1033 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/test_utils.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4809 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/utils.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.075916 alibi-0.9.2/alibi/utils/
--rw-r--r--   0 janis     (1000) janis     (1000)     1276 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5000 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/approximation_methods.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2652 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/data.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3592 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/discretizer.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12076 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/distance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    31339 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)      582 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/distributions.py
--rw-r--r--   0 janis     (1000) janis     (1000)      513 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/download.py
--rw-r--r--   0 janis     (1000) janis     (1000)      320 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/frameworks.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2915 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4666 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/kernel.py
--rw-r--r--   0 janis     (1000) janis     (1000)    15255 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/lang_model.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4718 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/mapping.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5365 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/missing_optional_dependency.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.075916 alibi-0.9.2/alibi/utils/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)      194 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/mocked_opt_dep.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1014 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_data.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3193 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_distance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    15565 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1631 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2855 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_import_optional.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1103 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_mapping.py
--rw-r--r--   0 janis     (1000) janis     (1000)      398 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_misc.py
--rw-r--r--   0 janis     (1000) janis     (1000)      919 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tf.py
--rw-r--r--   0 janis     (1000) janis     (1000)    22959 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/visualization.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1707 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/wrappers.py
--rw-r--r--   0 janis     (1000) janis     (1000)      212 2023-04-28 13:41:49.000000 alibi-0.9.2/alibi/version.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.045915 alibi-0.9.2/alibi.egg-info/
--rw-r--r--   0 janis     (1000) janis     (1000)    20875 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/PKG-INFO
--rw-r--r--   0 janis     (1000) janis     (1000)     5394 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/SOURCES.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/dependency_links.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/not-zip-safe
--rw-r--r--   0 janis     (1000) janis     (1000)      649 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/requires.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        6 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/top_level.txt
--rw-r--r--   0 janis     (1000) janis     (1000)     2066 2023-04-28 13:44:02.079249 alibi-0.9.2/setup.cfg
--rw-r--r--   0 janis     (1000) janis     (1000)     2937 2023-04-28 13:41:02.000000 alibi-0.9.2/setup.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.434628 alibi-0.9.3/
+-rw-r--r--   0 janis     (1000) janis     (1000)    11354 2023-06-21 11:43:55.000000 alibi-0.9.3/LICENSE
+-rw-r--r--   0 janis     (1000) janis     (1000)       58 2023-06-21 11:43:55.000000 alibi-0.9.3/MANIFEST.in
+-rw-r--r--   0 janis     (1000) janis     (1000)    20926 2023-06-21 13:28:31.434628 alibi-0.9.3/PKG-INFO
+-rw-r--r--   0 janis     (1000) janis     (1000)    19975 2023-06-21 11:44:13.000000 alibi-0.9.3/README.md
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.414628 alibi-0.9.3/alibi/
+-rw-r--r--   0 janis     (1000) janis     (1000)      187 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/api/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     7096 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/defaults.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6960 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/interfaces.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/api/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2793 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/tests/test_interfaces.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/confidence/
+-rw-r--r--   0 janis     (1000) janis     (1000)      251 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    18571 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/model_linearity.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/confidence/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8326 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/tests/test_model_linearity.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2174 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/tests/test_trustscore.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8182 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/trustscore.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/data/
+-rw-r--r--   0 janis     (1000) janis     (1000)   116015 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/data/cats.tar.gz
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/datasets/
+-rw-r--r--   0 janis     (1000) janis     (1000)      451 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12940 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/default.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1037 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/tensorflow.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/datasets/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4559 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/tests/test_datasets.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1813 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/exceptions.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/
+-rw-r--r--   0 janis     (1000) janis     (1000)     2230 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    29966 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/ale.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/anchors/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    35805 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4371 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_explanation.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    28076 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_image.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    49264 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12848 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_tabular_distributed.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    24277 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_text.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    27223 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/language_model_text_sampler.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    16961 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/text_samplers.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/backends/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4211 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    39331 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/cfrl_tabular.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/backends/pytorch/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/pytorch/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    17733 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6141 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_tabular.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/backends/tensorflow/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/tensorflow/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    19783 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6379 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    35184 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cem.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    66395 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cfproto.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    44884 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    23850 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cfrl_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    27167 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/counterfactual.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    56311 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/integrated_gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    73509 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/partial_dependence.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    39110 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/pd_variance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    45107 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/permutation_importance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    80156 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/shap_wrappers.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/similarity/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/similarity/backends/
+-rw-r--r--   0 janis     (1000) janis     (1000)     1321 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4753 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/base.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4341 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8837 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    13302 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/grad.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2654 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/metrics.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/explainers/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    11006 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/conftest.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    17481 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_ale.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2582 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     7874 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_image.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    16247 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    18774 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_text.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1572 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_cem.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6681 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_cfproto.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    20718 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_cfrl.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4900 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_counterfactual.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    37074 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_integrated_gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    42674 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_partial_dependence.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    28620 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_pd_variance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    23539 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_permutation_importance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    65433 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_shap_wrappers.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     5894 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/conftest.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     5864 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_backends.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    17977 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     9302 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3086 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/utils.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/models/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/pytorch/
+-rw-r--r--   0 janis     (1000) janis     (1000)      477 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2748 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3094 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8134 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/cfrl_models.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4952 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/metrics.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12988 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/model.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/pytorch/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1767 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      647 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3778 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_cfrl_models.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1847 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_metrics.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    21220 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_model.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/tensorflow/
+-rw-r--r--   0 janis     (1000) janis     (1000)      486 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2913 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3378 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8692 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/cfrl_models.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/tensorflow/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1655 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/test_actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      643 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/test_autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3708 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/test_cfrl_models.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/prototypes/
+-rw-r--r--   0 janis     (1000) janis     (1000)      250 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    32709 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/protoselect.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/prototypes/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    11674 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/tests/test_protoselect.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3195 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/tests/test_utils.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    16214 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/saving.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      622 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/conftest.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     7230 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/test_dep_management.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    18797 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/test_saving.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1033 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/test_utils.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4809 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/utils.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.431295 alibi-0.9.3/alibi/utils/
+-rw-r--r--   0 janis     (1000) janis     (1000)     1276 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4968 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/approximation_methods.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2652 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/data.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3592 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/discretizer.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12076 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/distance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    31311 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/distributed.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      582 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/distributions.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      513 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/download.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      320 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/frameworks.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2915 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4666 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/kernel.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    15019 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/lang_model.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4718 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/mapping.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     5365 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/missing_optional_dependency.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.434628 alibi-0.9.3/alibi/utils/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      194 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/mocked_opt_dep.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1014 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_data.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3193 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_distance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    15565 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_distributed.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1631 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2855 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_import_optional.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1103 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_mapping.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      398 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_misc.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      919 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tf.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    22911 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/visualization.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1707 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/wrappers.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      212 2023-06-21 13:27:29.000000 alibi-0.9.3/alibi/version.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi.egg-info/
+-rw-r--r--   0 janis     (1000) janis     (1000)    20926 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/PKG-INFO
+-rw-r--r--   0 janis     (1000) janis     (1000)     5394 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/SOURCES.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/dependency_links.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/not-zip-safe
+-rw-r--r--   0 janis     (1000) janis     (1000)      649 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/requires.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)        6 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/top_level.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)     2121 2023-06-21 13:28:31.434628 alibi-0.9.3/setup.cfg
+-rw-r--r--   0 janis     (1000) janis     (1000)     2994 2023-06-21 11:43:55.000000 alibi-0.9.3/setup.py
```

### Comparing `alibi-0.9.2/LICENSE` & `alibi-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/PKG-INFO` & `alibi-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.2
+Version: 0.9.3
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 Provides-Extra: shap
 Provides-Extra: tensorflow
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: alibi Version: 0.9.2 Summary: Algorithms for
+Metadata-Version: 2.1 Name: alibi Version: 0.9.3 Summary: Algorithms for
 monitoring and explaining machine learning models Home-page: https://
 github.com/SeldonIO/alibi Author: Seldon Technologies Ltd. Author-email:
 hello@seldon.io License: Apache 2.0 Classifier: Intended Audience :: Science/
 Research Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Scientific/Engineering Requires-Python: >=3.7 Description-Content-
-Type: text/markdown Provides-Extra: ray Provides-Extra: shap Provides-Extra:
-tensorflow Provides-Extra: torch Provides-Extra: all License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+ray Provides-Extra: shap Provides-Extra: tensorflow Provides-Extra: torch
+Provides-Extra: all License-File: LICENSE
                                  [Alibi Logo]
  [![Build Status](https://github.com/SeldonIO/alibi-detect/workflows/CI/
 badge.svg?branch=master)][#build-status] [![Documentation Status](https://
 readthedocs.org/projects/alibi/badge/?version=latest)][#docs-package] [!
 [codecov](https://codecov.io/gh/SeldonIO/alibi/branch/master/graph/badge.svg)]
 (https://codecov.io/gh/SeldonIO/alibi) [![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/alibi?logo=pypi&style=flat&color=blue)][#pypi-
```

### Comparing `alibi-0.9.2/README.md` & `alibi-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/api/defaults.py` & `alibi-0.9.3/alibi/api/defaults.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/api/interfaces.py` & `alibi-0.9.3/alibi/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/api/tests/test_interfaces.py` & `alibi-0.9.3/alibi/api/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/confidence/model_linearity.py` & `alibi-0.9.3/alibi/confidence/model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/confidence/tests/test_model_linearity.py` & `alibi-0.9.3/alibi/confidence/tests/test_model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/confidence/tests/test_trustscore.py` & `alibi-0.9.3/alibi/confidence/tests/test_trustscore.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/confidence/trustscore.py` & `alibi-0.9.3/alibi/confidence/trustscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         if len(X.shape) > 2:
             logger.warning('Reshaping data from {0} to {1} so k-d trees can '
                            'be built.'.format(X.shape, X.reshape(X.shape[0], -1).shape))
             X = X.reshape(X.shape[0], -1)
 
         # make sure Y represents predicted classes, not one-hot encodings
         if len(Y.shape) > 1:
-            Y = np.argmax(Y, axis=1)  # type: ignore
+            Y = np.argmax(Y, axis=1)
 
         if self.filter == 'probability_knn':
             X_filter, Y_filter = self.filter_by_probability_knn(X, Y)
 
         for c in range(self.classes):
 
             if self.filter is None:
@@ -166,15 +166,15 @@
 
         Returns
         -------
         Batch with trust scores and the closest not predicted class.
         """
         # make sure Y represents predicted classes, not probabilities
         if len(Y.shape) > 1:
-            Y = np.argmax(Y, axis=1)  # type: ignore
+            Y = np.argmax(Y, axis=1)
 
         # KDTree needs 2D data
         if len(X.shape) > 2:
             logger.warning('Reshaping data from {0} to {1} so k-d trees can '
                            'be queried.'.format(X.shape, X.reshape(X.shape[0], -1).shape))
             X = X.reshape(X.shape[0], -1)
```

### Comparing `alibi-0.9.2/alibi/data/cats.tar.gz` & `alibi-0.9.3/alibi/data/cats.tar.gz`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/datasets/default.py` & `alibi-0.9.3/alibi/datasets/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
         # labels
         name = member.name.split('_')
         target.append(int(name.pop(1)))
         target_names.append('_'.join(name).split('.')[0])
     tar.close()
 
-    images = np.concatenate(images, axis=0)  # type: ignore[assignment]
+    images = np.concatenate(images, axis=0)
     targets = np.asarray(target)
     if return_X_y:
         return images, targets  # type: ignore[return-value] # TODO: allow redefiniton
     else:
         return Bunch(data=images, target=targets, target_names=target_names)
```

### Comparing `alibi-0.9.2/alibi/datasets/tensorflow.py` & `alibi-0.9.3/alibi/datasets/tensorflow.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/datasets/tests/test_datasets.py` & `alibi-0.9.3/alibi/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/exceptions.py` & `alibi-0.9.3/alibi/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/__init__.py` & `alibi-0.9.3/alibi/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/ale.py` & `alibi-0.9.3/alibi/explainers/ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/anchors/anchor_base.py` & `alibi-0.9.3/alibi/explainers/anchors/anchor_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/anchors/anchor_explanation.py` & `alibi-0.9.3/alibi/explainers/anchors/anchor_explanation.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/anchors/anchor_image.py` & `alibi-0.9.3/alibi/explainers/anchors/anchor_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             labels = self.compare_labels(raw_data)
             covered_true = raw_data[labels][: self.n_covered_ex]
             covered_true = [scale_image(img) for img in covered_true]
             covered_false = raw_data[np.logical_not(labels)][: self.n_covered_ex]
             covered_false = [scale_image(img) for img in covered_false]
             # coverage set to -1.0 as we can't compute 'true' coverage for this model
 
-            return [covered_true, covered_false, labels.astype(int), data, -1.0, anchor[0]]  # type: ignore
+            return [covered_true, covered_false, labels.astype(int), data, -1.0, anchor[0]]
 
         else:
             data = self._choose_superpixels(num_samples)
             data[:, anchor[1]] = 1  # superpixels in candidate anchor are not perturbed
 
             return [data]
```

### Comparing `alibi-0.9.2/alibi/explainers/anchors/anchor_tabular.py` & `alibi-0.9.3/alibi/explainers/anchors/anchor_tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
             # and go straight to treating unknown features
             return
 
         end_idx = np.searchsorted(np.cumsum(nb_partial_anchors), num_samples)
 
         # replace partial anchors with partial anchors drawn from the training dataset
         # samp_idxs are arrays of training set row indices from where partial anchors are extracted for replacement
-        for idx, n_samp in enumerate(nb_partial_anchors[start_idx:end_idx + 1], start=start_idx):  # type: ignore[misc]
+        for idx, n_samp in enumerate(nb_partial_anchors[start_idx:end_idx + 1], start=start_idx):
             if num_samples >= n_samp:
                 samp_idxs = partial_anchor_rows[n_anchor_feats - idx - 1]
                 num_samples -= n_samp
             else:
                 if num_samples <= partial_anchor_rows[n_anchor_feats - idx - 1].shape[0]:
                     samp_idxs = np.random.choice(partial_anchor_rows[n_anchor_feats - idx - 1], num_samples)
                 else:
```

### Comparing `alibi-0.9.2/alibi/explainers/anchors/anchor_tabular_distributed.py` & `alibi-0.9.3/alibi/explainers/anchors/anchor_tabular_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/anchors/anchor_text.py` & `alibi-0.9.3/alibi/explainers/anchors/anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/anchors/language_model_text_sampler.py` & `alibi-0.9.3/alibi/explainers/anchors/language_model_text_sampler.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/anchors/text_samplers.py` & `alibi-0.9.3/alibi/explainers/anchors/text_samplers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/backends/cfrl_base.py` & `alibi-0.9.3/alibi/explainers/backends/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/backends/cfrl_tabular.py` & `alibi-0.9.3/alibi/explainers/backends/cfrl_tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,15 +506,15 @@
 
         # Permute columns and cast to object
         np_X_inv = np_X_inv[:, inv_perm].astype(object)
 
         # Cast numerical features to desired data types
         for i, fn in enumerate(feature_names):
             if i in numerical_ids:
-                ft_type = feature_types[fn] if fn in feature_types else float  # type: ignore[index,operator]
+                ft_type = feature_types[fn] if fn in feature_types else float
 
                 # Round `int` type features to the closest integer number to avoid rounding error when casting to `int`.
                 # The casting to `np.float32` is due to previous casting to `object` which raises an error when
                 # applying `np.rint` (i.e., 'TypeError: loop of ufunc does not support argument 0 of type float which
                 # has no callable rint method')
                 if ft_type == int:
                     np_X_inv[:, i] = np.rint(np_X_inv[:, i].astype(np.float32))
```

### Comparing `alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_base.py` & `alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,20 +471,20 @@
     Y_m = torch.tensor(Y_m).float().to(device)  # type: ignore
     Y_t = torch.tensor(Y_t).float().to(device)  # type: ignore
     C = torch.tensor(C).float().to(device) if (C is not None) else None  # type: ignore
     R_tilde = torch.tensor(R_tilde).float().to(device)  # type: ignore
 
     # Define state by concatenating the input embedding, the classification label, the target label, and optionally
     # the conditional vector if exists.
-    state = [Z, Y_m, Y_t] + ([C] if (C is not None) else [])  # type: ignore
+    state = [Z, Y_m, Y_t] + ([C] if (C is not None) else [])
     state = torch.cat(state, dim=1).to(device)  # type: ignore
 
     # Define input for critic, compute q-values and append critic's loss.
     input_critic = torch.cat([state, Z_cf_tilde], dim=1).float()  # type: ignore
-    output_critic = critic(input_critic).squeeze(1)  # type: ignore
+    output_critic = critic(input_critic).squeeze(1)
     loss_critic = F.mse_loss(output_critic, R_tilde)  # type: ignore
     losses.update({"critic_loss": loss_critic.item()})
 
     # Update critic by gradient step.
     optimizer_critic.zero_grad()
     loss_critic.backward()
     optimizer_critic.step()
```

### Comparing `alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_tabular.py` & `alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_base.py` & `alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_tabular.py` & `alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/cem.py` & `alibi-0.9.3/alibi/explainers/cem.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,17 +486,17 @@
             Returns
             -------
             Bool whether PP or PN conditions hold.
             """
             if not isinstance(x, (float, int, np.int64)):
                 x = np.copy(x)
                 if self.mode == "PP":
-                    x[y] -= self.kappa  # type:ignore
+                    x[y] -= self.kappa
                 elif self.mode == "PN":
-                    x[y] += self.kappa  # type:ignore
+                    x[y] += self.kappa
                 x = np.argmax(x)  # type:ignore
             if self.mode == "PP":
                 return x == y
             else:
                 return x != y
 
         # set the lower and upper bounds for the constant 'c' to scale the attack loss term
@@ -550,16 +550,16 @@
                     if i % self.update_num_grad == 0 and i > 0:  # compute numerical gradients
                         c = self.const.eval(session=self.sess)
                         X_der_batch = np.concatenate(X_der_batch)
                         X_der_batch_s = np.concatenate(X_der_batch_s)
                         grads_num = self.get_gradients(X_der_batch, Y) * c
                         grads_num_s = self.get_gradients(X_der_batch_s, Y) * c
                         # clip gradients
-                        grads_num = np.clip(grads_num, self.clip[0], self.clip[1])  # type:ignore
-                        grads_num_s = np.clip(grads_num_s, self.clip[0], self.clip[1])  # type: ignore
+                        grads_num = np.clip(grads_num, self.clip[0], self.clip[1])
+                        grads_num_s = np.clip(grads_num_s, self.clip[0], self.clip[1])
                         X_der_batch, X_der_batch_s = [], []
 
                 # compute and clip gradients defined in graph
                 grads_vars_graph = self.sess.run(self.compute_grads)
                 grads_graph = [g for g, _ in grads_vars_graph][0]
                 grads_graph = np.clip(grads_graph, self.clip[0], self.clip[1])
 
@@ -597,20 +597,20 @@
                     print('\nIteration: {}; Const: {}'.format(i, const[0]))
                     print('Loss total: {:.3f}, loss attack: {:.3f}'.format(loss_tot, loss_attack))
                     print('L2: {:.3f}, L1: {:.3f}, loss AE: {:.3f}'.format(loss_l2, loss_l1, loss_ae))
                     print('Target proba: {:.2f}, max non target proba: {:.2f}'.format(target_proba,
                                                                                       nontarget_proba_max))
                     print('Gradient graph min/max: {:.3f}/{:.3f}'.format(grads_graph.min(), grads_graph.max()))
                     print('Gradient graph mean/abs mean: {:.3f}/{:.3f}'
-                          .format(np.mean(grads_graph), np.mean(np.abs(grads_graph))))  # type: ignore
+                          .format(np.mean(grads_graph), np.mean(np.abs(grads_graph))))
                     if not self.model:
                         print('Gradient numerical attack min/max: {:.3f}/{:.3f}'
-                              .format(grads_num.min(), grads_num.max()))  # type: ignore
-                        print('Gradient numerical mean/abs mean: {:.3f}/{:.3f}'
-                              .format(np.mean(grads_num), np.mean(np.abs(grads_num))))  # type: ignore
+                              .format(grads_num.min(), grads_num.max()))
+                        print('Gradient numerical mean/abs mean: {:.3f}/{:.3f}'  # type: ignore[str-format]
+                              .format(np.mean(grads_num), np.mean(np.abs(grads_num))))
                     sys.stdout.flush()
 
                 # update best perturbation (distance) and class probabilities
                 # if beta * L1 + L2 < current best and predicted label is the same as the initial label (for PP) or
                 # different from the initial label (for PN); update best current step or global perturbations
                 for batch_idx, (dist, proba, adv_idx) in enumerate(zip(loss_l1_l2, pred_proba, adv)):
                     # current step
```

### Comparing `alibi-0.9.2/alibi/explainers/cfproto.py` & `alibi-0.9.3/alibi/explainers/cfproto.py`

 * *Files 1% similar despite different names*

```diff
@@ -738,25 +738,25 @@
                 raise ValueError('d_type needs to be "abdm", "mvdm" or "abdm-mvdm". '
                                  '{} is not supported.'.format(d_type))
 
             # pairwise distances for categorical variables
             if d_type == 'abdm':
                 d_pair = abdm(train_data_bin, self.cat_vars_ord, cat_vars_bin)
             elif d_type == 'mvdm':
-                d_pair = mvdm(train_data_ord, preds, self.cat_vars_ord, alpha=1)  # type: ignore
+                d_pair = mvdm(train_data_ord, preds, self.cat_vars_ord, alpha=1)
 
             # combined distance measure
             if d_type == 'abdm-mvdm':
                 if w is None:
                     msg = "Must specify a value for `w` if using d_type='abdm-mvdm'"
                     raise ValueError(msg)
 
                 # pairwise distances
                 d_abdm = abdm(train_data_bin, self.cat_vars_ord, cat_vars_bin)
-                d_mvdm = mvdm(train_data_ord, preds, self.cat_vars_ord, alpha=1)  # type: ignore
+                d_mvdm = mvdm(train_data_ord, preds, self.cat_vars_ord, alpha=1)
 
                 # multidim scaled distances
                 d_abs_abdm, _ = multidim_scaling(d_abdm, n_components=2, use_metric=True,
                                                  feature_range=self.feature_range,  # type: ignore[arg-type]
                                                  standardize_cat_vars=standardize_cat_vars,
                                                  smooth=smooth, center=center,
                                                  update_feature_range=False)
@@ -806,15 +806,15 @@
             logger.warning('No encoder specified. Using k-d trees to represent class prototypes.')
             if trustscore_kwargs is not None:
                 ts = TrustScore(**trustscore_kwargs)
             else:
                 ts = TrustScore()
             if self.is_cat:  # map categorical to numerical data
                 train_data = ord_to_num(train_data_ord, self.d_abs)
-            ts.fit(train_data, preds, classes=self.classes)  # type: ignore
+            ts.fit(train_data, preds, classes=self.classes)
             self.kdtrees = ts.kdtrees
             self.X_by_class = ts.X_kdtree
 
         return self
 
     def loss_fn(self, pred_proba: np.ndarray, Y: np.ndarray) -> np.ndarray:
         """
@@ -1003,16 +1003,16 @@
 
             Returns
             -------
             Bool whether counterfactual conditions hold.
             """
             if not isinstance(x, (float, int, np.int64)):
                 x = np.copy(x)
-                x[y] += self.kappa  # type: ignore
-                x = np.argmax(x)  # type: ignore
+                x[y] += self.kappa
+                x = np.argmax(x)  # type: ignore[assignment]
             return x != y
 
         # define target classes for prototype if not specified yet
         if target_class is None:
             target_class = list(range(self.classes))
             target_class.remove(np.argmax(Y, axis=1))
             if verbose:
@@ -1127,16 +1127,16 @@
                         X_der_batch = np.concatenate(X_der_batch)
                         X_der_batch_s = np.concatenate(X_der_batch_s)
                         grads_num = self.get_gradients(X_der_batch, Y, cat_vars_ord=self.cat_vars_ord,
                                                        grads_shape=pert_shape[1:]) * c
                         grads_num_s = self.get_gradients(X_der_batch_s, Y, cat_vars_ord=self.cat_vars_ord,
                                                          grads_shape=pert_shape[1:]) * c
                         # clip gradients
-                        grads_num = np.clip(grads_num, self.clip[0], self.clip[1])  # type: ignore
-                        grads_num_s = np.clip(grads_num_s, self.clip[0], self.clip[1])  # type: ignore
+                        grads_num = np.clip(grads_num, self.clip[0], self.clip[1])
+                        grads_num_s = np.clip(grads_num_s, self.clip[0], self.clip[1])
                         X_der_batch, X_der_batch_s = [], []
 
                 # compute and clip gradients defined in graph
                 grads_vars_graph = self.sess.run(self.compute_grads)
                 grads_graph = [g for g, _ in grads_vars_graph][0]
                 grads_graph = np.clip(grads_graph, self.clip[0], self.clip[1])
 
@@ -1198,20 +1198,20 @@
                     print('Loss total: {:.3f}, loss attack: {:.3f}'.format(loss_tot, loss_attack))
                     print('L2: {:.3f}, L1: {:.3f}, loss AE: {:.3f}'.format(loss_l2, loss_l1, loss_ae))
                     print('Loss proto: {:.3f}'.format(loss_proto))
                     print('Target proba: {:.2f}, max non target proba: {:.2f}'.format(target_proba,
                                                                                       nontarget_proba_max))
                     print('Gradient graph min/max: {:.3f}/{:.3f}'.format(grads_graph.min(), grads_graph.max()))
                     print('Gradient graph mean/abs mean: {:.3f}/{:.3f}'
-                          .format(np.mean(grads_graph), np.mean(np.abs(grads_graph))))  # type: ignore
+                          .format(np.mean(grads_graph), np.mean(np.abs(grads_graph))))
                     if not self.model:
                         print('Gradient numerical attack min/max: {:.3f}/{:.3f}'
-                              .format(grads_num.min(), grads_num.max()))  # type: ignore
-                        print('Gradient numerical mean/abs mean: {:.3f}/{:.3f}'
-                              .format(np.mean(grads_num), np.mean(np.abs(grads_num))))  # type: ignore
+                              .format(grads_num.min(), grads_num.max()))
+                        print('Gradient numerical mean/abs mean: {:.3f}/{:.3f}'  # type: ignore[str-format]
+                              .format(np.mean(grads_num), np.mean(np.abs(grads_num))))
                     sys.stdout.flush()
 
                 # update best perturbation (distance) and class probabilities
                 # if beta * L1 + L2 < current best and predicted label is different from the initial label:
                 # update best current step or global perturbations
                 for batch_idx, (dist, proba, adv_idx) in enumerate(zip(loss_l1_l2, pred_proba, adv)):
                     Y_class = np.argmax(Y[batch_idx])
```

### Comparing `alibi-0.9.2/alibi/explainers/cfrl_base.py` & `alibi-0.9.3/alibi/explainers/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/cfrl_tabular.py` & `alibi-0.9.3/alibi/explainers/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/counterfactual.py` & `alibi-0.9.3/alibi/explainers/counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/integrated_gradients.py` & `alibi-0.9.3/alibi/explainers/integrated_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -937,15 +937,15 @@
         self._is_list = isinstance(X, list)
         self._is_np = isinstance(X, np.ndarray)
         if forward_kwargs is None:
             forward_kwargs = {}
 
         if self._is_list:
             X = cast(List[np.ndarray], X)  # help mypy out
-            self.orig_dummy_input = [np.zeros((1,) + xx.shape[1:], dtype=xx.dtype) for xx in X]  # type: ignore
+            self.orig_dummy_input = [np.zeros((1,) + xx.shape[1:], dtype=xx.dtype) for xx in X]
             nb_samples = len(X[0])
             input_dtypes = [xx.dtype for xx in X]
             # Formatting baselines in case of models with multiple inputs
             if baselines is None:
                 baselines = [None for _ in range(len(X))]  # type: ignore
             else:
                 if not isinstance(baselines, list):
@@ -963,38 +963,38 @@
                 x, baseline = X[i], baselines[i]  # type: ignore
                 # format and check baselines
                 baseline = _format_baseline(x, baseline)
                 baselines[i] = baseline  # type: ignore
 
         elif self._is_np:
             X = cast(np.ndarray, X)  # help mypy out
-            self.orig_dummy_input = np.zeros((1,) + X.shape[1:], dtype=X.dtype)  # type: ignore
+            self.orig_dummy_input = np.zeros((1,) + X.shape[1:], dtype=X.dtype)
             nb_samples = len(X)
-            input_dtypes = [X.dtype]  # type: ignore
+            input_dtypes = [X.dtype]
             # Formatting baselines for models with a single input
             baselines = _format_baseline(X, baselines)  # type: ignore # TODO: validate/narrow baselines type
 
         else:
             raise ValueError("Input must be a np.ndarray or a list of np.ndarray")
 
         # defining integral method
         step_sizes_func, alphas_func = approximation_parameters(self.method)
         step_sizes, alphas = step_sizes_func(self.n_steps), alphas_func(self.n_steps)
-        target = _format_target(target, nb_samples)  # type: ignore[assignment]
+        target = _format_target(target, nb_samples)
 
         if self._is_list:
             X = cast(List[np.ndarray], X)  # help mypy out
             # Attributions calculation in case of multiple inputs
             if not self._has_inputs:
                 # Inferring model's inputs from data points for models with no explicit inputs
                 # (typically subclassed models)
                 inputs = [tf.keras.Input(shape=xx.shape[1:], dtype=xx.dtype) for xx in X]
                 self.model(inputs, **forward_kwargs)
 
-            _validate_output(self.model, target)  # type: ignore[arg-type]
+            _validate_output(self.model, target)
             _check_target(self.model.output_shape, target, nb_samples)
             if self.layer is None:
                 # No layer passed, attributions computed with respect to the inputs
                 attributions = self._compute_attributions_list_input(X,
                                                                      baselines,  # type: ignore[arg-type]
                                                                      target,
                                                                      step_sizes,
@@ -1172,15 +1172,15 @@
         if forward_kwargs is None:
             forward_kwargs = {}
         attrs_dtypes = [xx.dtype for xx in X]
 
         # define paths in features' space
         paths = []
         for i in range(len(X)):
-            x, baseline = X[i], baselines[i]  # type: ignore
+            x, baseline = X[i], baselines[i]
             # construct paths
             path = np.concatenate([baseline + alphas[i] * (x - baseline) for i in range(self.n_steps)], axis=0)
             paths.append(path)
 
         if forward_kwargs:
             paths_kwargs: Optional[dict] = {k: np.concatenate([forward_kwargs[k]
                                             for _ in range(self.n_steps)], axis=0)
@@ -1248,15 +1248,15 @@
         # calculate attributions from gradients batches
         attributions = []
         for j in range(len(attrs_dtypes)):
             sum_int = _calculate_sum_int(batches, self.model,
                                          target, target_paths,
                                          self.n_steps, nb_samples,
                                          step_sizes, j)
-            norm = X[j] - baselines[j]  # type: ignore
+            norm = X[j] - baselines[j]
             attribution = norm * sum_int
             attributions.append(attribution)
 
         return attributions
 
     def _compute_attributions_tensor_input(self,
                                            X: Union[np.ndarray, tf.Tensor],
```

### Comparing `alibi-0.9.2/alibi/explainers/partial_dependence.py` & `alibi-0.9.3/alibi/explainers/partial_dependence.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         super().__init__(meta=copy.deepcopy(DEFAULT_META_PD))
         self.predictor = predictor
         self.feature_names = feature_names
         self.categorical_names = categorical_names
         self.target_names = target_names
         self.verbose = verbose
 
-    def explain(self,  # type: ignore[override]
+    def explain(self,
                 X: np.ndarray,
                 features: Optional[List[Union[int, Tuple[int, int]]]] = None,
                 kind: Literal['average', 'individual', 'both'] = 'average',
                 percentiles: Tuple[float, float] = (0., 1.),
                 grid_resolution: int = 100,
                 grid_points: Optional[Dict[int, Union[List, np.ndarray]]] = None) -> Explanation:
         """
@@ -564,15 +564,15 @@
 
         super().__init__(predictor=predictor,
                          feature_names=feature_names,
                          categorical_names=categorical_names,
                          target_names=target_names,
                          verbose=verbose)
 
-    def explain(self,  # type: ignore[override]
+    def explain(self,
                 X: np.ndarray,
                 features: Optional[List[Union[int, Tuple[int, int]]]] = None,
                 kind: Literal['average', 'individual', 'both'] = 'average',
                 percentiles: Tuple[float, float] = (0., 1.),
                 grid_resolution: int = 100,
                 grid_points: Optional[Dict[int, Union[List, np.ndarray]]] = None) -> Explanation:
 
@@ -1116,20 +1116,20 @@
         See :py:meth:`alibi.explainers.partial_dependence.plot_pd`.
     """
     if n_ice == 'all':
         return ice_values
 
     _, N = ice_values.shape
     if isinstance(n_ice, numbers.Integral):
-        if n_ice >= N:  # type: ignore[operator]
+        if n_ice >= N:
             logger.warning('`n_ice` is greater than the number of instances in the reference dataset. '
                            'Automatically setting `n_ice` to the number of instances in the reference dataset.')
             return ice_values
 
-        if n_ice <= 0:  # type: ignore[operator]
+        if n_ice <= 0:
             raise ValueError('`n_ice` must be an integer grater than 0.')
 
         indices = np.random.choice(a=N, size=n_ice, replace=False)
         return ice_values[:, indices]
 
     if isinstance(n_ice, list):
         n_ice = np.unique(n_ice)  # type: ignore[assignment]
```

### Comparing `alibi-0.9.2/alibi/explainers/pd_variance.py` & `alibi-0.9.3/alibi/explainers/pd_variance.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             # `pdv` is a tensor of size `T x N1 x ... Nk`, where `T` is the number
             # of targets and `Ni` is the number of feature values along the axis `i`
             if f in self.pd_explainer.categorical_names:  # type: ignore[operator]
                 ft_var = PartialDependenceVariance._compute_pd_variance_cat(pdv)
             else:
                 ft_var = PartialDependenceVariance._compute_pd_variance_num(pdv)
             # add extra dimension for later concatenation along the axis 0
-            feature_variance.append(ft_var[None, ...])  # type: ignore[index]
+            feature_variance.append(ft_var[None, ...])
 
         # stack the feature importance such that the array has the shape `F x T x N1 ... N(k-1)`
         return np.concatenate(feature_variance, axis=0)
 
     @staticmethod
     def _compute_pd_variance_num(pd_values: np.ndarray) -> np.ndarray:
         """
@@ -457,15 +457,15 @@
     n_targets = len(target_names)
 
     if isinstance(ax, plt.Axes) and n_targets != 1:
         ax.set_axis_off()  # treat passed axis as a canvas for subplots
         fig = ax.figure
         n_cols = min(n_cols, n_targets)
         n_rows = math.ceil(n_targets / n_cols)
-        axes = np.empty((n_rows, n_cols), dtype=object)   # type: ignore[attr-defined]
+        axes = np.empty((n_rows, n_cols), dtype=object)
         axes_ravel = axes.ravel()
         gs = GridSpec(n_rows, n_cols)
 
         for i, spec in enumerate(list(gs)[:n_targets]):
             axes_ravel[i] = fig.add_subplot(spec)
     else:
         if isinstance(ax, plt.Axes):
```

### Comparing `alibi-0.9.2/alibi/explainers/permutation_importance.py` & `alibi-0.9.3/alibi/explainers/permutation_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
         if metric_fns is None:
             return {}
 
         if callable(metric_fns):
             return {metric_type: metric_fns}
 
         if isinstance(metric_fns, str):
-            metric_fns = [metric_fns]  # type: ignore[assignment]
+            metric_fns = [metric_fns]
 
         if isinstance(metric_fns, list):
             dict_metric_fns = {}
             METRIC_FNS = LOSS_FNS if metric_type == 'loss' else SCORE_FNS
 
             for metric_fn in metric_fns:
                 if not isinstance(metric_fn, str):
```

### Comparing `alibi-0.9.2/alibi/explainers/shap_wrappers.py` & `alibi-0.9.3/alibi/explainers/shap_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
             if self.use_groups:
                 background_data.groups = groups
                 background_data.group_names = group_names
                 background_data.group_size = len(groups)
 
         return background_data
 
-    @_get_data.register(np.ndarray)  # type: ignore
+    @_get_data.register(np.ndarray)
     def _(self, background_data, *args, **kwargs) -> Union[np.ndarray, shap_utils.Data]:
         """
         Initialises background data if the user passes an `np.ndarray` object as input.
         If the user specifies feature grouping then a `shap_utils.DenseData` object
         is returned. Weights are handled separately to avoid triggering assertion
         correct inside `shap` library. Otherwise, the original data is returned and
         is handled by the `shap` library internally.
@@ -594,15 +594,15 @@
         group_names, groups, weights = args
         new_args = (group_names, groups, weights) if weights is not None else (group_names, groups)
         if self.use_groups:
             return shap_utils.DenseData(background_data, *new_args)
         else:
             return background_data
 
-    @_get_data.register(sparse.spmatrix)  # type: ignore
+    @_get_data.register(sparse.spmatrix)
     def _(self, background_data, *args, **kwargs) -> Union[shap_utils.Data, sparse.spmatrix]:
         """
         Initialises background data if the user passes a sparse matrix as input. If the
         user specifies feature grouping, then the sparse array is converted to a dense
         array. Otherwise, the original array is returned and handled internally by `shap`
         library.
         """
@@ -619,15 +619,15 @@
             return shap_utils.DenseData(
                 background_data,
                 *new_args,
             )
 
         return background_data
 
-    @_get_data.register(pd.core.frame.DataFrame)  # type: ignore
+    @_get_data.register(pd.core.frame.DataFrame)
     def _(self, background_data, *args, **kwargs) -> Union[shap_utils.Data, pd.core.frame.DataFrame]:
         """
         Initialises background data if the user passes a `pandas.core.frame.DataFrame` as input.
         If the user has specified groups and given a data frame, it initialises a `shap_utils.DenseData`
         object explicitly as this is not handled by `shap` library internally. Otherwise, data initialisation,
         is left to the `shap` library.
         """
@@ -650,15 +650,15 @@
                     background_data.values,
                     list(background_data.columns),
                     *new_args,
                 )
         else:
             return background_data
 
-    @_get_data.register(pd.core.frame.Series)  # type: ignore
+    @_get_data.register(pd.core.frame.Series)
     def _(self, background_data, *args, **kwargs) -> Union[shap_utils.Data, pd.core.frame.Series]:
         """
         Initialises background data if the user passes a `pandas.Series` object as input.
         Original object is returned as this is initialised internally by `shap` is there
         is no group structure specified. Otherwise, a `shap_utils.DenseData` object
         is initialised.
         """
@@ -926,15 +926,15 @@
             shap_values = summarised_shap
 
         raw_predictions = self._explainer.linkfv(self.predictor(X))
 
         if self.task != 'regression':
             argmax_pred = np.argmax(np.atleast_2d(raw_predictions), axis=1)
         else:
-            argmax_pred = []  # type: ignore
+            argmax_pred = []
         importances = rank_by_importance(shap_values, feature_names=self.feature_names)
 
         if isinstance(X, sparse.spmatrix):
             X = X.toarray()
         else:
             X = np.array(X)
 
@@ -1526,21 +1526,21 @@
         # check if interactions were computed
         if len(shap_output[0].shape) == 3:
             shap_interaction_values = shap_output
             # shap values are the sum over all shap interaction values for each instance
             shap_values = [interactions.sum(axis=2) for interactions in shap_output]
         else:
             shap_interaction_values = [np.array([])]
-            shap_values = shap_output  # type: ignore
+            shap_values = shap_output
         if summarise_result:
             self._check_result_summarisation(summarise_result, cat_vars_start_idx, cat_vars_enc_dim)
         if self.summarise_result:
             summarised_shap = []
             for shap_array in shap_values:
-                summarised_shap.append(sum_categories(shap_array, cat_vars_start_idx, cat_vars_enc_dim))  # type: ignore
+                summarised_shap.append(sum_categories(shap_array, cat_vars_start_idx, cat_vars_enc_dim))
             shap_values = summarised_shap
             if shap_interaction_values[0].size != 0:
                 summarised_shap_interactions = []
                 for shap_array in shap_interaction_values:
                     summarised_shap_interactions.append(
                         sum_categories(shap_array, cat_vars_start_idx, cat_vars_enc_dim)
                     )
@@ -1568,15 +1568,15 @@
                         probas = expit(raw_predictions)
                     else:
                         probas = raw_predictions
                     argmax_pred = (probas > 0.5).astype(int)
                 else:
                     argmax_pred = np.argmax(np.atleast_2d(raw_predictions), axis=1)
 
-        importances = rank_by_importance(shap_values, feature_names=self.feature_names)  # type: ignore
+        importances = rank_by_importance(shap_values, feature_names=self.feature_names)
 
         if self._explainer.model.model_type == 'catboost':
             import catboost  # noqa: F811
             if isinstance(X, catboost.Pool):
                 X = X.get_features()
         # output explanation dictionary
         data = copy.deepcopy(DEFAULT_DATA_TREE_SHAP)
```

### Comparing `alibi-0.9.2/alibi/explainers/similarity/backends/__init__.py` & `alibi-0.9.3/alibi/explainers/similarity/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/base.py` & `alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/base.py` & `alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/similarity/base.py` & `alibi-0.9.3/alibi/explainers/similarity/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/similarity/grad.py` & `alibi-0.9.3/alibi/explainers/similarity/grad.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/similarity/metrics.py` & `alibi-0.9.3/alibi/explainers/similarity/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/conftest.py` & `alibi-0.9.3/alibi/explainers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_ale.py` & `alibi-0.9.3/alibi/explainers/tests/test_ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_anchor_base.py` & `alibi-0.9.3/alibi/explainers/tests/test_anchor_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_anchor_image.py` & `alibi-0.9.3/alibi/explainers/tests/test_anchor_image.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_anchor_tabular.py` & `alibi-0.9.3/alibi/explainers/tests/test_anchor_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_anchor_text.py` & `alibi-0.9.3/alibi/explainers/tests/test_anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_cem.py` & `alibi-0.9.3/alibi/explainers/tests/test_cem.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_cfproto.py` & `alibi-0.9.3/alibi/explainers/tests/test_cfproto.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_cfrl.py` & `alibi-0.9.3/alibi/explainers/tests/test_cfrl.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_counterfactual.py` & `alibi-0.9.3/alibi/explainers/tests/test_counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_integrated_gradients.py` & `alibi-0.9.3/alibi/explainers/tests/test_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_partial_dependence.py` & `alibi-0.9.3/alibi/explainers/tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_pd_variance.py` & `alibi-0.9.3/alibi/explainers/tests/test_pd_variance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_permutation_importance.py` & `alibi-0.9.3/alibi/explainers/tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_shap_wrappers.py` & `alibi-0.9.3/alibi/explainers/tests/test_shap_wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/conftest.py` & `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_backends.py` & `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_backends.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py` & `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py` & `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/explainers/tests/utils.py` & `alibi-0.9.3/alibi/explainers/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/actor_critic.py` & `alibi-0.9.3/alibi/models/pytorch/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/autoencoder.py` & `alibi-0.9.3/alibi/models/pytorch/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/cfrl_models.py` & `alibi-0.9.3/alibi/models/pytorch/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/metrics.py` & `alibi-0.9.3/alibi/models/pytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/model.py` & `alibi-0.9.3/alibi/models/pytorch/model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/tests/test_actor_critic.py` & `alibi-0.9.3/alibi/models/pytorch/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/tests/test_autoencoder.py` & `alibi-0.9.3/alibi/models/pytorch/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/tests/test_cfrl_models.py` & `alibi-0.9.3/alibi/models/pytorch/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/tests/test_metrics.py` & `alibi-0.9.3/alibi/models/pytorch/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/pytorch/tests/test_model.py` & `alibi-0.9.3/alibi/models/pytorch/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/tensorflow/actor_critic.py` & `alibi-0.9.3/alibi/models/tensorflow/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/tensorflow/autoencoder.py` & `alibi-0.9.3/alibi/models/tensorflow/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/tensorflow/cfrl_models.py` & `alibi-0.9.3/alibi/models/tensorflow/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/tensorflow/tests/test_actor_critic.py` & `alibi-0.9.3/alibi/models/tensorflow/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/tensorflow/tests/test_autoencoder.py` & `alibi-0.9.3/alibi/models/tensorflow/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/models/tensorflow/tests/test_cfrl_models.py` & `alibi-0.9.3/alibi/models/tensorflow/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/prototypes/protoselect.py` & `alibi-0.9.3/alibi/prototypes/protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/prototypes/tests/test_protoselect.py` & `alibi-0.9.3/alibi/prototypes/tests/test_protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/prototypes/tests/test_utils.py` & `alibi-0.9.3/alibi/prototypes/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/saving.py` & `alibi-0.9.3/alibi/saving.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
     # load the rest of the explainer
     return _helper_load_CounterfactualRL(path, predictor, explainer)
 
 
 def _save_SimilarityExplainer(explainer: 'GradientSimilarity', path: Union[str, os.PathLike]) -> None:
     predictor = explainer.predictor
-    explainer.predictor = None  # type: ignore[assignment]
+    explainer.predictor = None
 
     with open(Path(path, 'explainer.dill'), 'wb') as f:
         dill.dump(explainer, f, recurse=True)
 
     explainer.predictor = predictor
```

### Comparing `alibi-0.9.2/alibi/tests/conftest.py` & `alibi-0.9.3/alibi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/tests/test_dep_management.py` & `alibi-0.9.3/alibi/tests/test_dep_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     opt_dep
         The name of the optional dependency that is being tested.
     """
     lib_obj = [obj for obj in dir(module) if not obj.startswith('_')]
     for item_name in lib_obj:
         item = getattr(module, item_name)
         if not isinstance(item, ModuleType):
-            pass_contexts = dependencies[item_name]  # type: ignore
+            pass_contexts = dependencies[item_name]
             try:
-                item.test  # type: ignore # noqa
+                item.test  # noqa
             except AttributeError:
                 assert opt_dep in pass_contexts or 'default' in pass_contexts or opt_dep == 'all', \
                     (f'{item_name} was imported instead of an instance of MissingDependency. '
                      f'Are your sure {item} is dependent on {opt_dep}?')
             except ImportError:
                 assert opt_dep not in pass_contexts and 'default' not in pass_contexts and opt_dep != 'all', \
                     (f'{item_name} has been imported as an instance of MissingDependency. '
```

### Comparing `alibi-0.9.2/alibi/tests/test_saving.py` & `alibi-0.9.3/alibi/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/tests/test_utils.py` & `alibi-0.9.3/alibi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/tests/utils.py` & `alibi-0.9.3/alibi/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/__init__.py` & `alibi-0.9.3/alibi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/approximation_methods.py` & `alibi-0.9.3/alibi/utils/approximation_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
      multipliers/coefficients for the inputs of integrand in the range of [0, 1].
 
     """
 
     def step_sizes(n: int) -> List[float]:
         assert n > 0, "The number of steps has to be larger than zero"
         # Scaling from 2 to 1
-        return list(0.5 * np.polynomial.legendre.leggauss(n)[1])  # type: ignore
+        return list(0.5 * np.polynomial.legendre.leggauss(n)[1])
 
     def alphas(n: int) -> List[float]:
         assert n > 0, "The number of steps has to be larger than zero"
         # Scaling from [-1, 1] to [0, 1]
-        return list(0.5 * (1 + np.polynomial.legendre.leggauss(n)[0]))  # type: ignore
+        return list(0.5 * (1 + np.polynomial.legendre.leggauss(n)[0]))
 
     return step_sizes, alphas
```

### Comparing `alibi-0.9.2/alibi/utils/data.py` & `alibi-0.9.3/alibi/utils/data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/discretizer.py` & `alibi-0.9.3/alibi/utils/discretizer.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/distance.py` & `alibi-0.9.3/alibi/utils/distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/distributed.py` & `alibi-0.9.3/alibi/utils/distributed.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
         if algorithm == 'default':
             logger.warning(
                 "No algorithm specified in distributed option, default target function will be selected."
             )
         self.target_fcn = default_target_fcn
         # check global scope for any specific target function
         if concatenate_results:
-            self.concatenate = concatenate_minibatches  # type: ignore[assignment]
+            self.concatenate = concatenate_minibatches
         if f"{algorithm}_target_fcn" in globals():
             self.target_fcn = globals()[f"{algorithm}_target_fcn"]
 
         if not ray.is_initialized():
             logger.info(f"Initialising ray on {self.n_processes} processes!")
             ray.init(num_cpus=self.n_processes)
```

### Comparing `alibi-0.9.2/alibi/utils/distributions.py` & `alibi-0.9.3/alibi/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/download.py` & `alibi-0.9.3/alibi/utils/download.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/gradients.py` & `alibi-0.9.3/alibi/utils/gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/kernel.py` & `alibi-0.9.3/alibi/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/lang_model.py` & `alibi-0.9.3/alibi/utils/lang_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,15 @@
         """
         self.model_path = model_path
 
         if preloading:
             # set model (for performance reasons the `call` method is wrapped in tf.function)
             self.model = TFAutoModelForMaskedLM.from_pretrained(model_path)
 
-            # To understand the type: ignore see https://github.com/python/mypy/issues/2427
-            self.caller = tf.function(self.model.call, experimental_relax_shapes=True)  # type: ignore[assignment]
+            self.caller = tf.function(self.model.call, experimental_relax_shapes=True)
 
             # set tokenizer
             self.tokenizer = AutoTokenizer.from_pretrained(model_path)
 
     def from_disk(self, path: Union[str, Path]):
         """
         Loads a model from disk.
@@ -73,16 +72,15 @@
         ----------
         path
             Path to the checkpoint.
         """
         # set model (for performance reasons the `call` method is wrapped in tf.function)
         self.model = TFAutoModelForMaskedLM.from_pretrained(path, local_files_only=True)
 
-        # To understand the type: ignore see https://github.com/python/mypy/issues/2427
-        self.caller = tf.function(self.model.call, experimental_relax_shapes=True)  # type: ignore[assignment]
+        self.caller = tf.function(self.model.call, experimental_relax_shapes=True)
 
         # set tokenizer
         self.tokenizer = AutoTokenizer.from_pretrained(path, local_files_only=True)
 
     def to_disk(self, path: Union[str, Path]):
         """
         Saves a model to disk.
```

### Comparing `alibi-0.9.2/alibi/utils/mapping.py` & `alibi-0.9.3/alibi/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/missing_optional_dependency.py` & `alibi-0.9.3/alibi/utils/missing_optional_dependency.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/tests/test_data.py` & `alibi-0.9.3/alibi/utils/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/tests/test_distance.py` & `alibi-0.9.3/alibi/utils/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/tests/test_distributed.py` & `alibi-0.9.3/alibi/utils/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/tests/test_gradients.py` & `alibi-0.9.3/alibi/utils/tests/test_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/tests/test_import_optional.py` & `alibi-0.9.3/alibi/utils/tests/test_import_optional.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/tests/test_mapping.py` & `alibi-0.9.3/alibi/utils/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/tf.py` & `alibi-0.9.3/alibi/utils/tf.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi/utils/visualization.py` & `alibi-0.9.3/alibi/utils/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,26 +60,26 @@
 ):
     attr_combined = np.sum(attr, axis=2)
     # Choose appropriate signed values and rescale, removing given outlier percentage.
     if VisualizeSign[sign] == VisualizeSign.all:
         threshold = _cumulative_sum_threshold(np.abs(attr_combined), 100 - outlier_perc)
     elif VisualizeSign[sign] == VisualizeSign.positive:
         attr_combined = (attr_combined > 0) * attr_combined
-        threshold = _cumulative_sum_threshold(attr_combined, 100 - outlier_perc)  # type: ignore
+        threshold = _cumulative_sum_threshold(attr_combined, 100 - outlier_perc)
     elif VisualizeSign[sign] == VisualizeSign.negative:
         attr_combined = (attr_combined < 0) * attr_combined
         threshold = -1 * _cumulative_sum_threshold(
             np.abs(attr_combined), 100 - outlier_perc
         )
     elif VisualizeSign[sign] == VisualizeSign.absolute_value:
         attr_combined = np.abs(attr_combined)
-        threshold = _cumulative_sum_threshold(attr_combined, 100 - outlier_perc)  # type: ignore
+        threshold = _cumulative_sum_threshold(attr_combined, 100 - outlier_perc)
     else:
         raise AssertionError("Visualize Sign type is not valid.")
-    return _normalize_scale(attr_combined, threshold)  # type: ignore
+    return _normalize_scale(attr_combined, threshold)
 
 
 def visualize_image_attr(
         attr: ndarray,
         original_image: Union[None, ndarray] = None,
         method: str = "heat_map",
         sign: str = "absolute_value",
```

### Comparing `alibi-0.9.2/alibi/utils/wrappers.py` & `alibi-0.9.3/alibi/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi.egg-info/PKG-INFO` & `alibi-0.9.3/alibi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.2
+Version: 0.9.3
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 Provides-Extra: shap
 Provides-Extra: tensorflow
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: alibi Version: 0.9.2 Summary: Algorithms for
+Metadata-Version: 2.1 Name: alibi Version: 0.9.3 Summary: Algorithms for
 monitoring and explaining machine learning models Home-page: https://
 github.com/SeldonIO/alibi Author: Seldon Technologies Ltd. Author-email:
 hello@seldon.io License: Apache 2.0 Classifier: Intended Audience :: Science/
 Research Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Scientific/Engineering Requires-Python: >=3.7 Description-Content-
-Type: text/markdown Provides-Extra: ray Provides-Extra: shap Provides-Extra:
-tensorflow Provides-Extra: torch Provides-Extra: all License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+ray Provides-Extra: shap Provides-Extra: tensorflow Provides-Extra: torch
+Provides-Extra: all License-File: LICENSE
                                  [Alibi Logo]
  [![Build Status](https://github.com/SeldonIO/alibi-detect/workflows/CI/
 badge.svg?branch=master)][#build-status] [![Documentation Status](https://
 readthedocs.org/projects/alibi/badge/?version=latest)][#docs-package] [!
 [codecov](https://codecov.io/gh/SeldonIO/alibi/branch/master/graph/badge.svg)]
 (https://codecov.io/gh/SeldonIO/alibi) [![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/alibi?logo=pypi&style=flat&color=blue)][#pypi-
```

### Comparing `alibi-0.9.2/alibi.egg-info/SOURCES.txt` & `alibi-0.9.3/alibi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibi-0.9.2/alibi.egg-info/requires.txt` & `alibi-0.9.3/alibi.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 numpy<2.0.0,>=1.16.2
 pandas<3.0.0,>=1.0.0
 scikit-learn<2.0.0,>=1.0.0
 spacy[lookups]<4.0.0,>=2.0.0
 blis<0.8.0
-scikit-image<0.21,>=0.17.2
+scikit-image<0.22,>=0.17.2
 requests<3.0.0,>=2.21.0
 Pillow<10.0,>=5.4.1
 attrs<24.0.0,>=19.2.0
 scipy<2.0.0,>=1.1.0
 matplotlib<4.0.0,>=3.0.0
 typing-extensions>=3.7.4.3
 dill<0.4.0,>=0.3.0
 transformers<5.0.0,>=4.7.0
 tqdm<5.0.0,>=4.28.1
 
 [all]
 ray<3.0.0,>=0.8.7
 shap<0.42.0,>=0.40.0
-numba!=0.54.0,<0.57.0,>=0.50.0
+numba!=0.54.0,<0.58.0,>=0.50.0
 tensorflow!=2.6.0,!=2.6.1,<2.13.0,>=2.0.0
-torch<2.0.0,>=1.9.0
+torch<3.0.0,>=1.9.0
 
 [ray]
 ray<3.0.0,>=0.8.7
 
 [shap]
 shap<0.42.0,>=0.40.0
-numba!=0.54.0,<0.57.0,>=0.50.0
+numba!=0.54.0,<0.58.0,>=0.50.0
 
 [tensorflow]
 tensorflow!=2.6.0,!=2.6.1,<2.13.0,>=2.0.0
 
 [torch]
 torch<2.0.0,>=1.9.0
```

### Comparing `alibi-0.9.2/setup.cfg` & `alibi-0.9.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 	doc/source/conf.py
 	.eggs/
 
 [mypy]
 ignore_missing_imports = True
 no_implicit_optional = True
 show_error_codes = True
+warn_unused_ignores = True
+warn_redundant_casts = True
 
 [mypy-conf]
 ignore_errors = True
 
 [tox:tox]
 envlist = 
 	default
```

### Comparing `alibi-0.9.2/setup.py` & `alibi-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 exec(open('alibi/version.py').read())
 
 extras_require = {
     'ray': ['ray>=0.8.7, <3.0.0'],
     # shap is separated due to build issues, see https://github.com/slundberg/shap/pull/1802
     'shap': [
         'shap>=0.40.0, <0.42.0',  # versioning: https://github.com/SeldonIO/alibi/issues/333
-        'numba>=0.50.0, !=0.54.0, <0.57.0',  # Avoid 0.54 due to: https://github.com/SeldonIO/alibi/issues/466
+        'numba>=0.50.0, !=0.54.0, <0.58.0',  # Avoid 0.54 due to: https://github.com/SeldonIO/alibi/issues/466
     ],
+
     'tensorflow': ['tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.13.0'],
     'torch': ['torch>=1.9.0, <2.0.0'],
     'all': [
         'ray>=0.8.7, <3.0.0',
         'shap>=0.40.0, <0.42.0',
-        'numba>=0.50.0, !=0.54.0, <0.57.0',
+        'numba>=0.50.0, !=0.54.0, <0.58.0',
         'tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.13.0',
-        'torch>=1.9.0, <2.0.0'
+        'torch>=1.9.0, <3.0.0'
     ]
 }
 
 if __name__ == '__main__':
     setup(name='alibi',
           author='Seldon Technologies Ltd.',
           author_email='hello@seldon.io',
@@ -43,15 +44,15 @@
           # lower bounds based on Debian Stable versions where available
           install_requires=[
               'numpy>=1.16.2, <2.0.0',
               'pandas>=1.0.0, <3.0.0',
               'scikit-learn>=1.0.0, <2.0.0',
               'spacy[lookups]>=2.0.0, <4.0.0',
               'blis<0.8.0',  # Windows memory issues https://github.com/explosion/thinc/issues/771
-              'scikit-image>=0.17.2, <0.21',  # introduced `start_label` argument for `slic`
+              'scikit-image>=0.17.2, <0.22',  # introduced `start_label` argument for `slic`
               'requests>=2.21.0, <3.0.0',
               'Pillow>=5.4.1, <10.0',
               'attrs>=19.2.0, <24.0.0',
               'scipy>=1.1.0, <2.0.0',
               'matplotlib>=3.0.0, <4.0.0',
               'typing-extensions>=3.7.4.3',
               'dill>=0.3.0, <0.4.0',
@@ -65,10 +66,11 @@
               "Intended Audience :: Science/Research",
               "Operating System :: OS Independent",
               "Programming Language :: Python :: 3",
               "Programming Language :: Python :: 3.7",
               "Programming Language :: Python :: 3.8",
               "Programming Language :: Python :: 3.9",
               "Programming Language :: Python :: 3.10",
+              "Programming Language :: Python :: 3.11",
               "License :: OSI Approved :: Apache Software License",
               "Topic :: Scientific/Engineering",
           ])
```

