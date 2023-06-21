# Comparing `tmp/antspynet-0.2.1.tar.gz` & `tmp/antspynet-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspynet-0.2.1.tar", last modified: Thu Feb 23 16:20:14 2023, max compression
+gzip compressed data, was "antspynet-0.2.2.tar", last modified: Wed Jun 21 17:16:41 2023, max compression
```

## Comparing `antspynet-0.2.1.tar` & `antspynet-0.2.2.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-02-23 16:20:14.382554 antspynet-0.2.1/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-01-13 14:27:03.000000 antspynet-0.2.1/LICENSE.md
--rw-r--r--   0 stnava     (501) staff       (20)     8181 2023-02-23 16:20:14.382372 antspynet-0.2.1/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     7760 2023-01-29 14:38:52.000000 antspynet-0.2.1/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-02-23 16:20:14.359011 antspynet-0.2.1/antspynet/
--rw-r--r--   0 stnava     (501) staff       (20)      115 2019-07-02 00:37:42.000000 antspynet-0.2.1/antspynet/__init__.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-02-23 16:20:14.369782 antspynet-0.2.1/antspynet/architectures/
--rw-r--r--   0 stnava     (501) staff       (20)     2974 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/architectures/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)    14057 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_alexnet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     2090 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_autoencoder_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8296 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_convolutional_autoencoder_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     3121 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_custom_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    36597 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/architectures/create_custom_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    14211 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_cycle_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    19564 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_deep_back_projection_network_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    10368 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_deep_convolutional_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8187 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_deep_denoise_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6197 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     1704 2022-10-06 18:43:49.000000 antspynet-0.2.1/antspynet/architectures/create_dense_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    13539 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_densenet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    19534 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_denseunet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6163 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_expanded_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     5198 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_image_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    12707 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_improved_wasserstein_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    13493 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/architectures/create_partial_convolution_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    17281 2021-06-11 18:37:29.000000 antspynet-0.2.1/antspynet/architectures/create_resnet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8637 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_resnet_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    27712 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_resunet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     7749 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    16664 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_super_resolution_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    21492 2022-01-20 13:35:28.000000 antspynet-0.2.1/antspynet/architectures/create_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6447 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_vanilla_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    11244 2023-01-29 14:38:52.000000 antspynet-0.2.1/antspynet/architectures/create_vgg_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    11233 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_wasserstein_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    15261 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/architectures/create_wide_resnet_model.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-02-23 16:20:14.381996 antspynet-0.2.1/antspynet/utilities/
--rw-r--r--   0 stnava     (501) staff       (20)     4055 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)     8814 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/utilities/attention_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     5082 2022-10-06 18:43:49.000000 antspynet-0.2.1/antspynet/utilities/brain_age.py
--rw-r--r--   0 stnava     (501) staff       (20)    10772 2022-10-06 18:43:49.000000 antspynet-0.2.1/antspynet/utilities/brain_extraction.py
--rw-r--r--   0 stnava     (501) staff       (20)     8303 2022-10-06 18:43:49.000000 antspynet-0.2.1/antspynet/utilities/claustrum_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     8886 2021-05-12 17:54:13.000000 antspynet-0.2.1/antspynet/utilities/cortical_thickness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3156 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/cropping_and_padding_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     1002 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/utilities/custom_activation_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)    10618 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/custom_convolution_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)     8323 2023-01-29 14:38:52.000000 antspynet-0.2.1/antspynet/utilities/custom_metrics.py
--rw-r--r--   0 stnava     (501) staff       (20)     5826 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/utilities/custom_normalization_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)    12823 2021-12-13 15:03:29.000000 antspynet-0.2.1/antspynet/utilities/data_augmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     6820 2022-10-06 18:43:49.000000 antspynet-0.2.1/antspynet/utilities/deep_atropos.py
--rw-r--r--   0 stnava     (501) staff       (20)     8009 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/utilities/deep_embedded_clustering_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    40400 2022-03-28 17:21:25.000000 antspynet-0.2.1/antspynet/utilities/deep_flash.py
--rw-r--r--   0 stnava     (501) staff       (20)     1688 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/utilities/denseunet_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    20746 2021-05-19 10:17:59.000000 antspynet-0.2.1/antspynet/utilities/desikan_killiany_tourville_labeling.py
--rw-r--r--   0 stnava     (501) staff       (20)     9993 2023-02-23 16:10:49.000000 antspynet-0.2.1/antspynet/utilities/extract_image_patches.py
--rw-r--r--   0 stnava     (501) staff       (20)     5021 2022-10-06 18:43:50.000000 antspynet-0.2.1/antspynet/utilities/get_antsxnet_data.py
--rw-r--r--   0 stnava     (501) staff       (20)    16456 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/get_pretrained_network.py
--rw-r--r--   0 stnava     (501) staff       (20)     8601 2021-11-04 16:22:25.000000 antspynet-0.2.1/antspynet/utilities/hippmapp3r_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     4847 2021-03-14 11:58:14.000000 antspynet-0.2.1/antspynet/utilities/histogram_warp_image_intensities.py
--rw-r--r--   0 stnava     (501) staff       (20)    19508 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/histology.py
--rw-r--r--   0 stnava     (501) staff       (20)     4969 2021-06-11 14:16:25.000000 antspynet-0.2.1/antspynet/utilities/hypothalamus_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)    11265 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/inpainting.py
--rw-r--r--   0 stnava     (501) staff       (20)    18789 2021-10-08 13:19:44.000000 antspynet-0.2.1/antspynet/utilities/lung_extraction.py
--rw-r--r--   0 stnava     (501) staff       (20)     6562 2021-10-08 13:19:44.000000 antspynet-0.2.1/antspynet/utilities/lung_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)    12055 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/utilities/mixture_density_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     1606 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/utilities/mri_super_resolution.py
--rw-r--r--   0 stnava     (501) staff       (20)    18169 2020-10-20 16:09:02.000000 antspynet-0.2.1/antspynet/utilities/neural_style_transfer.py
--rw-r--r--   0 stnava     (501) staff       (20)     8722 2021-10-08 13:19:44.000000 antspynet-0.2.1/antspynet/utilities/preprocess_image.py
--rw-r--r--   0 stnava     (501) staff       (20)    17035 2022-01-20 13:35:28.000000 antspynet-0.2.1/antspynet/utilities/quality_assessment.py
--rw-r--r--   0 stnava     (501) staff       (20)    11102 2021-12-13 15:03:29.000000 antspynet-0.2.1/antspynet/utilities/randomly_transform_image_data.py
--rw-r--r--   0 stnava     (501) staff       (20)    11224 2022-01-20 13:35:28.000000 antspynet-0.2.1/antspynet/utilities/reconstruct_image_from_patches.py
--rw-r--r--   0 stnava     (501) staff       (20)     2856 2023-01-29 14:38:52.000000 antspynet-0.2.1/antspynet/utilities/regression_match_image.py
--rw-r--r--   0 stnava     (501) staff       (20)    11048 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/resample_tensor_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     2518 2023-01-29 14:38:52.000000 antspynet-0.2.1/antspynet/utilities/simulate_bias_field.py
--rw-r--r--   0 stnava     (501) staff       (20)    14538 2020-12-08 17:22:14.000000 antspynet-0.2.1/antspynet/utilities/spatial_transformer_network_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    11177 2021-03-31 13:36:08.000000 antspynet-0.2.1/antspynet/utilities/super_resolution_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     8426 2023-02-23 16:04:54.000000 antspynet-0.2.1/antspynet/utilities/ukbb.py
--rw-r--r--   0 stnava     (501) staff       (20)     2871 2021-05-18 23:52:34.000000 antspynet-0.2.1/antspynet/utilities/unet_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    47089 2023-01-29 14:38:52.000000 antspynet-0.2.1/antspynet/utilities/white_matter_hyperintensity_segmentation.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-02-23 16:20:14.360327 antspynet-0.2.1/antspynet.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)     8181 2023-02-23 16:20:14.000000 antspynet-0.2.1/antspynet.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     3732 2023-02-23 16:20:14.000000 antspynet-0.2.1/antspynet.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-02-23 16:20:14.000000 antspynet-0.2.1/antspynet.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2022-10-19 12:51:12.000000 antspynet-0.2.1/antspynet.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)       99 2023-02-23 16:20:14.000000 antspynet-0.2.1/antspynet.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)       54 2023-02-23 16:20:14.000000 antspynet-0.2.1/antspynet.egg-info/top_level.txt
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-02-23 16:20:14.382603 antspynet-0.2.1/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      791 2023-02-23 16:19:21.000000 antspynet-0.2.1/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.249667 antspynet-0.2.2/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-06-06 13:36:51.000000 antspynet-0.2.2/LICENSE.md
+-rw-r--r--   0 stnava     (501) staff       (20)     8207 2023-06-21 17:16:41.249465 antspynet-0.2.2/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     7786 2023-06-21 17:14:39.000000 antspynet-0.2.2/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.235776 antspynet-0.2.2/antspynet/
+-rw-r--r--   0 stnava     (501) staff       (20)      115 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/__init__.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.242016 antspynet-0.2.2/antspynet/architectures/
+-rw-r--r--   0 stnava     (501) staff       (20)     3120 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)    14057 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_alexnet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2090 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_autoencoder_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8296 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_convolutional_autoencoder_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3121 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_custom_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    36597 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_custom_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    14211 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_cycle_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    19564 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_deep_back_projection_network_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    10368 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_deep_convolutional_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8187 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_deep_denoise_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6197 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1704 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_dense_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    13539 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_densenet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    19534 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_denseunet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    15888 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_diffusion_probabilistic_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6163 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_expanded_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     5198 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_image_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    12707 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_improved_wasserstein_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    13493 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_partial_convolution_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    17281 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_resnet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8637 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_resnet_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    27712 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_resunet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     7749 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    16664 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_super_resolution_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    21492 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6447 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_vanilla_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11244 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_vgg_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11233 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_wasserstein_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    15261 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_wide_resnet_model.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.249170 antspynet-0.2.2/antspynet/utilities/
+-rw-r--r--   0 stnava     (501) staff       (20)     4284 2023-06-09 14:56:59.000000 antspynet-0.2.2/antspynet/utilities/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8814 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/attention_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     5082 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/brain_age.py
+-rw-r--r--   0 stnava     (501) staff       (20)    10772 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/brain_extraction.py
+-rw-r--r--   0 stnava     (501) staff       (20)    17672 2023-06-21 17:14:39.000000 antspynet-0.2.2/antspynet/utilities/cerebellum_morphology.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8303 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/claustrum_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8886 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/cortical_thickness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3104 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/cropping_and_padding_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1002 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/custom_activation_layers.py
+-rw-r--r--   0 stnava     (501) staff       (20)    10664 2023-06-06 13:37:10.000000 antspynet-0.2.2/antspynet/utilities/custom_convolution_layers.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8323 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/custom_metrics.py
+-rw-r--r--   0 stnava     (501) staff       (20)     5826 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/custom_normalization_layers.py
+-rw-r--r--   0 stnava     (501) staff       (20)    13137 2023-06-09 14:56:59.000000 antspynet-0.2.2/antspynet/utilities/data_augmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6820 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/deep_atropos.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8009 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/deep_embedded_clustering_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    40348 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/deep_flash.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1688 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/denseunet_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    20746 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/desikan_killiany_tourville_labeling.py
+-rw-r--r--   0 stnava     (501) staff       (20)     9997 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/extract_image_patches.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6901 2023-06-09 14:56:59.000000 antspynet-0.2.2/antspynet/utilities/gaussian_diffusion_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     5812 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/get_antsxnet_data.py
+-rw-r--r--   0 stnava     (501) staff       (20)    17128 2023-06-21 17:14:39.000000 antspynet-0.2.2/antspynet/utilities/get_pretrained_network.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8601 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/hippmapp3r_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4847 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/histogram_warp_image_intensities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    29323 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/histology.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4969 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/hypothalamus_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11285 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/inpainting.py
+-rw-r--r--   0 stnava     (501) staff       (20)    18785 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/lung_extraction.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6558 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/lung_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)    12055 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/mixture_density_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1606 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/mri_super_resolution.py
+-rw-r--r--   0 stnava     (501) staff       (20)    18169 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/neural_style_transfer.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8722 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/preprocess_image.py
+-rw-r--r--   0 stnava     (501) staff       (20)    17035 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/quality_assessment.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11102 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/randomly_transform_image_data.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11224 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/reconstruct_image_from_patches.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2856 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/regression_match_image.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11048 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/resample_tensor_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2518 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/simulate_bias_field.py
+-rw-r--r--   0 stnava     (501) staff       (20)    14538 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/spatial_transformer_network_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11177 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/super_resolution_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8426 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/ukbb.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2871 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/unet_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    46891 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/white_matter_hyperintensity_segmentation.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.236753 antspynet-0.2.2/antspynet.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)     8207 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     3898 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-06 13:37:14.000000 antspynet-0.2.2/antspynet.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)       99 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       54 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/top_level.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-06-21 17:16:41.249716 antspynet-0.2.2/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      791 2023-06-21 17:15:26.000000 antspynet-0.2.2/setup.py
```

### Comparing `antspynet-0.2.1/LICENSE.md` & `antspynet-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/PKG-INFO` & `antspynet-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: antspynet
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of deep learning architectures ported to the python language and tools for basic medical image processing.
 Home-page: https://github.com/ANTsX/ANTsPyNet
 Author: Nicholas J. Tustison and Brian B. Avants and Nick Cullen
 Author-email: ntustison@gmail.com
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.md
 
-[![Build Status](https://travis-ci.org/ANTsX/ANTsPyNet.svg?branch=master)](https://travis-ci.org/ANTsX/ANTsPyNet)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
 
 # ANTsPyNet
 
 A collection of deep learning architectures and applications ported to the python language and tools for basic medical image processing. Based on `keras` and `tensorflow` with cross-compatibility with our R analog [ANTsRNet](https://github.com/ANTsX/ANTsRNet/).
 
 Documentation page [https://antsx.github.io/ANTsPyNet/](https://antsx.github.io/ANTsPyNet/).
@@ -88,14 +88,15 @@
 * [HippMapp3r hippocampal segmentation](https://pubmed.ncbi.nlm.nih.gov/31609046/)
 * [Sysu white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/30125711/)
 * [HyperMapp3r white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/35088930/)
 * [Hypothalamus segmentation](https://pubmed.ncbi.nlm.nih.gov/32853816/)
 * [Claustrum segmentation](https://arxiv.org/abs/2008.03465)
 * [Deep Flash](https://www.medrxiv.org/content/10.1101/2023.01.17.23284693v1)
 * Desikan-Killiany-Tourville cortical labeling
+* Cerebellum segmentation, parcellation, and thickness
 * Lung extraction
     * [Proton](https://www.ncbi.nlm.nih.gov/pubmed/30195415)
     * CT
 * [Functional lung segmentation](https://www.medrxiv.org/content/10.1101/2021.03.04.21252588v2)
 * [Neural style transfer](https://arxiv.org/abs/1508.06576)
 * Image quality assessment
     * [TID2013](https://www.sciencedirect.com/science/article/pii/S0923596514001490)
```

### Comparing `antspynet-0.2.1/README.md` & `antspynet-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://travis-ci.org/ANTsX/ANTsPyNet.svg?branch=master)](https://travis-ci.org/ANTsX/ANTsPyNet)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
 
 # ANTsPyNet
 
 A collection of deep learning architectures and applications ported to the python language and tools for basic medical image processing. Based on `keras` and `tensorflow` with cross-compatibility with our R analog [ANTsRNet](https://github.com/ANTsX/ANTsRNet/).
 
 Documentation page [https://antsx.github.io/ANTsPyNet/](https://antsx.github.io/ANTsPyNet/).
@@ -78,14 +78,15 @@
 * [HippMapp3r hippocampal segmentation](https://pubmed.ncbi.nlm.nih.gov/31609046/)
 * [Sysu white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/30125711/)
 * [HyperMapp3r white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/35088930/)
 * [Hypothalamus segmentation](https://pubmed.ncbi.nlm.nih.gov/32853816/)
 * [Claustrum segmentation](https://arxiv.org/abs/2008.03465)
 * [Deep Flash](https://www.medrxiv.org/content/10.1101/2023.01.17.23284693v1)
 * Desikan-Killiany-Tourville cortical labeling
+* Cerebellum segmentation, parcellation, and thickness
 * Lung extraction
     * [Proton](https://www.ncbi.nlm.nih.gov/pubmed/30195415)
     * CT
 * [Functional lung segmentation](https://www.medrxiv.org/content/10.1101/2021.03.04.21252588v2)
 * [Neural style transfer](https://arxiv.org/abs/1508.06576)
 * Image quality assessment
     * [TID2013](https://www.sciencedirect.com/science/article/pii/S0923596514001490)
```

### Comparing `antspynet-0.2.1/antspynet/architectures/__init__.py` & `antspynet-0.2.2/antspynet/architectures/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .create_denseunet_model import create_denseunet_model_2d, create_denseunet_model_3d
 from .create_custom_unet_model import create_nobrainer_unet_model_3d
 from .create_custom_unet_model import create_hippmapp3r_unet_model_3d
 from .create_custom_unet_model import create_hypermapp3r_unet_model_3d
 from .create_custom_unet_model import create_sysu_media_unet_model_2d
 from .create_custom_unet_model import create_hypothalamus_unet_model_3d
 from .create_partial_convolution_unet_model import create_partial_convolution_unet_model_2d, create_partial_convolution_unet_model_3d
+from .create_diffusion_probabilistic_unet_model import create_diffusion_probabilistic_unet_model_2d, create_diffusion_probabilistic_unet_model_3d
 
 from .create_custom_model import create_simple_fully_convolutional_network_model_3d
 
 from .create_vanilla_gan_model import VanillaGanModel
 from .create_deep_convolutional_gan_model import DeepConvolutionalGanModel
 from .create_wasserstein_gan_model import WassersteinGanModel
 from .create_improved_wasserstein_gan_model import ImprovedWassersteinGanModel
```

### Comparing `antspynet-0.2.1/antspynet/architectures/create_alexnet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_alexnet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_autoencoder_model.py` & `antspynet-0.2.2/antspynet/architectures/create_autoencoder_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_convolutional_autoencoder_model.py` & `antspynet-0.2.2/antspynet/architectures/create_convolutional_autoencoder_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_custom_model.py` & `antspynet-0.2.2/antspynet/architectures/create_custom_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_custom_unet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_custom_unet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_cycle_gan_model.py` & `antspynet-0.2.2/antspynet/architectures/create_cycle_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_deep_back_projection_network_model.py` & `antspynet-0.2.2/antspynet/architectures/create_deep_back_projection_network_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_deep_convolutional_gan_model.py` & `antspynet-0.2.2/antspynet/architectures/create_deep_convolutional_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_deep_denoise_super_resolution_model.py` & `antspynet-0.2.2/antspynet/architectures/create_deep_denoise_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py` & `antspynet-0.2.2/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_dense_model.py` & `antspynet-0.2.2/antspynet/architectures/create_dense_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_densenet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_densenet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_denseunet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_denseunet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_expanded_super_resolution_model.py` & `antspynet-0.2.2/antspynet/architectures/create_expanded_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_image_super_resolution_model.py` & `antspynet-0.2.2/antspynet/architectures/create_image_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_improved_wasserstein_gan_model.py` & `antspynet-0.2.2/antspynet/architectures/create_improved_wasserstein_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_partial_convolution_unet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_partial_convolution_unet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_resnet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_resnet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_resnet_super_resolution_model.py` & `antspynet-0.2.2/antspynet/architectures/create_resnet_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_resunet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_resunet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py` & `antspynet-0.2.2/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_super_resolution_gan_model.py` & `antspynet-0.2.2/antspynet/architectures/create_super_resolution_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_unet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_unet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_vanilla_gan_model.py` & `antspynet-0.2.2/antspynet/architectures/create_vanilla_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_vgg_model.py` & `antspynet-0.2.2/antspynet/architectures/create_vgg_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_wasserstein_gan_model.py` & `antspynet-0.2.2/antspynet/architectures/create_wasserstein_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/architectures/create_wide_resnet_model.py` & `antspynet-0.2.2/antspynet/architectures/create_wide_resnet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/__init__.py` & `antspynet-0.2.2/antspynet/utilities/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
 from .custom_normalization_layers import InstanceNormalization
 
 from .custom_activation_layers import LogSoftmax
 
 from .custom_convolution_layers import PartialConv2D, PartialConv3D
 
+from .gaussian_diffusion_utilities import GaussianDiffusion
+
 from .cropping_and_padding_utilities import crop_image_center
 from .cropping_and_padding_utilities import pad_or_crop_image_to_size
 from .cropping_and_padding_utilities import pad_image_by_factor
 
 from .histogram_warp_image_intensities import histogram_warp_image_intensities
 from .simulate_bias_field import simulate_bias_field
 
@@ -60,26 +62,29 @@
 from .brain_extraction import brain_extraction
 from .inpainting import whole_head_inpainting
 from .cortical_thickness import cortical_thickness
 from .cortical_thickness import longitudinal_cortical_thickness
 from .histology import arterial_lesion_segmentation
 from .histology import allen_ex5_brain_extraction
 from .histology import allen_histology_brain_mask
+from .histology import allen_histology_cerebellum_mask
 from .histology import allen_histology_hemispherical_coronal_mask
+from .histology import allen_histology_super_resolution
 from .lung_extraction import lung_extraction
 from .white_matter_hyperintensity_segmentation import sysu_media_wmh_segmentation
 from .white_matter_hyperintensity_segmentation import ew_david
 from .white_matter_hyperintensity_segmentation import hypermapp3r_segmentation
 from .claustrum_segmentation import claustrum_segmentation
 from .hypothalamus_segmentation import hypothalamus_segmentation
 from .hippmapp3r_segmentation import hippmapp3r_segmentation
 from .deep_flash import deep_flash
 from .deep_flash import deep_flash_deprecated
 from .deep_atropos import deep_atropos
 from .desikan_killiany_tourville_labeling import desikan_killiany_tourville_labeling
+from .cerebellum_morphology import cerebellum_morphology
 from .brain_age import brain_age
 from .mri_super_resolution import mri_super_resolution
 from .quality_assessment import tid_neural_image_assessment
 from .quality_assessment import random_mask
 from .lung_segmentation import el_bicho
 
 from .neural_style_transfer import neural_style_transfer
```

### Comparing `antspynet-0.2.1/antspynet/utilities/attention_utilities.py` & `antspynet-0.2.2/antspynet/utilities/attention_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/brain_age.py` & `antspynet-0.2.2/antspynet/utilities/brain_age.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/brain_extraction.py` & `antspynet-0.2.2/antspynet/utilities/brain_extraction.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/claustrum_segmentation.py` & `antspynet-0.2.2/antspynet/utilities/claustrum_segmentation.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/cortical_thickness.py` & `antspynet-0.2.2/antspynet/utilities/cortical_thickness.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/cropping_and_padding_utilities.py` & `antspynet-0.2.2/antspynet/utilities/cropping_and_padding_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     Crop the center of an image.
 
     Arguments
     ---------
     image : ANTsImage
         Input image
 
-    crop_size: n-D tuple (depending on dimensionality).
+    crop_size: n-D tuple
         Width, height, depth (if 3-D), and time (if 4-D) of crop region.
 
     Returns
     -------
-    A list (or array) of patches.
+    ANTs image.
 
     Example
     -------
     >>> import ants
     >>> image = ants.image_read(ants.get_ants_data('r16'))
     >>> cropped_image = crop_image_center(image, crop_size=(64, 64))
     """
@@ -56,15 +56,15 @@
         Input image
 
     factor: scalar or n-D tuple
         Padding factor
 
     Returns
     -------
-    A padded image
+    ANTs image.
 
     Example
     -------
     >>> import ants
     >>> image = ants.image_read(ants.get_ants_data('r16'))
     >>> padded_image = pad_image_by_factor(image, factor=4)
     """
```

### Comparing `antspynet-0.2.1/antspynet/utilities/custom_activation_layers.py` & `antspynet-0.2.2/antspynet/utilities/custom_activation_layers.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/custom_convolution_layers.py` & `antspynet-0.2.2/antspynet/utilities/custom_convolution_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import backend as K
-from keras.utils import conv_utils
+# from keras.utils import conv_utils
+import tensorflow.keras.utils as conv_utils
 from keras.layers import InputSpec, Conv2D, Conv3D
 
 class PartialConv2D(Conv2D):
 
     """
     Implementation of the 2-D partial convolution layer based on
```

### Comparing `antspynet-0.2.1/antspynet/utilities/custom_metrics.py` & `antspynet-0.2.2/antspynet/utilities/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/custom_normalization_layers.py` & `antspynet-0.2.2/antspynet/utilities/custom_normalization_layers.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/data_augmentation.py` & `antspynet-0.2.2/antspynet/utilities/data_augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                       segmentation_image_list=None,
                       pointset_list=None,
                       number_of_simulations=10,
                       reference_image=None,
                       transform_type='affineAndDeformation',
                       noise_model='additivegaussian',
                       noise_parameters=(0.0, 0.05),
-                      sd_simulated_bias_field=0.05,
+                      sd_simulated_bias_field=1.0,
                       sd_histogram_warping=0.05,
                       sd_affine=0.05,
                       output_numpy_file_prefix=None,
                       verbose=False
                      ):
 
     """
@@ -232,24 +232,25 @@
                        parameters = (random.uniform(0.0, noise_parameters[0]))
                        image = ants.add_noise_to_image(image,
                                                        noise_model="speckle",
                                                        noise_parameters=parameters)
                    else:
                        raise ValueError("Unrecognized noise model.")
 
-
             # Simulated bias field
 
             if sd_simulated_bias_field > 0:
 
                 if verbose:
                     print("        Adding simulated bias field.")
 
-                bias_field = simulate_bias_field(image, sd_bias_field=sd_simulated_bias_field)
-                image = image * (bias_field + 1)
+                log_field = simulate_bias_field(image, number_of_points=10, sd_bias_field=sd_simulated_bias_field, number_of_fitting_levels=2, mesh_size=10)
+                log_field = log_field.iMath("Normalize")
+                field_array = np.power(np.exp(log_field.numpy()), random.sample((2, 3, 4), 1)[0])
+                image = image * ants.from_numpy(field_array, origin=image.origin, spacing=image.spacing, direction=image.direction)                
 
             # Histogram intensity warping
 
             if sd_histogram_warping > 0:
 
                 if verbose:
                     print("        Performing intensity histogram warping.")
```

### Comparing `antspynet-0.2.1/antspynet/utilities/deep_atropos.py` & `antspynet-0.2.2/antspynet/utilities/deep_atropos.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/deep_embedded_clustering_utilities.py` & `antspynet-0.2.2/antspynet/utilities/deep_embedded_clustering_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/deep_flash.py` & `antspynet-0.2.2/antspynet/utilities/deep_flash.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,15 @@
     # use_hierarchical_parcellation : boolean
     #     If True, use u-net model with additional outputs of the medial temporal lobe
     #     region, hippocampal, and entorhinal/perirhinal/parahippocampal regions.  Otherwise
     #     the only additional output is the medial temporal lobe.
     #
     # use_contralaterality : boolean
     #     Use both hemispherical models to also predict the corresponding contralateral
-    #     segmentation and use both sets of priors to produce the results.  Mainly used
-    #     for debugging.
+    #     segmentation and use both sets of priors to produce the results.  
 
     use_hierarchical_parcellation = True
     use_contralaterality = True
 
     ################################
     #
     # Preprocess images
@@ -117,15 +116,15 @@
     t1_preprocessed = t1
     t1_mask = None
     t1_preprocessed_flipped = None
     t1_template = ants.image_read(get_antsxnet_data("deepFlashTemplateT1SkullStripped"))
     template_transforms = None
     if do_preprocessing:
 
-        if verbose == True:
+        if verbose:
             print("Preprocessing T1.")
 
         # Brain extraction
         probability_mask = brain_extraction(t1_preprocessed, modality="t1",
             antsxnet_cache_directory=antsxnet_cache_directory, verbose=verbose)
         t1_mask = ants.threshold_image(probability_mask, 0.5, 1, 1, 0)
         t1_preprocessed = t1_preprocessed * t1_mask
@@ -152,15 +151,15 @@
     t2_preprocessed_flipped = None
     t2_template = None
     if t2 is not None:
         t2_template = ants.image_read(get_antsxnet_data("deepFlashTemplateT2SkullStripped"))
         t2_template = ants.copy_image_info(t1_template, t2_template)
         if do_preprocessing:
 
-            if verbose == True:
+            if verbose:
                 print("Preprocessing T2.")
 
             # Brain extraction
             t2_preprocessed = t2_preprocessed * t1_mask
 
             # Do bias correction
             t2_preprocessed = ants.n4_bias_field_correction(t2_preprocessed, t1_mask, shrink_factor=4, verbose=verbose)
```

### Comparing `antspynet-0.2.1/antspynet/utilities/denseunet_utilities.py` & `antspynet-0.2.2/antspynet/utilities/denseunet_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/desikan_killiany_tourville_labeling.py` & `antspynet-0.2.2/antspynet/utilities/desikan_killiany_tourville_labeling.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/extract_image_patches.py` & `antspynet-0.2.2/antspynet/utilities/extract_image_patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             for d in range(dimensionality):
                 mask_indices[:, d] = np.subtract(mask_indices[:, d], mid_patch_index[d])
 
             number_of_extracted_patches = min(max_number_of_patches, mask_indices.shape[0])
 
             if randomize:
                 random_indices = mask_indices[
-                  random.sample(range(mask_indices.shape[0]), number_of_extracted_patches), :]
+                  random.sample(range(mask_indices.shape[0] + 1), number_of_extracted_patches), :]
             else:
                 random_indices = mask_indices
 
         else:
 
             for d in range(dimensionality):
                 random_indices[:, d] = random.sample(range(image_size[d] - patch_size[d] + 1), max_number_of_patches)
```

### Comparing `antspynet-0.2.1/antspynet/utilities/get_antsxnet_data.py` & `antspynet-0.2.2/antspynet/utilities/get_antsxnet_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,16 +29,14 @@
     A filename string
 
     Example
     -------
     >>> template_file = get_antsxnet_data('biobank')
     """
 
-    from ..utilities import brain_extraction
-
     def switch_data(argument):
         switcher = {
             "biobank": "https://ndownloader.figshare.com/files/22429242",
             "croppedMni152": "https://ndownloader.figshare.com/files/22933754",
             "croppedMni152Priors": "https://ndownloader.figshare.com/files/27688437",
             "deepFlashPriors": "https://figshare.com/ndownloader/files/31208272",
             "deepFlashTemplateT1": "https://figshare.com/ndownloader/files/31207795",
@@ -56,15 +54,20 @@
             "priorDeepFlashRightLabels": "https://ndownloader.figshare.com/files/25422101",
             "adni": "https://ndownloader.figshare.com/files/25516361",
             "ixi": "https://ndownloader.figshare.com/files/25516358",
             "kirby": "https://ndownloader.figshare.com/files/25620107",
             "mni152": "https://ndownloader.figshare.com/files/25516349",
             "nki": "https://ndownloader.figshare.com/files/25516355",
             "nki10": "https://ndownloader.figshare.com/files/25516346",
-            "oasis": "https://ndownloader.figshare.com/files/25516352"
+            "oasis": "https://ndownloader.figshare.com/files/25516352",
+            "magetTemplate": "https://figshare.com/ndownloader/files/41052572",
+            "magetTemplateBrainMask": "https://figshare.com/ndownloader/files/41052569",
+            "magetCerebellumTemplate": "https://figshare.com/ndownloader/files/41052581",
+            "magetCerebellumTemplatePriors": "https://figshare.com/ndownloader/files/41052578",
+            "magetCerebellumxTemplate0GenericAffine": "https://figshare.com/ndownloader/files/41052575"            
         }
         return(switcher.get(argument, "Invalid argument."))
 
     if file_id == None:
         raise ValueError("Missing file id.")
 
     valid_list = ("biobank",
@@ -87,26 +90,34 @@
                   "adni",
                   "ixi",
                   "kirby",
                   "mni152",
                   "nki",
                   "nki10",
                   "oasis",
+                  "magetTemplate",
+                  "magetTemplateBrainMask",
+                  "magetCerebellumTemplate",
+                  "magetCerebellumTemplatePriors",
+                  "magetCerebellumxTemplate0GenericAffine",
                   "show")
 
     if not file_id in valid_list:
         raise ValueError("No data with the id you passed - try \"show\" to get list of valid ids.")
 
     if file_id == "show":
        return(valid_list)
 
     url = switch_data(file_id)
 
     if target_file_name == None:
-        target_file_name = file_id + ".nii.gz"
+        if file_id == "magetCerebellumxTemplate0GenericAffine":
+            target_file_name = file_id + ".mat"
+        else:
+            target_file_name = file_id + ".nii.gz"
 
     if antsxnet_cache_directory == None:
         antsxnet_cache_directory = "ANTsXNet"
 
     # keras get_file does not work on read-only file systems. It will attempt to download the file even
     # if it exists. This is a problem for shared cache directories and read-only containers.
     #
```

### Comparing `antspynet-0.2.1/antspynet/utilities/get_pretrained_network.py` & `antspynet-0.2.2/antspynet/utilities/get_pretrained_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
             "brainExtractionRobustFA": "https://figshare.com/ndownloader/files/34870410",
             "brainExtractionNoBrainer": "https://ndownloader.figshare.com/files/22598039",
             "brainExtractionInfantT1T2": "https://ndownloader.figshare.com/files/22968833",
             "brainExtractionInfantT1": "https://ndownloader.figshare.com/files/22968836",
             "brainExtractionInfantT2": "https://ndownloader.figshare.com/files/22968830",
             "brainSegmentation": "https://ndownloader.figshare.com/files/13900010",
             "brainSegmentationPatchBased": "https://ndownloader.figshare.com/files/14249717",
+            "cerebellumWhole": "https://figshare.com/ndownloader/files/41228604",
+            "cerebellumTissue": "https://figshare.com/ndownloader/files/41107724",
+            "cerebellumLabels": "https://figshare.com/ndownloader/files/41168678",
             "claustrum_axial_0": "https://ndownloader.figshare.com/files/27844068",
             "claustrum_axial_1": "https://ndownloader.figshare.com/files/27844059",
             "claustrum_axial_2": "https://ndownloader.figshare.com/files/27844062",
             "claustrum_coronal_0": "https://ndownloader.figshare.com/files/27844074",
             "claustrum_coronal_1": "https://ndownloader.figshare.com/files/27844071",
             "claustrum_coronal_2": "https://ndownloader.figshare.com/files/27844065",
             "ctHumanLung": "https://ndownloader.figshare.com/files/20005217",
@@ -87,14 +90,17 @@
             "dktOuter": "https://ndownloader.figshare.com/files/23765132",
             "dktOuterWithSpatialPriors": "https://ndownloader.figshare.com/files/24230768",
             "elBicho": "https://ndownloader.figshare.com/files/26736779",
             "ex5_coronal_weights": "https://figshare.com/ndownloader/files/38035968",
             "ex5_sagittal_weights": "https://figshare.com/ndownloader/files/38035965",
             "allen_brain_mask_weights" : "https://figshare.com/ndownloader/files/36999880",
             "allen_brain_leftright_coronal_mask_weights" : "",
+            "allen_cerebellum_coronal_mask_weights" : "",
+            "allen_cerebellum_sagittal_mask_weights" : "",
+            "allen_sr_weights" : "",
             "ewDavidSysu": "https://ndownloader.figshare.com/files/28757622", # "https://ndownloader.figshare.com/files/28403973",
             "ewDavidSysuRankedIntensity": "https://ndownloader.figshare.com/files/28403937",
             "ewDavidSysuT1Only": "https://ndownloader.figshare.com/files/28757628", #"https://ndownloader.figshare.com/files/28403934",
             "ewDavidSysuFlairOnly": "https://ndownloader.figshare.com/files/28757625", # "https://ndownloader.figshare.com/files/28403931",
             "ewDavidSysuWithAttention": "https://ndownloader.figshare.com/files/28757631", # "https://ndownloader.figshare.com/files/28431312",
             "ewDavidSysuWithAttentionT1Only": "https://ndownloader.figshare.com/files/28757646", # "https://ndownloader.figshare.com/files/28403970",
             "ewDavidSysuWithAttentionFlairOnly": "https://ndownloader.figshare.com/files/28757643", # "https://ndownloader.figshare.com/files/28403943",
@@ -164,14 +170,17 @@
                   "brainExtractionRobustFA",
                   "brainExtractionNoBrainer",
                   "brainExtractionInfantT1T2",
                   "brainExtractionInfantT1",
                   "brainExtractionInfantT2",
                   "brainSegmentation",
                   "brainSegmentationPatchBased",
+                  "cerebellumWhole",
+                  "cerebellumTissue",
+                  "cerebellumLabels",
                   "claustrum_axial_0",
                   "claustrum_axial_1",
                   "claustrum_axial_2",
                   "claustrum_coronal_0",
                   "claustrum_coronal_1",
                   "claustrum_coronal_2",
                   "ctHumanLung",
@@ -198,14 +207,17 @@
                   "dktInner",
                   "dktOuter",
                   "dktOuterWithSpatialPriors",
                   "ex5_coronal_weights",
                   "ex5_sagittal_weights",
                   "allen_brain_mask_weights",
                   "allen_brain_leftright_coronal_mask_weights",
+                  "allen_cerebellum_coronal_mask_weights",
+                  "allen_cerebellum_sagittal_mask_weights",
+                  "allen_sr_weights",
                   "elBicho",
                   "ewDavidSysu",
                   "ewDavidSysuRankedIntensity",
                   "ewDavidSysuT1Only",
                   "ewDavidSysuFlairOnly",
                   "ewDavidSysuWithAttention",
                   "ewDavidSysuWithAttentionT1Only",
```

### Comparing `antspynet-0.2.1/antspynet/utilities/hippmapp3r_segmentation.py` & `antspynet-0.2.2/antspynet/utilities/hippmapp3r_segmentation.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/histogram_warp_image_intensities.py` & `antspynet-0.2.2/antspynet/utilities/histogram_warp_image_intensities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/histology.py` & `antspynet-0.2.2/antspynet/utilities/histology.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import ants
+import warnings
 
 def arterial_lesion_segmentation(image,
                                  antsxnet_cache_directory=None,
                                  verbose=False):
 
     """
     Perform arterial lesion segmentation using U-net.
@@ -512,7 +513,258 @@
         np.expand_dims(segmentation_matrix, axis=0), image_channels[0] * 0 + 1)[0]
 
     return_dict = {'segmentation_image' : segmentation_image,
                    'probability_images' : probability_images}
     return(return_dict)
 
 
+def allen_histology_cerebellum_mask(image,
+                                    which_axis=2,
+                                    view = 'sagittal',
+                                    antsxnet_cache_directory=None,
+                                    verbose=False):
+
+    """
+    Determine cerebellum foreground of Allen's mouse data.
+
+    Arguments
+    ---------
+    image : ANTsImage
+        input image
+
+    which_axis : integer
+        If 3-D image, which_axis specifies the direction of the "view".
+
+    antsxnet_cache_directory : string
+        Destination directory for storing the downloaded template and model weights.
+        Since these can be resused, if is None, these data will be downloaded to a
+        ~/.keras/ANTsXNet/.
+
+    verbose : boolean
+        Print progress to the screen.
+
+    Returns
+    -------
+    Foreground probability image.
+
+    Example
+    -------
+    >>> output = allen_histology_cerebellum_mask(histology_image)
+    """
+
+    from ..architectures import create_unet_model_2d
+    from ..utilities import get_pretrained_network
+
+    if antsxnet_cache_directory == None:
+        antsxnet_cache_directory = "ANTsXNet"
+
+    if which_axis < 0 or which_axis > 2:
+        raise ValueError("Chosen axis not supported.")
+
+    weights_file_name = None
+    if view == "sagittal":
+        weights_file_name = get_pretrained_network("allen_cerebellum_sagittal_mask_weights",
+            antsxnet_cache_directory=antsxnet_cache_directory)
+    elif view == "coronal":   
+        weights_file_name = get_pretrained_network("allen_cerebellum_coronal_mask_weights",
+            antsxnet_cache_directory=antsxnet_cache_directory)
+    else:
+        raise ValueError("Unrecognized option for view.  Must be sagittal or coronal.")    
+
+    resampled_image_size = (512, 512)
+    original_slice_shape = image.shape
+    if image.dimension > 2:
+        original_slice_shape = tuple(np.delete(np.array(image.shape), which_axis))
+
+    unet_model = create_unet_model_2d((*resampled_image_size, 1),
+        number_of_outputs=1, mode="sigmoid",
+        number_of_filters=(64, 96, 128, 256, 512),
+        convolution_kernel_size=(3, 3), deconvolution_kernel_size=(2, 2),
+        dropout_rate=0.0, weight_decay=0,
+        additional_options=("initialConvolutionKernelSize[5]", "attentionGating"))
+    unet_model.load_weights(weights_file_name)
+
+    if verbose:
+        print("Preprocessing:  Resampling.")
+
+    number_of_channels = image.components
+    number_of_slices = 1
+    if image.dimension > 2:
+        number_of_slices = image.shape[which_axis]
+    
+    image_channels = list()
+    if number_of_channels == 1:
+        image_channels.append(image)
+    else:
+        image_channels = ants.split_channels(image)
+     
+    batch_X = np.zeros((number_of_channels * number_of_slices, *resampled_image_size, 1))
+    
+    count = 0
+    for i in range(number_of_channels):
+        image_channel_array = image_channels[i].numpy()
+        for j in range(number_of_slices):
+            slice = None
+            if image.dimension > 2:
+                if which_axis == 0:
+                    image_channel_slice_array = np.squeeze(image_channel_array[j,:,:])
+                elif which_axis == 1:
+                    image_channel_slice_array = np.squeeze(image_channel_array[:,j,:])
+                else:
+                    image_channel_slice_array = np.squeeze(image_channel_array[:,:,j])
+                slice = ants.from_numpy(image_channel_slice_array)
+            else:
+                slice = image_channels[i]
+            if slice.max() > slice.min():
+                slice_resampled = ants.resample_image(slice, resampled_image_size, use_voxels=True, interp_type=0)
+                slice_array = slice_resampled.numpy()
+                slice_array = (slice_array - slice_array.min()) / (slice_array.max() - slice_array.min())
+                batch_X[count,:,:,0] = slice_array
+            count = count + 1
+
+    if verbose:
+        print("Prediction: ")
+
+    predicted_data = unet_model.predict(batch_X, verbose=int(verbose))
+    if number_of_channels > 1:
+        if verbose:
+            print("Averaging across channels.")
+        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0) 
+        predicted_data = np.zeros((number_of_slices, *resampled_image_size, 1))
+        for i in range(number_of_channels):
+            predicted_data = (predicted_data * i + predicted_data_temp[i]) / (i + 1)
+
+    if verbose:
+        print("Post-processing:  resampling to original space.")
+
+    foreground_probability_array = np.zeros(image.shape)
+    for j in range(number_of_slices):
+        slice_resampled = ants.from_numpy(np.squeeze(predicted_data[j,:,:,0]))
+        slice = ants.resample_image(slice_resampled, original_slice_shape, use_voxels=True, interp_type=0)
+        if image.dimension == 2: 
+            foreground_probability_array[:,:] = slice.numpy()
+        else:
+            if which_axis == 0:
+                foreground_probability_array[j,:,:] = slice.numpy()
+            elif which_axis == 1:
+                foreground_probability_array[:,j,:] = slice.numpy()
+            else:
+                foreground_probability_array[:,:,j] = slice.numpy()
+
+    origin = image.origin
+    spacing = image.spacing
+    direction = image.direction
+
+    foreground_probability_image = ants.from_numpy(foreground_probability_array,
+        origin=origin, spacing=spacing, direction=direction)
+
+    return(foreground_probability_image)
+
+def allen_histology_super_resolution(image,
+                                     antsxnet_cache_directory=None,
+                                     verbose=False):
+
+    """
+    Super resolution (2x) of a single image slice (256x256 -> 512x512)
+
+    Arguments
+    ---------
+    image : ANTsImage or ANTsImage list
+        input image or input image list
+
+    antsxnet_cache_directory : string
+        Destination directory for storing the downloaded template and model weights.
+        Since these can be resused, if is None, these data will be downloaded to a
+        ~/.keras/ANTsXNet/.
+
+    verbose : boolean
+        Print progress to the screen.
+
+    Returns
+    -------
+    Super resolution image of size 512x512 voxels (or a list depending on the input)
+
+    Example
+    -------
+    >>> output = allen_histology_super_resolution(histology_image)
+    """
+
+    from ..architectures import create_deep_back_projection_network_model_2d
+    from ..utilities import get_pretrained_network
+    from ..utilities import regression_match_image
+
+    image_list = list()
+    if isinstance(image, list):
+        image_list = image
+    else:
+        image_list.append(image)
+
+    lr_image_size = (256, 256)
+    sr_image_size = (512, 512)
+    
+    image_lr_list = list()
+    for i in range(len(image_list)):
+
+        if image_list[i].components != 3:
+            raise ValueError("Number of image channels should be 3 (rgb).")
+        if image_list[i].dimension != 2:
+            raise ValueError("Input image should be 2-D.")
+                
+        do_resample = False
+        if image_list[i].shape != lr_image_size:
+            warnings.warn("Resampling input image to (256, 256).")
+            do_resample = True
+
+        image_lr = ants.image_clone(image_list[i])
+        image_lr_channels = ants.split_channels(image_lr)
+        for c in range(len(image_lr_channels)):
+            if do_resample:
+                image_lr_channels[c] = ants.resample_image(image_lr_channels[c], resample_params=lr_image_size, 
+                                                           use_voxels=True, interp_type=0)
+            image_lr_channels[c] = ((image_lr_channels[c] - image_lr_channels[c].min()) / 
+                                    (image_lr_channels[c].max() - image_lr_channels[c].min()))
+        image_lr = ants.merge_channels(image_lr_channels)
+        image_lr_list.append(image_lr)
+
+    if antsxnet_cache_directory == None:
+        antsxnet_cache_directory = "ANTsXNet"
+
+    weights_file_name = get_pretrained_network("allen_sr_weights",
+        antsxnet_cache_directory=antsxnet_cache_directory)
+
+    sr_model = create_deep_back_projection_network_model_2d((*lr_image_size, 3),
+        number_of_outputs=3, convolution_kernel_size=(6, 6), strides=(2, 2))
+    sr_model.load_weights(weights_file_name)
+
+    batch_X = np.zeros((len(image_lr_list), *lr_image_size, 3))
+    for i in range(len(image_lr_list)):
+        batch_X[i,:,:,:] = image_lr_list[i].numpy()
+    
+    if verbose:
+        print("Prediction: ")
+
+    predicted_data = sr_model.predict(batch_X, verbose=int(verbose))
+    
+    if verbose:
+        print("Regression match output image.")
+
+    spacing_factor = (lr_image_size[0] - 1) / (sr_image_size[0] - 1)
+    
+    image_sr_list = list()
+    for i in range(len(image_lr_list)):
+        image_sr = ants.from_numpy(predicted_data[i,:,:,:], origin=image_list[i].origin,
+                                   direction=image_list[i].direction, 
+                                   spacing=(spacing_factor * image_list[i].spacing[0], 
+                                            spacing_factor * image_list[i].spacing[1]),
+                                   has_components=True)
+        image_channels = ants.split_channels(image_list[i])
+        image_sr_channels = ants.split_channels(image_sr)
+        for c in range(len(image_sr_channels)):
+            image_lr_channel_resampled = ants.resample_image(image_channels[c], resample_params=sr_image_size, 
+                                                             use_voxels=True, interp_type=0)
+            image_sr_channels[c] = regression_match_image(image_sr_channels[c], image_lr_channel_resampled)
+        image_sr_list.append(ants.merge_channels(image_sr_channels))
+
+    if isinstance(image, list):
+        return(image_sr_list)
+    else:
+        return(image_sr_list[0])
```

### Comparing `antspynet-0.2.1/antspynet/utilities/hypothalamus_segmentation.py` & `antspynet-0.2.2/antspynet/utilities/hypothalamus_segmentation.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/inpainting.py` & `antspynet-0.2.2/antspynet/utilities/inpainting.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Modality image type.  Options include:
             * "t1": T1-weighted MRI.
             * "flair": FLAIR MRI.
 
     slicewise : boolean
         Two models per modality are available for processing the data.  One model
         is based on training/prediction using 2-D axial slice data whereas the
-        other us
+        other uses 64x64x64 patches.
 
     antsxnet_cache_directory : string
         Destination directory for storing the downloaded template and model weights.
         Since these can be resused, if is None, these data will be downloaded to a
         ~/.keras/ANTsXNet/.
 
     verbose : boolean
```

### Comparing `antspynet-0.2.1/antspynet/utilities/lung_extraction.py` & `antspynet-0.2.2/antspynet/utilities/lung_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
         permutations.append((1, 0, 2))
         permutations.append((1, 2, 0))
 
         probability_image = ants.image_clone(image) * 0
 
         current_start_slice = 0
         for d in range(len(dimensions_to_predict)):
-            current_end_slice = current_start_slice + preprocessed_image.shape[dimensions_to_predict[d]] - 1
+            current_end_slice = current_start_slice + preprocessed_image.shape[dimensions_to_predict[d]]
             which_batch_slices = range(current_start_slice, current_end_slice)
 
             prediction_per_dimension = prediction[which_batch_slices,:,:,0]
             prediction_array = np.transpose(np.squeeze(prediction_per_dimension), permutations[dimensions_to_predict[d]])
             prediction_image = ants.copy_image_info(image,
                 pad_or_crop_image_to_size(ants.from_numpy(prediction_array),
                 image.shape))
```

### Comparing `antspynet-0.2.1/antspynet/utilities/lung_segmentation.py` & `antspynet-0.2.2/antspynet/utilities/lung_segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
     probability_images = list()
     for l in range(number_of_classification_labels):
         probability_images.append(ants.image_clone(mask) * 0)
 
     current_start_slice = 0
     for d in range(len(dimensions_to_predict)):
-        current_end_slice = current_start_slice + preprocessed_image.shape[dimensions_to_predict[d]] - 1
+        current_end_slice = current_start_slice + preprocessed_image.shape[dimensions_to_predict[d]]
         which_batch_slices = range(current_start_slice, current_end_slice)
 
         for l in range(number_of_classification_labels):
             prediction_per_dimension = prediction[which_batch_slices,:,:,l]
             prediction_array = np.transpose(np.squeeze(prediction_per_dimension), permutations[dimensions_to_predict[d]])
             prediction_image = ants.copy_image_info(ventilation_image,
                 pad_or_crop_image_to_size(ants.from_numpy(prediction_array),
```

### Comparing `antspynet-0.2.1/antspynet/utilities/mixture_density_utilities.py` & `antspynet-0.2.2/antspynet/utilities/mixture_density_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/mri_super_resolution.py` & `antspynet-0.2.2/antspynet/utilities/mri_super_resolution.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/neural_style_transfer.py` & `antspynet-0.2.2/antspynet/utilities/neural_style_transfer.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/preprocess_image.py` & `antspynet-0.2.2/antspynet/utilities/preprocess_image.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/quality_assessment.py` & `antspynet-0.2.2/antspynet/utilities/quality_assessment.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/randomly_transform_image_data.py` & `antspynet-0.2.2/antspynet/utilities/randomly_transform_image_data.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/reconstruct_image_from_patches.py` & `antspynet-0.2.2/antspynet/utilities/reconstruct_image_from_patches.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/regression_match_image.py` & `antspynet-0.2.2/antspynet/utilities/regression_match_image.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/resample_tensor_utilities.py` & `antspynet-0.2.2/antspynet/utilities/resample_tensor_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/simulate_bias_field.py` & `antspynet-0.2.2/antspynet/utilities/simulate_bias_field.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/spatial_transformer_network_utilities.py` & `antspynet-0.2.2/antspynet/utilities/spatial_transformer_network_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/super_resolution_utilities.py` & `antspynet-0.2.2/antspynet/utilities/super_resolution_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/ukbb.py` & `antspynet-0.2.2/antspynet/utilities/ukbb.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/unet_utilities.py` & `antspynet-0.2.2/antspynet/utilities/unet_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.1/antspynet/utilities/white_matter_hyperintensity_segmentation.py` & `antspynet-0.2.2/antspynet/utilities/white_matter_hyperintensity_segmentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -162,18 +162,18 @@
     ################################
     #
     # Build models and load weights
     #
     ################################
 
     number_of_models = 1
-    if use_ensemble == True:
+    if use_ensemble:
         number_of_models = 3
 
-    if verbose == True:
+    if verbose:
         print("White matter hyperintensity:  retrieving model weights.")
 
     unet_models = list()
     for i in range(number_of_models):
         if number_of_channels == 1:
             weights_file_name = get_pretrained_network("sysuMediaWmhFlairOnlyModel" + str(i),
                 antsxnet_cache_directory=antsxnet_cache_directory)
@@ -202,15 +202,15 @@
 
     batchX = np.zeros((total_number_of_slices, *image_size, number_of_channels))
 
     slice_count = 0
     for d in range(len(dimensions_to_predict)):
         number_of_slices = flair_preprocessed_warped.shape[dimensions_to_predict[d]]
 
-        if verbose == True:
+        if verbose:
             print("Extracting slices for dimension ", dimensions_to_predict[d], ".")
 
         for i in range(number_of_slices):
             flair_slice = pad_or_crop_image_to_size(ants.slice_image(flair_preprocessed_warped, dimensions_to_predict[d], i), image_size)
             batchX[slice_count,:,:,0] = flair_slice.numpy()
             if number_of_channels == 2:
                 t1_slice = pad_or_crop_image_to_size(ants.slice_image(t1_preprocessed_warped, dimensions_to_predict[d], i), image_size)
@@ -219,15 +219,15 @@
 
     ################################
     #
     # Do prediction and then restack into the image
     #
     ################################
 
-    if verbose == True:
+    if verbose:
         print("Prediction.")
 
     prediction = unet_models[0].predict(np.transpose(batchX, axes=(0, 2, 1, 3)), verbose=verbose)
     if number_of_models > 1:
         for i in range(1, number_of_models, 1):
             prediction += unet_models[i].predict(np.transpose(batchX, axes=(0, 2, 1, 3)), verbose=verbose)
     prediction /= number_of_models
@@ -325,21 +325,21 @@
 
     ################################
     #
     # Preprocess images
     #
     ################################
 
-    if verbose == True:
+    if verbose:
         print("*************  Preprocessing  ***************")
         print("")
 
     t1_preprocessed = t1
     brain_mask = None
-    if do_preprocessing == True:
+    if do_preprocessing:
         t1_preprocessing = preprocess_brain_image(t1,
             truncate_intensity=(0.01, 0.99),
             brain_extraction_modality="t1",
             do_bias_correction=True,
             do_denoising=False,
             antsxnet_cache_directory=antsxnet_cache_directory,
             verbose=verbose)
@@ -351,29 +351,29 @@
         brain_mask = ants.threshold_image(t1, 0, 0, 0, 1)
 
     t1_preprocessed_mean = t1_preprocessed[brain_mask > 0].mean()
     t1_preprocessed_std = t1_preprocessed[brain_mask > 0].std()
     t1_preprocessed[brain_mask > 0] = (t1_preprocessed[brain_mask > 0] - t1_preprocessed_mean) / t1_preprocessed_std
 
     flair_preprocessed = flair
-    if do_preprocessing == True:
+    if do_preprocessing:
         flair_preprocessing = preprocess_brain_image(flair,
             truncate_intensity=(0.01, 0.99),
             brain_extraction_modality=None,
             do_bias_correction=True,
             do_denoising=False,
             antsxnet_cache_directory=antsxnet_cache_directory,
             verbose=verbose)
         flair_preprocessed = flair_preprocessing["preprocessed_image"] * brain_mask
 
     flair_preprocessed_mean = flair_preprocessed[brain_mask > 0].mean()
     flair_preprocessed_std = flair_preprocessed[brain_mask > 0].std()
     flair_preprocessed[brain_mask > 0] = (flair_preprocessed[brain_mask > 0] - flair_preprocessed_mean) / flair_preprocessed_std
 
-    if verbose == True:
+    if verbose:
         print("    HyperMapp3r: reorient input images.")
 
     channel_size = 2
     input_image_size = (224, 224, 224)
     template_array = np.ones(input_image_size)
     template_direction = np.eye(3)
     template_direction[1, 1] = -1.0
@@ -390,31 +390,30 @@
 
     t1_preprocessed_warped = ants.apply_ants_transform_to_image(xfrm, t1_preprocessed, reorient_template)
     batchX[0,:,:,:,0] = t1_preprocessed_warped.numpy()
 
     flair_preprocessed_warped = ants.apply_ants_transform_to_image(xfrm, flair_preprocessed, reorient_template)
     batchX[0,:,:,:,1] = flair_preprocessed_warped.numpy()
 
-    if verbose == True:
+    if verbose:
         print("    HyperMapp3r: generate network and load weights.")
 
     model = create_hypermapp3r_unet_model_3d((*input_image_size, 2))
     weights_file_name = get_pretrained_network("hyperMapp3r", antsxnet_cache_directory=antsxnet_cache_directory)
     model.load_weights(weights_file_name)
 
-    if verbose == True:
+    if verbose:
         print("    HyperMapp3r: prediction.")
 
-    if verbose == True:
+    if verbose:
         print("    HyperMapp3r: Monte Carlo iterations (SpatialDropout).")
 
     prediction_array = np.zeros(input_image_size)
     for i in range(number_of_monte_carlo_iterations):
-        tf.random.set_seed(i)
-        if verbose == True:
+        if verbose:
             print("        Monte Carlo iteration", i + 1, "out of", number_of_monte_carlo_iterations)
         prediction_array = (np.squeeze(model.predict(batchX, verbose=verbose)) + i * prediction_array) / (i + 1)
 
     prediction_image = ants.from_numpy(prediction_array, origin=reorient_template.origin,
         spacing=reorient_template.spacing, direction=reorient_template.direction)
 
     xfrm_inv = xfrm.invert()
@@ -536,28 +535,28 @@
         # #
         # # Preprocess images
         # #
         # ################################
 
         # t1_preprocessed = t1
         # t1_preprocessing = None
-        # if do_preprocessing == True:
+        # if do_preprocessing:
         #     t1_preprocessing = preprocess_brain_image(t1,
         #         truncate_intensity=(0.01, 0.99),
         #         brain_extraction_modality="t1",
         #         template="croppedMni152",
         #         template_transform_type="antsRegistrationSyNQuickRepro[a]",
         #         do_bias_correction=True,
         #         do_denoising=False,
         #         antsxnet_cache_directory=antsxnet_cache_directory,
         #         verbose=verbose)
         #     t1_preprocessed = t1_preprocessing["preprocessed_image"] * t1_preprocessing['brain_mask']
 
         # flair_preprocessed = flair
-        # if do_preprocessing == True:
+        # if do_preprocessing:
         #     flair_preprocessing = preprocess_brain_image(flair,
         #         truncate_intensity=(0.01, 0.99),
         #         brain_extraction_modality="t1",
         #         do_bias_correction=True,
         #         do_denoising=False,
         #         antsxnet_cache_directory=antsxnet_cache_directory,
         #         verbose=verbose)
@@ -596,15 +595,15 @@
 
         # ################################
         # #
         # # Do prediction and normalize to native space
         # #
         # ################################
 
-        # if verbose == True:
+        # if verbose:
         #     print("ew_david:  prediction.")
 
         # batchX = np.zeros((8, *patch_size, channel_size))
 
         # t1_preprocessed = (t1_preprocessed - t1_preprocessed.mean()) / t1_preprocessed.std()
         # t1_patches = extract_image_patches(t1_preprocessed, patch_size=patch_size,
         #                                     max_number_of_patches="all", stride_length=stride_length,
@@ -621,15 +620,15 @@
 
         # probability_images = list()
         # for i in range(len(labels)):
         #     print("Reconstructing image", classes[i])
         #     reconstructed_image = reconstruct_image_from_patches(predicted_data[:,:,:,:,i],
         #         domain_image=t1_preprocessed, stride_length=stride_length)
 
-        #     if do_preprocessing == True:
+        #     if do_preprocessing:
         #         probability_images.append(ants.apply_transforms(fixed=t1,
         #             moving=reconstructed_image,
         #             transformlist=t1_preprocessing['template_transforms']['invtransforms'],
         #             whichtoinvert=[True], interpolator="linear", verbose=verbose))
         #     else:
         #         probability_images.append(reconstructed_image)
 
@@ -647,15 +646,15 @@
         if "-ri" in which_model:
             use_rank_intensity_scaling = True
 
         t1_preprocessed = None
         t1_preprocessing = None
         brain_mask = None
         if t1 is not None:
-            if do_preprocessing == True:
+            if do_preprocessing:
                 t1_preprocessing = preprocess_brain_image(t1,
                     truncate_intensity=(0.01, 0.995),
                     brain_extraction_modality="t1",
                     do_bias_correction=False,
                     do_denoising=False,
                     antsxnet_cache_directory=antsxnet_cache_directory,
                     verbose=verbose)
@@ -666,15 +665,15 @@
         if use_t1_segmentation:
             atropos_seg = deep_atropos(t1, do_preprocessing=True, verbose=verbose)
             t1_segmentation = atropos_seg['segmentation_image']
 
         flair_preprocessed = None
         if flair is not None:
             flair_preprocessed = flair
-            if do_preprocessing == True:
+            if do_preprocessing:
                 if brain_mask is None:
                     flair_preprocessing = preprocess_brain_image(flair,
                         truncate_intensity=(0.01, 0.995),
                         brain_extraction_modality="flair",
                         do_bias_correction=False,
                         do_denoising=False,
                         antsxnet_cache_directory=antsxnet_cache_directory,
@@ -773,15 +772,15 @@
             unet_model = create_unet_model_2d((*template_size, channel_size),
                 number_of_outputs=1, mode="sigmoid",
                 number_of_filters=(64, 96, 128, 256, 512), dropout_rate=0.0,
                 convolution_kernel_size=(3, 3), deconvolution_kernel_size=(2, 2),
                 weight_decay=0,
                 additional_options=("nnUnetActivationStyle", "attentionGating", "initialConvolutionKernelSize[5]"))
 
-        if verbose == True:
+        if verbose:
             print("ewDavid:  retrieving model weights.")
 
         weights_file_name = None
         if which_model == "sysu" and flair is not None and t1 is not None:
             weights_file_name = get_pretrained_network("ewDavidSysu", antsxnet_cache_directory=antsxnet_cache_directory)
         elif which_model == "sysu-ri" and flair is not None and t1 is not None:
             weights_file_name = get_pretrained_network("ewDavidSysuRankedIntensity", antsxnet_cache_directory=antsxnet_cache_directory)
@@ -952,15 +951,15 @@
 
                 number_of_slices = None
                 if batch_t1 is not None:
                     number_of_slices = batch_t1.shape[dimensions_to_predict[d]]
                 else:
                     number_of_slices = batch_flair.shape[dimensions_to_predict[d]]
 
-                if verbose == True:
+                if verbose:
                     print("Extracting slices for dimension ", dimensions_to_predict[d])
 
                 for i in range(number_of_slices):
 
                     brain_mask_slice = pad_or_crop_image_to_size(ants.slice_image(batch_brain_mask, dimensions_to_predict[d], i), template_size)
 
                     channel_count = 0
@@ -983,15 +982,15 @@
 
             ################################
             #
             # Do prediction and then restack into the image
             #
             ################################
 
-            if verbose == True:
+            if verbose:
                 if n == 0:
                     print("Prediction")
                 else:
                     print("Prediction (simulation " + str(n) + ")")
 
             prediction = unet_model.predict(batchX, verbose=verbose)
```

### Comparing `antspynet-0.2.1/antspynet.egg-info/PKG-INFO` & `antspynet-0.2.2/antspynet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: antspynet
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of deep learning architectures ported to the python language and tools for basic medical image processing.
 Home-page: https://github.com/ANTsX/ANTsPyNet
 Author: Nicholas J. Tustison and Brian B. Avants and Nick Cullen
 Author-email: ntustison@gmail.com
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.md
 
-[![Build Status](https://travis-ci.org/ANTsX/ANTsPyNet.svg?branch=master)](https://travis-ci.org/ANTsX/ANTsPyNet)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
 
 # ANTsPyNet
 
 A collection of deep learning architectures and applications ported to the python language and tools for basic medical image processing. Based on `keras` and `tensorflow` with cross-compatibility with our R analog [ANTsRNet](https://github.com/ANTsX/ANTsRNet/).
 
 Documentation page [https://antsx.github.io/ANTsPyNet/](https://antsx.github.io/ANTsPyNet/).
@@ -88,14 +88,15 @@
 * [HippMapp3r hippocampal segmentation](https://pubmed.ncbi.nlm.nih.gov/31609046/)
 * [Sysu white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/30125711/)
 * [HyperMapp3r white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/35088930/)
 * [Hypothalamus segmentation](https://pubmed.ncbi.nlm.nih.gov/32853816/)
 * [Claustrum segmentation](https://arxiv.org/abs/2008.03465)
 * [Deep Flash](https://www.medrxiv.org/content/10.1101/2023.01.17.23284693v1)
 * Desikan-Killiany-Tourville cortical labeling
+* Cerebellum segmentation, parcellation, and thickness
 * Lung extraction
     * [Proton](https://www.ncbi.nlm.nih.gov/pubmed/30195415)
     * CT
 * [Functional lung segmentation](https://www.medrxiv.org/content/10.1101/2021.03.04.21252588v2)
 * [Neural style transfer](https://arxiv.org/abs/1508.06576)
 * Image quality assessment
     * [TID2013](https://www.sciencedirect.com/science/article/pii/S0923596514001490)
```

### Comparing `antspynet-0.2.1/antspynet.egg-info/SOURCES.txt` & `antspynet-0.2.2/antspynet.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 antspynet/architectures/create_deep_back_projection_network_model.py
 antspynet/architectures/create_deep_convolutional_gan_model.py
 antspynet/architectures/create_deep_denoise_super_resolution_model.py
 antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py
 antspynet/architectures/create_dense_model.py
 antspynet/architectures/create_densenet_model.py
 antspynet/architectures/create_denseunet_model.py
+antspynet/architectures/create_diffusion_probabilistic_unet_model.py
 antspynet/architectures/create_expanded_super_resolution_model.py
 antspynet/architectures/create_image_super_resolution_model.py
 antspynet/architectures/create_improved_wasserstein_gan_model.py
 antspynet/architectures/create_partial_convolution_unet_model.py
 antspynet/architectures/create_resnet_model.py
 antspynet/architectures/create_resnet_super_resolution_model.py
 antspynet/architectures/create_resunet_model.py
@@ -36,28 +37,30 @@
 antspynet/architectures/create_vgg_model.py
 antspynet/architectures/create_wasserstein_gan_model.py
 antspynet/architectures/create_wide_resnet_model.py
 antspynet/utilities/__init__.py
 antspynet/utilities/attention_utilities.py
 antspynet/utilities/brain_age.py
 antspynet/utilities/brain_extraction.py
+antspynet/utilities/cerebellum_morphology.py
 antspynet/utilities/claustrum_segmentation.py
 antspynet/utilities/cortical_thickness.py
 antspynet/utilities/cropping_and_padding_utilities.py
 antspynet/utilities/custom_activation_layers.py
 antspynet/utilities/custom_convolution_layers.py
 antspynet/utilities/custom_metrics.py
 antspynet/utilities/custom_normalization_layers.py
 antspynet/utilities/data_augmentation.py
 antspynet/utilities/deep_atropos.py
 antspynet/utilities/deep_embedded_clustering_utilities.py
 antspynet/utilities/deep_flash.py
 antspynet/utilities/denseunet_utilities.py
 antspynet/utilities/desikan_killiany_tourville_labeling.py
 antspynet/utilities/extract_image_patches.py
+antspynet/utilities/gaussian_diffusion_utilities.py
 antspynet/utilities/get_antsxnet_data.py
 antspynet/utilities/get_pretrained_network.py
 antspynet/utilities/hippmapp3r_segmentation.py
 antspynet/utilities/histogram_warp_image_intensities.py
 antspynet/utilities/histology.py
 antspynet/utilities/hypothalamus_segmentation.py
 antspynet/utilities/inpainting.py
```

### Comparing `antspynet-0.2.1/setup.py` & `antspynet-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open("README.md").read()
 
 setup(name='antspynet',
-      version='0.2.1',
+      version='0.2.2',
       description='A collection of deep learning architectures ported to the python language and tools for basic medical image processing.',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/ANTsX/ANTsPyNet',
       author='Nicholas J. Tustison and Brian B. Avants and Nick Cullen',
       author_email='ntustison@gmail.com',
       packages=['antspynet','antspynet/architectures','antspynet/utilities'],
```

