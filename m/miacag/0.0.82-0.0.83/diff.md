# Comparing `tmp/miacag-0.0.82.tar.gz` & `tmp/miacag-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miacag-0.0.82.tar", last modified: Fri May 26 10:09:43 2023, max compression
+gzip compressed data, was "miacag-0.0.83.tar", last modified: Wed Jun 21 13:42:39 2023, max compression
```

## Comparing `miacag-0.0.82.tar` & `miacag-0.0.83.tar`

### file list

```diff
@@ -1,186 +1,192 @@
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-01 15:05:05.000000 miacag-0.0.82/LICENSE
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      129 2022-09-01 15:05:05.000000 miacag-0.0.82/MANIFEST.in
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-05-26 10:09:43.438565 miacag-0.0.82/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      111 2022-10-20 03:13:52.000000 miacag-0.0.82/README.md
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/_3D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/classification/_3D/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3800 2022-09-20 09:25:18.000000 miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/_3D/stenosis_detection_rca/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9668 2022-09-20 09:25:18.000000 miacag-0.0.82/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/classification/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      823 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/config.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3229 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/options.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      881 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/update_configs.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/dataloader/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Classification/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Classification/_2D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12802 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    14190 2023-05-19 09:24:28.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    71072 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/dataset_mil_2d.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Classification/_3D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2088 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_avi_video.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9581 2023-05-16 11:27:04.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    24226 2023-05-19 09:12:51.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    72019 2022-11-04 15:43:12.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataset_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Classification/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9370 2023-05-17 13:50:58.000000 miacag-0.0.82/miacag/dataloader/Classification/get_dataloader_classification.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2440 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/DistributedWeightedSampler.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Representation/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Representation/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10772 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Representation/get_dataloader_representation.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5611 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/dataloader_base.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    24810 2023-05-19 06:35:38.000000 miacag-0.0.82/miacag/dataloader/dataloader_base_monai.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6113 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/dataloader/get_dataloader.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/metrics/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/metrics/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1180 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/metrics/cumulativeSumming.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4969 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/metrics/metrics.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13559 2023-05-23 12:24:10.000000 miacag-0.0.82/miacag/metrics/metrics_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/model_utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9549 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/model_utils/GradCam_model.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/model_utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12046 2023-05-23 13:56:02.000000 miacag-0.0.82/miacag/model_utils/eval_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4045 2023-05-19 07:50:15.000000 miacag-0.0.82/miacag/model_utils/get_loss_func.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2023-05-19 08:49:06.000000 miacag-0.0.82/miacag/model_utils/get_optimizer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10922 2023-05-24 05:35:58.000000 miacag-0.0.82/miacag/model_utils/get_test_pipeline.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9286 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/model_utils/grad_cam_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12228 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/model_utils/predict_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1576 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/model_utils/scheduler.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      785 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/model_utils/siam_loss.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6720 2023-05-23 12:03:48.000000 miacag-0.0.82/miacag/model_utils/train_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8774 2023-05-19 08:51:15.000000 miacag-0.0.82/miacag/models/BuildModel.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/backbone_encoders/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/backbone_encoders/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/backbone_encoders/tabular/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/backbone_encoders/tabular/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      212 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/backbone_encoders/tabular/base_encoders.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      670 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/cnns.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/dino_utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-16 12:42:02.000000 miacag-0.0.82/miacag/models/dino_utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6468 2023-05-17 12:25:03.000000 miacag-0.0.82/miacag/models/dino_utils/dino_pretrained.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13826 2023-05-19 09:49:15.000000 miacag-0.0.82/miacag/models/get_encoder.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/mae_st_util/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-04-25 13:02:50.000000 miacag-0.0.82/miacag/models/mae_st_util/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3130 2023-04-25 13:03:31.000000 miacag-0.0.82/miacag/models/mae_st_util/logging.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6395 2023-04-25 13:05:51.000000 miacag-0.0.82/miacag/models/mae_st_util/models_vit.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4915 2023-04-25 13:44:14.000000 miacag-0.0.82/miacag/models/mae_st_util/video_vit.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    11884 2023-05-19 06:59:56.000000 miacag-0.0.82/miacag/models/milmodel3d.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12926 2023-05-17 12:55:21.000000 miacag-0.0.82/miacag/models/milmodel_from_features.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1769 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/mlps.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13303 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/models/modeling_finetune.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13780 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/models/modeling_pretrain.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8584 2023-05-23 10:13:32.000000 miacag-0.0.82/miacag/models/modules.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13824 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/models/pretrained_vit.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/models/torchhub/2D/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D/r50/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/models/torchhub/2D/r50/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_16x4/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_32x3/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_32x3/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/r2plus1_18/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/r2plus1_18/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/x3d_s/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/x3d_s/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/plots/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/plots/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1983 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/plots/angle_plotter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      408 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/plots/getDataFromPdf.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      795 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/plots/plot_histogram.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4724 2023-05-25 10:22:04.000000 miacag-0.0.82/miacag/plots/plot_pathology_treatment_pred.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5167 2023-05-25 11:08:34.000000 miacag-0.0.82/miacag/plots/plot_predict_coronary_pathology.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10561 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/plots/plot_roc_auc_all.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1277 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/plots/plot_scatter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1245 2023-01-27 08:30:25.000000 miacag-0.0.82/miacag/plots/plot_test.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    33279 2023-05-22 15:55:28.000000 miacag-0.0.82/miacag/plots/plotter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4543 2023-01-27 08:26:48.000000 miacag-0.0.82/miacag/plots/query_plot_agg_max.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/postprocessing/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3593 2022-12-16 18:58:11.000000 miacag-0.0.82/miacag/postprocessing/aggregate_pr_group.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1880 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/append_results.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4331 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/count_stenosis_pr_group.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5354 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/estimate_vessel_disease.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2527 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/predictor.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/preprocessing/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1319 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/add_columns.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1412 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/copy_column.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1321 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/copy_table.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/datasetFingerpring.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    21523 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/datasetFingerprint.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3232 2023-05-25 09:45:44.000000 miacag-0.0.82/miacag/preprocessing/labels_map.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7064 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/pre_process.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/preprocessing/process_labels/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/process_labels/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-12-16 18:59:24.000000 miacag-0.0.82/miacag/preprocessing/process_labels/process_dominance.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15711 2023-03-02 17:26:57.000000 miacag-0.0.82/miacag/preprocessing/process_labels/process_total_occ.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3631 2023-05-23 08:44:57.000000 miacag-0.0.82/miacag/preprocessing/split_train_val.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2344 2022-12-16 18:58:52.000000 miacag-0.0.82/miacag/preprocessing/transform_missing_floats.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2521 2022-12-16 18:58:58.000000 miacag-0.0.82/miacag/preprocessing/transform_stenosis.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4756 2023-01-10 15:49:41.000000 miacag-0.0.82/miacag/preprocessing/transform_thresholds.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2591 2022-12-16 18:59:17.000000 miacag-0.0.82/miacag/preprocessing/transform_total_occlusion.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/preprocessing/utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1402 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/utils/check_experiments.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13571 2023-01-10 16:02:18.000000 miacag-0.0.82/miacag/scripts/aggregate_and_plot.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/angiography_classifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/angiography_classifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4842 2023-05-19 07:46:19.000000 miacag-0.0.82/miacag/scripts/angiography_classifier/predict_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13266 2023-05-23 10:33:43.000000 miacag-0.0.82/miacag/scripts/angiography_classifier/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2206 2023-05-19 07:46:41.000000 miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3675 2023-02-28 09:02:39.000000 miacag-0.0.82/miacag/scripts/compare_PCI_notPCI.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6510 2023-03-02 16:02:03.000000 miacag-0.0.82/miacag/scripts/predict_patologi_eyeball_vs_estimated.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/pretraining_downstreams/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/scripts/pretraining_downstreams/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    21016 2023-05-25 10:58:02.000000 miacag-0.0.82/miacag/scripts/pretraining_downstreams/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_identifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    22900 2023-05-19 07:46:49.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    16479 2023-05-19 07:46:55.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_regression/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_regression/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    27314 2023-05-19 07:47:03.000000 miacag-0.0.82/miacag/scripts/stenosis_regression/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_regression_full/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_regression_full/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7325 2023-05-19 07:47:08.000000 miacag-0.0.82/miacag/scripts/stenosis_regression_full/submit_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2933 2023-05-19 08:24:26.000000 miacag-0.0.82/miacag/tester.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/tests/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/tests/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2109 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/tests/test_sql_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4836 2023-05-19 08:16:57.000000 miacag-0.0.82/miacag/trainer.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3070 2023-05-23 12:08:55.000000 miacag-0.0.82/miacag/utils/common_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1313 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/utils/script_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6241 2023-05-23 10:53:47.000000 miacag-0.0.82/miacag/utils/sql_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag.egg-info/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5720 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/SOURCES.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/dependency_links.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        7 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/top_level.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      106 2022-09-01 15:05:05.000000 miacag-0.0.82/pyproject.toml
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      524 2023-05-26 10:09:43.438565 miacag-0.0.82/setup.cfg
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.284072 miacag-0.0.83/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-01 15:05:05.000000 miacag-0.0.83/LICENSE
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      129 2022-09-01 15:05:05.000000 miacag-0.0.83/MANIFEST.in
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-06-21 13:42:39.284072 miacag-0.0.83/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      111 2022-10-20 03:13:52.000000 miacag-0.0.83/README.md
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.264072 miacag-0.0.83/miacag/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.264072 miacag-0.0.83/miacag/configs/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/configs/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.264072 miacag-0.0.83/miacag/configs/classification/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.264072 miacag-0.0.83/miacag/configs/classification/_3D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/configs/classification/_3D/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.264072 miacag-0.0.83/miacag/configs/classification/_3D/lca_rca/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/configs/classification/_3D/lca_rca/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3800 2022-09-20 09:25:18.000000 miacag-0.0.83/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.264072 miacag-0.0.83/miacag/configs/classification/_3D/stenosis_detection_rca/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9668 2022-09-20 09:25:18.000000 miacag-0.0.83/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/configs/classification/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      823 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/configs/config.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3229 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/configs/options.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      881 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/configs/update_configs.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.268072 miacag-0.0.83/miacag/dataloader/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.268072 miacag-0.0.83/miacag/dataloader/Classification/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.268072 miacag-0.0.83/miacag/dataloader/Classification/_2D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.83/miacag/dataloader/Classification/_2D/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12802 2022-11-01 13:34:24.000000 miacag-0.0.83/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    14704 2023-06-12 11:17:44.000000 miacag-0.0.83/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    14443 2023-06-12 06:51:35.000000 miacag-0.0.83/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil_fast.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    80089 2023-06-12 18:45:31.000000 miacag-0.0.83/miacag/dataloader/Classification/_2D/dataset_mil_2d.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.268072 miacag-0.0.83/miacag/dataloader/Classification/_3D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/Classification/_3D/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2088 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/Classification/_3D/dataloader_avi_video.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9593 2023-06-06 13:41:33.000000 miacag-0.0.83/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    24226 2023-05-19 09:12:51.000000 miacag-0.0.83/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    72019 2022-11-04 15:43:12.000000 miacag-0.0.83/miacag/dataloader/Classification/_3D/dataset_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/Classification/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9250 2023-06-12 12:04:38.000000 miacag-0.0.83/miacag/dataloader/Classification/get_dataloader_classification.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2440 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/DistributedWeightedSampler.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.268072 miacag-0.0.83/miacag/dataloader/Representation/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/Representation/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10772 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/Representation/get_dataloader_representation.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5611 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/dataloader/dataloader_base.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    24861 2023-06-21 11:28:36.000000 miacag-0.0.83/miacag/dataloader/dataloader_base_monai.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6369 2023-06-12 11:56:51.000000 miacag-0.0.83/miacag/dataloader/get_dataloader.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8311 2023-06-11 16:59:22.000000 miacag-0.0.83/miacag/features.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.268072 miacag-0.0.83/miacag/metrics/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/metrics/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1180 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/metrics/cumulativeSumming.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4969 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/metrics/metrics.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    14578 2023-06-07 05:00:08.000000 miacag-0.0.83/miacag/metrics/metrics_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    26641 2023-06-20 07:05:24.000000 miacag-0.0.83/miacag/metrics/survival_metrics.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.272072 miacag-0.0.83/miacag/model_utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9549 2023-05-15 17:03:06.000000 miacag-0.0.83/miacag/model_utils/GradCam_model.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/model_utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12143 2023-06-07 08:00:28.000000 miacag-0.0.83/miacag/model_utils/eval_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5173 2023-06-07 04:52:22.000000 miacag-0.0.83/miacag/model_utils/get_loss_func.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2023-05-19 08:49:06.000000 miacag-0.0.83/miacag/model_utils/get_optimizer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10929 2023-06-07 08:08:04.000000 miacag-0.0.83/miacag/model_utils/get_test_pipeline.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9286 2023-06-11 16:29:37.000000 miacag-0.0.83/miacag/model_utils/grad_cam_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15597 2023-06-07 09:44:23.000000 miacag-0.0.83/miacag/model_utils/predict_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1576 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/model_utils/scheduler.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      785 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/model_utils/siam_loss.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7563 2023-06-12 08:59:56.000000 miacag-0.0.83/miacag/model_utils/train_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.272072 miacag-0.0.83/miacag/models/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8635 2023-06-21 08:35:56.000000 miacag-0.0.83/miacag/models/BuildModel.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.272072 miacag-0.0.83/miacag/models/backbone_encoders/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/backbone_encoders/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.272072 miacag-0.0.83/miacag/models/backbone_encoders/tabular/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/backbone_encoders/tabular/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      212 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/backbone_encoders/tabular/base_encoders.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      670 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/cnns.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.272072 miacag-0.0.83/miacag/models/dino_utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-16 12:42:02.000000 miacag-0.0.83/miacag/models/dino_utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6468 2023-06-11 11:55:49.000000 miacag-0.0.83/miacag/models/dino_utils/dino_pretrained.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15116 2023-06-21 11:52:48.000000 miacag-0.0.83/miacag/models/get_encoder.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/mae_st_util/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-04-25 13:02:50.000000 miacag-0.0.83/miacag/models/mae_st_util/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3130 2023-04-25 13:03:31.000000 miacag-0.0.83/miacag/models/mae_st_util/logging.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6395 2023-04-25 13:05:51.000000 miacag-0.0.83/miacag/models/mae_st_util/models_vit.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4915 2023-04-25 13:44:14.000000 miacag-0.0.83/miacag/models/mae_st_util/video_vit.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12414 2023-06-21 11:30:12.000000 miacag-0.0.83/miacag/models/milmodel3d.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12926 2023-05-17 12:55:21.000000 miacag-0.0.83/miacag/models/milmodel_from_features.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1769 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/mlps.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13303 2023-05-15 17:03:06.000000 miacag-0.0.83/miacag/models/modeling_finetune.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13780 2023-05-15 17:03:06.000000 miacag-0.0.83/miacag/models/modeling_pretrain.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8591 2023-06-06 13:17:02.000000 miacag-0.0.83/miacag/models/modules.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13824 2023-05-15 17:03:06.000000 miacag-0.0.83/miacag/models/pretrained_vit.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/2D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.83/miacag/models/torchhub/2D/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/2D/r50/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.83/miacag/models/torchhub/2D/r50/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/2D+T/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/torchhub/2D+T/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/2D+T/mvit_base_16x4/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/2D+T/mvit_base_32x3/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/torchhub/2D+T/mvit_base_32x3/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/2D+T/r2plus1_18/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/torchhub/2D+T/r2plus1_18/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/models/torchhub/2D+T/x3d_s/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/torchhub/2D+T/x3d_s/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/models/torchhub/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    20482 2023-06-20 12:15:50.000000 miacag-0.0.83/miacag/models/vision_transformer.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/plots/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/plots/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1983 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/plots/angle_plotter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      408 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/plots/getDataFromPdf.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      795 2022-11-01 13:34:24.000000 miacag-0.0.83/miacag/plots/plot_histogram.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4724 2023-05-25 10:22:04.000000 miacag-0.0.83/miacag/plots/plot_pathology_treatment_pred.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4143 2023-06-20 06:13:43.000000 miacag-0.0.83/miacag/plots/plot_predict_coronary_pathology.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15341 2023-06-20 06:26:18.000000 miacag-0.0.83/miacag/plots/plot_roc_auc_all.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1277 2022-11-01 13:34:24.000000 miacag-0.0.83/miacag/plots/plot_scatter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1245 2023-01-27 08:30:25.000000 miacag-0.0.83/miacag/plots/plot_test.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1847 2023-06-11 20:34:28.000000 miacag-0.0.83/miacag/plots/plot_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    33682 2023-06-11 19:55:44.000000 miacag-0.0.83/miacag/plots/plotter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4543 2023-01-27 08:26:48.000000 miacag-0.0.83/miacag/plots/query_plot_agg_max.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.276072 miacag-0.0.83/miacag/postprocessing/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/postprocessing/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3593 2022-12-16 18:58:11.000000 miacag-0.0.83/miacag/postprocessing/aggregate_pr_group.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1880 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/postprocessing/append_results.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4331 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/postprocessing/count_stenosis_pr_group.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5354 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/postprocessing/estimate_vessel_disease.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2527 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/predictor.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/preprocessing/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1319 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/add_columns.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1412 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/copy_column.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1321 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/copy_table.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/datasetFingerpring.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    21523 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/datasetFingerprint.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3232 2023-06-11 04:34:30.000000 miacag-0.0.83/miacag/preprocessing/labels_map.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7064 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/pre_process.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/preprocessing/process_labels/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/process_labels/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-12-16 18:59:24.000000 miacag-0.0.83/miacag/preprocessing/process_labels/process_dominance.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15711 2023-03-02 17:26:57.000000 miacag-0.0.83/miacag/preprocessing/process_labels/process_total_occ.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3519 2023-06-06 12:35:35.000000 miacag-0.0.83/miacag/preprocessing/split_train_val.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2344 2022-12-16 18:58:52.000000 miacag-0.0.83/miacag/preprocessing/transform_missing_floats.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2521 2022-12-16 18:58:58.000000 miacag-0.0.83/miacag/preprocessing/transform_stenosis.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4825 2023-06-11 04:43:49.000000 miacag-0.0.83/miacag/preprocessing/transform_thresholds.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2591 2022-12-16 18:59:17.000000 miacag-0.0.83/miacag/preprocessing/transform_total_occlusion.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/preprocessing/utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1402 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/preprocessing/utils/check_experiments.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/scripts/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13571 2023-01-10 16:02:18.000000 miacag-0.0.83/miacag/scripts/aggregate_and_plot.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/angiography_classifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/scripts/angiography_classifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4842 2023-05-19 07:46:19.000000 miacag-0.0.83/miacag/scripts/angiography_classifier/predict_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13266 2023-05-23 10:33:43.000000 miacag-0.0.83/miacag/scripts/angiography_classifier/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/angiography_classifier_stenosis_identifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2206 2023-05-19 07:46:41.000000 miacag-0.0.83/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3675 2023-02-28 09:02:39.000000 miacag-0.0.83/miacag/scripts/compare_PCI_notPCI.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6510 2023-03-02 16:02:03.000000 miacag-0.0.83/miacag/scripts/predict_patologi_eyeball_vs_estimated.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/pretraining_downstreams/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-15 17:03:06.000000 miacag-0.0.83/miacag/scripts/pretraining_downstreams/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    26111 2023-06-21 11:46:30.000000 miacag-0.0.83/miacag/scripts/pretraining_downstreams/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/stenosis_identifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/scripts/stenosis_identifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    22900 2023-05-19 07:46:49.000000 miacag-0.0.83/miacag/scripts/stenosis_identifier/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/stenosis_identifier_mil/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/scripts/stenosis_identifier_mil/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    16479 2023-05-19 07:46:55.000000 miacag-0.0.83/miacag/scripts/stenosis_identifier_mil/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/stenosis_regression/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/scripts/stenosis_regression/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    27314 2023-05-19 07:47:03.000000 miacag-0.0.83/miacag/scripts/stenosis_regression/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/scripts/stenosis_regression_full/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/scripts/stenosis_regression_full/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7325 2023-05-19 07:47:08.000000 miacag-0.0.83/miacag/scripts/stenosis_regression_full/submit_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2933 2023-05-19 08:24:26.000000 miacag-0.0.83/miacag/tester.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/tests/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/tests/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2109 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/tests/test_sql_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4891 2023-06-12 07:02:45.000000 miacag-0.0.83/miacag/trainer.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.280072 miacag-0.0.83/miacag/utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3438 2023-06-06 14:24:44.000000 miacag-0.0.83/miacag/utils/common_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1313 2022-09-01 15:05:05.000000 miacag-0.0.83/miacag/utils/script_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6241 2023-06-11 04:23:29.000000 miacag-0.0.83/miacag/utils/sql_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4083 2023-06-07 08:14:39.000000 miacag-0.0.83/miacag/utils/survival_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-06-21 13:42:39.264072 miacag-0.0.83/miacag.egg-info/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-06-21 13:42:39.000000 miacag-0.0.83/miacag.egg-info/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5952 2023-06-21 13:42:39.000000 miacag-0.0.83/miacag.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-06-21 13:42:39.000000 miacag-0.0.83/miacag.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        7 2023-06-21 13:42:39.000000 miacag-0.0.83/miacag.egg-info/top_level.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      106 2022-09-01 15:05:05.000000 miacag-0.0.83/pyproject.toml
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      524 2023-06-21 13:42:39.284072 miacag-0.0.83/setup.cfg
```

### Comparing `miacag-0.0.82/LICENSE` & `miacag-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/PKG-INFO` & `miacag-0.0.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miacag
-Version: 0.0.82
+Version: 0.0.83
 Summary: miacag angio DL tools
 Home-page: https://github.com/ChristianEschen/miacag
 Author: Christian Eschen
 Author-email: christian_eschen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml` & `miacag-0.0.83/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml` & `miacag-0.0.83/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/configs/config.py` & `miacag-0.0.83/miacag/configs/config.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/configs/options.py` & `miacag-0.0.83/miacag/configs/options.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/configs/update_configs.py` & `miacag-0.0.83/miacag/configs/update_configs.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py` & `miacag-0.0.83/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py` & `miacag-0.0.83/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil_fast.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,21 @@
             df,
             config)
         if config['weighted_sampler'] == 'True':
             self.getSampler()
         self.features = self.get_input_features(self.df)
         self.set_data_path(self.features)
         self.df = reorder_rows(self.df)
+        if self.config['loss']['name'][0] == 'NNL':
+            event = ['event']
+        else:
+            event = []
         self.data = self.df[
             self.features + config['labels_names'] +
-            ['rowid', "SOPInstanceUID"]]
+            ['rowid', "SOPInstanceUID"] + event]
         self.data = self.data.to_dict('records')
 
     def __call__(self):
         # define transforms for image
 
         train_transforms = [
                 LoadImaged(keys=self.features),
@@ -183,19 +187,22 @@
     def __init__(self, df, config):
         super(val_monai_classification_loader, self).__init__(df,
                                                               config)
 
         self.features = self.get_input_features(self.df)
         self.set_data_path(self.features)
         self.df = reorder_rows(self.df)
-
+        if self.config['loss']['name'][0] == 'NNL':
+            event = ['event']
+        else:
+            event = []
         self.data = self.df[
             self.features + config['labels_names'] +
             ['rowid', "SOPInstanceUID", "PatientID",
-             "StudyInstanceUID", "SeriesInstanceUID"]]
+             "StudyInstanceUID", "SeriesInstanceUID"] + event]
         self.data = self.data.to_dict('records')
 
 
     def __call__(self):
         val_transforms = [
                 LoadImaged(keys=self.features),
                 EnsureChannelFirstD(keys=self.features),
```

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/_2D/dataset_mil_2d.py` & `miacag-0.0.83/miacag/dataloader/Classification/_3D/dataset_mil.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,36 +46,42 @@
     tqdm, has_tqdm = optional_import("tqdm", "4.47.0", min_version, "tqdm")
 
 lmdb, _ = optional_import("lmdb")
 pd, _ = optional_import("pandas")
 from monai.transforms import CenterSpatialCropd, RandSpatialCropd, SpatialPad
 
 
+def cropperCenter(key, h, w, d):
+    cropper = CenterSpatialCropd(
+                    keys=key,
+                    roi_size=[h, w, d])
+    return cropper
+
 def div_diff_tuple(diff):
     val1 = diff%2
     if val1 == 0:
         return int(diff/2), int(diff/2)
     else:
         return int(diff/2)+1, int(diff/2)
 
 def get_random_patches_cache(stacked_data, config):
     nr_patches = config['loaders']['nr_patches_max_cache']
     if nr_patches != "None":
-        if stacked_data.shape[-1] <= nr_patches:
-            diff = nr_patches - stacked_data.shape[-1]
+        if stacked_data.shape[0] <= nr_patches:
+            diff = nr_patches - stacked_data.shape[0]
             pad_tuple = div_diff_tuple(diff)
             stacked_data = torch.nn.functional.pad(
                 stacked_data,
-                (pad_tuple[0], pad_tuple[1], 0, 0, 0, 0, 0, 0),
+                (0, 0, 0, 0, 0, 0, 0, 0, pad_tuple[0], pad_tuple[1]),
                 "constant", 0)
             return stacked_data
         else:
             idx = random.sample(
-                range(stacked_data.shape[-1]), nr_patches)
-            stacked_data = stacked_data[:, :, :, idx]
+                range(stacked_data.shape[0]), nr_patches)
+            stacked_data = stacked_data[idx]
             return stacked_data
     else:
         return stacked_data
 
 
 def get_random_patches(stacked_data, config):
     nr_patches = config['loaders']['nr_patches']
@@ -128,51 +134,75 @@
     def __len__(self) -> int:
         return len(self.data)
 
     def _transform(self, index: int):
         """
         Fetch single data item from `self.data`.
         """
+        cropper = cropperCenter(self.features[0],
+                                self.config['loaders']['Crop_height'],
+                                self.config['loaders']['Crop_width'],
+                                self.config['loaders']['Crop_depth']
+                                )
         data_i = self.data[index]
         #post_trans = Compose([ToTensord(keys=["img"])])
         data_i_list = []
 
         for data_i_i in data_i[self.features[0]]:
             data_i_i = {
                 self.features[0]: data_i_i}
             for n in self.config['labels_names']:
 
                 data_i_i[n] = data_i[n]
+            # data_i_i = apply_transform(
+            #     self.transform, data_i_i) \
+            #     if self.transform is not None else data_i
             for _transform in self.transform.transforms:
                 # execute all the deterministic transforms
                 if isinstance(_transform, Randomizable) \
                         or not isinstance(_transform, Transform):
                     break
                 # this is to be consistent with CacheDataset even -
                 # though it's not in a multi-thread situation.
                 _xform = deepcopy(_transform) if \
                     isinstance(_transform, ThreadUnsafe) else _transform
                 data_i_i = apply_transform(_xform, data_i_i)
 
-        
-            data_i_list.append(data_i_i)
-        stacked_data = torch.concat(
-            [i[self.features[0]] for i in data_i_list], dim=3)
-        # stacked_data = get_random_patches_cache(
-        #     stacked_data,
-        #     self.config)
-        stacked_data = stacked_data.permute(3, 0, 1, 2)
+            data_i_list.append(cropper(data_i_i))
+        stacked_data = torch.stack([i['DcmPathFlatten'] for i in data_i_list], dim=0)
         data_i_i['inputs'] = stacked_data
         data_i_i["rowid"] = data_i["rowid"]
         data_i_i['DcmPathFlatten_paths'] = data_i['DcmPathFlatten']
         data_i_i["SOPInstanceUID"] = data_i["SOPInstanceUID"]
         data_i_i["SeriesInstanceUID"] = data_i["SeriesInstanceUID"]
         data_i_i["StudyInstanceUID"] = data_i["StudyInstanceUID"]
         data_i_i["PatientID"] = data_i["PatientID"]
         data_i_i['inputs'] = stacked_data
+       # data_i_i['DcmPathFlatten_paths'] = data_i['DcmPathFlatten']
+        data_i_i["rowid"] = data_i["rowid"]
+        if self.config['loaders']['val_method']['saliency'] == 'True':
+            crop = CenterSpatialCropd(
+                        keys='inputs',
+                        roi_size=[
+                            -1,
+                            self.config['loaders']['Crop_height'],
+                            self.config['loaders']['Crop_width'],
+                            self.config['loaders']['Crop_depth']])
+        else:
+            crop = RandSpatialCropd(
+                keys='inputs',
+                roi_size=[
+                    -1,
+                    self.config['loaders']['Crop_height'],
+                    self.config['loaders']['Crop_width'],
+                    self.config['loaders']['Crop_depth']],
+                random_size=False)
+        data_i_i['inputs'] = crop(data_i_i)['inputs']
+       # data_i_i["SOPInstanceUID"] = data_i["SOPInstanceUID"]
+       
         if self.config['loaders']['val_method']['max_patches'] != 'None':
             max_p = self.config['loaders']['val_method']['max_patches']
             data_i_i['inputs'] = data_i_i['inputs'][0:max_p]
         return data_i_i
 
     def __getitem__(self, index: Union[int, slice, Sequence[int]]):
         """
@@ -338,14 +368,19 @@
         Process the data from original state up to the first random element.
         Args:
             item_transformed: The data to be transformed
         Returns:
             the transformed element up to the first identified
             random transform object
         """
+        cropper = cropperCenter(self.features[0],
+                                self.config['loaders']['Crop_height'],
+                                self.config['loaders']['Crop_width'],
+                                self.config['loaders']['Crop_depth']
+                                )
         data_i_list = []
        # data_i = self.data[idx]
         for data_i_i in item_transformed[self.features[0]]:
             data_i_i = {
                 self.features[0]: data_i_i}
             for n in self.config['labels_names']:
                 data_i_i[n] = item_transformed[n]
@@ -356,30 +391,27 @@
                         or not isinstance(_transform, Transform):
                     break
                 # this is to be consistent with CacheDataset even -
                 # though it's not in a multi-thread situation.
                 _xform = deepcopy(_transform) if \
                     isinstance(_transform, ThreadUnsafe) else _transform
                 data_i_i = apply_transform(_xform, data_i_i)
-            data_i_list.append(data_i_i)
-        # stacked_data = torch.stack(
-        #     [i[self.features[0]] for i in data_i_list], dim=0)
-        stacked_data = torch.concat(
-            [i[self.features[0]] for i in data_i_list], dim=3)
-        # stacked_data = get_random_patches_cache(
-        #     stacked_data,
-        #     self.config)
-        stacked_data = stacked_data.permute(3, 0, 1, 2)
+            data_i_list.append(cropper(data_i_i))
+        stacked_data = torch.stack(
+            [i[self.features[0]] for i in data_i_list], dim=0)
         data_i_i['inputs'] = stacked_data
         data_i_i["rowid"] = item_transformed["rowid"]
         data_i_i['DcmPathFlatten_paths'] = item_transformed['DcmPathFlatten']
         data_i_i["SOPInstanceUID"] = item_transformed["SOPInstanceUID"]
         data_i_i["SeriesInstanceUID"] = item_transformed["SeriesInstanceUID"]
         data_i_i["StudyInstanceUID"] = item_transformed["StudyInstanceUID"]
         data_i_i["PatientID"] = item_transformed["PatientID"]
+        if self.config['loaders']['val_method']['max_patches'] != 'None':
+            max_p = self.config['loaders']['val_method']['max_patches']
+            data_i_i['inputs'] = data_i_i['inputs'][0:max_p]
 
         return data_i_i
 
     def _post_transform(self, item_transformed):
         """
         Process the data from before the first random transform to the final state ready for evaluation.
         Args:
@@ -390,45 +422,33 @@
         if not isinstance(self.transform, Compose):
             raise ValueError("transform must be an instance of monai.transforms.Compose.")
         start_post_randomize_run = False
        # for _transform in self.transform.transforms:
         if self.config['loaders']['mode'] not in ['testing', 'prediction']:
             raise ValueError(
                 "persistent loaders is only supported for prediction mode")
-       # if 
-        # if self.config['loaders']['val_method']['saliency'] == 'True':
-        #     crop = CenterSpatialCropd(
-        #                 keys='inputs',
-        #                 roi_size=[
-        #                     -1,
-        #                     self.config['loaders']['Crop_height'],
-        #                     self.config['loaders']['Crop_width'],
-        #                     self.config['loaders']['Crop_depth']])
-        # else:
-        #     crop = RandSpatialCropd(
-        #         keys='inputs',
-        #         roi_size=[
-        #             -1,
-        #             self.config['loaders']['Crop_height'],
-        #             self.config['loaders']['Crop_width'],
-        #             self.config['loaders']['Crop_depth']],
-        #         random_size=False)
-        item_transformed['inputs'] = item_transformed['inputs']
-
-            # persistant 
-            # if (
-            #     start_post_randomize_run
-            #     or isinstance(_transform, Randomizable)
-            #     or not isinstance(_transform, Transform)
-            # ):
-            #     start_post_randomize_run = True
-            # if isinstance(_transform, Randomizable) or not isinstance(_transform, Transform):
-            #     item_transformed = apply_transform(_transform, item_transformed)
-       # print('ugly hack for prediction mode with mil')
-       # item_transformed['inputs'] = item_transformed['inputs'][:,:, :,:, 0:self.config['loaders']['Crop_depth']]
+        if self.config['loaders']['val_method']['saliency'] == 'True':
+            crop = CenterSpatialCropd(
+                        keys='inputs',
+                        roi_size=[
+                            -1,
+                            self.config['loaders']['Crop_height'],
+                            self.config['loaders']['Crop_width'],
+                            self.config['loaders']['Crop_depth']])
+        else:
+            crop = RandSpatialCropd(
+                keys='inputs',
+                roi_size=[
+                    -1,
+                    self.config['loaders']['Crop_height'],
+                    self.config['loaders']['Crop_width'],
+                    self.config['loaders']['Crop_depth']],
+                random_size=False)
+        item_transformed['inputs'] = crop(item_transformed)['inputs']
+
         return item_transformed
 
     def _cachecheck(self, item_transformed):
         """
         A function to cache the expensive input data transform operations
         so that huge data sets (larger than computer memory) can be processed
         on the fly as needed, and intermediate results written to disk for
@@ -892,21 +912,20 @@
                 _xform = deepcopy(_transform) if isinstance(_transform, ThreadUnsafe) else _transform
                 if self.as_contiguous:
                     data_i_i = convert_to_contiguous(data_i_i, memory_format=torch.contiguous_format)
                 data_i_i = deepcopy(data_i_i)
                 data_i_i = apply_transform(_transform, data_i_i)
 
             #    transformed_i.append(data_i_i)
-            data_i_list.append(data_i_i)
+            data_i_list.append(cropper(data_i_i))
 
-        stacked_data = torch.concat([i[self.features[0]] for i in data_i_list], dim=3)
+        stacked_data = torch.stack([i[self.features[0]] for i in data_i_list], dim=0)
         stacked_data = get_random_patches_cache(
             stacked_data,
             self.config)
-        stacked_data = stacked_data.permute(3, 0, 1, 2)
         data_i_i[self.features[0]] = stacked_data
 
         if self.as_contiguous:
             data_i_i = convert_to_contiguous(data_i_i, memory_format=torch.contiguous_format)
         data_i_i["rowid"] = data_i["rowid"]
        # data_i_i['DcmPathFlatten_paths'] = data_i['DcmPathFlatten']
        # data_i_i["SOPInstanceUID"] = data_i["SOPInstanceUID"]
```

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_avi_video.py` & `miacag-0.0.83/miacag/dataloader/Classification/_3D/dataloader_avi_video.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py` & `miacag-0.0.83/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         super(base_monai_loader, self).__init__(
             df,
             config)
         if config['weighted_sampler'] == 'True':
             self.getSampler()
         self.features = self.get_input_features(self.df)
         self.set_data_path(self.features)
-        self.data = self.df[self.features + config['labels_names'] + ['rowid']]
+        self.data = self.df[self.features + config['labels_names'] + ['rowid'] + ['event']]
         self.data = self.data.to_dict('records')
 
     def transformations(self):
         self.transforms = [
             LoadImaged(keys=self.features),
             EnsureChannelFirstD(keys=self.features),
             self.resampleORresize(),
```

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py` & `miacag-0.0.83/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataset_mil.py` & `miacag-0.0.83/miacag/dataloader/Classification/_2D/dataset_mil_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import os
 
 import collections.abc
 from curses.ascii import SO
 import math
 import pickle
 import shutil
 import sys
@@ -33,55 +33,51 @@
 from torch.utils.data import Subset
 
 from monai.data.utils import SUPPORTED_PICKLE_MOD, convert_tables_to_dicts, pickle_hashing
 from monai.transforms import Compose, Randomizable, ThreadUnsafe, Transform, apply_transform, convert_to_contiguous
 from monai.utils import MAX_SEED, deprecated_arg, get_seed, look_up_option, min_version, optional_import
 from monai.utils.misc import first
 from torch.utils.data.dataloader import default_collate
-
+import monai
 if TYPE_CHECKING:
     from tqdm import tqdm
 
     has_tqdm = True
 else:
     tqdm, has_tqdm = optional_import("tqdm", "4.47.0", min_version, "tqdm")
 
 lmdb, _ = optional_import("lmdb")
 pd, _ = optional_import("pandas")
 from monai.transforms import CenterSpatialCropd, RandSpatialCropd, SpatialPad
 
-
-def cropperCenter(key, h, w, d):
-    cropper = CenterSpatialCropd(
-                    keys=key,
-                    roi_size=[h, w, d])
-    return cropper
+def replicate_list(lst, m):
+    return (lst * ((m // len(lst)) + 1))[:m]
 
 def div_diff_tuple(diff):
     val1 = diff%2
     if val1 == 0:
         return int(diff/2), int(diff/2)
     else:
         return int(diff/2)+1, int(diff/2)
 
 def get_random_patches_cache(stacked_data, config):
     nr_patches = config['loaders']['nr_patches_max_cache']
     if nr_patches != "None":
-        if stacked_data.shape[0] <= nr_patches:
-            diff = nr_patches - stacked_data.shape[0]
+        if stacked_data.shape[-1] <= nr_patches:
+            diff = nr_patches - stacked_data.shape[-1]
             pad_tuple = div_diff_tuple(diff)
             stacked_data = torch.nn.functional.pad(
                 stacked_data,
-                (0, 0, 0, 0, 0, 0, 0, 0, pad_tuple[0], pad_tuple[1]),
+                (pad_tuple[0], pad_tuple[1], 0, 0, 0, 0, 0, 0),
                 "constant", 0)
             return stacked_data
         else:
             idx = random.sample(
-                range(stacked_data.shape[0]), nr_patches)
-            stacked_data = stacked_data[idx]
+                range(stacked_data.shape[-1]), nr_patches)
+            stacked_data = stacked_data[:, :, :, idx]
             return stacked_data
     else:
         return stacked_data
 
 
 def get_random_patches(stacked_data, config):
     nr_patches = config['loaders']['nr_patches']
@@ -98,14 +94,201 @@
             idx = random.sample(
                 range(stacked_data.shape[0]), nr_patches)
             stacked_data = stacked_data[idx]
             return stacked_data
     else:
         return stacked_data
 
+class MILDataset(_TorchDataset):
+    """
+    A generic dataset with a length property and an optional callable data transform
+    when fetching a data sample.
+    If passing slicing indices, will return a PyTorch Subset, for example: `data: Subset = dataset[1:4]`,
+    for more details, please check: https://pytorch.org/docs/stable/data.html#torch.utils.data.Subset
+
+    For example, typical input data can be a list of dictionaries::
+
+        [{                            {                            {
+             'img': 'image1.nii.gz',      'img': 'image2.nii.gz',      'img': 'image3.nii.gz',
+             'seg': 'label1.nii.gz',      'seg': 'label2.nii.gz',      'seg': 'label3.nii.gz',
+             'extra': 123                 'extra': 456                 'extra': 789
+         },                           },                           }]
+    """
+
+    def __init__(self, config: Sequence, features: Sequence,
+                 data: Sequence, transform: Optional[Callable] = None,
+                 phase: str = 'train') -> None:
+        """
+        Args:
+            data: input data to load and transform to generate dataset for model.
+            transform: a callable data transform on input data.
+
+        """
+        self.data = data
+        self.transform = transform
+        self.features = features
+        self.config = config
+        self.phase = phase
+
+        self.pre_transforms = self.get_pretransformers()
+        self.post_transformations = self.post_transforms()
+
+    def __len__(self) -> int:
+        return len(self.data)
+
+    def get_pretransformers(self):
+        pre_transforms = [
+            monai.transforms.LoadImaged(keys=self.features),
+            monai.transforms.EnsureChannelFirstD(keys=self.features),
+            monai.transforms.RandSpatialCropd(
+                keys=self.features,
+                roi_size=[
+                    -1,
+                    -1,
+                    1],
+                random_size=False),
+            ]
+        if self.phase == 'train':
+            pre_transforms = pre_transforms + [
+                monai.transforms.RandRotate90d(
+                self.features, prob=0.1, max_k=3,
+                spatial_axes=(0, 1))]
+        pre_transforms = Compose(pre_transforms)
+        return pre_transforms
+       # self.pre_transforms = pre_transforms
+    
+    def post_transforms(self):
+        if self.config['cpu'] == 'True':
+            device = 'cpu'
+        else:
+            device = "cuda:{}".format(os.environ['LOCAL_RANK'])
+        post_transforms = [
+            monai.transforms.Resized(
+                        keys=self.features,
+                        spatial_size=(
+                                    self.config['loaders']['Resize_height'],
+                                    self.config['loaders']['Resize_width'],
+                                    self.config['loaders']['nr_patches'])),
+           # monai.transforms.DeleteItemsd(keys=self.features[0]+"_meta_dict.[0-9]\\|[0-9]", use_re=True),
+            monai.transforms.SpatialPadd(
+                keys=self.features,
+                spatial_size=[self.config['loaders']['Crop_height'],
+                              self.config['loaders']['Crop_width'],
+                              self.config['loaders']['nr_patches']]),
+            monai.transforms.RepeatChanneld(keys=self.features, repeats=3),
+            monai.transforms.ScaleIntensityd(keys=self.features),
+            monai.transforms.NormalizeIntensityd(
+                keys=self.features,
+                subtrahend=(0.485, 0.456, 0.406),
+                divisor=(0.229, 0.224, 0.225),
+                channel_wise=True),
+           # monai.transforms.ToDeviced(keys=self.features, device=device)
+            ]
+        
+        if self.phase == 'train':
+            phase_transforms = [monai.transforms.RandAffined(
+                        keys=self.features,
+                        mode="bilinear",
+                        prob=0.2,
+                        spatial_size=(self.config['loaders']['Resize_height'],
+                                      self.config['loaders']['Resize_width'],
+                                      self.config['loaders']['nr_patches']),
+                        scale_range=(0.15, 0.15, 0),
+                        padding_mode="zeros"),
+            monai.transforms.RandAffined(
+                    keys=self.features,
+                    mode="bilinear",
+                    prob=0.2,
+                    spatial_size=(self.config['loaders']['Resize_height'],
+                                  self.config['loaders']['Resize_width'],
+                                  self.config['loaders']['nr_patches']),
+                    translate_range=(
+                         int(0.22*self.config['loaders']['Resize_height']),
+                         int(0.22*self.config['loaders']['Resize_width']),
+                         int(0.5*self.config['loaders']['nr_patches'])),
+                    padding_mode="zeros"),
+            monai.transforms.RandAffined(
+                        keys=self.features,
+                        mode="bilinear",
+                        prob=0.2,
+                        rotate_range=(0, 0, 0.17),
+                        spatial_size=(self.config['loaders']['Resize_height'],
+                                      self.config['loaders']['Resize_width'],
+                                      self.config['loaders']['nr_patches']),
+                        padding_mode="zeros"),]
+        else:
+            phase_transforms = []
+
+        post_transforms = post_transforms + phase_transforms + [
+            monai.transforms.ConcatItemsd(keys=self.features, name='inputs'),
+            monai.transforms.DeleteItemsd(keys=self.features),
+            ]
+        post_transforms = Compose(post_transforms)
+        return post_transforms
+
+    def _transform(self, index: int):
+        """
+        Fetch single data item from `self.data`.
+        """
+        data_i = self.data[index]
+        #post_trans = Compose([ToTensord(keys=["img"])])
+        data_i_list = []
+        # replicate list
+        data_i['DcmPathFlatten'] = replicate_list(data_i['DcmPathFlatten'], self.config['loaders']['nr_patches'])
+
+        data_i["SOPInstanceUID"] = replicate_list(data_i["SOPInstanceUID"], self.config['loaders']['nr_patches'])
+        data_i["SeriesInstanceUID"] = replicate_list(data_i["SeriesInstanceUID"], self.config['loaders']['nr_patches'])
+        data_i["StudyInstanceUID"] = replicate_list(data_i["StudyInstanceUID"], self.config['loaders']['nr_patches'])
+
+
+        # start while loop. Should stop when all patches are loaded
+        while len(data_i_list) < self.config['loaders']['nr_patches']:
+            for data_i_i in data_i[self.features[0]]:
+                data_i_i = {
+                    self.features[0]: data_i_i}
+                for n in self.config['labels_names']:
+
+                    data_i_i[n] = data_i[n]
+                 #   data_i_i[n] = self.pre_transforms(data_i_i)
+                    data_idx = self.pre_transforms(data_i_i)
+                    data_i_list.append(data_idx)
+        stacked_data = torch.concat(
+            [i[self.features[0]] for i in data_i_list], dim=3)
+        data_i_i['DcmPathFlatten'] = stacked_data
+        data_i_i = self.post_transformations(data_i_i)
+        
+        # stacked_data = get_random_patches_cache(
+        #     stacked_data,
+        #     self.config)
+        data_i_i['inputs'] = data_i_i['inputs'].permute(3, 0, 1, 2)
+        #data_i_i['inputs'] = stacked_data
+        data_i_i["rowid"] = data_i["rowid"]
+        if self.config['loss']['name'][0] == 'NNL':
+            data_i_i["event"] = data_i["event"]
+        data_i_i['DcmPathFlatten_paths'] = data_i['DcmPathFlatten']
+        data_i_i["SOPInstanceUID"] = data_i["SOPInstanceUID"]
+        data_i_i["SeriesInstanceUID"] = data_i["SeriesInstanceUID"]
+        data_i_i["StudyInstanceUID"] = data_i["StudyInstanceUID"]
+        data_i_i["PatientID"] = data_i["PatientID"]
+      #  if self.config['loaders']['val_method']['max_patches'] != 'None':
+       #     max_p = self.config['loaders']['val_method']['max_patches']
+       #     data_i_i['inputs'] = data_i_i['inputs'][0:max_p]
+        return data_i_i
+
+    def __getitem__(self, index: Union[int, slice, Sequence[int]]):
+        if isinstance(index, slice):
+            # dataset[:42]
+            start, stop, step = index.indices(len(self))
+            indices = range(start, stop, step)
+            return Subset(dataset=self, indices=indices)
+        if isinstance(index, collections.abc.Sequence):
+            # dataset[[1, 3, 4]]
+            return Subset(dataset=self, indices=index)
+        return self._transform(index)
+
 
 class Dataset(_TorchDataset):
     """
     A generic dataset with a length property and an optional callable data transform
     when fetching a data sample.
     If passing slicing indices, will return a PyTorch Subset, for example: `data: Subset = dataset[1:4]`,
     for more details, please check: https://pytorch.org/docs/stable/data.html#torch.utils.data.Subset
@@ -134,75 +317,53 @@
     def __len__(self) -> int:
         return len(self.data)
 
     def _transform(self, index: int):
         """
         Fetch single data item from `self.data`.
         """
-        cropper = cropperCenter(self.features[0],
-                                self.config['loaders']['Crop_height'],
-                                self.config['loaders']['Crop_width'],
-                                self.config['loaders']['Crop_depth']
-                                )
         data_i = self.data[index]
         #post_trans = Compose([ToTensord(keys=["img"])])
         data_i_list = []
 
         for data_i_i in data_i[self.features[0]]:
             data_i_i = {
                 self.features[0]: data_i_i}
             for n in self.config['labels_names']:
 
                 data_i_i[n] = data_i[n]
-            # data_i_i = apply_transform(
-            #     self.transform, data_i_i) \
-            #     if self.transform is not None else data_i
             for _transform in self.transform.transforms:
                 # execute all the deterministic transforms
                 if isinstance(_transform, Randomizable) \
                         or not isinstance(_transform, Transform):
                     break
                 # this is to be consistent with CacheDataset even -
                 # though it's not in a multi-thread situation.
                 _xform = deepcopy(_transform) if \
                     isinstance(_transform, ThreadUnsafe) else _transform
                 data_i_i = apply_transform(_xform, data_i_i)
 
-            data_i_list.append(cropper(data_i_i))
-        stacked_data = torch.stack([i['DcmPathFlatten'] for i in data_i_list], dim=0)
+        
+            data_i_list.append(data_i_i)
+        stacked_data = torch.concat(
+            [i[self.features[0]] for i in data_i_list], dim=3)
+        # stacked_data = get_random_patches_cache(
+        #     stacked_data,
+        #     self.config)
+        stacked_data = stacked_data.permute(3, 0, 1, 2)
         data_i_i['inputs'] = stacked_data
         data_i_i["rowid"] = data_i["rowid"]
+        if self.config['loss']['name'][0] == 'NNL':
+            data_i_i["event"] = data_i["event"]
         data_i_i['DcmPathFlatten_paths'] = data_i['DcmPathFlatten']
         data_i_i["SOPInstanceUID"] = data_i["SOPInstanceUID"]
         data_i_i["SeriesInstanceUID"] = data_i["SeriesInstanceUID"]
         data_i_i["StudyInstanceUID"] = data_i["StudyInstanceUID"]
         data_i_i["PatientID"] = data_i["PatientID"]
         data_i_i['inputs'] = stacked_data
-       # data_i_i['DcmPathFlatten_paths'] = data_i['DcmPathFlatten']
-        data_i_i["rowid"] = data_i["rowid"]
-        if self.config['loaders']['val_method']['saliency'] == 'True':
-            crop = CenterSpatialCropd(
-                        keys='inputs',
-                        roi_size=[
-                            -1,
-                            self.config['loaders']['Crop_height'],
-                            self.config['loaders']['Crop_width'],
-                            self.config['loaders']['Crop_depth']])
-        else:
-            crop = RandSpatialCropd(
-                keys='inputs',
-                roi_size=[
-                    -1,
-                    self.config['loaders']['Crop_height'],
-                    self.config['loaders']['Crop_width'],
-                    self.config['loaders']['Crop_depth']],
-                random_size=False)
-        data_i_i['inputs'] = crop(data_i_i)['inputs']
-       # data_i_i["SOPInstanceUID"] = data_i["SOPInstanceUID"]
-       
         if self.config['loaders']['val_method']['max_patches'] != 'None':
             max_p = self.config['loaders']['val_method']['max_patches']
             data_i_i['inputs'] = data_i_i['inputs'][0:max_p]
         return data_i_i
 
     def __getitem__(self, index: Union[int, slice, Sequence[int]]):
         """
@@ -368,19 +529,14 @@
         Process the data from original state up to the first random element.
         Args:
             item_transformed: The data to be transformed
         Returns:
             the transformed element up to the first identified
             random transform object
         """
-        cropper = cropperCenter(self.features[0],
-                                self.config['loaders']['Crop_height'],
-                                self.config['loaders']['Crop_width'],
-                                self.config['loaders']['Crop_depth']
-                                )
         data_i_list = []
        # data_i = self.data[idx]
         for data_i_i in item_transformed[self.features[0]]:
             data_i_i = {
                 self.features[0]: data_i_i}
             for n in self.config['labels_names']:
                 data_i_i[n] = item_transformed[n]
@@ -391,27 +547,31 @@
                         or not isinstance(_transform, Transform):
                     break
                 # this is to be consistent with CacheDataset even -
                 # though it's not in a multi-thread situation.
                 _xform = deepcopy(_transform) if \
                     isinstance(_transform, ThreadUnsafe) else _transform
                 data_i_i = apply_transform(_xform, data_i_i)
-            data_i_list.append(cropper(data_i_i))
-        stacked_data = torch.stack(
-            [i[self.features[0]] for i in data_i_list], dim=0)
+            data_i_list.append(data_i_i)
+        # stacked_data = torch.stack(
+        #     [i[self.features[0]] for i in data_i_list], dim=0)
+        stacked_data = torch.concat(
+            [i[self.features[0]] for i in data_i_list], dim=3)
+        # stacked_data = get_random_patches_cache(
+        #     stacked_data,
+        #     self.config)
+        stacked_data = stacked_data.permute(3, 0, 1, 2)
         data_i_i['inputs'] = stacked_data
         data_i_i["rowid"] = item_transformed["rowid"]
+        data_i_i["event"] = item_transformed["event"]
         data_i_i['DcmPathFlatten_paths'] = item_transformed['DcmPathFlatten']
         data_i_i["SOPInstanceUID"] = item_transformed["SOPInstanceUID"]
         data_i_i["SeriesInstanceUID"] = item_transformed["SeriesInstanceUID"]
         data_i_i["StudyInstanceUID"] = item_transformed["StudyInstanceUID"]
         data_i_i["PatientID"] = item_transformed["PatientID"]
-        if self.config['loaders']['val_method']['max_patches'] != 'None':
-            max_p = self.config['loaders']['val_method']['max_patches']
-            data_i_i['inputs'] = data_i_i['inputs'][0:max_p]
 
         return data_i_i
 
     def _post_transform(self, item_transformed):
         """
         Process the data from before the first random transform to the final state ready for evaluation.
         Args:
@@ -422,33 +582,45 @@
         if not isinstance(self.transform, Compose):
             raise ValueError("transform must be an instance of monai.transforms.Compose.")
         start_post_randomize_run = False
        # for _transform in self.transform.transforms:
         if self.config['loaders']['mode'] not in ['testing', 'prediction']:
             raise ValueError(
                 "persistent loaders is only supported for prediction mode")
-        if self.config['loaders']['val_method']['saliency'] == 'True':
-            crop = CenterSpatialCropd(
-                        keys='inputs',
-                        roi_size=[
-                            -1,
-                            self.config['loaders']['Crop_height'],
-                            self.config['loaders']['Crop_width'],
-                            self.config['loaders']['Crop_depth']])
-        else:
-            crop = RandSpatialCropd(
-                keys='inputs',
-                roi_size=[
-                    -1,
-                    self.config['loaders']['Crop_height'],
-                    self.config['loaders']['Crop_width'],
-                    self.config['loaders']['Crop_depth']],
-                random_size=False)
-        item_transformed['inputs'] = crop(item_transformed)['inputs']
-
+       # if 
+        # if self.config['loaders']['val_method']['saliency'] == 'True':
+        #     crop = CenterSpatialCropd(
+        #                 keys='inputs',
+        #                 roi_size=[
+        #                     -1,
+        #                     self.config['loaders']['Crop_height'],
+        #                     self.config['loaders']['Crop_width'],
+        #                     self.config['loaders']['Crop_depth']])
+        # else:
+        #     crop = RandSpatialCropd(
+        #         keys='inputs',
+        #         roi_size=[
+        #             -1,
+        #             self.config['loaders']['Crop_height'],
+        #             self.config['loaders']['Crop_width'],
+        #             self.config['loaders']['Crop_depth']],
+        #         random_size=False)
+        item_transformed['inputs'] = item_transformed['inputs']
+
+            # persistant 
+            # if (
+            #     start_post_randomize_run
+            #     or isinstance(_transform, Randomizable)
+            #     or not isinstance(_transform, Transform)
+            # ):
+            #     start_post_randomize_run = True
+            # if isinstance(_transform, Randomizable) or not isinstance(_transform, Transform):
+            #     item_transformed = apply_transform(_transform, item_transformed)
+       # print('ugly hack for prediction mode with mil')
+       # item_transformed['inputs'] = item_transformed['inputs'][:,:, :,:, 0:self.config['loaders']['Crop_depth']]
         return item_transformed
 
     def _cachecheck(self, item_transformed):
         """
         A function to cache the expensive input data transform operations
         so that huge data sets (larger than computer memory) can be processed
         on the fly as needed, and intermediate results written to disk for
@@ -912,25 +1084,28 @@
                 _xform = deepcopy(_transform) if isinstance(_transform, ThreadUnsafe) else _transform
                 if self.as_contiguous:
                     data_i_i = convert_to_contiguous(data_i_i, memory_format=torch.contiguous_format)
                 data_i_i = deepcopy(data_i_i)
                 data_i_i = apply_transform(_transform, data_i_i)
 
             #    transformed_i.append(data_i_i)
-            data_i_list.append(cropper(data_i_i))
+            data_i_list.append(data_i_i)
 
-        stacked_data = torch.stack([i[self.features[0]] for i in data_i_list], dim=0)
+        stacked_data = torch.concat([i[self.features[0]] for i in data_i_list], dim=3)
         stacked_data = get_random_patches_cache(
             stacked_data,
             self.config)
+        stacked_data = stacked_data.permute(3, 0, 1, 2)
         data_i_i[self.features[0]] = stacked_data
 
         if self.as_contiguous:
             data_i_i = convert_to_contiguous(data_i_i, memory_format=torch.contiguous_format)
         data_i_i["rowid"] = data_i["rowid"]
+        if self.config['loss']['name'][0] == 'NNL':
+            data_i_i["event"] = data_i["event"]
        # data_i_i['DcmPathFlatten_paths'] = data_i['DcmPathFlatten']
        # data_i_i["SOPInstanceUID"] = data_i["SOPInstanceUID"]
 
         return data_i_i
 
 
     def _transform(self, index: int):
```

### Comparing `miacag-0.0.82/miacag/dataloader/Classification/get_dataloader_classification.py` & `miacag-0.0.83/miacag/dataloader/Classification/get_dataloader_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     def __init__(self, config) -> None:
         self.config = config
         self.df, self.connection = getDataFromDatabase(self.config)
         # if self.config['loaders']['mode'] != 'prediction':
         #     self.df = self.df.dropna(subset=config["labels_names"], how='any')
         if self.config['loaders']['mode'] == 'prediction':
             for col in self.config['labels_names']:
+                #try:
                 self.df[col].values[:] = 0
+                # except:
+                #     print('column not found')
+                #     pass
 
         if self.config['loaders']['mode'] in ['prediction', 'testing']:
             self.val_df = self.df
         else:
             self.train_df = self.df[self.df['phase'] == 'train']
             self.val_df = self.df[self.df['phase'] == 'val']
 
@@ -98,39 +102,30 @@
                 even_divisible=True,
                 shuffle=True)
             
         val_ds = val_monai_classification_loader(
                 self.val_df,
                 config)
         val_ds = val_ds()
-
-        # if config['task_type'] == 'mil_classification':
-        #     collate = list_data_collate_mil
-        # else:
-        #     collate = pad_list_data_collate
-        
         train_loader = ThreadDataLoader(
             train_ds,
             sampler=sampler,
             batch_size=config['loaders']['batchSize'],
             shuffle=False,
             num_workers=0, #config['num_workers'],
             collate_fn=pad_list_data_collate,
             pin_memory=False,) #True if config['cpu'] == "False" else False,)
-
-       # return train_loader, val_loader, train_ds, val_ds
         with torch.no_grad():
             val_loader = ThreadDataLoader(
                 val_ds,
                 batch_size=config['loaders']['batchSize'],
                 shuffle=False,
                 num_workers=0,
                 collate_fn=pad_list_data_collate, #pad_list_data_collate if config['loaders']['val_method']['type'] == 'sliding_window' else list_data_collate,
                 pin_memory=False,)
-      
         return train_loader, val_loader, train_ds, val_ds
 
     def get_classificationloader_patch_lvl_test(self, config):
         if config['loaders']['format'] == 'dicom':
             if config['task_type'] in ['classification', "regression"]:
                 from miacag.dataloader.Classification._3D. \
                     dataloader_monai_classification_3D import \
```

### Comparing `miacag-0.0.82/miacag/dataloader/DistributedWeightedSampler.py` & `miacag-0.0.83/miacag/dataloader/DistributedWeightedSampler.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/dataloader/Representation/get_dataloader_representation.py` & `miacag-0.0.83/miacag/dataloader/Representation/get_dataloader_representation.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/dataloader/dataloader_base.py` & `miacag-0.0.83/miacag/dataloader/dataloader_base.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/dataloader/dataloader_base_monai.py` & `miacag-0.0.83/miacag/dataloader/dataloader_base_monai.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,15 @@
                 channel_wise=True)
         elif self.config['model']['backbone'] == 'r2plus1_18':
             normalize = NormalizeIntensityd(
                 keys=self.features,
                 subtrahend=(0.43216, 0.394666, 0.37645),
                 divisor=(0.22803, 0.22145, 0.216989),
                 channel_wise=True)
-        elif self.config['model']['backbone'] in ['r50', 'dinov2_vits14']:
+        elif self.config['model']['backbone'] in ['r50', 'dinov2_vits14', 'vit_small', 'vit_large', 'vit_huge', 'vit_giant']:
             normalize = NormalizeIntensityd(
                 keys=self.features,
                 subtrahend=(0.485, 0.456, 0.406),
                 divisor=(0.229, 0.224, 0.225),
                 channel_wise=True)
         else:
             raise ValueError('not implemented')
```

### Comparing `miacag-0.0.82/miacag/dataloader/get_dataloader.py` & `miacag-0.0.83/miacag/dataloader/get_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,41 @@
             data[label_name] = torch.nan_to_num(data[label_name], nan=99998)
             data[label_name] = data[label_name].long()
         elif config['loss']['name'][c] == 'BCE_multilabel':
             data[label_name] = torch.nan_to_num(data[label_name], nan=99998)
             data[label_name] = data[label_name].long()
         elif config['loss']['name'][c] in ['MSE', '_L1', 'L1smooth']:
             data[label_name] = data[label_name].float()
+        elif config['loss']['name'][c] in ['NNL']:
+            data[label_name] = data[label_name].float()
+            data['event'] = data['event'].int()
         else:
-            raise ValueError("model dimension not implemented")
+            raise ValueError("model loss not implemented")
     return data
 
 
 def to_device(data, device, fields):
     for field in fields:
+        if field.startswith('duration'):
+            data['event'] = data['event'].to(device)
         data[field] = data[field].to(device)
     return data
 
 
 def get_data_from_loader(data, config, device, val_phase=False):
     if config['loaders']['store_memory'] is True:
         data = {
                 'inputs': data[0],
                 config['labels_names']: data[1]
                 }
     if config['task_type'] in ["classification", "regression", "mil_classification"]:
         data = to_device(data, device, ['inputs'])
         data = to_dtype(data, config)
         data = to_device(data, device, config['labels_names'])
+       # if 
         #print('data shape', data['inputs'].shape)
     elif config['task_type'] == "representation_learning":
         if val_phase is False:
             if config['loaders']['store_memory'] is False:
                 data['inputs'] = data['inputs'].to(device)
                 if config['model']['dimension'] == '2D':
                     data['inputs'] = torch.cat(
@@ -88,15 +94,14 @@
                                "regression",
                                "mil_classification"]:
         from miacag.dataloader.Classification.get_dataloader_classification import \
             ClassificationLoader
         CL = ClassificationLoader(config)
         train_loader, val_loader, train_ds, val_ds = \
             CL.get_classification_loader_train(config)
-
         val_loader.sampler.data_source.data = \
             val_loader.sampler.data_source.data * \
             config['loaders']['val_method']['samples']
     elif config['task_type'] == 'segmentation':
         from dataloader.Segmentation.get_dataloader_segmentation import \
             SegmentationLoader
         SL = SegmentationLoader()
```

### Comparing `miacag-0.0.82/miacag/metrics/cumulativeSumming.py` & `miacag-0.0.83/miacag/metrics/cumulativeSumming.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/metrics/metrics.py` & `miacag-0.0.83/miacag/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/metrics/metrics_utils.py` & `miacag-0.0.83/miacag/metrics/metrics_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,14 +116,16 @@
             dicts[metrics[i]] = RMSEMetric(reduction='mean')
         elif metrics[i].startswith('total'):
             dicts[metrics[i]] = CumulativeAverage()
         elif metrics[i].startswith('acc_top_1'):
             dicts[metrics[i]] = ConfusionMatrixMetric(
                 metric_name='accuracy', reduction="mean",
                 include_background=False)
+        elif metrics[i].startswith('NNL'):
+            dicts[metrics[i]] = CumulativeAverage()
         else:
             raise NotImplementedError(
                 'This metric {} is not implemented!'.format(metrics[i]))
         #dicts[metrics[i]].count = dicts[metrics[i]].count.to(device)
         #dicts[metrics[i]].sum = dicts[metrics[i]].sum.to(device)
     return dicts
 
@@ -254,14 +256,17 @@
             losses_metric[loss] = running_losses[loss]
         elif loss.startswith('L1smooth'):
             running_losses[loss].append(losses[loss])
             losses_metric[loss] = running_losses[loss]
         elif loss.startswith('total'):
             running_losses[loss].append(losses[loss])
             losses_metric[loss] = running_losses[loss]
+        elif loss.startswith('NNL'):
+            running_losses[loss].append(losses[loss])
+            losses_metric[loss] = running_losses[loss]
         else:
             raise ValueError("Invalid loss %s" % repr(loss))
     return losses_metric
 
 
 def wrap_outputs(outputs, count_loss, loss_name, count_label):
     if loss_name.startswith('CE'):
@@ -308,14 +313,17 @@
     return metrics, losses_metric
 
 
 def normalize_metrics(running_metrics, device):
     metric_dict = {}
     for running_metric in running_metrics:
         if running_metric.startswith('CE'):
+            running_metrics[running_metric].val = running_metrics[running_metric].val.to(device)
+            running_metrics[running_metric].count = running_metrics[running_metric].count.to(device)# Move to GPU memory if available
+            running_metrics[running_metric].sum = running_metrics[running_metric].sum.to(device)
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('BCE'):
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('total'):
             running_metrics[running_metric].val = running_metrics[running_metric].val.to(device)
             running_metrics[running_metric].count = running_metrics[running_metric].count.to(device)# Move to GPU memory if available
             running_metrics[running_metric].sum = running_metrics[running_metric].sum.to(device)
@@ -327,14 +335,19 @@
         elif running_metric.startswith('L1smooth'):
             running_metrics[running_metric].val = running_metrics[running_metric].val.to(device)
             running_metrics[running_metric].count = running_metrics[running_metric].count.to(device)# Move to GPU memory if available
             running_metrics[running_metric].sum = running_metrics[running_metric].sum.to(device)
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('_L1'):
             metric_tb = running_metrics[running_metric].aggregate().item()
+        elif running_metric.startswith('NNL'):
+            running_metrics[running_metric].val = running_metrics[running_metric].val.to(device)
+            running_metrics[running_metric].count = running_metrics[running_metric].count.to(device)# Move to GPU memory if available
+            running_metrics[running_metric].sum = running_metrics[running_metric].sum.to(device)
+            metric_tb = running_metrics[running_metric].aggregate().item()
         else:
             metric_tb = running_metrics[running_metric].aggregate()[0].item()
         metric_dict[running_metric] = metric_tb
         running_metrics[running_metric].reset()
     return running_metrics, metric_dict
```

### Comparing `miacag-0.0.82/miacag/model_utils/GradCam_model.py` & `miacag-0.0.83/miacag/model_utils/GradCam_model.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/model_utils/eval_utils.py` & `miacag-0.0.83/miacag/model_utils/eval_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,16 @@
             df[logit_conf] = softmax_transform(torch.tensor(df[logit])).tolist()
         elif config['loss']['name'][c] == 'MSE':
             logits_return.append(logit.float())
         elif config['loss']['name'][c] in ['_L1', 'L1smooth']:
             df[logit_conf] = df[logit]
         elif config['loss']['name'][c].startswith('BCE'):
             logits_return.append(torch.nn.Sigmoid()(logit.float()))
+        elif config['loss']['name'][c].startswith('NNL'):
+            df[logit_conf] = df[logit]
         else:
             raise(ValueError('this loss type is not implemented'))
     return df
 
 
 def getListOfLogits(logits):
     unrolled_logits = []
```

### Comparing `miacag-0.0.82/miacag/model_utils/get_optimizer.py` & `miacag-0.0.83/miacag/model_utils/get_optimizer.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/model_utils/get_test_pipeline.py` & `miacag-0.0.83/miacag/model_utils/get_test_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             val_df[label_name + '_confidences'].apply(pd.to_numeric)
         val_df_conf = pd.DataFrame()
         val_df_conf[label_name + '_confidences'] = val_df.groupby(
             'rowid')[label_name + '_confidences'].apply(np.mean)
         if config['loss']['name'][count].startswith('CE'):
             val_df_conf[label_name + '_predictions'] = \
                 val_df_conf[label_name + '_confidences'].apply(np.argmax)
-        elif config['loss']['name'][count] in ['MSE', '_L1', 'L1smooth']:
+        elif config['loss']['name'][count] in ['MSE', '_L1', 'L1smooth', 'NNL']:
             val_df_conf[label_name + '_predictions'] = \
                 val_df_conf[label_name + '_confidences'].astype(float)
         elif config['loss']['name'][count] == 'BCE_multilabel':
             val_df_conf[label_name + '_predictions'] = \
                 val_df_conf[label_name + '_confidences'].apply(
                     np.round).astype(int)
         else:
```

### Comparing `miacag-0.0.82/miacag/model_utils/grad_cam_utils.py` & `miacag-0.0.83/miacag/model_utils/grad_cam_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/model_utils/predict_utils.py` & `miacag-0.0.83/miacag/model_utils/predict_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import shutil
 import os
 import numpy as np
 from miacag.plots.plot_histogram import plot_histogram
 from miacag.metrics.metrics_utils import mkDir
 from miacag.models.BuildModel import ModelBuilder
 from miacag.model_utils.grad_cam_utils import prepare_model_for_sm
+import pandas as pd
+
 
 class Predictor(TestPipeline):
     def __init__(self, model, criterion, config, device, test_loader):
         self.model = model
         self.criterion = criterion
         self.config = config
         self.device = device
@@ -271,7 +273,85 @@
     _, a = model.module.module.get_attention(data['inputs'])
     max_index = torch.argmax(a).item()
     if config['cpu'] == 'True':
         a = a.detach().numpy()
     else:
         a = a.cpu().detach().numpy()
     return a, max_index
+
+def compute_baseline_hazards(df, max_duration, config):
+        """Computes the Breslow estimates form the data defined by `input` and `target`
+        (if `None` use training data).
+
+        Typically call
+        model.compute_baseline_hazards() after fitting.
+        
+        Keyword Arguments:
+            input  -- Input data (train input) (default: {None})
+            target  -- Target data (train target) (default: {None})
+            max_duration {float} -- Don't compute estimates for duration higher (default: {None})
+            sample {float or int} -- Compute estimates of subsample of data (default: {None})
+            batch_size {int} -- Batch size (default: {8224})
+            set_hazards {bool} -- Set hazards in model object, or just return hazards. (default: {True})
+        
+        Returns:
+            pd.Series -- Pandas series with baseline hazards. Index is duration_col.
+        """
+ 
+        base_haz = _compute_baseline_hazards(df, max_duration, config)
+        #if set_hazards:
+        bch = compute_baseline_cumulative_hazards(set_hazards=True, baseline_hazards_=base_haz)
+        return base_haz, bch
+    
+
+def compute_baseline_cumulative_hazards(set_hazards=True, baseline_hazards_=None):
+    """See `compute_baseline_hazards. This is the cumulative version."""
+
+    bch = (baseline_hazards_
+            .cumsum()
+            .rename('baseline_cumulative_hazards'))
+    return bch
+
+def _compute_baseline_hazards(df_target, max_duration, config):
+    if max_duration is None:
+        max_duration = np.inf
+
+
+    df_target['expg'] = np.exp(df_target[[config['labels_names'][0]+'_predictions']])
+    return (df_target
+            .groupby(config['labels_names'])
+            .agg({'expg': 'sum', 'event': 'sum'})
+            .sort_index(ascending=False)
+            .assign(expg=lambda x: x['expg'].cumsum())
+            .pipe(lambda x: x['event']/x['expg'])
+            .fillna(0.)
+            .iloc[::-1]
+            .loc[lambda x: x.index <= max_duration]
+            .rename('baseline_hazards'))
+
+
+def predict_surv_df(df, baseline_hazards_, bch, config):
+    """Predict survival function for `input`. S(x, t) = exp(-H(x, t))
+    Require computed baseline hazards.
+
+    Arguments:
+        input {np.array, tensor or tuple} -- Input x passed to net.
+
+    Keyword Arguments:
+        max_duration {float} -- Don't compute estimates for duration higher (default: {None})
+        batch_size {int} -- Batch size (default: {8224})
+        baseline_hazards_ {pd.Series} -- Baseline hazards. If `None` used `model.baseline_hazards_` (default: {None})
+        eval_ {bool} -- If 'True', use 'eval' mode on net. (default: {True})
+        num_workers {int} -- Number of workers in created dataloader (default: {0})
+
+    Returns:
+        pd.DataFrame -- Survival estimates. One columns for each individual.
+    """
+    return np.exp(-_predict_cumulative_hazards(df, baseline_hazards_, bch, config))
+    
+def _predict_cumulative_hazards(df, baseline_hazards_, bch, config):
+    max_duration = None
+    max_duration = np.inf if max_duration is None else max_duration
+    bch = bch.loc[lambda x: x.index <= max_duration]
+    df['expg'] = np.exp(df[[config['labels_names'][0]+'_predictions']])
+    return pd.DataFrame(bch.values.reshape(-1, 1).dot(df["expg"].to_numpy().reshape(1,-1)), 
+                        index=bch.index)
```

### Comparing `miacag-0.0.82/miacag/model_utils/scheduler.py` & `miacag-0.0.83/miacag/model_utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/model_utils/siam_loss.py` & `miacag-0.0.83/miacag/model_utils/siam_loss.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/model_utils/train_utils.py` & `miacag-0.0.83/miacag/model_utils/train_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from miacag.model_utils.eval_utils import get_loss
 from miacag.configs.config import save_config
 from miacag.metrics.metrics_utils import flatten, \
     unroll_list_in_dict
 import os
 from miacag.utils.common_utils import stack_labels, get_loss
 from miacag.utils.common_utils import get_losses_class, wrap_outputs_to_dict
+from miacag.models.BuildModel import ModelBuilder
+from miacag.models.modules import get_loss_names_groups
 
 
 def set_random_seeds(random_seed=0):
     torch.manual_seed(random_seed)
     torch.backends.cudnn.deterministic = True
     torch.backends.cudnn.benchmark = False
     np.random.seed(random_seed)
@@ -142,14 +144,33 @@
     if config["cpu"] == "False":
         device = "cuda:{}".format(os.environ['LOCAL_RANK'])
     else:
         device = 'cpu'
     device = torch.device(device)
     return device
 
+def fake_saving_ddp_model_wrapper(config, model_file_path):
+    device = get_device(config)
+    config['datasetFingerprintFile'] = None
+    config['loaders']['mode'] = 'training'
+    config['loss']['groups_names'], config['loss']['groups_counts'], \
+        config['loss']['group_idx'], config['groups_weights'] \
+        = get_loss_names_groups(config)
+    config['use_DDP'] = 'True'
+    if config["cpu"] == "False":
+        torch.cuda.set_device(device)
+        torch.backends.cudnn.benchmark = True
+
+    BuildModel = ModelBuilder(config, device)
+    model = BuildModel()
+    if config["cpu"] == "False":
+        torch.save(model.module.state_dict(), model_file_path)
+    else:
+        torch.save(model.state_dict(), model_file_path)
+
 
 def save_model(model, writer, config):
     model_file_path = os.path.join(writer.log_dir, 'model.pt')
     model_encoder_file_path = os.path.join(
             writer.log_dir, 'model_encoder.pt')
 
     if config["cpu"] == "False":
```

### Comparing `miacag-0.0.82/miacag/models/BuildModel.py` & `miacag-0.0.83/miacag/models/BuildModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,18 +113,14 @@
                 channels=self.convert_string_to_tuple(
                     self.config['model']['channels']),
                 strides=self.convert_string_to_tuple(self.config['model']['strides'])
                 )
 
         elif self.config['model']['model_name'] == 'DynUNet':
             print('to be implemented')
-            #unpack_fingerprint(self, config)
-            # import monai.networks.nets as m
-            # model = m.DYNUNet(
-        else:
             raise ValueError('model not implemented')
 
         if path_model != "None":
             model.load_state_dict(torch.load(path_model))
         return model
 
     def get_model(self):
```

### Comparing `miacag-0.0.82/miacag/models/cnns.py` & `miacag-0.0.83/miacag/models/cnns.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/dino_utils/dino_pretrained.py` & `miacag-0.0.83/miacag/models/dino_utils/dino_pretrained.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/get_encoder.py` & `miacag-0.0.83/miacag/models/get_encoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from monai.networks import nets
 from torch import nn
 import torch
 import os
+import miacag.models.vision_transformer as vit
 from dinov2.models.vision_transformer import \
     vit_large, vit_small
 #from timm.models import create_model
 #from models import modeling_finetune
 from collections import OrderedDict
 #from miacag.models.milmodel_from_features import MILModel
 
@@ -17,15 +18,15 @@
         return x
 
 
 def getPretrainedWeights(config, model, device):
     if config['model']['pretrained'] == "True":
         if config['model']['backbone'] not in [
             'debug_3d', "vit_base_patch16_224", "vit_large_patch16_224",
-            "vit_small_patch16_224"]:
+            "vit_small_patch16_224", 'dinov2_vits14', "vit_small"]:
             if torch.distributed.get_rank() == 0:
                 dirname = os.path.dirname(__file__)
                 model_path = os.path.join(
                                 dirname,
                                 "torchhub",
                                 config['model']['dimension'],
                                 config['model']['backbone'],
@@ -37,19 +38,30 @@
                 if config['model']['backbone'] in \
                         ['x3d_s', 'slowfast8x8', "mvit_base_16x4", 'mvit_base_32x3']:
 
                     model.load_state_dict(loaded_model['model_state'])
                 else:
                     model.load_state_dict(loaded_model)
         else:
-            model = load_from_checkpoint(
-                model,
-                config['model']['pretrain_model'],
-                config,
-                model_key='model|module')
+            if config['model']['backbone'] in ['dinov2_vits14', "vit_small"]:
+                loaded_model = torch.load(
+                        os.path.join(config['model']['pretrain_model'], 'model.pt'),
+                        map_location=device)
+                if config['model']['backbone'] in ['vit_small', 'vit_large', 'vit_huge', 'vit_giant']:
+                    if config['loaders']['mode'] != 'testing':
+                        loaded_model = {k.replace("module.", ""): v for k, v in loaded_model['target_encoder'].items()}
+                model.load_state_dict(loaded_model)
+
+            else:
+                raise ValueError('not implemented')
+                # model = load_from_checkpoint(
+                #     model,
+                #     os.path.join(config['model']['pretrain_model'], 'model.pt'),
+                #     config,
+                #     model_key='model|module')
             # loaded_model = torch.load(config['model']['pretrain_model'],
             #                           map_location=device)
             # remove all values from loaded_model dict starting with decoder
             # loaded_model = {k:v for k,v in loaded_model['model'].items() if not k.startswith("decoder")}
 
     elif config['model']['pretrained'] == "None":
         pass
@@ -172,15 +184,24 @@
         model = vit_small(
                 patch_size=14,
                 img_size=config['loaders']['Resize_height'],
                 init_values=1.0,
                 block_chunks=0)
         model = getPretrainedWeights(config, model, device)
         in_features = model.norm.normalized_shape[0]
-       
+    
+    elif config['model']['backbone'] in ['vit_small',
+                                         'vit_large',
+                                         'vit_huge',
+                                         'vit_giant']:
+        model = vit.__dict__[config['model']['backbone']](
+            img_size=[config['loaders']['Resize_height']],
+            patch_size=config['mask']['patch_size'])
+        model = getPretrainedWeights(config, model, device)
+        in_features = model.norm.normalized_shape[0]
     else:
         raise ValueError('not implemented')
 
             
     return model, in_features
```

### Comparing `miacag-0.0.82/miacag/models/mae_st_util/logging.py` & `miacag-0.0.83/miacag/models/mae_st_util/logging.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/mae_st_util/models_vit.py` & `miacag-0.0.83/miacag/models/mae_st_util/models_vit.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/mae_st_util/video_vit.py` & `miacag-0.0.83/miacag/models/mae_st_util/video_vit.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/milmodel3d.py` & `miacag-0.0.83/miacag/models/milmodel3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from miacag.models.modules import EncoderModel, ImageToScalarModel
 import torch
 import torch.nn as nn
 from miacag.models.get_encoder import get_encoder, modelsRequiredPermute
 from miacag.models.modules import maybePermuteInput, get_final_layer
 from monai.utils.module import optional_import
 from miacag.models.modules import unique_counts
-
+import torch.nn.functional as F
 models, _ = optional_import("torchvision.models")
 
 
 class MILModel(ImageToScalarModel):
     def __init__(
         self,
         config,
@@ -306,12 +306,20 @@
     def reduce_feature_space(self, x):
         if self.config['model']['dimension'] in ['3D', '2D+T']:
             if self.config['model']['backbone'] not in ["mvit_base_16x4", "mvit_base_32x3"]:
                 x = x.mean(dim=(-3, -2, -1))
             else:
                 pass
         elif self.config['model']['dimension'] in ['2D']:
-            if self.config['model']['backbone'] not in ["dinov2_vits14"]:
+            if self.config['model']['backbone'] not in ["dinov2_vits14",
+                                                        'vit_small', 'vit_large',
+                                                        'vit_huge', 'vit_giant']:
                 x = x.mean(dim=(-2, -1))
+            elif self.config['model']['backbone'] in ['vit_small', 'vit_large',
+                                                      'vit_huge', 'vit_giant']:
+                x = F.layer_norm(x, (x.size(-1),))
+                x = x.mean(dim=(-2))
+            else:
+                raise ValueError('not implemented for this backbone')
         else:
             raise ValueError('this dimension is not implemented')
         return x
```

### Comparing `miacag-0.0.82/miacag/models/milmodel_from_features.py` & `miacag-0.0.83/miacag/models/milmodel_from_features.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/mlps.py` & `miacag-0.0.83/miacag/models/mlps.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/modeling_finetune.py` & `miacag-0.0.83/miacag/models/modeling_finetune.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/modeling_pretrain.py` & `miacag-0.0.83/miacag/models/modeling_pretrain.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/models/modules.py` & `miacag-0.0.83/miacag/models/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                         # nn.Linear(
                         #     self.in_features, self.in_features),
                         nn.Linear(
                             self.in_features, count_loss)
                         ).to(device))
             # test if loss_type startswith three conditions
             
-            elif loss_type.startswith(tuple(['MSE', '_L1', 'L1smooth'])):
+            elif loss_type.startswith(tuple(['MSE', '_L1', 'L1smooth', 'NNL'])):
                 # if config['model']['sigm'] == 'True':
                 self.fcs.append(
                     nn.Sequential(
                         # nn.Linear(
                         #     self.in_features, self.in_features),
                         nn.Linear(
                             self.in_features,
```

### Comparing `miacag-0.0.82/miacag/models/pretrained_vit.py` & `miacag-0.0.83/miacag/models/pretrained_vit.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/plots/angle_plotter.py` & `miacag-0.0.83/miacag/plots/angle_plotter.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/plots/plot_histogram.py` & `miacag-0.0.83/miacag/plots/plot_histogram.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/plots/plot_pathology_treatment_pred.py` & `miacag-0.0.83/miacag/plots/plot_pathology_treatment_pred.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/plots/plot_roc_auc_all.py` & `miacag-0.0.83/miacag/plots/plot_roc_auc_all.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier
 import os
 from sklearn.metrics import roc_curve, roc_auc_score
 from miacag.utils.script_utils import mkFolder
 from miacag.plots.plotter import rename_columns
+from miacag.plots.plot_utils import get_mean_lower_upper
+import statsmodels.api as sm
 
 def generate_data():
     data = datasets.load_breast_cancer()
 
     X = data.data
     y = data.target
 
@@ -114,22 +116,24 @@
 
 
 def transform_confidences_to_by_label_type(confidences, name):
     if name.startswith('ffr'):
         confidences = 1 - confidences
     elif name.startswith('sten'):
         pass
+    elif name.startswith('timi'):
+        pass
     else:
         raise ValueError('name is not ffr or sten')
     return confidences
 
 
 def plot_roc_all(result_table, trues_names, confidences_names, output_plots, plot_type, config, theshold=0.5):
        # Define a result table as a DataFrame
-    roc_result_table = pd.DataFrame(columns=['segments', 'fpr','tpr','auc'])
+    roc_result_table = pd.DataFrame(columns=['segments', 'fpr','tpr','auc', 'auc_lower', 'auc_upper'])
 
     probas = []
     trues = []
     idx = 0
     for seg in confidences_names:
         if config['task_type'] != 'mil_classification':
             result_table_copy, maybeRCA = select_relevant_data(result_table, seg, trues_names[idx])
@@ -146,21 +150,29 @@
         mask_propa = np.isnan(yproba)
         mask_test = np.isnan(y_test)
         mask = mask_propa + mask_test
         y_test = y_test[~mask]
         yproba = yproba[~mask]
         yproba = np.clip(yproba, a_min=0, a_max=1)
         fpr, tpr, _ = roc_curve(y_test,  yproba)
+        mean_auc, upper_auc, lower_auc = get_mean_lower_upper(yproba, y_test, 'roc_auc_score')
+        upper_auc = np.clip(upper_auc, a_min=0, a_max=1)
+        lower_auc = np.clip(lower_auc, a_min=0, a_max=1)
+        if config['debugging']:
+            y_test[0] = 1
+            y_test[1] = 0
         auc = roc_auc_score(y_test, yproba)
         probas.append(yproba)
         trues.append(y_test)
         roc_result_table = roc_result_table.append({'segments':seg,
                                             'fpr':fpr, 
                                             'tpr':tpr, 
-                                            'auc':auc}, ignore_index=True)
+                                            'auc':auc,
+                                            'auc_lower':lower_auc,
+                                            'auc_upper': upper_auc}, ignore_index=True)
         
         idx += 1
     roc_result_table.set_index('segments', inplace=True)
     # concatenate list of numpy arrays for trues and probas
     probas = np.concatenate(probas)
     trues = np.concatenate(trues)
     # put them together in a dataframe
@@ -216,35 +228,131 @@
         location = 'LCA'
     fig = plt.figure(figsize=(8,6))
 
     for i in roc_result_table_2.index:
         #     df_plot, prediction_name, label_name)
         plt.plot(roc_result_table_2.loc[i]['fpr'], 
                 roc_result_table_2.loc[i]['tpr'], 
-                label="{}, AUC={:.3f}".format(i, roc_result_table_2.loc[i]['auc']))
+                label="{}, AUC={:.3f} ({:.3f}-{:-3f})".format(
+                    i, roc_result_table_2.loc[i]['auc'],
+                    roc_result_table_2.loc[i]['auc_lower'],
+                    roc_result_table_2.loc[i]['auc_upper']))
         
     plt.plot([0,1], [0,1], color='orange', linestyle='--')
 
     plt.xticks(np.arange(0.0, 1.1, step=0.1))
     plt.xlabel("False Positive Rate (1 - Specificity)", fontsize=15)
 
     plt.yticks(np.arange(0.0, 1.1, step=0.1))
     plt.ylabel("True Positive Rate (Sensitivity)", fontsize=15)
 
     plt.title('ROC Curve Analysis for ' + plot_type + ' estimation on ' + location, fontweight='bold', fontsize=15)
-    plt.legend(prop={'size':13}, loc='lower right')
+    plt.legend(prop={'size':10}, loc='lower right')
 
     plt.show()
     plt.savefig(os.path.join(
         output_plots, plot_type + '_' + location + '_roc_all.png'), dpi=100,
                 bbox_inches='tight')
     plt.savefig(os.path.join(
         output_plots, plot_type + '_' + location + '_roc_all.pdf'), dpi=100,
                 bbox_inches='tight')
 
+def plot_regression_all(result_table, trues_names, confidences_names, output_plots, config):
+       # Define a result table as a DataFrame
+    result_table_comb = pd.DataFrame(columns=['segments', 'mse_mean', 'mse_lower', 'mse_upper'])
+
+    # list comprehension to rename suffixes of elements in list from _confidences to _predictions
+    confidences_names = [i.replace('_confidences', '_predictions') for i in confidences_names]
+    probas = []
+    trues = []
+    idx = 0
+    for seg in confidences_names:
+        if config['task_type'] != 'mil_classification':
+            result_table_copy, maybeRCA = select_relevant_data(result_table, seg, trues_names[idx])
+        else:
+            result_table_copy = result_table.copy()
+            maybeRCA = ""
+        result_table_copy[confidences_names[idx]] = transform_confidences_to_by_label_type(
+            result_table_copy[confidences_names[idx]], seg)
+        y_test = result_table_copy[trues_names[idx]].values
+        yproba = result_table_copy[confidences_names[idx]].values
+        mask_propa = np.isnan(yproba)
+        mask_test = np.isnan(y_test)
+        mask = mask_propa + mask_test
+        y_test = y_test[~mask]
+        yproba = yproba[~mask]
+        #syproba = np.clip(yproba, a_min=0, a_max=1)
+       # fpr, tpr, _ = roc_curve(y_test,  yproba)
+        mean_mse, upper_mse, lower_mse = get_mean_lower_upper(yproba, y_test, 'mse_score')
+       # upper_mse = np.clip(upper_mse, a_min=0, a_max=1)
+       # lower_mse = np.clip(lower_mse, a_min=0, a_max=1)
+       # auc = roc_auc_score(y_test, yproba)
+        probas.append(yproba)
+        trues.append(y_test)
+        result_table_comb = result_table_comb.append({'segments':seg,
+                                            'mse_mean':mean_mse,
+                                            'mse_lower':lower_mse,
+                                            'mse_upper': upper_mse}, ignore_index=True)
+        
+        idx += 1
+
+    result_table_comb['probas'] = probas
+    result_table_comb['trues'] = trues
+#    from miacag.plots.plotter import plot_regression_density
+    label_name_ori = config['labels_names'][0]
+    # cat y_test and yproba to dataframe
+    df = pd.DataFrame({'y_test': y_test, 'yproba': yproba})
+    g = sns.lmplot(x='y_test', y='yproba', data=df)
+    X2 = sm.add_constant(df['y_test'])
+    est = sm.OLS(df['yproba'], X2)
+    est2 = est.fit()
+    r = est2.rsquared
+
+    if label_name_ori.startswith('timi'):
+        label_name = 'TIMI Flow'
+        plot_name = 'timi'
+    elif label_name_ori.startswith('ffr'):
+        plot_name = 'FFR'
+        label_name = 'FFR'
+    elif label_name_ori.startswith('sten'):
+        plot_name = 'stenosis'
+        label_name = 'Stenosis'
+    else:
+        raise ValueError('label_name_ori is not timi, ffr or sten')
+    result_table_comb.to_csv(
+        os.path.join
+        (output_plots, plot_name + '_regression.csv'))
+    for ax, title in zip(g.axes.flat, [label_name]):
+            ax.set_title(title)
+            ax.set_ylim(bottom=0.)
+            ax.text(0.05, 0.85,
+                    f'R-squared = {r:.3f}',
+                    fontsize=9, transform=ax.transAxes)
+            # ax.text(0.05, 0.9,
+            #         "p-value = " + p,
+            #         fontsize=9,
+            #         transform=ax.transAxes)
+            plt.xlabel("True")
+            plt.ylabel("Predicted")
+            plt.show()
+
+    plt.title(label_name)
+    plt.savefig(
+        os.path.join(
+            output_plots, plot_name + '_scatter.png'), dpi=100,
+        bbox_inches='tight')
+    plt.close()
+    # plot_regression_density(x=y_test, y=yproba,
+    #                                 cmap='jet', ylab='prediction', xlab='true',
+    #                                 bins=100,
+    #                                 figsize=(5, 4),
+    #                                 snsbins=60,
+    #                                 plot_type=plot_type,
+    #                                 output_folder=output_plots,
+    #                                 label_name_ori=label_name_ori)
 if __name__ == '__main__':
 
     output_plots = "/home/alatar/miacag/output_plots/"
     mkFolder(output_plots)
     result_table, confidences_names, \
         trues_names, dom_name, label_pred_names = generate_data()
     config = dict()
```

### Comparing `miacag-0.0.82/miacag/plots/plot_scatter.py` & `miacag-0.0.83/miacag/plots/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/plots/plot_test.py` & `miacag-0.0.83/miacag/plots/plot_test.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/plots/plotter.py` & `miacag-0.0.83/miacag/plots/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from sklearn import metrics
 import math
 import scipy
 from sklearn.metrics import r2_score
 import statsmodels.api as sm
 from decimal import Decimal
 from miacag.utils.script_utils import mkFolder
+
+
 def rename_columns(df, label_name):
     if '_1_prox' in label_name:
         value = '1: Proximal RCA'
     elif '_2_mi' in label_name:
         value = '2: Mid RCA'
     elif '_3_dist' in label_name:
         value = '3: Distale RCA'
@@ -609,14 +611,18 @@
         plt.close()
         return None
 
 
 def plotRegression(sql_config, label_names,
                    prediction_names, output_folder, group_aggregated=False):
     df, _ = getDataFromDatabase(sql_config)
+    from miacag.plots.plot_roc_auc_all import plot_regression_all
+    plot_regression_all(df,
+                        label_names, prediction_names,
+                        output_folder, sql_config)
 
     for c, label_name in enumerate(label_names):
         label_name_ori = label_name
         prediction_name = prediction_names[c]
         df_plot = df.dropna(
             subset=[label_name, prediction_name],
             how='any')
@@ -643,21 +649,27 @@
                     df_plot_rep[prediction_name],
                     sql_config['loss_name'][c])
 
         df_plot_rep[prediction_name] = np.clip(
             df_plot_rep[prediction_name], a_min=0, a_max=1)
 
         df_plot_rep = df_plot_rep.astype({prediction_name: float})
+        if label_name_ori.startswith('sten'):
+            plot_type = 'Stenosis'
+        elif label_name_ori.startswith('ffr'):
+            plot_type = 'FFR'
+        elif label_name_ori.startswith('timi'):
+            plot_type = 'TIMI flow'
         plot_regression_density(x=df_plot_rep[label_name],
                                 y=df_plot_rep[prediction_name],
                                 cmap='jet', ylab='prediction', xlab='true',
                                 bins=100,
                                 figsize=(5, 4),
                                 snsbins=60,
-                                plot_type='Stenosis' if label_name_ori.startswith('sten') else 'FFR',
+                                plot_type=plot_type,
                                 output_folder=output_folder,
                                 label_name_ori=label_name_ori)
     #remove nan
         g = sns.lmplot(x=label_name, y=prediction_name, data=df_plot_rep)
         X2 = sm.add_constant(df_plot_rep[label_name])
         est = sm.OLS(df_plot_rep[prediction_name], X2)
         est2 = est.fit()
@@ -670,18 +682,18 @@
 
         for ax, title in zip(g.axes.flat, [label_name]):
             ax.set_title(title)
             ax.set_ylim(bottom=0.)
             ax.text(0.05, 0.85,
                     f'R-squared = {r:.3f}',
                     fontsize=9, transform=ax.transAxes)
-            ax.text(0.05, 0.9,
-                    "p-value = " + p,
-                    fontsize=9,
-                    transform=ax.transAxes)
+            # ax.text(0.05, 0.9,
+            #         "p-value = " + p,
+            #         fontsize=9,
+            #         transform=ax.transAxes)
             plt.xlabel("True")
             plt.ylabel("Predicted")
             plt.show()
 
         plt.title(label_name)
         plt.savefig(
             os.path.join(
```

### Comparing `miacag-0.0.82/miacag/plots/query_plot_agg_max.py` & `miacag-0.0.83/miacag/plots/query_plot_agg_max.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/postprocessing/aggregate_pr_group.py` & `miacag-0.0.83/miacag/postprocessing/aggregate_pr_group.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/postprocessing/append_results.py` & `miacag-0.0.83/miacag/postprocessing/append_results.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/postprocessing/count_stenosis_pr_group.py` & `miacag-0.0.83/miacag/postprocessing/count_stenosis_pr_group.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/postprocessing/estimate_vessel_disease.py` & `miacag-0.0.83/miacag/postprocessing/estimate_vessel_disease.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/predictor.py` & `miacag-0.0.83/miacag/predictor.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/add_columns.py` & `miacag-0.0.83/miacag/preprocessing/add_columns.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/copy_column.py` & `miacag-0.0.83/miacag/preprocessing/copy_column.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/copy_table.py` & `miacag-0.0.83/miacag/preprocessing/copy_table.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/datasetFingerprint.py` & `miacag-0.0.83/miacag/preprocessing/datasetFingerprint.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/labels_map.py` & `miacag-0.0.83/miacag/preprocessing/labels_map.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/pre_process.py` & `miacag-0.0.83/miacag/preprocessing/pre_process.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/process_labels/process_dominance.py` & `miacag-0.0.83/miacag/preprocessing/process_labels/process_dominance.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/process_labels/process_total_occ.py` & `miacag-0.0.83/miacag/preprocessing/process_labels/process_total_occ.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/split_train_val.py` & `miacag-0.0.83/miacag/preprocessing/split_train_val.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,16 +45,17 @@
     def __init__(self, sql_config, labels_config=None):
         self.sql_config = sql_config
         self.df, self.connection = getDataFromDatabase(sql_config=sql_config)
         #self.df = self.df.dropna(subset=sql_config["labels_names"], how='any')
 
     def groupEntriesPrPatient(self, df):
         '''Grouping entries pr patients'''
-        X = df.drop(self.sql_config['labels_names'], 1)
-        y = df[self.sql_config['labels_names']]
+        # using DcmPathFlatten as dummy for splitting
+        X = df.drop('DcmPathFlatten', 1)
+        y = df['DcmPathFlatten']
         if self.sql_config['TestSize'] == 1:
             return None, df
         else:
             gs = GroupShuffleSplit(
                 n_splits=2,
                 test_size=self.sql_config['TestSize'],
                 random_state=0)
@@ -64,26 +65,26 @@
             df_val = df.iloc[val_ix]
             self.addPhase(df_train, df_val)
             return df_train, df_val
 
     def addPhase(self, train_df, val_df):
         train_df['phase'] = "train"
         val_df['phase'] = "val"
-        val_df = val_df[['phase', 'rowid'] + self.sql_config['labels_names']]
+        val_df = val_df[['phase', 'rowid']]
         train_df = train_df[
-            ['phase', 'rowid'] + self.sql_config['labels_names']]
+            ['phase', 'rowid']]
 
         update_cols(
                     val_df.to_dict('records'),
                     self.sql_config,
-                    ['phase'] + self.sql_config['labels_names'],)
+                    ['phase'],)
         update_cols(
                     train_df.to_dict('records'),
                     self.sql_config,
-                    ['phase'] + self.sql_config['labels_names'])
+                    ['phase'])
 
     def __call__(self):
         df = self.df[self.df['phase'] != 'test']
         self.train_df, self.val_df = self.groupEntriesPrPatient(df)
```

### Comparing `miacag-0.0.82/miacag/preprocessing/transform_missing_floats.py` & `miacag-0.0.83/miacag/preprocessing/transform_missing_floats.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/transform_stenosis.py` & `miacag-0.0.83/miacag/preprocessing/transform_stenosis.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/transform_thresholds.py` & `miacag-0.0.83/miacag/preprocessing/transform_thresholds.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,16 @@
             elif label_name.startswith('ffr'):
                 self.df[label_name][self.df[label_name] < 0] = 0
                 self.df[label_name] = \
                     np.where((
                         (self.df[label_name] >= 1) &
                         (~np.isnan(self.df[label_name]))),
                         1, self.df[label_name])
+            elif label_name.startswith('timi'):
+                pass
             else:
                 raise ValueError(
                     'this type of label to process is not implemented')
 
         if self.config['process_labels'] == 'True':
             proccoessor = ProcessLabelsOCC(self.df,
                                            self.sql_config['labels_names'],
```

### Comparing `miacag-0.0.82/miacag/preprocessing/transform_total_occlusion.py` & `miacag-0.0.83/miacag/preprocessing/transform_total_occlusion.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/preprocessing/utils/check_experiments.py` & `miacag-0.0.83/miacag/preprocessing/utils/check_experiments.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/aggregate_and_plot.py` & `miacag-0.0.83/miacag/scripts/aggregate_and_plot.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/angiography_classifier/predict_angio.py` & `miacag-0.0.83/miacag/scripts/angiography_classifier/predict_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/angiography_classifier/submit_angio.py` & `miacag-0.0.83/miacag/scripts/angiography_classifier/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py` & `miacag-0.0.83/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/compare_PCI_notPCI.py` & `miacag-0.0.83/miacag/scripts/compare_PCI_notPCI.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/predict_patologi_eyeball_vs_estimated.py` & `miacag-0.0.83/miacag/scripts/predict_patologi_eyeball_vs_estimated.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/pretraining_downstreams/submit_angio.py` & `miacag-0.0.83/miacag/scripts/stenosis_identifier/submit_angio.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,55 +2,49 @@
 import os
 import socket
 from datetime import datetime, timedelta
 import yaml
 from miacag.preprocessing.split_train_val import splitter
 from miacag.utils.sql_utils import copy_table, add_columns, \
     copyCol, changeDtypes
-import copy
-import numpy as np
+
 import pandas as pd
 from miacag.postprocessing.append_results import appendDataFrame
 import torch
 from miacag.trainer import train
 from miacag.tester import test
 from miacag.configs.config import load_config, maybe_create_tensorboard_logdir
 from miacag.configs.options import TrainOptions
 import argparse
 from miacag.preprocessing.labels_map import labelsMap
-from sklearn.preprocessing import LabelBinarizer
-from sklearn.metrics import roc_auc_score
 from miacag.preprocessing.utils.check_experiments import checkExpExists, \
     checkCsvExists
-from miacag.plots.plotter import plot_results, plotRegression
+from miacag.plots.plotter import plot_results
 import pandas as pd
-from miacag.preprocessing.transform_thresholds import transformThresholdRegression
+from miacag.preprocessing.transform_thresholds import transformThreshold
 from miacag.preprocessing.transform_missing_floats import transformMissingFloats
-from miacag.utils.script_utils import create_empty_csv, mkFolder, maybe_remove, write_file, test_for_file
+from miacag.utils.script_utils import create_empty_csv, mkFolder, maybe_remove, test_for_file, write_file
 from miacag.postprocessing.aggregate_pr_group import Aggregator
 from miacag.postprocessing.count_stenosis_pr_group \
     import CountSignificantStenoses
-from miacag.models.dino_utils import dino_pretrained
-from miacag.models.dino_utils.dino_pretrained import FeatureForwarder
-from miacag.utils.sql_utils import getDataFromDatabase
-from miacag.plots.plot_predict_coronary_pathology import run_plotter_ruc_multi_class
+
 parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
-    "--local_rank", type=int,
-    help="Local rank: torch.distributed.launch.")
+            "--local_rank", type=int,
+            help="Local rank: torch.distributed.launch.")
 parser.add_argument(
             "--local-rank", type=int,
             help="Local rank: torch.distributed.launch.")
 parser.add_argument(
-    "--num_workers", type=int,
-    help="Number of cpu workers for training")
+            "--num_workers", type=int,
+            help="Number of cpu workers for training")    
 parser.add_argument(
     '--config_path', type=str,
     help="path to folder with config files")
 
 
 def stenosis_identifier(cpu, num_workers, config_path, table_name_input=None):
     if table_name_input is None:
@@ -63,440 +57,443 @@
         os.path.join(config_path, i) for i in os.listdir(config_path)]
 
     for i in range(0, len(config_path)):
         print('loading config:', config_path[i])
         with open(config_path[i]) as file:
             config = yaml.load(file, Loader=yaml.FullLoader)
         mkFolder(config['output'])
-        config['master_port'] = os.environ['MASTER_PORT']
-        config['num_workers'] = num_workers
-        config['cpu'] = cpu
-        tensorboard_comment = os.path.basename(config_path[i])[:-5]
-        temp_file = os.path.join(config['output'], 'temp.txt')
-        torch.distributed.barrier()
-        if torch.distributed.get_rank() == 0:
-            maybe_remove(temp_file)
-            experiment_name = tensorboard_comment + '_' + \
-                "SEP_" + \
-                datetime.now().strftime('%b%d_%H-%M-%S')
-            write_file(temp_file, experiment_name)
-        torch.distributed.barrier()
-        experiment_name = test_for_file(temp_file)[0]
-        output_directory = os.path.join(
-                    config['output'],
-                    experiment_name)
-        mkFolder(output_directory)
-        output_config = os.path.join(output_directory,
-                                        os.path.basename(config_path[i]))
-        if table_name_input is None:
-            output_table_name = \
-                experiment_name + "_" + config['table_name']
+        csv_exists, output_csv_test = checkCsvExists(config['output'])
+        if csv_exists is False:
+            trans_label = \
+                [i + '_transformed' for i in config['labels_names']]
+            df_results = create_empty_csv(output_csv_test, trans_label)
         else:
-            output_table_name = table_name_input
+            df_results = pd.read_csv(output_csv_test)
 
-        output_plots = os.path.join(output_directory, 'plots')
-        mkFolder(output_plots)
+        exp_exists = checkExpExists(config_path[i], config['output'])
+        if exp_exists is False:
 
-        output_plots_train = os.path.join(output_plots, 'train')
-        output_plots_val = os.path.join(output_plots, 'val')
-        output_plots_test = os.path.join(output_plots, 'test')
-
-        mkFolder(output_plots_train)
-        mkFolder(output_plots_test)
-        mkFolder(output_plots_val)
-
-        # begin pipeline
-        # 1. copy table
-        os.system("mkdir -p {output_dir}".format(
-            output_dir=output_directory))
-        torch.distributed.barrier()
-        if torch.distributed.get_rank() == 0:
+            config['master_port'] = os.environ['MASTER_PORT']
+            config['num_workers'] = num_workers
+            config['cpu'] = cpu
+            tensorboard_comment = os.path.basename(config_path[i])[:-5]
+            temp_file = os.path.join(config['output'], 'temp.txt')
+            torch.distributed.barrier()
+            if torch.distributed.get_rank() == 0:
+                maybe_remove(temp_file)
+                experiment_name = tensorboard_comment + '_' + \
+                    "SEP_" + \
+                    datetime.now().strftime('%b%d_%H-%M-%S')
+                write_file(temp_file, experiment_name)
+            torch.distributed.barrier()
+            experiment_name = test_for_file(temp_file)[0]
+            output_directory = os.path.join(
+                        config['output'],
+                        experiment_name)
+            mkFolder(output_directory)
+            output_config = os.path.join(output_directory,
+                                         os.path.basename(config_path[i]))
             if table_name_input is None:
-                copy_table(sql_config={
+                output_table_name = \
+                    experiment_name + "_" + config['table_name']
+            else:
+                output_table_name = table_name_input
+
+            output_plots = os.path.join(output_directory, 'plots')
+            mkFolder(output_plots)
+
+            output_plots_train = os.path.join(output_plots, 'train')
+            output_plots_val = os.path.join(output_plots, 'val')
+            output_plots_test = os.path.join(output_plots, 'test')
+
+            mkFolder(output_plots_train)
+            mkFolder(output_plots_test)
+            mkFolder(output_plots_val)
+
+            # begin pipeline
+            # 1. copy table
+            os.system("mkdir -p {output_dir}".format(
+                output_dir=output_directory))
+            torch.distributed.barrier()
+            if torch.distributed.get_rank() == 0:
+                if table_name_input is None:
+                    copy_table(sql_config={
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'schema_name': config['schema_name'],
+                        'table_name_input': config['table_name'],
+                        'table_name_output': output_table_name})
+
+                # # 2. copy config
+                os.system(
+                    "cp {config_path} {config_file_temp}".format(
+                        config_path=config_path[i],
+                        config_file_temp=output_config))
+            # rename labels and add columns;
+            trans_label = [i + '_transformed' for i in config['labels_names']]
+            labels_names_original = config['labels_names']
+            config['labels_names'] = trans_label
+            # add placeholder for confidences
+            conf = [i + '_confidences' for i in config['labels_names']]
+            conf_agg = [i + '_confidences_aggregated' for i in config['labels_names']]
+            # add placeholder for predictions
+            pred = [i + '_predictions' for i in config['labels_names']]
+
+            torch.distributed.barrier()
+            if torch.distributed.get_rank() == 0:
+                add_columns({
                     'database': config['database'],
                     'username': config['username'],
                     'password': config['password'],
                     'host': config['host'],
                     'schema_name': config['schema_name'],
-                    'table_name_input': config['table_name'],
-                    'table_name_output': output_table_name})
+                    'table_name': output_table_name,
+                    'table_name_output': output_table_name},
+                            trans_label,
+                            ["float8"] * len(trans_label))
+                # copy content of labels
+                copyCol(
+                    {'database': config["database"],
+                        'username': config["username"],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_transform']},
+                    labels_names_original,
+                    trans_label)
 
-            # # 2. copy config
-            os.system(
-                "cp {config_path} {config_file_temp}".format(
-                    config_path=config_path[i],
-                    config_file_temp=output_config))
+                add_columns({
+                    'database': config['database'],
+                    'username': config['username'],
+                    'password': config['password'],
+                    'host': config['host'],
+                    'schema_name': config['schema_name'],
+                    'table_name': output_table_name,
+                    'table_name_output': output_table_name},
+                            conf,
+                            ["VARCHAR"] * len(conf))
+                add_columns({
+                    'database': config['database'],
+                    'username': config['username'],
+                    'password': config['password'],
+                    'host': config['host'],
+                    'schema_name': config['schema_name'],
+                    'table_name': output_table_name,
+                    'table_name_output': output_table_name},
+                            pred,
+                            ["float8"] * len(pred))
+
+                add_columns({
+                    'database': config['database'],
+                    'username': config['username'],
+                    'password': config['password'],
+                    'host': config['host'],
+                    'schema_name': config['schema_name'],
+                    'table_name': output_table_name,
+                    'table_name_output': output_table_name},
+                            conf_agg,
+                            ["float8"] * len(conf))
+                
 
+                add_columns({
+                    'database': config['database'],
+                    'username': config['username'],
+                    'password': config['password'],
+                    'host': config['host'],
+                    'schema_name': config['schema_name'],
+                    'table_name': output_table_name,
+                    'table_name_output': output_table_name},
+                            ["antalsignifikantestenoser_pred"],
+                            ["float8"])
 
-        torch.distributed.barrier()
-        if torch.distributed.get_rank() == 0:
-            # TODO dont split on labels names
-            splitter_obj = splitter(
-                {
+                # 3. split train and validation , and map labels
+                trans = transformMissingFloats({
                     'labels_names': config['labels_names'],
                     'database': config['database'],
                     'username': config['username'],
                     'password': config['password'],
                     'host': config['host'],
                     'schema_name': config['schema_name'],
                     'table_name': output_table_name,
-                    'query': config['query_split'],
+                    'query': config['query_transform'],
                     'TestSize': config['TestSize']})
-            splitter_obj()
-            # ...and map data['labels'] test
-        # 4.1 Pretrain encoder model
-        ## TODO add pretrain model
-        if not config['model']['freeze_backbone']:
-            print('ssl pretraining')
-            # train here...
-            config['freeze_backbone'] = True
-            
-        # loop through all indicator tasks
-        unique_index = list(dict.fromkeys(config['task_indicator']))
-        for task_index in unique_index:
-            config_new = copy.deepcopy(config)
-            run_task(config_new, task_index, output_directory, output_table_name,
-                    output_plots_train, output_plots_val, output_plots_test,
-                    cpu)
-            
+                trans()
 
-    print('config files processed', str(i+1))
-    print('config files to process in toal:', len(config_path))
-    return None
-
-def run_task(config, task_index, output_directory, output_table_name,
-             output_plots_train, output_plots_val, output_plots_test, cpu):
-    task_names = [
-        name for i, name in zip(config['task_indicator'],
-                                config['labels_names']) if i == task_index]
-    loss_names = [
-        name for i, name in zip(config['task_indicator'],
-                                config['loss']['name']) if i == task_index]
-    eval_names_train = [
-        name for i, name in zip(
-            config['task_indicator'],
-            config['eval_metric_train']['name']) if i == task_index]
-    eval_names_val = [
-        name for i, name in zip(
-            config['task_indicator'],
-            config['eval_metric_val']['name']) if i == task_index]
-    eval_names_val = [
-        name for i, name in zip(
-            config['task_indicator'],
-            config['eval_metric_val']['name']) if i == task_index]
-    # declare updated config
-    config_task = config.copy()
-    config_task['labels_names'] = task_names
-    config_task['loss']['name'] = loss_names
-    config_task['eval_metric_train']['name'] = eval_names_train
-    config_task['eval_metric_val']['name'] = eval_names_val
-    
-    torch.distributed.barrier()
-    config_task['output'] = output_directory
-    config_task['output_directory'] = output_directory
-    config_task['table_name'] = output_table_name
-    config_task['use_DDP'] = 'True'
-    config_task['datasetFingerprintFile'] = None
-        # rename labels and add columns;
-    trans_label = [i + '_transformed' for i in config_task['labels_names']]
-    labels_names_original = config_task['labels_names']
-    config_task['labels_names'] = trans_label
-    # add placeholder for confidences
-    conf = [i + '_confidences' for i in config_task['labels_names']]
-    # add placeholder for predictions
-    pred = [i + '_predictions' for i in config_task['labels_names']]
-    #
-
-    
-    # test if loss is regression type
-    if loss_names[0] in ['L1smooth', 'MSE']:
-        change_dtype_add_cols(config_task, output_table_name, trans_label, labels_names_original, conf, pred, "float8")
-        transform_regression_data(config_task, output_table_name, trans_label)
-    elif loss_names[0] in ['CE']:
-        change_dtype_add_cols_ints(config_task, output_table_name, trans_label, labels_names_original, conf, pred, "int8")
-        config_task['weighted_sampler'] == "True"
-    train(config_task)
-    # 5 eval model
-    test(config_task)
-
-    print('kill gpu processes')
-    torch.distributed.barrier()
-    # clear gpu memory
-    torch.cuda.empty_cache()
-
-    # plot results
-    if loss_names[0] in ['L1smooth', 'MSE']:
-        plot_regression_tasks(config_task, output_plots_train, output_plots_val, output_plots_test)
-    elif loss_names[0] in ['CE']:
-        plot_classification_tasks(config_task, output_table_name,
-                                  output_plots_train, output_plots_val, output_plots_test)
-        
-
-
-def change_dtype_add_cols_ints(config, output_table_name, trans_label, labels_names_original, conf, pred, type):
-    add_columns({
-        'database': config['database'],
-        'username': config['username'],
-        'password': config['password'],
-        'host': config['host'],
-        'schema_name': config['schema_name'],
-        'table_name': output_table_name,
-        'table_name_output': output_table_name},
-                trans_label,
-                ['VARCHAR'] * len(trans_label))
-    # copy content of labels
-    copyCol(
-        {'database': config["database"],
-            'username': config["username"],
-            'password': config['password'],
-            'host': config['host'],
-            'schema_name': config['schema_name'],
-            'table_name': output_table_name,
-            'query': config['query_transform']},
-        labels_names_original,
-        trans_label)
-    mapper_obj = labelsMap(
-                {
-                    'labels_names': labels_names_original,
+                trans_thres = transformThreshold({
+                    'labels_names': config['labels_names'],
                     'database': config['database'],
                     'username': config['username'],
                     'password': config['password'],
                     'host': config['host'],
                     'schema_name': config['schema_name'],
                     'table_name': output_table_name,
-                    'query': config['query_test'],
-                    'TestSize': 1},
-                config['labels_dict'])
-    mapper_obj()
-    changeDtypes(
-        {'database': config["database"],
-            'username': config["username"],
-            'password': config['password'],
-            'host': config['host'],
-            'schema_name': config['schema_name'],
-            'table_name': output_table_name,
-            'query': config['query_transform']},
-        trans_label,
-        ["int8"] * len(trans_label))
-
-    add_columns({
-        'database': config['database'],
-        'username': config['username'],
-        'password': config['password'],
-        'host': config['host'],
-        'schema_name': config['schema_name'],
-        'table_name': output_table_name,
-        'table_name_output': output_table_name},
-                conf,
-                ["VARCHAR"] * len(conf))
-    add_columns({
-        'database': config['database'],
-        'username': config['username'],
-        'password': config['password'],
-        'host': config['host'],
-        'schema_name': config['schema_name'],
-        'table_name': output_table_name,
-        'table_name_output': output_table_name},
-                pred,
-                [type] * len(pred))
-
-
-def transform_regression_data(config, output_table_name, trans_label):
-    trans = transformMissingFloats({
-        'labels_names': config['labels_names'],
-        'database': config['database'],
-        'username': config['username'],
-        'password': config['password'],
-        'host': config['host'],
-        'schema_name': config['schema_name'],
-        'table_name': output_table_name,
-        'query': config['query_transform'],
-        'TestSize': config['TestSize']})
-    trans()
-
-    trans_thres = transformThresholdRegression({
-        'labels_names': config['labels_names'],
-        'database': config['database'],
-        'username': config['username'],
-        'password': config['password'],
-        'host': config['host'],
-        'schema_name': config['schema_name'],
-        'table_name': output_table_name,
-        'query': config['query_transform'],
-        'TestSize': config['TestSize']},
-        config)
-    trans_thres()
-
-    # change dtypes for label
-
-
-def plot_regression_tasks(config_task, output_table_name, output_plots_train,
-                          output_plots_val, output_plots_test, conf):
-    # 6 plot results:
-    # train
-    plot_results({
-                'database': config_task['database'],
-                'username': config_task['username'],
-                'password': config_task['password'],
-                'host': config_task['host'],
-                'labels_names': config_task['labels_names'],
-                'schema_name': config_task['schema_name'],
-                'table_name': output_table_name,
-                'query': config_task['query_train_plot']},
-                config_task['labels_names'],
-                [i + "_predictions" for i in
-                    config_task['labels_names']],
-                output_plots_train,
-                config_task['model']['num_classes'],
-                config_task,
-                [i + "_confidences" for i in
-                    config_task['labels_names']]
-                )
+                    'query': config['query_transform'],
+                    'TestSize': config['TestSize']},
+                    config)
+                trans_thres()
+
+                # change dtypes for label
+                changeDtypes(
+                    {'database': config["database"],
+                        'username': config["username"],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_transform']},
+                    trans_label,
+                    ["int8"] * len(trans_label))
+                splitter_obj = splitter(
+                    {
+                        'labels_names': config['labels_names'],
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_split'],
+                        'TestSize': config['TestSize']})
+                splitter_obj()
+                # ...and map data['labels'] test
+            # 4. Train model
+            torch.distributed.barrier()
+            config['output'] = output_directory
+            config['output_directory'] = output_directory
+            config['table_name'] = output_table_name
+            config['use_DDP'] = 'True'
+            config['datasetFingerprintFile'] = None
+            train(config)
+
+            # 5 eval model
+
+            config['model']['pretrain_model'] = output_directory
+            test({**config, 'query': config["query_test"], 'TestSize': 1})
+
+
+
+            torch.distributed.barrier()
+            torch.distributed.destroy_process_group()
+            torch.cuda.empty_cache()
+
+            # plotting results
+            #torch.distributed.barrier()
+            #if torch.distributed.get_rank() == 0:
+            # 6 plot results:
+            # train
+            plot_results({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'table_name': output_table_name,
+                        'schema_name': config['schema_name'],
+                        'query': config['query_train_plot']},
+                        config['labels_names'],
+                        [i + "_predictions" for i in
+                            config['labels_names']],
+                        output_plots_train,
+                        config['model']['num_classes'],
+                        config,
+                        [i + "_confidences" for i in
+                            config['labels_names']]
+                        )
+
+            # aggregate stenosis for all groups :
+            # entryids or (PatientID, StudyInstanceUID)
+            agg = Aggregator({
+                                'labels_names': config['labels_names'],
+                                'database': config['database'],
+                                'username': config['username'],
+                                'password': config['password'],
+                                'host': config['host'],
+                                'schema_name': config['schema_name'],
+                                'table_name': output_table_name,
+                                'query':
+                                config['query_train_plot'],
+                                "num_classes":
+                                config["model"]["num_classes"],
+                                "loss_name": config['loss']['name']
+                                },
+                                [i + "_confidences" for i in
+                                config['labels_names']])
+            agg()
+            # plot results for entire cag
+            cag_segment = os.path.join(output_plots_train, 'cag_segment')
+            mkFolder(cag_segment)
+
+            plot_results({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'schema_name': config['schema_name'],
+                        'labels_names': config['labels_names'],
+                        'table_name': output_table_name,
+                        'query': config['query_count_stenosis_train']},
+                        config['labels_names'],
+                        [i + "_predictions" for i in
+                            config['labels_names']],
+                        cag_segment,
+                        config['model']['num_classes'],
+                        config,
+                        [i + "_confidences" for i in
+                            config['labels_names']],
+                        group_aggregated=True
+                        )
+
+            # val
+            plot_results({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'schema_name': config['schema_name'],
+                        'labels_names': config['labels_names'],
+                        'table_name': output_table_name,
+                        'query': config['query_val_plot']},
+                        config['labels_names'],
+                        [i + "_predictions" for i in
+                            config['labels_names']],
+                        output_plots_val,
+                        config['model']['num_classes'],
+                        config,
+                        [i + "_confidences" for i in
+                            config['labels_names']]
+                        )
+
+            # aggregate stenosis for all groups :
+            # entryids or (PatientID, StudyInstanceUID)
+            agg = Aggregator({
+                                'labels_names': config['labels_names'],
+                                'database': config['database'],
+                                'username': config['username'],
+                                'password': config['password'],
+                                'host': config['host'],
+                                'schema_name': config['schema_name'],
+                                'table_name': output_table_name,
+                                'query':
+                                config['query_val_plot'],
+                                "num_classes":
+                                config["model"]["num_classes"],
+                                "loss_name": config['loss']['name']},
+                                [i + "_confidences" for i in
+                                config['labels_names']])
+            agg()
+            # plot results for entire cag
+            cag_segment = os.path.join(output_plots_val, 'cag_segment')
+            mkFolder(cag_segment)
+
+            plot_results({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'table_name': output_table_name,
+                        'schema_name': config['schema_name'],
+                        'query': config['query_count_stenosis_val']},
+                        config['labels_names'],
+                        [i + "_predictions" for i in
+                            config['labels_names']],
+                        cag_segment,
+                        config['model']['num_classes'],
+                        config,
+                        confidence_names=[i + "_confidences" for i in
+                                            config['labels_names']],
+                        group_aggregated=True
+                        )
+
+            # test
+            plot_results({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_test_plot']},
+                        config['labels_names'],
+                        [i + "_predictions" for i in
+                            config['labels_names']],
+                        output_plots_test,
+                        config['model']['num_classes'],
+                        config,
+                        [i + "_confidences" for i in
+                            config['labels_names']]
+                        )
+            
+            # aggregate stenosis for all groups :
+            # entryids or (PatientID, StudyInstanceUID)
+            
+            agg = Aggregator({
+                                'labels_names': config['labels_names'],
+                                'database': config['database'],
+                                'username': config['username'],
+                                'password': config['password'],
+                                'host': config['host'],
+                                'schema_name': config['schema_name'],
+                                'table_name': output_table_name,
+                                'query':
+                                config['query_test_plot'],
+                                "num_classes":
+                                config["model"]["num_classes"],
+                                "loss_name": config['loss']['name']},
+                                [i + "_confidences" for i in
+                                config['labels_names']])
+            agg()
+            # plot results for entire cag
+            cag_segment = os.path.join(output_plots_test, 'cag_segment')
+            mkFolder(cag_segment)
+
+            plot_results({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_count_stenosis_test']},
+                        config['labels_names'],
+                        [i + "_predictions" for i in
+                            config['labels_names']],
+                        cag_segment,
+                        config['model']['num_classes'],
+                        config,
+                        confidence_names=[i + "_confidences" for i in
+                                            config['labels_names']],
+                        group_aggregated=True
+                        )
+
+
+            # # append results 
+            # csv_results = appendDataFrame(sql_config={
+            #                     'labels_names': config['labels_names'],
+            #                     'database': config['database'],
+            #                     'username': config['username'],
+            #                     'password': config['password'],
+            #                     'host': config['host'],
+            #                     'schema_name': config['schema_name'],
+            #                     'table_name': output_table_name,
+            #                     'query': config['query_test_plot']},
+            #                 df_results=df_results,
+            #                 experiment_name=experiment_name)
+            print('config files processed', str(i+1))
+            print('config files to process in toal:', len(config_path))
+          #  csv_results = pd.DataFrame(csv_results)
+            #csv_results.to_csv(output_csv_test, index=False, header=True)
+
+        if csv_exists:
+            return None
+        else:
+            return output_table_name
+
 
-    plotRegression({
-                'database': config_task['database'],
-                'username': config_task['username'],
-                'password': config_task['password'],
-                'host': config_task['host'],
-                'labels_names': config_task['labels_names'],
-                'schema_name': config_task['schema_name'],
-                'table_name': output_table_name,
-                'query': config_task['query_train_plot'],
-                'loss_name': config_task['loss']['name'],
-                'task_type': config_task['task_type']
-                },
-                config_task['labels_names'],
-                conf,
-                output_plots_train,
-                group_aggregated=False)
-        
-    # # val
-    # plot_results({
-    #             'database': config_task['database'],
-    #             'username': config_task['username'],
-    #             'password': config_task['password'],
-    #             'host': config_task['host'],
-    #             'labels_names': config_task['labels_names'],
-    #             'schema_name': config_task['schema_name'],
-    #             'table_name': output_table_name,
-    #             'query': config_task['query_val_plot']},
-    #             config_task['labels_names'],
-    #             [i + "_predictions" for i in
-    #                 config_task['labels_names']],
-    #             output_plots_val,
-    #             config_task['model']['num_classes'],
-    #             config_task,
-    #             [i + "_confidences" for i in
-    #                 config_task['labels_names']]
-    #             )
-
-    # plotRegression({
-    #             'database': config_task['database'],
-    #             'username': config_task['username'],
-    #             'password': config_task['password'],
-    #             'host': config_task['host'],
-    #             'labels_names': config_task['labels_names'],
-    #             'schema_name': config_task['schema_name'],
-    #             'table_name': output_table_name,
-    #             'query': config_task['query_val_plot'],
-    #             'loss_name': config_task['loss']['name'],
-    #             'task_type': config_task['task_type']
-    #             },
-    #             config_task['labels_names'],
-    #             conf,
-    #             output_plots_val,
-    #             group_aggregated=False)
-
-    # # test
-    # plot_results({
-    #             'database': config_task['database'],
-    #             'username': config_task['username'],
-    #             'password': config_task['password'],
-    #             'host': config_task['host'],
-    #             'labels_names': config_task['labels_names'],
-    #             'schema_name': config_task['schema_name'],
-    #             'table_name': output_table_name,
-    #             'query': config_task['query_test_plot']},
-    #             config_task['labels_names'],
-    #             [i + "_predictions" for i in
-    #                 config_task['labels_names']],
-    #             output_plots_test,
-    #             config_task['model']['num_classes'],
-    #             config_task,
-    #             [i + "_confidences" for i in
-    #                 config_task['labels_names']]
-    #             )
-
-    # plotRegression({
-    #             'database': config_task['database'],
-    #             'username': config_task['username'],
-    #             'password': config_task['password'],
-    #             'host': config_task['host'],
-    #             'labels_names': config_task['labels_names'],
-    #             'schema_name': config_task['schema_name'],
-    #             'table_name': output_table_name,
-    #             'query': config_task['query_test_plot'],
-    #             'loss_name': config_task['loss']['name'],
-    #             'task_type': config_task['task_type']
-    #             },
-    #             config_task['labels_names'],
-    #             conf,
-    #             output_plots_test,
-    #             group_aggregated=False)
-
-
-def plot_classification_tasks(config,
-                             output_table_name,
-                             output_plots_train, output_plots_val, output_plots_test):
-    df, conn = getDataFromDatabase({
-                            'database': config['database'],
-                            'username': config['username'],
-                            'password': config['password'],
-                            'host': config['host'],
-                            'labels_names': config['labels_names'],
-                            'schema_name': config['schema_name'],
-                            'table_name': output_table_name,
-                            'query': config['query_train_plot']})
-    # test if _confidences exists
-    if config['labels_names'][0] +"_confidences" in df.columns:
-        labels_names = config['labels_names'][0] +"_confidences"
-    elif config['labels_names'][0] +"_confid" in df.columns:
-        labels_names = config['labels_names'][0] +"_confid"
-    else:
-        raise ValueError("No confidence column found in database")
-        
-    df = df.dropna(subset=[labels_names], how="any")
-    y_scores = convert_string_to_numpy(df, column='koronarpatologi_nativekar_udfyldesforallept__transformed_confid')
-    label_binarizer = LabelBinarizer().fit(df[config['labels_names']])
-    y_onehot_test = label_binarizer.transform(df[config['labels_names']])
-    random_array = np.random.rand(4, 3)
-    y_scores = random_array / random_array.sum(axis=1, keepdims=True)
-    y_onehot_test = np.transpose(np.array([[1, 0, 2, 0]]))
-    label_binarizer = LabelBinarizer().fit(y_onehot_test)
-    y_onehot_test = label_binarizer.transform(y_onehot_test)
-    run_plotter_ruc_multi_class(y_scores, y_onehot_test,
-                                "corornay_pathology", "model",
-                                "roc_curve_coronar",
-                                output_plots_train)
-    #(y_score, y_onehot_test,
-                             #   type_outcome, model_name,
-                             #   ax, save_name, output_path):
-    print('hej')
-    return None
-
-
-def convert_string_to_numpy(df, column='koronarpatologi_nativekar_udfyldesforallept__transformed_confid'):
-    list_values = []
-
-    for row in df[column]:
-        # Transforming the string to a dictionary
-        row_dict = {int(k):float(v) for k,v in  (item.split(':') for item in row.strip('{}').split(';'))}
-        # Adding the values to a list
-        list_values.append(list(row_dict.values()))
-
-    # Transforming the list of lists to a numpy array
-    np_array = np.array(list_values)
-    
-    return np_array
 if __name__ == '__main__':
     args = parser.parse_args()
     stenosis_identifier(args.cpu, args.num_workers, args.config_path)
```

### Comparing `miacag-0.0.82/miacag/scripts/stenosis_identifier/submit_angio.py` & `miacag-0.0.83/miacag/scripts/stenosis_regression/submit_angio.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,37 +14,38 @@
 from miacag.tester import test
 from miacag.configs.config import load_config, maybe_create_tensorboard_logdir
 from miacag.configs.options import TrainOptions
 import argparse
 from miacag.preprocessing.labels_map import labelsMap
 from miacag.preprocessing.utils.check_experiments import checkExpExists, \
     checkCsvExists
-from miacag.plots.plotter import plot_results
+from miacag.plots.plotter import plot_results, plotRegression
 import pandas as pd
-from miacag.preprocessing.transform_thresholds import transformThreshold
+from miacag.preprocessing.transform_thresholds import transformThresholdRegression
 from miacag.preprocessing.transform_missing_floats import transformMissingFloats
-from miacag.utils.script_utils import create_empty_csv, mkFolder, maybe_remove, test_for_file, write_file
+from miacag.utils.script_utils import create_empty_csv, mkFolder, maybe_remove, write_file, test_for_file
 from miacag.postprocessing.aggregate_pr_group import Aggregator
 from miacag.postprocessing.count_stenosis_pr_group \
     import CountSignificantStenoses
 
+
 parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
-            "--local_rank", type=int,
-            help="Local rank: torch.distributed.launch.")
+    "--local_rank", type=int,
+    help="Local rank: torch.distributed.launch.")
 parser.add_argument(
             "--local-rank", type=int,
             help="Local rank: torch.distributed.launch.")
 parser.add_argument(
-            "--num_workers", type=int,
-            help="Number of cpu workers for training")    
+    "--num_workers", type=int,
+    help="Number of cpu workers for training")
 parser.add_argument(
     '--config_path', type=str,
     help="path to folder with config files")
 
 
 def stenosis_identifier(cpu, num_workers, config_path, table_name_input=None):
     if table_name_input is None:
@@ -58,20 +59,20 @@
 
     for i in range(0, len(config_path)):
         print('loading config:', config_path[i])
         with open(config_path[i]) as file:
             config = yaml.load(file, Loader=yaml.FullLoader)
         mkFolder(config['output'])
         csv_exists, output_csv_test = checkCsvExists(config['output'])
-        if csv_exists is False:
-            trans_label = \
-                [i + '_transformed' for i in config['labels_names']]
-            df_results = create_empty_csv(output_csv_test, trans_label)
-        else:
-            df_results = pd.read_csv(output_csv_test)
+        # if csv_exists is False:
+        #     trans_label = \
+        #         [i + '_transformed' for i in config['labels_names']]
+        #     df_results = create_empty_csv(output_csv_test, trans_label)
+        # else:
+        #     df_results = pd.read_csv(output_csv_test)
 
         exp_exists = checkExpExists(config_path[i], config['output'])
         if exp_exists is False:
 
             config['master_port'] = os.environ['MASTER_PORT']
             config['num_workers'] = num_workers
             config['cpu'] = cpu
@@ -133,14 +134,16 @@
             # rename labels and add columns;
             trans_label = [i + '_transformed' for i in config['labels_names']]
             labels_names_original = config['labels_names']
             config['labels_names'] = trans_label
             # add placeholder for confidences
             conf = [i + '_confidences' for i in config['labels_names']]
             conf_agg = [i + '_confidences_aggregated' for i in config['labels_names']]
+            conf_agg_t = [i + '_confidences_aggregated_thres' for i in config['labels_names']]
+
             # add placeholder for predictions
             pred = [i + '_predictions' for i in config['labels_names']]
 
             torch.distributed.barrier()
             if torch.distributed.get_rank() == 0:
                 add_columns({
                     'database': config['database'],
@@ -180,27 +183,35 @@
                     'password': config['password'],
                     'host': config['host'],
                     'schema_name': config['schema_name'],
                     'table_name': output_table_name,
                     'table_name_output': output_table_name},
                             pred,
                             ["float8"] * len(pred))
-
                 add_columns({
                     'database': config['database'],
                     'username': config['username'],
                     'password': config['password'],
                     'host': config['host'],
                     'schema_name': config['schema_name'],
                     'table_name': output_table_name,
                     'table_name_output': output_table_name},
                             conf_agg,
                             ["float8"] * len(conf))
+                add_columns({
+                    'database': config['database'],
+                    'username': config['username'],
+                    'password': config['password'],
+                    'host': config['host'],
+                    'schema_name': config['schema_name'],
+                    'table_name': output_table_name,
+                    'table_name_output': output_table_name},
+                            conf_agg_t,
+                            ["float8"] * len(conf))
                 
-
                 add_columns({
                     'database': config['database'],
                     'username': config['username'],
                     'password': config['password'],
                     'host': config['host'],
                     'schema_name': config['schema_name'],
                     'table_name': output_table_name,
@@ -217,15 +228,15 @@
                     'host': config['host'],
                     'schema_name': config['schema_name'],
                     'table_name': output_table_name,
                     'query': config['query_transform'],
                     'TestSize': config['TestSize']})
                 trans()
 
-                trans_thres = transformThreshold({
+                trans_thres = transformThresholdRegression({
                     'labels_names': config['labels_names'],
                     'database': config['database'],
                     'username': config['username'],
                     'password': config['password'],
                     'host': config['host'],
                     'schema_name': config['schema_name'],
                     'table_name': output_table_name,
@@ -240,15 +251,15 @@
                         'username': config["username"],
                         'password': config['password'],
                         'host': config['host'],
                         'schema_name': config['schema_name'],
                         'table_name': output_table_name,
                         'query': config['query_transform']},
                     trans_label,
-                    ["int8"] * len(trans_label))
+                    ["float8"] * len(trans_label))
                 splitter_obj = splitter(
                     {
                         'labels_names': config['labels_names'],
                         'database': config['database'],
                         'username': config['username'],
                         'password': config['password'],
                         'host': config['host'],
@@ -268,149 +279,209 @@
             train(config)
 
             # 5 eval model
 
             config['model']['pretrain_model'] = output_directory
             test({**config, 'query': config["query_test"], 'TestSize': 1})
 
-
-
+            print('kill gpu processes')
             torch.distributed.barrier()
-            torch.distributed.destroy_process_group()
             torch.cuda.empty_cache()
+            torch.distributed.destroy_process_group()
 
-            # plotting results
-            #torch.distributed.barrier()
-            #if torch.distributed.get_rank() == 0:
             # 6 plot results:
             # train
             plot_results({
                         'database': config['database'],
                         'username': config['username'],
                         'password': config['password'],
                         'host': config['host'],
                         'labels_names': config['labels_names'],
-                        'table_name': output_table_name,
                         'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
                         'query': config['query_train_plot']},
                         config['labels_names'],
                         [i + "_predictions" for i in
                             config['labels_names']],
                         output_plots_train,
                         config['model']['num_classes'],
                         config,
-                        [i + "_confidences" for i in
-                            config['labels_names']]
+                        confidence_names=[i + "_confidences" for i in
+                                            config['labels_names']]
                         )
-
+            plotRegression({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_train_plot'],
+                        'loss_name': config['loss']['name'],
+                        'task_type': config['task_type']
+                        },
+                        config['labels_names'],
+                        conf,
+                        output_plots_train)
+            
             # aggregate stenosis for all groups :
             # entryids or (PatientID, StudyInstanceUID)
             agg = Aggregator({
                                 'labels_names': config['labels_names'],
                                 'database': config['database'],
                                 'username': config['username'],
                                 'password': config['password'],
                                 'host': config['host'],
-                                'schema_name': config['schema_name'],
                                 'table_name': output_table_name,
+                                'schema_name': config['schema_name'],
                                 'query':
                                 config['query_train_plot'],
                                 "num_classes":
                                 config["model"]["num_classes"],
-                                "loss_name": config['loss']['name']
+                                'loss_name': config['loss']['name']
                                 },
                                 [i + "_confidences" for i in
                                 config['labels_names']])
             agg()
+
             # plot results for entire cag
             cag_segment = os.path.join(output_plots_train, 'cag_segment')
             mkFolder(cag_segment)
 
             plot_results({
                         'database': config['database'],
                         'username': config['username'],
                         'password': config['password'],
                         'host': config['host'],
-                        'schema_name': config['schema_name'],
                         'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
                         'table_name': output_table_name,
                         'query': config['query_count_stenosis_train']},
                         config['labels_names'],
                         [i + "_predictions" for i in
                             config['labels_names']],
                         cag_segment,
                         config['model']['num_classes'],
                         config,
-                        [i + "_confidences" for i in
-                            config['labels_names']],
+                        confidence_names=[i + "_confidences" for i in
+                                            config['labels_names']],
                         group_aggregated=True
                         )
-
+            plotRegression({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_count_stenosis_train'],
+                        'loss_name': config['loss']['name'],
+                        'task_type': config['task_type']
+                        },
+                        config['labels_names'],
+                        conf_agg,
+                        cag_segment,
+                        group_aggregated=True)
+                
             # val
             plot_results({
                         'database': config['database'],
                         'username': config['username'],
                         'password': config['password'],
                         'host': config['host'],
-                        'schema_name': config['schema_name'],
                         'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
                         'table_name': output_table_name,
                         'query': config['query_val_plot']},
                         config['labels_names'],
                         [i + "_predictions" for i in
                             config['labels_names']],
                         output_plots_val,
                         config['model']['num_classes'],
                         config,
-                        [i + "_confidences" for i in
-                            config['labels_names']]
+                        confidence_names=[i + "_confidences" for i in
+                                            config['labels_names']]
                         )
-
+            plotRegression({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_val_plot'],
+                        'loss_name': config['loss']['name'],
+                        'task_type': config['task_type']},
+                        config['labels_names'],
+                        conf,
+                        output_plots_val)
             # aggregate stenosis for all groups :
             # entryids or (PatientID, StudyInstanceUID)
             agg = Aggregator({
                                 'labels_names': config['labels_names'],
                                 'database': config['database'],
                                 'username': config['username'],
                                 'password': config['password'],
                                 'host': config['host'],
                                 'schema_name': config['schema_name'],
                                 'table_name': output_table_name,
                                 'query':
                                 config['query_val_plot'],
                                 "num_classes":
                                 config["model"]["num_classes"],
-                                "loss_name": config['loss']['name']},
+                                'loss_name': config['loss']['name']
+                                },
                                 [i + "_confidences" for i in
                                 config['labels_names']])
             agg()
+        
             # plot results for entire cag
             cag_segment = os.path.join(output_plots_val, 'cag_segment')
             mkFolder(cag_segment)
 
             plot_results({
                         'database': config['database'],
                         'username': config['username'],
                         'password': config['password'],
                         'host': config['host'],
                         'labels_names': config['labels_names'],
-                        'table_name': output_table_name,
                         'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
                         'query': config['query_count_stenosis_val']},
                         config['labels_names'],
                         [i + "_predictions" for i in
                             config['labels_names']],
                         cag_segment,
                         config['model']['num_classes'],
                         config,
                         confidence_names=[i + "_confidences" for i in
                                             config['labels_names']],
                         group_aggregated=True
                         )
 
+            plotRegression({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_count_stenosis_val'],
+                        'loss_name': config['loss']['name'],
+                        'task_type': config['task_type']},
+                        config['labels_names'],
+                        conf_agg,
+                        cag_segment,
+                        group_aggregated=True)
+
+
             # test
             plot_results({
                         'database': config['database'],
                         'username': config['username'],
                         'password': config['password'],
                         'host': config['host'],
                         'labels_names': config['labels_names'],
@@ -419,37 +490,51 @@
                         'query': config['query_test_plot']},
                         config['labels_names'],
                         [i + "_predictions" for i in
                             config['labels_names']],
                         output_plots_test,
                         config['model']['num_classes'],
                         config,
-                        [i + "_confidences" for i in
-                            config['labels_names']]
+                        confidence_names=[i + "_confidences" for i in
+                                            config['labels_names']]
                         )
-            
+            plotRegression({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_test_plot'],
+                        'loss_name': config['loss']['name'],
+                        'task_type': config['task_type']},
+                        config['labels_names'],
+                        conf,
+                        output_plots_test)
             # aggregate stenosis for all groups :
             # entryids or (PatientID, StudyInstanceUID)
-            
+
             agg = Aggregator({
                                 'labels_names': config['labels_names'],
                                 'database': config['database'],
                                 'username': config['username'],
                                 'password': config['password'],
                                 'host': config['host'],
                                 'schema_name': config['schema_name'],
                                 'table_name': output_table_name,
                                 'query':
                                 config['query_test_plot'],
                                 "num_classes":
                                 config["model"]["num_classes"],
-                                "loss_name": config['loss']['name']},
+                                'loss_name': config['loss']['name']},
                                 [i + "_confidences" for i in
                                 config['labels_names']])
             agg()
+
             # plot results for entire cag
             cag_segment = os.path.join(output_plots_test, 'cag_segment')
             mkFolder(cag_segment)
 
             plot_results({
                         'database': config['database'],
                         'username': config['username'],
@@ -465,32 +550,33 @@
                         cag_segment,
                         config['model']['num_classes'],
                         config,
                         confidence_names=[i + "_confidences" for i in
                                             config['labels_names']],
                         group_aggregated=True
                         )
+            plotRegression({
+                        'database': config['database'],
+                        'username': config['username'],
+                        'password': config['password'],
+                        'host': config['host'],
+                        'labels_names': config['labels_names'],
+                        'schema_name': config['schema_name'],
+                        'table_name': output_table_name,
+                        'query': config['query_count_stenosis_test'],
+                        'loss_name': config['loss']['name'],
+                        'task_type': config['task_type']},
+                        config['labels_names'],
+                        conf_agg,
+                        cag_segment,
+                        group_aggregated=True)
 
 
-            # # append results 
-            # csv_results = appendDataFrame(sql_config={
-            #                     'labels_names': config['labels_names'],
-            #                     'database': config['database'],
-            #                     'username': config['username'],
-            #                     'password': config['password'],
-            #                     'host': config['host'],
-            #                     'schema_name': config['schema_name'],
-            #                     'table_name': output_table_name,
-            #                     'query': config['query_test_plot']},
-            #                 df_results=df_results,
-            #                 experiment_name=experiment_name)
             print('config files processed', str(i+1))
             print('config files to process in toal:', len(config_path))
-          #  csv_results = pd.DataFrame(csv_results)
-            #csv_results.to_csv(output_csv_test, index=False, header=True)
 
         if csv_exists:
             return None
         else:
             return output_table_name
```

### Comparing `miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/submit_angio.py` & `miacag-0.0.83/miacag/scripts/stenosis_identifier_mil/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/scripts/stenosis_regression_full/submit_angio.py` & `miacag-0.0.83/miacag/scripts/stenosis_regression_full/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/tester.py` & `miacag-0.0.83/miacag/tester.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/tests/test_sql_utils.py` & `miacag-0.0.83/miacag/tests/test_sql_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/trainer.py` & `miacag-0.0.83/miacag/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,30 +60,30 @@
                                             len(train_loader))
 
     # Use AMP for speedup:
     scaler = torch.cuda.amp.GradScaler() \
         if config['loaders']['use_amp'] else None
     best_val_loss, best_val_epoch = None, None
     early_stop = False
-    if config['cache_num'] != 'None':
+    if config['cache_num'] not in ['standard', 'None']:
         train_ds.start()
 
     starter = time.time()
     #  ---- Start training loop ----#
     for epoch in range(0, config['trainer']['epochs']):
         print('epoch nr', epoch)
         # train one epoch
 
         train_one_epoch(model, criterion,
                         train_loader, device, epoch,
                         optimizer, lr_scheduler,
                         running_metric_train, running_loss_train,
                         writer, config, scaler)
 
-        if config['cache_num'] != 'None':
+        if config['cache_num'] not in  ['standard', 'None']:
             train_ds.update_cache()
 
         #  validation one epoch (but not necessarily each)
         if epoch % config['trainer']['validate_frequency'] == 0:
             metric_dict_val = val_one_epoch(model, criterion, config,
                                             val_loader, device,
                                             running_metric_val,
@@ -97,15 +97,15 @@
             # save model
             if best_val_epoch == epoch:
                 if torch.distributed.get_rank() == 0:
                     save_model(model, writer, config)
             if early_stop is True:
                 break
 
-    if config['cache_num'] != 'None':
+    if config['cache_num'] not in ['standard', 'None']:
         train_ds.shutdown()
 
     if early_stop is False:
         if torch.distributed.get_rank() == 0:
             save_model(model, writer, config)
     if torch.distributed.get_rank() == 0:
         saver(metric_dict_val, writer, config)
```

### Comparing `miacag-0.0.82/miacag/utils/common_utils.py` & `miacag-0.0.83/miacag/utils/common_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
         if label_name.partition("_")[0] == loss_name.partition("_")[-1]:
             if loss_name.startswith(tuple(['MSE', '_L1', 'L1smooth'])):
                 stacked_data.append(data[label_name])
             elif loss_name.startswith(tuple(['BCE_multilabel'])):
                 stacked_data.append(data[label_name])
             elif loss_name.startswith(tuple(['CE'])):
                 stacked_data.append(data[label_name])
+            elif loss_name.startswith(tuple(['NNL'])):
+                stacked_data.append(data[label_name])
             else:
                 raise ValueError('this loss is not implementeed:', loss_name)
     return torch.stack(stacked_data, 1)
 
 
 #
 def wrap_outputs_to_dict(outputs, config):
@@ -36,19 +38,23 @@
 
 # this function is used to get the loss for each task
 def get_losses_class(config, outputs, data, criterion, device):
     losses = []
     loss_tot = torch.tensor([0]).float()
     loss_tot = loss_tot.to(device)
     loss_tot = loss_tot.requires_grad_()
+
     for count_idx, loss_name in enumerate(config['loss']['groups_names']):
         labels = stack_labels(data, config, loss_name)
+        event = None
+        if loss_name.startswith('NNL'):
+            event = data['event']
         loss = get_loss(
             config, outputs[count_idx],
-            labels, criterion[count_idx], loss_name)
+            labels, criterion[count_idx], loss_name, event)
         #print('done')
         if torch.isnan(loss) == torch.tensor(True, device=device):
             #raise ValueError('the loss is nan!')
             # # ugly hack
             if count_idx == 0:
                 t = torch.tensor([1]).float()
                 
@@ -65,16 +71,19 @@
             losses.append(loss)
             loss_tot = loss_tot + loss
     losses = [loss_indi.item() for loss_indi in losses]
     losses = losses + [loss_tot.item()]
     return losses, loss_tot
 
 # get loss function
-def get_loss(config, outputs, labels, criterion, loss_name):
+def get_loss(config, outputs, labels, criterion, loss_name, event=None):
     if 'Siam' in config['loss']['name']:
         loss = criterion(outputs)
     elif loss_name.startswith('CE'):
         labels = torch.reshape(labels, (labels.shape[0], ))
         loss = criterion(outputs, labels)
+     #   loss = criterion(torch.tensor(outputs), labels)
+    elif loss_name.startswith('NNL'):
+        loss = criterion(outputs, labels, event)
     else:
         loss = criterion(outputs, labels)
     return loss
```

### Comparing `miacag-0.0.82/miacag/utils/script_utils.py` & `miacag-0.0.83/miacag/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag/utils/sql_utils.py` & `miacag-0.0.83/miacag/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.82/miacag.egg-info/PKG-INFO` & `miacag-0.0.83/miacag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miacag
-Version: 0.0.82
+Version: 0.0.83
 Summary: miacag angio DL tools
 Home-page: https://github.com/ChristianEschen/miacag
 Author: Christian Eschen
 Author-email: christian_eschen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miacag-0.0.82/miacag.egg-info/SOURCES.txt` & `miacag-0.0.83/miacag.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 miacag/__init__.py
+miacag/features.py
 miacag/predictor.py
 miacag/tester.py
 miacag/trainer.py
 miacag.egg-info/PKG-INFO
 miacag.egg-info/SOURCES.txt
 miacag.egg-info/dependency_links.txt
 miacag.egg-info/top_level.txt
@@ -26,26 +27,28 @@
 miacag/dataloader/dataloader_base_monai.py
 miacag/dataloader/get_dataloader.py
 miacag/dataloader/Classification/__init__.py
 miacag/dataloader/Classification/get_dataloader_classification.py
 miacag/dataloader/Classification/_2D/__init__.py
 miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py
 miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py
+miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil_fast.py
 miacag/dataloader/Classification/_2D/dataset_mil_2d.py
 miacag/dataloader/Classification/_3D/__init__.py
 miacag/dataloader/Classification/_3D/dataloader_avi_video.py
 miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py
 miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py
 miacag/dataloader/Classification/_3D/dataset_mil.py
 miacag/dataloader/Representation/__init__.py
 miacag/dataloader/Representation/get_dataloader_representation.py
 miacag/metrics/__init__.py
 miacag/metrics/cumulativeSumming.py
 miacag/metrics/metrics.py
 miacag/metrics/metrics_utils.py
+miacag/metrics/survival_metrics.py
 miacag/model_utils/GradCam_model.py
 miacag/model_utils/__init__.py
 miacag/model_utils/eval_utils.py
 miacag/model_utils/get_loss_func.py
 miacag/model_utils/get_optimizer.py
 miacag/model_utils/get_test_pipeline.py
 miacag/model_utils/grad_cam_utils.py
@@ -60,14 +63,15 @@
 miacag/models/milmodel3d.py
 miacag/models/milmodel_from_features.py
 miacag/models/mlps.py
 miacag/models/modeling_finetune.py
 miacag/models/modeling_pretrain.py
 miacag/models/modules.py
 miacag/models/pretrained_vit.py
+miacag/models/vision_transformer.py
 miacag/models/backbone_encoders/__init__.py
 miacag/models/backbone_encoders/tabular/__init__.py
 miacag/models/backbone_encoders/tabular/base_encoders.py
 miacag/models/dino_utils/__init__.py
 miacag/models/dino_utils/dino_pretrained.py
 miacag/models/mae_st_util/__init__.py
 miacag/models/mae_st_util/logging.py
@@ -86,14 +90,15 @@
 miacag/plots/getDataFromPdf.py
 miacag/plots/plot_histogram.py
 miacag/plots/plot_pathology_treatment_pred.py
 miacag/plots/plot_predict_coronary_pathology.py
 miacag/plots/plot_roc_auc_all.py
 miacag/plots/plot_scatter.py
 miacag/plots/plot_test.py
+miacag/plots/plot_utils.py
 miacag/plots/plotter.py
 miacag/plots/query_plot_agg_max.py
 miacag/postprocessing/__init__.py
 miacag/postprocessing/aggregate_pr_group.py
 miacag/postprocessing/append_results.py
 miacag/postprocessing/count_stenosis_pr_group.py
 miacag/postprocessing/estimate_vessel_disease.py
@@ -135,8 +140,9 @@
 miacag/scripts/stenosis_regression_full/__init__.py
 miacag/scripts/stenosis_regression_full/submit_angio.py
 miacag/tests/__init__.py
 miacag/tests/test_sql_utils.py
 miacag/utils/__init__.py
 miacag/utils/common_utils.py
 miacag/utils/script_utils.py
-miacag/utils/sql_utils.py
+miacag/utils/sql_utils.py
+miacag/utils/survival_utils.py
```

### Comparing `miacag-0.0.82/setup.cfg` & `miacag-0.0.83/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = miacag
-version = 0.0.82
+version = 0.0.83
 author = Christian Eschen
 author_email = christian_eschen@hotmail.com
 description = miacag angio DL tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ChristianEschen/miacag
 classifiers =
```

