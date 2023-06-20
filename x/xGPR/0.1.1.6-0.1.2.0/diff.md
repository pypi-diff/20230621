# Comparing `tmp/xGPR-0.1.1.6.tar.gz` & `tmp/xGPR-0.1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xGPR-0.1.1.6.tar", last modified: Thu Jun  8 22:04:04 2023, max compression
+gzip compressed data, was "xGPR-0.1.2.0.tar", last modified: Tue Jun 20 23:40:04 2023, max compression
```

## Comparing `xGPR-0.1.1.6.tar` & `xGPR-0.1.2.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/LICENSE
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/README.md
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/setup.cfg
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.1.6/setup.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.051120 xGPR-0.1.1.6/xGPR/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-08 22:03:12.000000 xGPR-0.1.1.6/xGPR/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.063120 xGPR-0.1.1.6/xGPR/cg_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/cg_linear_operators.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/cg_tools.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.063120 xGPR-0.1.1.6/xGPR/constants/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/constants/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/constants/constants.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.075120 xGPR-0.1.1.6/xGPR/data_handling/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/data_handling_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13221 2023-06-07 22:51:35.000000 xGPR-0.1.1.6/xGPR/data_handling/dataset_builder.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/minibatch_data_handler.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/offline_data_handling.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6843 2023-06-07 22:48:32.000000 xGPR-0.1.1.6/xGPR/data_handling/online_data_handling.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.079120 xGPR-0.1.1.6/xGPR/fitting_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/ams_grad_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.079120 xGPR-0.1.1.6/xGPR/kernels/
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.103120 xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13106 2023-05-25 01:08:51.000000 xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-05-25 15:24:30.000000 xGPR-0.1.1.6/xGPR/kernels/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.119120 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3718 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3151 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/matern.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6970 2023-05-25 01:05:26.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/polynomial.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1796 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11082 2023-03-30 18:48:37.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/rbf_linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7948 2023-05-25 01:09:48.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.163120 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8337 2023-05-25 01:05:52.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10322 2023-05-25 01:06:23.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/fht_conv1d.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7551 2023-05-25 15:40:52.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_arccos.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7065 2023-05-25 01:07:22.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_polysum.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-05-25 13:27:31.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14864 2023-03-30 15:55:38.000000 xGPR-0.1.1.6/xGPR/kernels/kernel_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.1.6/xGPR/kernels/srht_compressor.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.207120 xGPR-0.1.1.6/xGPR/optimizers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/bayes_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/crude_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/lb_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/optimizers/map_loss_bayes_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/pure_bayes_optimizer.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.239120 xGPR-0.1.1.6/xGPR/preconditioners/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.1.6/xGPR/preconditioners/inter_device_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_constructors.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/tuning_preconditioners.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.239120 xGPR-0.1.1.6/xGPR/random_feature_generation/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.243120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.243120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.247120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20803 2023-06-02 19:55:34.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12509 2023-05-25 00:59:46.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14218 2023-06-06 03:20:50.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.247120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.247120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.251120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.251120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.255120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23069 2023-06-02 19:55:30.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14619 2023-06-06 02:32:10.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
--rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.255120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27652 2023-04-05 19:56:01.000000 xGPR-0.1.1.6/xGPR/regression_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.259120 xGPR-0.1.1.6/xGPR/scoring_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/cho_solvers.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5699 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/exact_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/nmll_gradient_tools.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/probe_generators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.259120 xGPR-0.1.1.6/xGPR/static_layers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/static_layers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9825 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/static_layers/fast_conv.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/xGPR/tuning_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/hparam_scoring.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/xGPR/visualization_tools/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.1.6/xGPR/visualization_tools/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/visualization_tools/kernel_xpca.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-06 04:07:57.000000 xGPR-0.1.1.6/xGPR/xGP_Regression.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.051120 xGPR-0.1.1.6/xGPR.egg-info/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6956 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/SOURCES.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/dependency_links.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/requires.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/top_level.txt
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.338239 xGPR-0.1.2.0/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/LICENSE
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-20 23:40:04.338239 xGPR-0.1.2.0/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/README.md
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-20 23:40:04.338239 xGPR-0.1.2.0/setup.cfg
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.2.0/setup.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:03.946238 xGPR-0.1.2.0/xGPR/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-20 23:39:20.000000 xGPR-0.1.2.0/xGPR/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:03.958238 xGPR-0.1.2.0/xGPR/cg_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/cg_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/cg_toolkit/cg_linear_operators.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/cg_toolkit/cg_tools.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/cg_toolkit/cuda_cg_linear_operators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:03.978238 xGPR-0.1.2.0/xGPR/constants/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/constants/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.2.0/xGPR/constants/constants.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.014238 xGPR-0.1.2.0/xGPR/data_handling/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/data_handling/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/data_handling/data_handling_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13221 2023-06-07 22:51:35.000000 xGPR-0.1.2.0/xGPR/data_handling/dataset_builder.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/data_handling/minibatch_data_handler.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/data_handling/offline_data_handling.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6843 2023-06-07 22:48:32.000000 xGPR-0.1.2.0/xGPR/data_handling/online_data_handling.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.078238 xGPR-0.1.2.0/xGPR/fitting_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/fitting_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.2.0/xGPR/fitting_toolkit/ams_grad_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.2.0/xGPR/fitting_toolkit/cg_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.2.0/xGPR/fitting_toolkit/exact_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.2.0/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.2.0/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.098238 xGPR-0.1.2.0/xGPR/kernels/
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.114238 xGPR-0.1.2.0/xGPR/kernels/ARD_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.2.0/xGPR/kernels/ARD_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13201 2023-06-19 15:11:57.000000 xGPR-0.1.2.0/xGPR/kernels/ARD_kernels/mini_ard.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-06-16 16:46:38.000000 xGPR-0.1.2.0/xGPR/kernels/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.170238 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3507 2023-06-19 13:59:18.000000 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3206 2023-06-19 14:13:44.000000 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/matern.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7009 2023-06-19 14:10:03.000000 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/polynomial.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1951 2023-06-19 14:14:22.000000 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11293 2023-06-19 15:12:56.000000 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/rbf_linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8197 2023-06-19 15:13:21.000000 xGPR-0.1.2.0/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.222238 xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8097 2023-06-17 22:46:55.000000 xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10417 2023-06-19 15:13:46.000000 xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/fht_conv1d.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-06-19 15:14:09.000000 xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/graph_arccos.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7287 2023-06-19 15:14:30.000000 xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/graph_polysum.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7806 2023-06-19 15:16:23.000000 xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/graph_rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15507 2023-06-19 13:53:19.000000 xGPR-0.1.2.0/xGPR/kernels/kernel_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.2.0/xGPR/kernels/srht_compressor.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.278238 xGPR-0.1.2.0/xGPR/optimizers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/optimizers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/optimizers/bayes_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/optimizers/crude_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/optimizers/lb_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/optimizers/map_loss_bayes_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/optimizers/pure_bayes_optimizer.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.302239 xGPR-0.1.2.0/xGPR/preconditioners/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/preconditioners/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.2.0/xGPR/preconditioners/inter_device_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/preconditioners/rand_nys_constructors.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/preconditioners/rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/preconditioners/tuning_preconditioners.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.302239 xGPR-0.1.2.0/xGPR/random_feature_generation/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.306239 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.306239 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.310239 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21805 2023-06-20 23:27:23.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12508 2023-06-19 14:41:23.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15398 2023-06-20 23:28:13.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.310239 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.310239 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.314239 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.314239 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.318239 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23784 2023-06-20 23:29:00.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15776 2023-06-20 23:30:00.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
+-rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.318239 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27786 2023-06-19 23:39:23.000000 xGPR-0.1.2.0/xGPR/regression_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.322239 xGPR-0.1.2.0/xGPR/scoring_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/scoring_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/scoring_toolkit/approximate_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/scoring_toolkit/cho_solvers.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5907 2023-06-20 17:26:24.000000 xGPR-0.1.2.0/xGPR/scoring_toolkit/exact_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/scoring_toolkit/nmll_gradient_tools.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.2.0/xGPR/scoring_toolkit/probe_generators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.322239 xGPR-0.1.2.0/xGPR/static_layers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/static_layers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9524 2023-06-17 22:48:21.000000 xGPR-0.1.2.0/xGPR/static_layers/fast_conv.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.338239 xGPR-0.1.2.0/xGPR/tuning_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/tuning_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/tuning_toolkit/direct_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/tuning_toolkit/hparam_scoring.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:04.338239 xGPR-0.1.2.0/xGPR/visualization_tools/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.2.0/xGPR/visualization_tools/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.2.0/xGPR/visualization_tools/kernel_xpca.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-16 17:55:48.000000 xGPR-0.1.2.0/xGPR/xGP_Regression.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-20 23:40:03.958238 xGPR-0.1.2.0/xGPR.egg-info/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-20 23:40:03.000000 xGPR-0.1.2.0/xGPR.egg-info/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6956 2023-06-20 23:40:03.000000 xGPR-0.1.2.0/xGPR.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-20 23:40:03.000000 xGPR-0.1.2.0/xGPR.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-20 23:40:03.000000 xGPR-0.1.2.0/xGPR.egg-info/requires.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-20 23:40:03.000000 xGPR-0.1.2.0/xGPR.egg-info/top_level.txt
```

### Comparing `xGPR-0.1.1.6/LICENSE` & `xGPR-0.1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/PKG-INFO` & `xGPR-0.1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.1.6
+Version: 0.1.2.0
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.1.6/README.md` & `xGPR-0.1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/setup.py` & `xGPR-0.1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/cg_toolkit/cg_linear_operators.py` & `xGPR-0.1.2.0/xGPR/cg_toolkit/cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/cg_toolkit/cg_tools.pyx` & `xGPR-0.1.2.0/xGPR/cg_toolkit/cg_tools.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py` & `xGPR-0.1.2.0/xGPR/cg_toolkit/cuda_cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/constants/constants.py` & `xGPR-0.1.2.0/xGPR/constants/constants.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/data_handling/data_handling_baseclass.py` & `xGPR-0.1.2.0/xGPR/data_handling/data_handling_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/data_handling/dataset_builder.py` & `xGPR-0.1.2.0/xGPR/data_handling/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/data_handling/minibatch_data_handler.py` & `xGPR-0.1.2.0/xGPR/data_handling/minibatch_data_handler.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/data_handling/offline_data_handling.py` & `xGPR-0.1.2.0/xGPR/data_handling/offline_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/data_handling/online_data_handling.py` & `xGPR-0.1.2.0/xGPR/data_handling/online_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/fitting_toolkit/ams_grad_toolkit.py` & `xGPR-0.1.2.0/xGPR/fitting_toolkit/ams_grad_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py` & `xGPR-0.1.2.0/xGPR/fitting_toolkit/cg_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py` & `xGPR-0.1.2.0/xGPR/fitting_toolkit/exact_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py` & `xGPR-0.1.2.0/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py` & `xGPR-0.1.2.0/xGPR/fitting_toolkit/sgd_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/mini_ard.py` & `xGPR-0.1.2.0/xGPR/kernels/ARD_kernels/mini_ard.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
                 of split points across input arrays.
 
         Raises:
             ValueError: A ValueError is raised if the needed kernel_spec_parms
                 are not supplied, or if the split points supplied are invalid.
         """
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = True,
-                double_precision = double_precision)
+                double_precision = double_precision,
+                kernel_spec_parms = kernel_spec_parms)
         if len(self.xdim) != 2:
             raise ValueError("The dimensionality of the input is inappropriate for "
                         "the kernel you have selected.")
         if "split_points" not in kernel_spec_parms:
             raise ValueError("For the MiniARD kernel, 'kernel_specific_params' "
                     "must contain a list called 'split_points'.")
         if not isinstance(kernel_spec_parms["split_points"], list):
@@ -189,15 +190,15 @@
         """
         xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
                             dtype = self.dtype)
         xtrans[:,:,:self.xdim[1]] = (input_x * self.full_ard_weights[None,:])[:,None,:]
 
         output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
         self.feature_gen(xtrans, output_x, self.radem_diag, self.chi_arr,
-                self.hyperparams[1], self.num_threads)
+                self.hyperparams[1], self.num_threads, self.fit_intercept)
         return output_x
 
 
     def precompute_weights(self):
         """The kernel does not automatically generate precomputed weights,
         because for generating features during fitting or prediction,
         these are not necessary and would increase model size unnecessarily.
@@ -270,9 +271,9 @@
         if self.precomputed_weights is None:
             self.precompute_weights()
         x_retyped = self.zero_arr(input_x.shape, dtype = self.dtype)
         x_retyped[:] = input_x
         xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
         dz_dsigma = self.grad_fun(x_retyped, xtrans, self.precomputed_weights,
                 self.ard_position_key, self.full_ard_weights,
-                self.hyperparams[1], self.num_threads)
+                self.hyperparams[1], self.num_threads, self.fit_intercept)
         return xtrans, dz_dsigma
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/__init__.py` & `xGPR-0.1.2.0/xGPR/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/linear.py` & `xGPR-0.1.2.0/xGPR/kernels/basic_kernels/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,15 @@
 except:
     pass
 from ..kernel_baseclass import KernelBaseclass
 
 
 class Linear(KernelBaseclass):
     """The Linear kernel corresponds to Bayesian linear regression.
-    For other attributes not described here, see the baseclass.
-
-    Attributes:
-        fit_intercept (bool): Indicates whether we are fitting a
-            y-intercept or no y-intercept.
-        hyperparams (np.ndarray): This kernel has two
-            hyperparameters: lambda_ (noise), beta_ (amplitude).
+    For attributes not described here, see the baseclass.
     """
 
     def __init__(self, xdim, num_rffs, random_seed = 123,
                 device = "cpu", num_threads = 2,
                 double_precision = True,
                 kernel_spec_parms = {}):
         """Constructor.
@@ -43,15 +37,15 @@
         self.fit_intercept = True
         actual_rffs = xdim[1] + 1
         if "intercept" in kernel_spec_parms:
             if kernel_spec_parms["intercept"] is False:
                 self.fit_intercept = False
                 actual_rffs = xdim[1]
 
-        super().__init__(actual_rffs, xdim)
+        super().__init__(actual_rffs, xdim, kernel_spec_parms = kernel_spec_parms)
 
         if len(xdim) > 2:
             raise ValueError("The Linear kernel is only applicable for "
                     "fixed vector input.")
         self.hyperparams = np.ones((2))
         self.bounds = np.asarray([[1e-3,1e1], [0.125, 8]])
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/matern.py` & `xGPR-0.1.2.0/xGPR/kernels/basic_kernels/matern.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,16 @@
             double_precision (bool): If True, generate random features in double precision.
                 Otherwise, generate as single precision.
             kernel_spec_parms (dict): A dictionary of additional kernel-specific
                 attributes. In this case, should contain 'matern_nu'.
         """
         super().__init__(num_rffs, xdim, num_threads,
                 sine_cosine_kernel = True, random_seed = random_seed,
-                double_precision = double_precision)
+                double_precision = double_precision,
+                kernel_spec_parms = kernel_spec_parms)
         self.hyperparams = np.ones((3))
         if "matern_nu" not in kernel_spec_parms:
             raise ValueError("Tried to initialize a Matern kernel without supplying nu.")
 
         self.matern_nu = kernel_spec_parms["matern_nu"]
         if self.matern_nu < 1/2 or self.matern_nu > 5/2:
             raise ValueError("nu must be >= 1/2 and <= 5/2.")
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/polynomial.py` & `xGPR-0.1.2.0/xGPR/kernels/basic_kernels/polynomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 Otherwise, generate as single precision.
             kernel_spec_parms (dict): A dictionary of kernel-specific parameters.
                 In this case, must contain "polydegree", which is the degree
                 of the polynomial.
         """
 
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = False,
-                double_precision = double_precision)
+                double_precision = double_precision, kernel_spec_parms = kernel_spec_parms)
         if "polydegree" not in kernel_spec_parms:
             raise ValueError("For the Poly kernel, 'polydegree' must be "
                 "included as the degree of the polynomial.")
         self.polydegree = kernel_spec_parms["polydegree"]
         if self.polydegree < 2 or self.polydegree > 4:
             raise ValueError("Polydegree should be in the range from 2 to 4.")
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/rbf_linear.py` & `xGPR-0.1.2.0/xGPR/kernels/basic_kernels/rbf_linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,16 @@
         feature_gen: A reference to the wrapped C function that generates
             features.
         gradfun: A reference to the wrapped C function that calculates
             gradients.
     """
 
     def __init__(self, xdim, num_rffs, random_seed = 123, device = "cpu",
-                num_threads = 2, double_precision = False, **kwargs):
+                num_threads = 2, double_precision = False,
+                kernel_spec_parms = {}):
         """Constructor. Calls the KernelBaseclass
         constructor first.
 
         Args:
             num_rffs (int): The user-requested number of random Fourier features.
                 For sine-cosine kernels (RBF, Matern), this will be saved by the
                 class as num_rffs. Note that the number of input features (from xdim)
@@ -74,28 +75,30 @@
                 and M is number of timepoints or sequence elements (convolution
                 kernels only).
             num_threads (int): The number of threads to use for generating random
                 features if running on CPU. If running on GPU, this is ignored.
             random_seed (int): The seed to the random number generator.
             double_precision (bool): If True, generate random features in double precision.
                 Otherwise, generate as single precision.
+            kernel_spec_parms (dict): A dictionary of other optional kernel settings.
 
         Raises:
             ValueError: If a non 2d input array dimensionality is supplied.
         """
         if len(xdim) != 2:
             raise ValueError("The dimensionality of the input is inappropriate for "
                         "the kernel you have selected.")
 
         #Although this IS a sine_cosine kernel, we don't want the parent class
         #to enforce that num_rffs be a multiple of two (only needs to be true
         #for internal rffs), so we set sine_cosine_kernel to False.
         super().__init__(num_rffs, xdim, num_threads = num_threads,
                 sine_cosine_kernel = False,
-                double_precision = double_precision)
+                double_precision = double_precision,
+                kernel_spec_parms = kernel_spec_parms)
 
         self.internal_rffs = num_rffs - xdim[1]
         if self.internal_rffs <= 1 or not (self.internal_rffs / 2).is_integer():
             raise ValueError("For the RBFLinear kernel, the number of 'random' "
                     "features requested includes the number of features in "
                     "the input. So, for example, if the input is a length 100 "
                     "vector and training_rffs is 1000, 900 random features will "
@@ -172,15 +175,15 @@
                             dtype = self.dtype)
         xtrans[:,:,:self.xdim[1]] = input_x[:,None,:] * self.hyperparams[3]
 
         output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
         random_features = self.empty((input_x.shape[0], self.internal_rffs),
                         self.out_type)
         self.feature_gen(xtrans, random_features, self.radem_diag, self.chi_arr,
-                self.hyperparams[1], self.num_threads)
+                self.hyperparams[1], self.num_threads, self.fit_intercept)
 
         output_x[:,:self.internal_rffs] = random_features
         output_x[:,self.internal_rffs:] = input_x * self.hyperparams[2] * self.hyperparams[1]
         return output_x
 
 
     def kernel_specific_set_hyperparams(self):
@@ -215,14 +218,14 @@
         random_features = self.empty((input_x.shape[0], self.internal_rffs),
                 self.out_type)
         output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
         output_grad = self.zero_arr((input_x.shape[0], self.num_rffs, 2), self.out_type)
 
         output_grad[:,:self.internal_rffs,1:2] = self.gradfun(xtrans, random_features,
                         self.radem_diag, self.chi_arr, self.hyperparams[1],
-                        self.hyperparams[3], self.num_threads)
+                        self.hyperparams[3], self.num_threads, self.fit_intercept)
 
         output_grad[:,self.internal_rffs:,0] = input_x * self.hyperparams[1]
 
         output_x[:,:self.internal_rffs] = random_features
         output_x[:,self.internal_rffs:] = input_x * self.hyperparams[2] * self.hyperparams[1]
         return output_x, output_grad
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py` & `xGPR-0.1.2.0/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,16 @@
             features.
         gradfun: A reference to the wrapped C function that calculates
             gradients.
     """
 
     def __init__(self, num_rffs, xdim, num_threads = 2,
                             sine_cosine_kernel = True, random_seed = 123,
-                            double_precision = False):
+                            double_precision = False,
+                            kernel_spec_parms = {}):
         """Constructor for the SORFKernelBaseclass. Calls the KernelBaseclass
         constructor first.
 
         Args:
             num_rffs (int): The user-requested number of random Fourier features.
                 For sine-cosine kernels (RBF, Matern), this will be saved by the
                 class as num_rffs.
@@ -65,21 +66,23 @@
             sine_cosine_kernel (bool): If True, the kernel is a sine-cosine kernel,
                 meaning it will sample self.num_freqs frequencies and use the sine
                 and cosine of each to generate twice as many features
                 (self.num_rffs). sine-cosine kernels only accept num_rffs
                 that are even numbers.
             double_precision (bool): If True, generate random features in double precision.
                 Otherwise, generate as single precision.
+            kernel_spec_parms (dict): A dictionary of other kernel-specific settings.
 
         Raises:
             ValueError: If a non 2d input array dimensionality is supplied.
         """
         super().__init__(num_rffs, xdim, num_threads = num_threads,
                 sine_cosine_kernel = sine_cosine_kernel,
-                double_precision = double_precision)
+                double_precision = double_precision,
+                kernel_spec_parms = kernel_spec_parms)
         if len(xdim) != 2:
             raise ValueError("The dimensionality of the input is inappropriate for "
                         "the kernel you have selected.")
 
         self.padded_dims = 2**ceil(np.log2(max(xdim[-1], 2)))
 
         radem_array = np.asarray([-1,1], dtype=np.int8)
@@ -130,15 +133,15 @@
             xtrans: A cupy or numpy array containing the generated features.
         """
         xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
                             dtype = self.dtype)
         xtrans[:,:,:self.xdim[1]] = input_x[:,None,:] * self.hyperparams[2]
         output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
         self.feature_gen(xtrans, output_x, self.radem_diag, self.chi_arr,
-                self.hyperparams[1], self.num_threads)
+                self.hyperparams[1], self.num_threads, self.fit_intercept)
         return output_x
 
 
     def kernel_specific_set_hyperparams(self):
         """Provided for consistency with baseclass. This
         kernel has no kernel-specific properties that must
         be reset after hyperparameters are changed."""
@@ -165,9 +168,10 @@
                 output_x with respect to the kernel-specific hyperparameters.
         """
         xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
                             dtype = self.dtype)
         xtrans[:,:,:self.xdim[1]] = input_x[:,None,:]
         output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
         dz_dsigma = self.gradfun(xtrans, output_x, self.radem_diag, self.chi_arr,
-                self.hyperparams[1], self.hyperparams[2], self.num_threads)
+                self.hyperparams[1], self.hyperparams[2], self.num_threads,
+                self.fit_intercept)
         return output_x, dz_dsigma
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py` & `xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/conv_feature_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,32 +41,30 @@
             from S H D1 H D2 H D3 are correct.
         conv_func: A reference to either CPUConv1dTransform or
             GPUConv1dTransform, both Cython functions in compiled
             code, as appropriate based on the current device.
         stride_tricks: A reference to cp.lib.stride_tricks.as_strided
             or np.lib.stride_tricks.as_strided, as appropriate based
             on the current device.
-        subtract_mean (bool): Indicates whether mean should be subtracted.
         num_threads (int): Number of threads to use if running on CPU;
             ignored if running on GPU.
     """
 
     def __init__(self, seqwidth, num_rffs, random_seed = 123, device = "cpu",
-                    conv_width = 9, subtract_mean = False, num_threads = 2):
+                    conv_width = 9, num_threads = 2):
         """Constructor for FHT_Conv1d.
 
         Args:
             seqwidth (int): The number of features per timepoint / sequence element.
             num_rffs (int): The user-requested number of random Fourier features.
                 For sine-cosine kernels (RBF, Matern), this will be saved by the
                 class as num_rffs.
             random_seed (int): The seed to the random number generator.
             device (str): One of 'cpu', 'gpu'. Indicates the starting device.
             conv_width (int): The width of the convolution kernel. Defaults to 9.
-            subtract_mean (bool): Indicates whether mean should be subtracted.
             num_threads (int): Number of threads to use if running on CPU;
                 ignored if running on GPU.
 
         Raises:
             ValueError: A ValueError is raised if the dimensions of the input are
                 inappropriate given the conv_width.
         """
@@ -86,15 +84,14 @@
                                 replace=True)
         self.chi_arr = chi.rvs(df=self.padded_dims, size=self.init_calc_featsize,
                             random_state = random_seed)
 
         self.num_threads = num_threads
         self.conv_func = None
         self.stride_tricks = None
-        self.subtract_mean = subtract_mean
         self.device = device
 
 
     def kernel_specific_set_device(self, new_device):
         """Called by parent class when device is changed. Moves
         some of the object parameters to the appropriate device
         and updates convenience references to numpy / cupy
@@ -133,15 +130,15 @@
         #is a little dangerous to use.
         x_strided = self.stride_tricks(input_x, shape=(input_x.shape[0], num_slides,
                             self.dim2_no_padding),
                             strides=(input_x.strides[0], input_x.shape[2] *
                                 input_x.strides[2], input_x.strides[2]))
         reshaped_x[:,:,:self.dim2_no_padding] = x_strided
         self.conv_func(reshaped_x, self.radem_diag,
-                output_x, self.chi_arr, self.num_threads, self.subtract_mean)
+                output_x, self.chi_arr, self.num_threads)
         output_x = output_x[:,:self.num_rffs]
         return output_x
 
 
     @property
     def device(self):
         """Getter for the device property, which determines
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/fht_conv1d.py` & `xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/fht_conv1d.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,16 @@
                 attributes. In this case, should contain 'conv_width'.
 
         Raises:
             ValueError: A ValueError is raised if the dimensions of the input are
                 inappropriate given the conv_width.
         """
         super().__init__(num_rffs, xdim, num_threads = 2,
-                sine_cosine_kernel = True, double_precision = double_precision)
+                sine_cosine_kernel = True, double_precision = double_precision,
+                kernel_spec_parms = kernel_spec_parms)
         if len(xdim) != 3:
             raise ValueError("Tried to initialize the Conv1d kernel with a 2d x-"
                     "array! x should be a 3d array for Conv1d.")
         if "conv_width" not in kernel_spec_parms:
             raise ValueError("Conv_width not supplied to conv1d kernel!")
 
         self.hyperparams = np.ones((3))
@@ -164,15 +165,15 @@
                                 self.padded_dims), self.dtype)
         x_strided = self.stride_tricks(input_x, shape=(input_x.shape[0],
                             self.num_slides, self.dim2_no_padding),
                             strides=(input_x.strides[0], input_x.shape[2] * input_x.strides[2],
                                 input_x.strides[2]))
         reshaped_x[:,:,:self.dim2_no_padding] = x_strided * self.hyperparams[2]
         self.conv_func(reshaped_x, self.radem_diag, xtrans, self.chi_arr, self.num_threads,
-                self.hyperparams[1])
+                self.hyperparams[1], self.fit_intercept)
         return xtrans
 
 
     def kernel_specific_set_hyperparams(self):
         """Provided for consistency with baseclass. This
         kernel has no kernel-specific properties that must
         be reset after hyperparameters are changed."""
@@ -206,10 +207,10 @@
         x_strided = self.stride_tricks(input_x, shape=(input_x.shape[0],
                             self.num_slides, self.dim2_no_padding),
                             strides=(input_x.strides[0], input_x.shape[2] *
                                 input_x.strides[2], input_x.strides[2]))
         reshaped_x[:,:,:self.dim2_no_padding] = x_strided
         dz_dsigma = self.grad_func(reshaped_x, self.radem_diag,
                 output_x, self.chi_arr, self.num_threads, self.hyperparams[2],
-                self.hyperparams[1])
+                self.hyperparams[1], self.fit_intercept)
 
         return output_x, dz_dsigma
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_arccos.py` & `xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/graph_arccos.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
             adding 1 (to add a y-intercept).
         radem_diag: The diagonal matrices for the SORF transform. Type is int8.
         chi_arr: A diagonal array whose elements are drawn from the chi
             distribution. Ensures the marginals of the matrix resulting
             from S H D1 H D2 H D3 are correct.
         conv_func: A reference to the random feature generation function
             appropriate for the current device.
+        fit_intercept (bool): Determines whether to fit a y-intercept.
+            Defaults to True.
     """
 
     def __init__(self, xdim, num_rffs, random_seed = 123, device = "cpu",
                     num_threads = 2, double_precision = False, kernel_spec_parms = {}):
         """Constructor.
 
         Args:
@@ -66,15 +68,15 @@
                 kernel is order 1 or order 2.
 
         Raises:
             ValueError: A ValueError is raised if the dimensions of the input are
                 inappropriate given the conv_width.
         """
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = False,
-                double_precision = double_precision)
+                double_precision = double_precision, kernel_spec_parms = kernel_spec_parms)
         if len(xdim) != 3:
             raise ValueError("Tried to initialize the GraphArcCos kernel with a "
                     "2d x-array! x should be a 3d array for a graph kernel.")
 
         if "order" not in kernel_spec_parms:
             raise ValueError("For the GraphArcCosine kernel, 'order' must be "
                 "included to indicate an arc-cosine kernel of order 1 or 2.")
@@ -149,15 +151,16 @@
             raise ValueError("Input X must be a 3d array.")
         xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
         reshaped_x = self.zero_arr((input_x.shape[0], input_x.shape[1],
                                 self.padded_dims), self.dtype)
         reshaped_x[:,:,:input_x.shape[2]] = input_x
         reshaped_x[:,:,input_x.shape[2]] = 1.0
         self.conv_func(reshaped_x, self.radem_diag, xtrans, self.chi_arr,
-                self.num_threads, self.hyperparams[1], self.order)
+                self.num_threads, self.hyperparams[1], self.order,
+                self.fit_intercept)
         return xtrans
 
 
 
     def kernel_specific_gradient(self, input_x):
         """Since all kernels share the beta and lambda hyperparameters,
         the gradient for these can be calculated by the parent class.
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_polysum.py` & `xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/graph_polysum.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         graph_poly_func: A reference to the Cython-wrapped C function
             that will be used for random feature generation.
         padded_dims (int): The size of the expected input after zero
             padding.
         init_calc_freqsize (int): The number of features to generate.
             May be greater than num_rffs, in which case excess is
             discarded.
+        fit_intercept (bool): Determines whether to fit a y-intercept.
+            Defaults to True.
     """
 
     def __init__(self, xdim, num_rffs, random_seed = 123,
                 device = "cpu", num_threads = 2,
                 double_precision = False,
                 kernel_spec_parms = {}):
         """Constructor.
@@ -60,21 +62,22 @@
                 Otherwise, generate as single precision.
             kernel_spec_parms (dict): A dictionary of kernel-specific parameters.
                 In this case, must contain "polydegree", which is the degree
                 of the polynomial.
         """
 
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = False,
-                double_precision = double_precision)
+                double_precision = double_precision, kernel_spec_parms = kernel_spec_parms)
         if "polydegree" not in kernel_spec_parms:
             raise ValueError("For the GraphPoly kernel, 'polydegree' must be "
                 "included as the degree of the polynomial.")
         self.polydegree = kernel_spec_parms["polydegree"]
         if self.polydegree < 2 or self.polydegree > 4:
             raise ValueError("Polydegree should be in the range from 2 to 4.")
+
         self.hyperparams = np.ones((2))
         self.bounds = np.asarray([[1e-3,1e1], [0.2, 5]])
 
         self.padded_dims = 2**ceil(np.log2(max(xdim[2], 2)))
         num_repeats = ceil(self.num_freqs / self.padded_dims)
         self.init_calc_freqsize = num_repeats * self.padded_dims
 
@@ -138,14 +141,17 @@
         retyped_input[:,:,0] = 1
         output_x = self.zero_arr((input_x.shape[0], self.init_calc_freqsize),
                             dtype = self.dtype)
         self.graph_poly_func(retyped_input, self.radem_diag,
                 self.chi_arr, output_x, self.polydegree, self.num_threads)
         scaling_constant = self.hyperparams[1] * np.sqrt(1 / self.num_freqs)
         output_x = output_x[:,:self.num_rffs].astype(self.out_type) * scaling_constant
+
+        if self.fit_intercept:
+            output_x[:,-1] = self.hyperparams[1]
         return output_x
 
 
 
     def kernel_specific_gradient(self, input_x):
         """Since all kernels share the beta and lambda hyperparameters,
         the gradient for these can be calculated by the parent class.
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_rbf.py` & `xGPR-0.1.2.0/xGPR/kernels/convolution_kernels/graph_rbf.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 Otherwise, generate as single precision.
 
         Raises:
             ValueError: A ValueError is raised if the dimensions of the input are
                 inappropriate given the conv_width.
         """
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = True,
-                double_precision = double_precision)
+                double_precision = double_precision, kernel_spec_parms = kernel_spec_parms)
         if len(xdim) != 3:
             raise ValueError("Tried to initialize the GraphRBF kernel with a "
                     "2d x-array! x should be a 3d array for GraphRBF.")
 
         self.hyperparams = np.ones((3))
         self.bounds = np.asarray([[1e-3,1e1], [0.2, 5], [1e-2, 1e2]])
         rng = np.random.default_rng(random_seed)
@@ -134,15 +134,15 @@
         if len(input_x.shape) != 3:
             raise ValueError("Input X must be a 3d array.")
         xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
         reshaped_x = self.zero_arr((input_x.shape[0], input_x.shape[1],
                                 self.padded_dims), self.dtype)
         reshaped_x[:,:,:input_x.shape[2]] = input_x * self.hyperparams[2]
         self.conv_func(reshaped_x, self.radem_diag, xtrans, self.chi_arr,
-                self.num_threads, self.hyperparams[1])
+                self.num_threads, self.hyperparams[1], self.fit_intercept)
         return xtrans
 
 
 
     def kernel_specific_gradient(self, input_x):
         """Since all kernels share the beta and lambda hyperparameters,
         the gradient for these can be calculated by the parent class.
@@ -163,9 +163,9 @@
             raise ValueError("Input X must be a 3d array.")
         output_x = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
         reshaped_x = self.zero_arr((input_x.shape[0], input_x.shape[1],
                                 self.padded_dims), self.dtype)
         reshaped_x[:,:,:input_x.shape[2]] = input_x
         dz_dsigma = self.grad_func(reshaped_x, self.radem_diag,
                 output_x, self.chi_arr, self.num_threads, self.hyperparams[2],
-                self.hyperparams[1])
+                self.hyperparams[1], self.fit_intercept)
         return output_x, dz_dsigma
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/kernel_baseclass.py` & `xGPR-0.1.2.0/xGPR/kernels/kernel_baseclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,21 @@
             found using float64 for FHT to provide any significant improvement on
             benchmark problems).
         out_type: A reference to either np.float64 or cp.float64 depending on
             device.
         empty: A reference to either np.emtpy or cp.empty depending on self.device.
         double_precision (bool): If True, generate random features in double precision.
             Otherwise, generate as single precision.
+        fit_intercept (bool): Whether to fit a y-intercept. Defaults to True but can
+            be set to False by adding "intercept":False to kernel_spec_parms.
     """
 
     def __init__(self, num_rffs, xdim, num_threads = 2,
-            sine_cosine_kernel = False, double_precision = False):
+            sine_cosine_kernel = False, double_precision = False,
+            kernel_spec_parms = {}):
         """Constructor for the KernelBaseclass.
 
         Args:
             num_rffs (int): The user-requested number of random Fourier features.
                 For sine-cosine kernels (RBF, Matern), this will be saved by the
                 class as num_rffs.
             xdim (tuple): The dimensions of the input. Either (N, D) or (N, M, D)
@@ -72,39 +75,49 @@
             sine_cosine_kernel (bool): If True, the kernel is a sine-cosine kernel,
                 meaning it will sample self.num_freqs frequencies and use the sine
                 and cosine of each to generate twice as many features
                 (self.num_rffs). sine-cosine kernels only accept num_rffs
                 that are even numbers.
             double_precision (bool): If True, generate random features in double precision.
                 Otherwise, generate as single precision.
+            kernel_spec_parms (dict): A dictionary of kernel settings / kernel-specific
+                parameters.
 
         Raises:
             ValueError: Raises a ValueError if a sine-cosine kernel is requested
                 but num_rffs is not an integer multiple of 2.
         """
         self.double_precision = double_precision
+        if num_rffs < 2:
+            raise ValueError("num_rffs should always be >= 2.")
+
         if sine_cosine_kernel:
-            if num_rffs <= 1 or not (num_rffs / 2).is_integer():
+            if not (num_rffs / 2).is_integer():
                 raise ValueError("For sine-cosine kernels (e.g. matern, rbf) "
                         "the number of random fourier features must be an integer "
                         "multiple of two.")
             self.num_freqs = int(num_rffs / 2)
             self.num_rffs = num_rffs
         else:
             self.num_freqs = num_rffs
             self.num_rffs = num_rffs
+
+        self.fit_intercept = True
+        if "intercept" in kernel_spec_parms:
+            if kernel_spec_parms["intercept"] is False:
+                self.fit_intercept = False
+
         self.xdim = xdim
         self.hyperparams = None
         self.bounds = None
 
         self.num_threads = num_threads
 
 
 
-
     @abc.abstractmethod
     def transform_x(self, input_x):
         """Kernel classes must implement a method that generates
         random features for a given set of inputs."""
 
     @abc.abstractmethod
     def kernel_specific_set_device(self, new_device):
@@ -196,18 +209,20 @@
         Returns:
             valid_data (bool): True if input was acceptable,
                 False otherwise.
         """
         valid_data = True
         if len(input_x.shape) != len(self.xdim):
             valid_data = False
-        if len(self.xdim) == 3:
+        elif len(self.xdim) == 3:
             if input_x.shape[2] != self.xdim[2]:
                 valid_data = False
-        if input_x.shape[1] != self.xdim[1]:
+            if input_x.shape[1] < 1:
+                valid_data = False
+        elif input_x.shape[1] != self.xdim[1]:
             valid_data = False
         return valid_data
 
 
 
     def get_hyperparams(self, logspace = True):
         """Returns the kernel hyperparameters. We have not used the property
```

### Comparing `xGPR-0.1.1.6/xGPR/kernels/srht_compressor.py` & `xGPR-0.1.2.0/xGPR/kernels/srht_compressor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/optimizers/bayes_grid_optimizer.py` & `xGPR-0.1.2.0/xGPR/optimizers/bayes_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/optimizers/crude_grid_optimizer.py` & `xGPR-0.1.2.0/xGPR/optimizers/crude_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/optimizers/lb_optimizer.py` & `xGPR-0.1.2.0/xGPR/optimizers/lb_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/optimizers/map_loss_bayes_optimizer.py` & `xGPR-0.1.2.0/xGPR/optimizers/map_loss_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/optimizers/pure_bayes_optimizer.py` & `xGPR-0.1.2.0/xGPR/optimizers/pure_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py` & `xGPR-0.1.2.0/xGPR/preconditioners/cuda_rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/preconditioners/inter_device_preconditioners.py` & `xGPR-0.1.2.0/xGPR/preconditioners/inter_device_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_constructors.py` & `xGPR-0.1.2.0/xGPR/preconditioners/rand_nys_constructors.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_preconditioners.py` & `xGPR-0.1.2.0/xGPR/preconditioners/rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/preconditioners/tuning_preconditioners.py` & `xGPR-0.1.2.0/xGPR/preconditioners/tuning_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 cimport numpy as np
 cimport cython
 from cython cimport floating
 from libc cimport stdint
 from libc.stdint cimport uintptr_t
 from libc.stdint cimport int8_t, int32_t
+from libcpp cimport bool
 import math
 
 
 
 cdef extern from "convolution_ops/conv1d_operations.h" nogil:
     const char *conv1dPrep_[T](int8_t *radem, T reshapedX[],
             int numThreads, int reshapedDim0,
@@ -46,15 +47,15 @@
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuConv1dMaxpool(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
                 np.ndarray[np.float64_t, ndim=2] outputArray,
                 np.ndarray[floating, ndim=1] chiArr,
-                int numThreads, bint subtractMean = False):
+                int numThreads):
     """Uses wrapped C extensions to perform random feature generation
     with ReLU activation and maxpooling.
 
     Args:
         reshapedX (np.ndarray): An array from which
             the features will be generated. Is not modified. Must
             be of shape (N x D x C) where C is a power of 2. Should
@@ -65,16 +66,14 @@
         outputArray (np.ndarray): An N x R array in which the output features
             will be stored.
         chiArr (np.ndarray): A stack of diagonal matrices stored as an
             array of shape (R) drawn from a chi distribution.
         num_threads (int): This argument is so that this function has
             the same interface as the CPU SORF Transform. It is not
             needed for the GPU transform and is ignored.
-        subtractMean (bool): If True, subtract the mean of each row from
-            that row.
     """
     cdef const char *errCode
     cdef int i, startPosition, cutoff
     cdef np.ndarray[floating, ndim=3] reshapedXCopy = reshapedX.copy()
     cdef np.ndarray[np.float64_t, ndim=2] gradient
     cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
 
@@ -119,16 +118,14 @@
                     reshapedX.shape[2], i * reshapedX.shape[2],
                     radem.shape[2])
             if errCode.decode("UTF-8") != "no_error":
                 raise Exception("Fatal error encountered during random feature generation.")
         
             reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
             outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
-            if subtractMean:
-                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
 
             cutoff += reshapedX.shape[2]
             startPosition += reshapedX.shape[2]
     elif reshapedX.dtype == "float64" and chiArr.dtype == "float64":
         for i in range(num_repeats):
             reshapedXCopy[:] = reshapedX
             errCode = conv1dPrep_[double](&radem[0,0,0],
@@ -137,30 +134,29 @@
                     reshapedX.shape[2], i * reshapedX.shape[2],
                     radem.shape[2])
             if errCode.decode("UTF-8") != "no_error":
                 raise Exception("Fatal error encountered during random feature generation.")
         
             reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
             outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
-            if subtractMean:
-                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
 
             cutoff += reshapedX.shape[2]
             startPosition += reshapedX.shape[2]
     else:
         raise ValueError("Unexpected types passed to wrapped C++ function.")
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuConv1dFGen(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
                 np.ndarray[np.float64_t, ndim=2] outputArray,
                 np.ndarray[floating, ndim=1] chiArr,
-                int numThreads, double beta_):
+                int numThreads, double beta_,
+                bool fitIntercept = False):
     """Uses wrapped C functions to generate random features for FHTConv1d, GraphConv1d,
     and related kernels. This function cannot be used to calculate the gradient
     so is only used for forward pass only (during fitting, inference, non-gradient-based
     optimization). It does not multiply by the lengthscales, so caller should do this.
     (This enables this function to also be used for GraphARD kernels if desired.)
 
     Args:
@@ -173,14 +169,16 @@
             Rademacher distribution. Shape must be (3 x D x C).
         outputArray (np.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
         chiArr (np.ndarray): A stack of diagonal matrices stored as an
             array of shape m * C drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
         beta_ (float): The amplitude.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
     cdef np.ndarray[floating, ndim=3] reshapedXCopy = np.zeros((reshapedX.shape[0],
                         reshapedX.shape[1], reshapedX.shape[2]), dtype=reshapedX.dtype)
@@ -209,16 +207,14 @@
     if not radem.shape[2] % reshapedX.shape[2] == 0:
         raise ValueError("radem should be an integer multiple of shape[2].")
 
     if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
         or not chiArr.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments is not C contiguous.")
 
-    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
-    scalingTerm *= beta_
 
     if chiArr.dtype == "float32" and reshapedX.dtype == "float32":
         errCode = convRBFFeatureGen_[float](&radem[0,0,0], <float*>addr_input,
                 <float*>addr_copy_buffer, <float*>addr_chi, &outputArray[0,0],
                 numThreads, reshapedX.shape[0],
                 reshapedX.shape[1], reshapedX.shape[2],
                 chiArr.shape[0], radem.shape[2])
@@ -230,26 +226,34 @@
                 chiArr.shape[0], radem.shape[2])
     else:
         raise ValueError("Unexpected types passed to wrapped C++ function.")
 
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered while performing convolution.")
 
-    outputArray *= scalingTerm
-
+    if fitIntercept:
+        scalingTerm = np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+        scalingTerm *= beta_
+        outputArray *= scalingTerm
+        outputArray[:,0] = beta_
+    else:
+        scalingTerm = np.sqrt(2 / <double>(chiArr.shape[0]))
+        scalingTerm *= beta_
+        outputArray *= scalingTerm
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuConvGrad(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
                 np.ndarray[np.float64_t, ndim=2] outputArray,
                 np.ndarray[floating, ndim=1] chiArr,
                 int numThreads, float sigma,
-                float beta_):
+                float beta_,
+                bool fitIntercept = False):
     """Performs feature generation for RBF-based convolution kernels while
     also performing gradient calculations.
 
     Args:
         reshapedX (np.ndarray): Raw data reshaped so that a convolution can be
             performed on it using orthogonal random features with the SORF
             operation. This array is not modified in place -- rather the features
@@ -260,14 +264,16 @@
         outputArray (np.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
         chiArr (np.ndarray): A stack of diagonal matrices stored as an
             array of shape m * C drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
         sigma (float): The lengthscale.
         beta_ (float): The amplitude.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
 
     Returns:
         gradient (np.ndarray); An array of shape output.shape[0] x output.shape[1] x 1.
     """
@@ -302,17 +308,14 @@
                 "reshapedX.shape[2].")
 
     if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
         or not chiArr.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments to cpuGraphConv1dTransform is not "
                 "C contiguous.")
 
-    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
-    scalingTerm *= beta_
-
     if chiArr.dtype == "float32" and reshapedX.dtype == "float32":
         errCode = convRBFGrad_[float](&radem[0,0,0], <float*>addr_input,
                     <float*>addr_copy_buffer, <float*>addr_chi, &outputArray[0,0],
                     &gradient[0,0,0], sigma,
                     numThreads, reshapedX.shape[0],
                     reshapedX.shape[1], reshapedX.shape[2],
                     chiArr.shape[0], radem.shape[2])
@@ -325,29 +328,40 @@
                     chiArr.shape[0], radem.shape[2])
     else:
         raise ValueError("Unexpected types passed to wrapped C++ function.")
 
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered while performing graph convolution.")
 
-    outputArray *= scalingTerm
-    gradient *= scalingTerm
+    if fitIntercept:
+        scalingTerm = np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+        scalingTerm *= beta_
+        outputArray *= scalingTerm
+        gradient *= scalingTerm
+        outputArray[:,0] = beta_
+        gradient[:,0] = 0
+    else:
+        scalingTerm = np.sqrt(2 / <double>(chiArr.shape[0]))
+        scalingTerm *= beta_
+        outputArray *= scalingTerm
+        gradient *= scalingTerm
     return gradient
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuConv1dArcCosFGen(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
                 np.ndarray[np.float64_t, ndim=2] outputArray,
                 np.ndarray[floating, ndim=1] chiArr,
                 int numThreads, double beta_,
-                int kernelOrder):
+                int kernelOrder,
+                bool fitIntercept = False):
     """Uses wrapped C functions to generate random features for ArcCosine kernels
     on sequences and graphs.
 
     Args:
         reshapedX (np.ndarray): Raw data reshaped so that a convolution can be
             performed on it using orthogonal random features with the SORF
             operation. This array is not modified in place -- rather the features
@@ -358,14 +372,16 @@
         outputArray (np.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
         chiArr (np.ndarray): A stack of diagonal matrices stored as an
             array of shape m * C drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
         beta_ (float): The amplitude.
         kernelOrder (int): The order of the arc-cosine kernel.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
     cdef np.ndarray[floating, ndim=3] reshapedXCopy = np.zeros((reshapedX.shape[0],
                         reshapedX.shape[1], reshapedX.shape[2]), dtype=reshapedX.dtype)
@@ -418,8 +434,16 @@
             kernelOrder)
     else:
         raise ValueError("Unexpected types passed to wrapped C++ function.")
 
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered while performing convolution.")
 
-    outputArray *= scalingTerm
+    if fitIntercept:
+        scalingTerm = np.sqrt(1 / <double>(chiArr.shape[0] - 1))
+        scalingTerm *= beta_
+        outputArray *= scalingTerm
+        outputArray[:,0] = beta_
+    else:
+        scalingTerm = np.sqrt(1 / <double>(chiArr.shape[0]))
+        scalingTerm *= beta_
+        outputArray *= scalingTerm
```

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
             outputArray[:,startPosition:cutoff] = np.sum(preSumFeats, axis=1)
 
             cutoff += reshapedX.shape[2]
             startPosition += reshapedX.shape[2]
 
 
 
-
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuPolyFHT(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
                 np.ndarray[floating, ndim=3] chiArr,
                 np.ndarray[floating, ndim=3] outputArray,
                 int polydegree, int numThreads):
```

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 cimport numpy as np
 cimport cython
 from cython cimport floating
 from libc cimport stdint
 from libc.stdint cimport uintptr_t
 from libc.stdint cimport int8_t, int32_t
+from libcpp cimport bool
 import math
 
 
 
 
 
 cdef extern from "rbf_ops/rbf_ops.h" nogil:
@@ -41,15 +42,16 @@
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuRBFFeatureGen(np.ndarray[floating, ndim=3] inputArray,
                 np.ndarray[np.float64_t, ndim=2] outputArray,
                 np.ndarray[np.int8_t, ndim=3] radem,
                 np.ndarray[floating, ndim=1] chiArr,
-                double betaHparam, int numThreads):
+                double betaHparam, int numThreads,
+                bool fitIntercept = False):
     """Wraps floatRBFFeatureGen from double_specialized_ops and uses
     it to to generate random features for an RBF kernel (this same routine
     can also be used for Matern, ARD and MiniARD). This wrapper performs all
     of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
         inputArray (np.ndarray): The array on which the SORF transform will be performed.
@@ -58,14 +60,16 @@
         outputArray (np.ndarray): The output array in which the generated features will
             be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
         radem (np.ndarray): A stack of diagonal matrices of type int8_t
             of shape (3 x D x C).
         chiArr (np.ndarray): An array of shape (numFreqs).
         betaHparam (double): The amplitude hyperparameter.
         numThreads (int): Number of threads to run.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or unacceptable inputs
             are supplied.
     """
     cdef const char *errCode
     cdef float logdim
@@ -95,15 +99,18 @@
     if not radem.dtype == "int8":
         raise ValueError("radem must be of type int8.")
     logdim = np.log2(inputArray.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
         raise ValueError("dim2 of the input array to RBF feature gen functions "
                             "must be a power of 2 >= 2.")
 
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
+    if fitIntercept:
+        rbfNormConstant = betaHparam * np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+    else:
+        rbfNormConstant = betaHparam * np.sqrt(2 / <double>chiArr.shape[0])
 
     if inputArray.dtype == "float32" and outputArray.dtype == "float64" \
             and chiArr.dtype == "float32":
         errCode = rbfFeatureGen_[float](<float*>addr_input, &radem[0,0,0],
                 <float*>addr_chi, &outputArray[0,0], rbfNormConstant,
                 inputArray.shape[0], inputArray.shape[1],
                 inputArray.shape[2], chiArr.shape[0],
@@ -115,27 +122,30 @@
                 inputArray.shape[0], inputArray.shape[1],
                 inputArray.shape[2], chiArr.shape[0],
                 numThreads);
     else:
         raise ValueError("The input, output and chiArr arrays do not have expected types.")
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered in RBF feature gen.")
+    if fitIntercept:
+        outputArray[:,0] = betaHparam
 
 
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuRBFGrad(np.ndarray[floating, ndim=3] inputArray,
                 np.ndarray[np.float64_t, ndim=2] outputArray,
                 np.ndarray[np.int8_t, ndim=3] radem,
                 np.ndarray[floating, ndim=1] chiArr,
-                double betaHparam, float sigmaHparam, int numThreads):
+                double betaHparam, float sigmaHparam, int numThreads,
+                bool fitIntercept = False):
     """Wraps floatRBFFeatureGen from double_specialized_ops and uses
     it to to generate random features for an RBF kernel (this same routine
     can also be used for Matern, ARD and MiniARD). This wrapper performs all
     of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
         inputArray (np.ndarray): The array on which the SORF transform will be performed.
@@ -145,14 +155,16 @@
             be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
         radem (np.ndarray): A stack of diagonal matrices of type int8_t
             of shape (3 x D x C).
         chiArr (np.ndarray): An array of shape (numFreqs).
         betaHparam (double): The amplitude hyperparameter.
         sigmaHparam (float): The sigma hyperparameter.
         numThreads (int): Number of threads to run.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or unacceptable inputs
             are supplied.
 
     Returns:
         gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
@@ -188,15 +200,18 @@
     if not radem.dtype == "int8":
         raise ValueError("radem must be of type int8.")
     logdim = np.log2(inputArray.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
         raise ValueError("dim2 of the input array to RBF feature gen functions "
                             "must be a power of 2 >= 2.")
 
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
+    if fitIntercept:
+        rbfNormConstant = betaHparam * np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+    else:
+        rbfNormConstant = betaHparam * np.sqrt(2 / <double>chiArr.shape[0])
 
     if inputArray.dtype == "float32" and outputArray.dtype == "float64" and \
             chiArr.dtype == "float32":
         errCode = rbfGrad_[float](<float*>addr_input, &radem[0,0,0],
                 <float*>addr_chi, &outputArray[0,0], &gradient[0,0,0],
                 rbfNormConstant, sigmaHparam,
                 inputArray.shape[0], inputArray.shape[1],
@@ -210,87 +225,100 @@
                 inputArray.shape[0], inputArray.shape[1],
                 inputArray.shape[2], chiArr.shape[0],
                 numThreads)
     else:
         raise ValueError("The input, output and chiArr arrays do not have expected types.")
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered in RBF feature gen.")
+    if fitIntercept:
+        outputArray[:,0] = betaHparam
+        gradient[:,0] = 0
     return gradient
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cpuMiniARDGrad(np.ndarray[floating, ndim=2] inputX,
-                np.ndarray[np.float64_t, ndim=2] randomFeats,
+                np.ndarray[np.float64_t, ndim=2] outputArray,
                 np.ndarray[floating, ndim=2] precompWeights,
                 np.ndarray[np.int32_t, ndim=1] sigmaMap,
                 np.ndarray[np.float64_t, ndim=1] sigmaVals,
-                double betaHparam, int numThreads):
+                double betaHparam, int numThreads,
+                bool fitIntercept = False):
     """Performs gradient calculations for the MiniARD kernel, using
     pregenerated features and precomputed weights.
 
     Args:
         inputX (np.ndarray): The original input data.
-        randomFeats (np.ndarray): The random features generated using the FHT-
+        outputArray (np.ndarray): The random features generated using the FHT-
             based procedure.
         precompWeights (np.ndarray): The FHT-rf gen procedure applied to an
             identity matrix.
         sigmaMap (np.ndarray): An array mapping which lengthscales correspond
             to which positions in the input.
         sigmaVals (np.ndarray): The lengthscale values, in an array of the same
             dimensionality as the input.
         betaHparam (double): The amplitude hyperparameter.
         numThreads (int): Number of threads to run.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or unacceptable inputs
             are supplied.
 
     Returns:
         gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
             the gradient w/r/t sigma.
     """
     cdef const char *errCode
     cdef float logdim
     cdef double rbfNormConstant
-    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((randomFeats.shape[0],
-                        randomFeats.shape[1], sigmaMap.max() + 1))
+    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((outputArray.shape[0],
+                        outputArray.shape[1], sigmaMap.max() + 1))
 
 
     if inputX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if inputX.shape[0] != randomFeats.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
+    if inputX.shape[0] != outputArray.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
         raise ValueError("Incorrect array dims passed to a wrapped RBF "
                     "feature gen function.")
-    if randomFeats.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
+    if outputArray.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
             precompWeights.shape[1] or sigmaVals.shape[0] != sigmaMap.shape[0]:
         raise ValueError("Incorrect array dims passed to a wrapped RBF "
                     "feature gen function.")
 
-    if not inputX.flags["C_CONTIGUOUS"] or not randomFeats.flags["C_CONTIGUOUS"] or not \
+    if not inputX.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"] or not \
             precompWeights.flags["C_CONTIGUOUS"] or not sigmaMap.flags["C_CONTIGUOUS"] \
             or not sigmaVals.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
                 "C contiguous.")
 
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>precompWeights.shape[0])
+    if fitIntercept:
+        rbfNormConstant = betaHparam * np.sqrt(2.0 / (<double>precompWeights.shape[0] - 0.5))
+    else:
+        rbfNormConstant = betaHparam * np.sqrt(2 / <double>precompWeights.shape[0])
+
     cdef uintptr_t addr_input = inputX.ctypes.data
     cdef uintptr_t addr_precomp_weights = precompWeights.ctypes.data
 
     if inputX.dtype == "float32" and precompWeights.dtype == "float32":
-        errCode = ardGrad_[float](<float*>addr_input, &randomFeats[0,0],
+        errCode = ardGrad_[float](<float*>addr_input, &outputArray[0,0],
                 <float*>addr_precomp_weights, &sigmaMap[0], &sigmaVals[0],
                 &gradient[0,0,0], inputX.shape[0], inputX.shape[1],
                 gradient.shape[2], precompWeights.shape[0],
                 rbfNormConstant, numThreads)
     elif inputX.dtype == "float64" and precompWeights.dtype == "float64":
-        errCode = ardGrad_[double](<double*>addr_input, &randomFeats[0,0],
+        errCode = ardGrad_[double](<double*>addr_input, &outputArray[0,0],
                 <double*>addr_precomp_weights, &sigmaMap[0], &sigmaVals[0],
                 &gradient[0,0,0], inputX.shape[0], inputX.shape[1],
                 gradient.shape[2], precompWeights.shape[0],
                 rbfNormConstant, numThreads)
     else:
         raise ValueError("Unexpected array types passed to wrapped C++ function.")
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered in RBF feature gen.")
+    if fitIntercept:
+        outputArray[:,0] = betaHparam
+        gradient[:,0,:] = 0
     return gradient
```

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 cimport numpy as np
 cimport cython
 from libc cimport stdint
 import cupy as cp
 from libc.stdint cimport uintptr_t
 import math
 from libc.stdint cimport int8_t, int32_t
+from libcpp cimport bool
 
 
 cdef extern from "convolution_ops/convolution.h" nogil:
     const char *conv1dPrep[T](int8_t *radem,
                 T reshapedx[], int reshapeddim0, 
                 int reshapeddim1, int reshapeddim2,
                 int startposition, int numfreqs)
@@ -41,15 +42,15 @@
             int numFreqs, int rademShape2, double scalingTerm,
             int kernelOrder)
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def gpuConv1dMaxpool(reshapedX, radem, outputArray, chiArr,
-        int numThreads, bint subtractMean = False):
+        int numThreads):
     """Uses wrapped C extensions to perform random feature generation
     with ReLU activation and maxpooling. TODO: Transfer the loop
     and sum operations in here to a Cuda kernel and wrap.
 
     Args:
         reshapedX (cp.ndarray): An array of type float32 from which
             the features will be generated. Is not modified. Must
@@ -61,16 +62,14 @@
         outputArray (cp.ndarray): An N x R array in which the output features
             will be stored.
         chiArr (cp.ndarray): A stack of diagonal matrices stored as an
             array of shape (R) drawn from a chi distribution.
         num_threads (int): This argument is so that this function has
             the same interface as the CPU SORF Transform. It is not
             needed for the GPU transform and is ignored.
-        subtractMean (bool): If True, subtract the mean of each row from
-            that row.
     """
     cdef const char *errCode
     cdef int i, startPosition, cutoff
     cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
     reshapedXCopy = reshapedX.copy()
     cdef uintptr_t addr_reshapedCopy = reshapedXCopy.data.ptr
     cdef uintptr_t addr_radem = radem.data.ptr
@@ -128,16 +127,14 @@
                     reshapedX.shape[2], i * reshapedX.shape[2],
                     radem.shape[2])
             if errCode.decode("UTF-8") != "no_error":
                 raise Exception("Fatal error encountered in floatGpuConv1dTransform_.")
         
             reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
             outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
-            if subtractMean:
-                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
 
             cutoff += reshapedX.shape[2]
             startPosition += reshapedX.shape[2]
     elif outputArray.dtype == "float64" and reshapedX.dtype == "float64" and \
             chiArr.dtype == "float64":
         for i in range(num_repeats):
             reshapedXCopy[:] = reshapedX
@@ -146,29 +143,27 @@
                     reshapedX.shape[2], i * reshapedX.shape[2],
                     radem.shape[2])
             if errCode.decode("UTF-8") != "no_error":
                 raise Exception("Fatal error encountered in floatGpuConv1dTransform_.")
         
             reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
             outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
-            if subtractMean:
-                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
 
             cutoff += reshapedX.shape[2]
             startPosition += reshapedX.shape[2]
     else:
         raise ValueError("Inconsistent types passed to a wrapped C++ function.")
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def gpuConv1dFGen(reshapedX, radem, outputArray, chiArr,
-                int numThreads, float beta_):
+                int numThreads, float beta_, bool fitIntercept = False):
     """Uses wrapped C functions to generate random features for FHTConv1d, GraphConv1d,
     and related kernels. This function cannot be used to calculate the gradient
     so is only used for forward pass only (during fitting, inference, non-gradient-based
     optimization). It does not multiply by the lengthscales, so caller should do this.
     (This enables this function to also be used for GraphARD kernels if desired.)
 
     Args:
@@ -180,14 +175,16 @@
         radem (cp.ndarray): A stack of diagonal matrices with elements drawn from the
             Rademacher distribution. Shape must be (3 x D x C).
         outputArray (cp.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
         chiArr (cp.ndarray): A stack of diagonal matrices drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
         beta (float): The amplitude.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
     cdef double scalingTerm
 
@@ -234,15 +231,18 @@
     cdef uintptr_t addr_reshapedX = reshapedX.data.ptr
     cdef uintptr_t addr_featureArray = featureArray.data.ptr
     cdef uintptr_t addr_radem = radem.data.ptr
     cdef uintptr_t addr_chi = chiArr.data.ptr
     cdef uintptr_t addr_output = outputArray.data.ptr
 
 
-    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    if fitIntercept:
+        scalingTerm = np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+    else:
+        scalingTerm = np.sqrt(2 / <double>chiArr.shape[0])
     scalingTerm *= beta_
 
     if outputArray.dtype == "float64" and reshapedX.dtype == "float32" and \
             chiArr.dtype == "float32":
         errCode = convRBFFeatureGen[float](<int8_t*>addr_radem, <float*>addr_reshapedX,
                     <float*>addr_featureArray, <float*>addr_chi,
                     <double*>addr_output, reshapedX.shape[0], reshapedX.shape[1],
@@ -254,21 +254,24 @@
                     <double*>addr_output, reshapedX.shape[0], reshapedX.shape[1], 
                     reshapedX.shape[2], chiArr.shape[0], radem.shape[2], scalingTerm)
     else:
         raise ValueError("Incorrect data types supplied.")
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered while performing FHT RF generation.")
 
+    if fitIntercept:
+        outputArray[:,0] = beta_
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def gpuConvGrad(reshapedX, radem, outputArray, chiArr,
-                int numThreads, float sigma, float beta_):
+                int numThreads, float sigma, float beta_,
+                bool fitIntercept = False):
     """Performs feature generation for the GraphRBF kernel while also performing
     gradient calculations.
 
     Args:
         reshapedX (cp.ndarray): Raw data reshaped so that a convolution can be
             performed on it using orthogonal random features with the SORF
             operation. This array is not modified in place -- rather the features
@@ -278,14 +281,16 @@
             Rademacher distribution. Shape must be (3 x D x C).
         outputArray (cp.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
         chiArr (cp.ndarray): A stack of diagonal matrices drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
         sigma (float): The lengthscale.
         beta (float): The amplitude.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
 
     Returns:
         gradient (cp.ndarray); An array of shape output.shape[0] x output.shape[1] x 1.
     """
@@ -341,15 +346,18 @@
     cdef uintptr_t addr_featureArray = featureArray.data.ptr
     cdef uintptr_t addr_radem = radem.data.ptr
     cdef uintptr_t addr_chi = chiArr.data.ptr
     cdef uintptr_t addr_output = outputArray.data.ptr
     cdef uintptr_t addr_gradient = gradient.data.ptr
 
 
-    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    if fitIntercept:
+        scalingTerm = np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+    else:
+        scalingTerm = np.sqrt(2 / <double>chiArr.shape[0])
     scalingTerm *= beta_
 
     if outputArray.dtype == "float64" and reshapedX.dtype == "float32" and \
             chiArr.dtype == "float32":
         errCode = convRBFFeatureGrad[float](<int8_t*>addr_radem, <float*>addr_reshapedX,
             <float*>addr_featureArray, <float*>addr_chi,
             <double*>addr_output, <double*>addr_gradient, sigma,
@@ -363,22 +371,27 @@
             <double*>addr_gradient, sigma,
             reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
             chiArr.shape[0], radem.shape[2], scalingTerm)
     else:
         raise ValueError("Incorrect data types supplied.")
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered while performing FHT RF generation.")
+
+    if fitIntercept:
+        outputArray[:,0] = beta_
+        gradient[:,0] = 0
     return gradient
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def gpuConv1dArcCosFGen(reshapedX, radem, outputArray, chiArr,
-                int numThreads, float beta_, int kernelOrder):
+                int numThreads, float beta_, int kernelOrder,
+                bool fitIntercept = False):
     """Uses wrapped C functions to generate random features for arccosine kernels
     for sequences and graphs.
 
     Args:
         reshapedX (cp.ndarray): Raw data reshaped so that a convolution can be
             performed on it using orthogonal random features with the SORF
             operation. This array is not modified in place -- rather the features
@@ -389,14 +402,16 @@
         outputArray (cp.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
         chiArr (cp.ndarray): A stack of diagonal matrices drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT. Supplied for consistency
             with CPU-wrapper functions, since it is not actually used.
         beta (float): The amplitude.
         kernelOrder (int): The order of the arccosine kernel.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
     cdef double scalingTerm
 
@@ -446,15 +461,18 @@
     cdef uintptr_t addr_reshapedX = reshapedX.data.ptr
     cdef uintptr_t addr_featureArray = featureArray.data.ptr
     cdef uintptr_t addr_radem = radem.data.ptr
     cdef uintptr_t addr_chi = chiArr.data.ptr
     cdef uintptr_t addr_output = outputArray.data.ptr
 
 
-    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    if fitIntercept:
+        scalingTerm = np.sqrt(1 / <double>(chiArr.shape[0] - 1))
+    else:
+        scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
     scalingTerm *= beta_
 
     if outputArray.dtype == "float64" and reshapedX.dtype == "float32" and \
             chiArr.dtype == "float32":
         errCode = convArcCosFeatureGen[float](<int8_t*>addr_radem, <float*>addr_reshapedX,
             <float*>addr_featureArray, <float*>addr_chi, <double*>addr_output,
             reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
@@ -465,7 +483,10 @@
             <double*>addr_featureArray, <double*>addr_chi, <double*>addr_output,
             reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
             chiArr.shape[0], radem.shape[2], scalingTerm, kernelOrder)
     else:
         raise ValueError("Incorrect data types supplied.")
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered while performing FHT RF generation.")
+
+    if fitIntercept:
+        outputArray[:,0] = beta_
```

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 cimport numpy as np
 cimport cython
 from libc cimport stdint
 import cupy as cp
 from libc.stdint cimport uintptr_t
 import math
 from libc.stdint cimport int8_t, int32_t
+from libcpp cimport bool
 
 
 
 cdef extern from "rbf_ops/rbf_ops.h" nogil:
     const char *RBFFeatureGen[T](T cArray[], int8_t *radem,
                 T chiArr[], double *outputArray,
                 double rbfNormConstant,
@@ -34,15 +35,16 @@
                 int dim1, int numLengthscales, int numFreqs,
                 double rbfNormConstant);
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cudaRBFFeatureGen(inputArray, outputArray, radem,
-                chiArr, double betaHparam, int numThreads):
+                chiArr, double betaHparam, int numThreads,
+                fitIntercept = False):
     """Wraps RBFFeatureGen from double_specialized_ops and uses
     it to to generate random features for an RBF kernel (this same routine
     can also be used for Matern, ARD and MiniARD). This wrapper performs all
     of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
         inputArray (cp.ndarray): The array on which the SORF transform will be performed.
@@ -52,14 +54,16 @@
             be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
         radem (cp.ndarray): A stack of diagonal matrices of type int8_t
             of shape (3 x D x C).
         chiArr (cp.ndarray): A matrix of shape (numFreqs).
         betaHparam (double): The amplitude hyperparameter.
         numThreads (int): Not currently used, accepted only to preserve
             shared interface with CPU functions.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
     cdef float logdim
     cdef double rbfNormConstant
@@ -92,15 +96,18 @@
         raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
 
     logdim = np.log2(inputArray.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
         raise ValueError("dim2 of the input array to RBF feature gen functions "
                             "must be a power of 2 >= 2.")
 
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
+    if fitIntercept:
+        rbfNormConstant = betaHparam * np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+    else:
+        rbfNormConstant = betaHparam * np.sqrt(2 / <double>chiArr.shape[0])
 
     if inputArray.dtype == "float32" and outputArray.dtype == "float64" and \
             chiArr.dtype == "float32":
         errCode = RBFFeatureGen[float](<float*>addr_input, <int8_t*>addr_radem,
                 <float*>addr_chi, <double*>addr_output, rbfNormConstant,
                 inputArray.shape[0], inputArray.shape[1],
                 inputArray.shape[2], chiArr.shape[0]);
@@ -111,23 +118,24 @@
                 inputArray.shape[0], inputArray.shape[1],
                 inputArray.shape[2], chiArr.shape[0]);
     else:
         raise ValueError("The input and chiArr arrays are of inconsistent types.")
 
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered in CudaRBFFeatureGen.")
-
+    if fitIntercept:
+        outputArray[:,0] = betaHparam
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def cudaRBFGrad(inputArray, outputArray, radem,
                 chiArr, double betaHparam, double sigmaHparam,
-                int numThreads):
+                int numThreads, bool fitIntercept = False):
     """Wraps RBFFeatureGen and uses
     it to to generate random features for an RBF kernel
     together with the gradient. This wrapper performs all
     of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
         inputArray (cp.ndarray): The array on which the SORF transform will be performed.
@@ -137,14 +145,16 @@
         radem (cp.ndarray): A stack of diagonal matrices of type int8_t
             of shape (3 x D x C).
         chiArr (cp.ndarray): A matrix of shape (numFreqs).
         betaHparam (double): The amplitude hyperparameter.
         sigmaHparam (double): The sigma hyperparameter.
         numThreads (int): Not currently used, accepted only to preserve
             shared interface with CPU functions.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
 
     Returns:
         gradient (cp.ndarray): An array containing the gradient values.
     """
@@ -183,15 +193,18 @@
         raise ValueError("radem must be of type int8.")
     logdim = np.log2(inputArray.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
         raise ValueError("dim2 of the input array to RBF feature gen functions "
                             "must be a power of 2 >= 2.")
 
 
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
+    if fitIntercept:
+        rbfNormConstant = betaHparam * np.sqrt(2.0 / (<double>chiArr.shape[0] - 0.5))
+    else:
+        rbfNormConstant = betaHparam * np.sqrt(2 / <double>chiArr.shape[0])
 
     if inputArray.dtype == "float32" and outputArray.dtype == "float64" and \
             chiArr.dtype == "float32":
         errCode = RBFFeatureGrad[float](<float*>addr_input, <int8_t*>addr_radem,
                 <float*>addr_chi, <double*>addr_output, <double*>addr_gradient,
                 rbfNormConstant, sigmaHparam,
                 inputArray.shape[0], inputArray.shape[1],
@@ -203,108 +216,120 @@
                 rbfNormConstant, sigmaHparam,
                 inputArray.shape[0], inputArray.shape[1],
                 inputArray.shape[2], chiArr.shape[0]);
     else:    
         raise ValueError("The input and chiArr arrays are of inconsistent types.")
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered in doubleCudaRBFFeatureGen.")
+    if fitIntercept:
+        outputArray[:,0] = betaHparam
+        gradient[:,0] = 0
     return gradient
 
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def cudaMiniARDGrad(inputX, randomFeats, precompWeights,
-                sigmaMap, sigmaVals, double betaHparam, int numThreads):
+def cudaMiniARDGrad(inputX, outputArray, precompWeights,
+                sigmaMap, sigmaVals, double betaHparam, int numThreads,
+                bool fitIntercept = False):
     """Performs gradient calculations for the MiniARD kernel, using
     pregenerated features and precomputed weights.
 
     Args:
         inputX (np.ndarray): The original input data.
-        randomFeats (np.ndarray): The random features generated using the FHT-
+        outputArray (np.ndarray): The random features generated using the FHT-
             based procedure.
         precompWeights (np.ndarray): The FHT-rf gen procedure applied to an
             identity matrix.
         sigmaMap (np.ndarray): An array mapping which lengthscales correspond
             to which positions in the input.
         sigmaVals (cp.ndarray): The lengthscale values, in an array of the same
             dimensionality as the input.
         betaHparam (double): The amplitude hyperparameter.
         numThreads (int): Number of threads to run.
+        fitIntercept (bool): Whether to fit a y-intercept (in this case,
+            the first random feature generated should be set to 1).
 
     Raises:
         ValueError: A ValueError is raised if unexpected or unacceptable inputs
             are supplied.
 
     Returns:
         gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
             the gradient w/r/t sigma.
     """
     cdef const char *errCode
     cdef float logdim
     cdef double rbfNormConstant
     cdef int numLengthscales = sigmaMap.max() + 1
-    gradient = cp.zeros((randomFeats.shape[0],
-                        randomFeats.shape[1], numLengthscales))
+    gradient = cp.zeros((outputArray.shape[0],
+                        outputArray.shape[1], numLengthscales))
 
-    if len(inputX.shape) != 2 or len(randomFeats.shape) != 2 or \
+    if len(inputX.shape) != 2 or len(outputArray.shape) != 2 or \
             len(precompWeights.shape) != 2 or len(sigmaMap.shape) != 1:
         raise ValueError("The input arrays to a wrapped RBF feature gen function have incorrect "
                 "shapes.")
 
     if inputX.shape[0] == 0 or inputX.shape[1] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if inputX.shape[0] != randomFeats.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
+    if inputX.shape[0] != outputArray.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
         raise ValueError("Incorrect array dims passed to a wrapped RBF "
                     "feature gen function.")
-    if randomFeats.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
+    if outputArray.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
             precompWeights.shape[1] or sigmaVals.shape[0] != sigmaMap.shape[0]:
         raise ValueError("Incorrect array dims passed to a wrapped RBF "
                     "feature gen function.")
 
-    if not inputX.flags["C_CONTIGUOUS"] or not randomFeats.flags["C_CONTIGUOUS"] or not \
+    if not inputX.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"] or not \
             precompWeights.flags["C_CONTIGUOUS"] or not sigmaMap.flags["C_CONTIGUOUS"] or \
             not sigmaVals.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
                 "C contiguous.")
 
 
     cdef uintptr_t addr_input = inputX.data.ptr
-    cdef uintptr_t addr_random_feats = randomFeats.data.ptr
+    cdef uintptr_t addr_random_feats = outputArray.data.ptr
 
     cdef uintptr_t addr_sigma_map = sigmaMap.data.ptr
     cdef int32_t *sigmaMap_ptr = <int32_t*>addr_sigma_map
     cdef uintptr_t addr_sigma_vals = sigmaVals.data.ptr
 
     cdef uintptr_t addr_grad = gradient.data.ptr
     cdef uintptr_t addr_precomp_weights = precompWeights.data.ptr
 
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>precompWeights.shape[0])
+    if fitIntercept:
+        rbfNormConstant = betaHparam * np.sqrt(2.0 / (<double>precompWeights.shape[0] - 0.5))
+    else:
+        rbfNormConstant = betaHparam * np.sqrt(2 / <double>precompWeights.shape[0])
 
     if inputX.dtype == "float32" and precompWeights.dtype == "float32" and \
-            randomFeats.dtype == "float64" and sigmaMap.dtype == "int32" and \
+            outputArray.dtype == "float64" and sigmaMap.dtype == "int32" and \
             sigmaVals.dtype == "float64":
         errCode = ardCudaGrad[float](<float*>addr_input, <double*>addr_random_feats,
                 <float*>addr_precomp_weights, <int32_t*>addr_sigma_map,
                 <double*>addr_sigma_vals,
                 <double*>addr_grad, inputX.shape[0], inputX.shape[1],
                 gradient.shape[2], precompWeights.shape[0],
                 rbfNormConstant)
 
     elif inputX.dtype == "float64" and precompWeights.dtype == "float64" and \
-            randomFeats.dtype == "float64" and sigmaMap.dtype == "int32" and \
+            outputArray.dtype == "float64" and sigmaMap.dtype == "int32" and \
             sigmaVals.dtype == "float64":
         errCode = ardCudaGrad[double](<double*>addr_input, <double*>addr_random_feats,
                 <double*>addr_precomp_weights, <int32_t*>addr_sigma_map,
                 <double*>addr_sigma_vals,
                 <double*>addr_grad, inputX.shape[0], inputX.shape[1],
                 gradient.shape[2], precompWeights.shape[0],
                 rbfNormConstant)
     else:
         raise ValueError("The input arrays to a wrapped RBF feature gen function have incorrect "
                 "types.")
 
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered in RBF feature gen.")
+    if fitIntercept:
+        outputArray[:,0] = betaHparam
+        gradient[:,0,:] = 0
     return gradient
```

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.2.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/regression_baseclass.py` & `xGPR-0.1.2.0/xGPR/regression_baseclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,14 +327,17 @@
                 xbatch = xbatch.astype(np.float32)
             ybatch = ybatch * dataset.get_ystd() + dataset.get_ymean()
             np.save(xfile, xbatch)
             np.save(yfile, ybatch)
             xfiles.append(xfile)
             yfiles.append(yfile)
             max_chunk_size = max(max_chunk_size, xbatch.shape[0])
+            if self.device == "gpu":
+                mempool = cp.get_default_memory_pool()
+                mempool.free_all_blocks()
 
         tuning_dataset = build_offline_fixed_vector_dataset(xfiles,
                             yfiles, chunk_size = max_chunk_size,
                             skip_safety_checks = True)
         tuning_dataset.pretransformed = True
         tuning_dataset.parent_xdim = dataset.get_xdim()
```

### Comparing `xGPR-0.1.1.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py` & `xGPR-0.1.2.0/xGPR/scoring_toolkit/approximate_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/scoring_toolkit/cho_solvers.py` & `xGPR-0.1.2.0/xGPR/scoring_toolkit/cho_solvers.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/scoring_toolkit/exact_nmll_calcs.py` & `xGPR-0.1.2.0/xGPR/scoring_toolkit/exact_nmll_calcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,24 @@
     y_trans_y = 0.0
     if dataset.pretransformed:
         for xfeatures, ydata in dataset.get_chunked_data():
             z_trans_y += xfeatures.T @ ydata
             z_trans_z += xfeatures.T @ xfeatures
             y_trans_y += ydata.T @ ydata
     else:
-        for xdata, ydata in dataset.get_chunked_data():
+        for i, (xdata, ydata) in enumerate(dataset.get_chunked_data()):
             xfeatures = kernel.transform_x(xdata)
             z_trans_y += xfeatures.T @ ydata
             z_trans_z += xfeatures.T @ xfeatures
             y_trans_y += ydata.T @ ydata
+            if i % 2 == 0:
+                if kernel.device == "gpu":
+                    mempool = cp.get_default_memory_pool()
+                    mempool.free_all_blocks()
+                
     return z_trans_z, z_trans_y, float(y_trans_y)
 
 
 
 def direct_weight_calc(chol_z_trans_z, z_trans_y, kernel):
     """Calculates the cholesky decomposition of (z^T z + lambda)^-1
     and then uses this to calculate the weights as (z^T z + lambda)^-1 z^T y.
```

### Comparing `xGPR-0.1.1.6/xGPR/scoring_toolkit/nmll_gradient_tools.py` & `xGPR-0.1.2.0/xGPR/scoring_toolkit/nmll_gradient_tools.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/scoring_toolkit/probe_generators.py` & `xGPR-0.1.2.0/xGPR/scoring_toolkit/probe_generators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/static_layers/fast_conv.py` & `xGPR-0.1.2.0/xGPR/static_layers/fast_conv.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         f_per_kernel (int): The number of features per convolution kernel
             width.
         zero_arr: A convenience reference to either np.zeros or cp.zeros,
             depending on device.
     """
 
     def __init__(self, seq_width, device = "cpu", random_seed = 123,
-            conv_width = [9], num_features = 512, mode = "maxpool"):
+            conv_width = [9], num_features = 512):
         """Constructor for the FastConv1d class.
 
         Args:
             seq_width (int): The anticipated width (number of features) of
                 each input sequence / series.
             device (str): Must be one of ['cpu', 'gpu']. Indicates the current
                 device for the feature extractor.
@@ -57,39 +57,32 @@
                 > 1, the num_features must be an integer multiple of
                 the length of the list. num_features / len(conv_width)
                 features are generated for each convolution kernel
                 width.
             num_features (int): The number of random features to generate.
                 More = improved performance but slower feature extraction
                 and slower model training. Defaults to 512.
-            mode (str): One of 'maxpool', 'maxpool_loc'.
-                'maxpool_loc' adjusts the result based on global mean pooling.
 
         Raises:
             ValueError: If an unrecognized kernel type or other invalid
                 input is supplied.
         """
         self.zero_arr = np.zeros
         if len(conv_width) > 3:
             raise ValueError("Currently only up to three conv_widths "
                     "are generated at one time.")
         if num_features % len(conv_width) != 0:
             raise ValueError("The number of features for the FastConv1d "
                     "must be an integer multiple of the number of "
                     "desired convolution widths.")
 
-        if mode == "maxpool_loc":
-            subtract_mean = True
-        else:
-            subtract_mean = False
-
         self.f_per_kernel = int(num_features / len(conv_width))
         self.conv_kernel = [FHTMaxpoolConv1dFeatureExtractor(seq_width,
                             self.f_per_kernel, random_seed, device = device,
-                            conv_width = c, subtract_mean = subtract_mean) for c in conv_width]
+                            conv_width = c) for c in conv_width]
         self.device = device
 
         self.seq_width = seq_width
         self.num_features = num_features
```

### Comparing `xGPR-0.1.1.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py` & `xGPR-0.1.2.0/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py` & `xGPR-0.1.2.0/xGPR/tuning_toolkit/direct_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/tuning_toolkit/hparam_scoring.py` & `xGPR-0.1.2.0/xGPR/tuning_toolkit/hparam_scoring.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/visualization_tools/kernel_xpca.py` & `xGPR-0.1.2.0/xGPR/visualization_tools/kernel_xpca.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR/xGP_Regression.py` & `xGPR-0.1.2.0/xGPR/xGP_Regression.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.6/xGPR.egg-info/PKG-INFO` & `xGPR-0.1.2.0/xGPR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.1.6
+Version: 0.1.2.0
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.1.6/xGPR.egg-info/SOURCES.txt` & `xGPR-0.1.2.0/xGPR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

