# Comparing `tmp/delia-1.2.0.tar.gz` & `tmp/delia-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delia-1.2.0.tar", last modified: Tue Jun 20 15:28:16 2023, max compression
+gzip compressed data, was "delia-1.2.1.tar", last modified: Wed Jun 21 13:09:30 2023, max compression
```

## Comparing `delia-1.2.0.tar` & `delia-1.2.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.416128 delia-1.2.0/
--rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    15339 2023-06-20 15:28:16.416128 delia-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    14707 2023-06-20 15:23:09.000000 delia-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.315293 delia-1.2.0/delia/
--rw-rw-rw-   0        0        0      583 2023-06-20 15:27:34.000000 delia-1.2.0/delia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.324396 delia-1.2.0/delia/databases/
--rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.2.0/delia/databases/__init__.py
--rw-rw-rw-   0        0        0    13272 2023-06-20 15:23:09.000000 delia-1.2.0/delia/databases/patients_database.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.327416 delia-1.2.0/delia/extractors/
--rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.2.0/delia/extractors/__init__.py
--rw-rw-rw-   0        0        0    14578 2023-06-20 15:23:09.000000 delia-1.2.0/delia/extractors/patients_data_extractor.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.331461 delia-1.2.0/delia/radiomics/
--rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.2.0/delia/radiomics/__init__.py
--rw-rw-rw-   0        0        0    11664 2023-06-20 15:23:09.000000 delia-1.2.0/delia/radiomics/radiomics_dataset.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.333458 delia-1.2.0/delia/readers/
--rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.2.0/delia/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.335998 delia-1.2.0/delia/readers/image/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/image/__init__.py
--rw-rw-rw-   0        0        0    11258 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/image/dicom_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.342644 delia-1.2.0/delia/readers/patient_data/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/patient_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.346924 delia-1.2.0/delia/readers/patient_data/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/patient_data/factories/__init__.py
--rw-rw-rw-   0        0        0     5110 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/factories/base_patient_data_factory.py
--rw-rw-rw-   0        0        0     8114 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/factories/patient_data_factories.py
--rw-rw-rw-   0        0        0     3974 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/patient_data_query_context.py
--rw-rw-rw-   0        0        0      943 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/patient_data_query_strategy.py
--rw-rw-rw-   0        0        0    10030 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/patient_data_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.354035 delia-1.2.0/delia/readers/segmentation/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/segmentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.363035 delia-1.2.0/delia/readers/segmentation/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/segmentation/factories/__init__.py
--rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.2.0/delia/readers/segmentation/factories/base_segmentation_factory.py
--rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.2.0/delia/readers/segmentation/factories/dicom_segmentation_factories.py
--rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.2.0/delia/readers/segmentation/factories/segment.py
--rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/segmentation/factories/segmentation.py
--rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.2.0/delia/readers/segmentation/segmentation_context.py
--rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.2.0/delia/readers/segmentation/segmentation_reader.py
--rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.2.0/delia/readers/segmentation/segmentation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.369205 delia-1.2.0/delia/transforms/
--rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.2.0/delia/transforms/__init__.py
--rw-rw-rw-   0        0        0    13141 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/applications.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.379481 delia-1.2.0/delia/transforms/array_space/
--rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.2.0/delia/transforms/array_space/__init__.py
--rw-rw-rw-   0        0        0     5085 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/array_space/matching_centroid_spatial_crop.py
--rw-rw-rw-   0        0        0     3096 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/array_space/matching_crop_foreground.py
--rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.2.0/delia/transforms/array_space/tools.py
--rw-rw-rw-   0        0        0     2544 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/array_space/transform.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.385077 delia-1.2.0/delia/transforms/data/
--rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.2.0/delia/transforms/data/__init__.py
--rw-rw-rw-   0        0        0     4558 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/data/copy_segmentations.py
--rw-rw-rw-   0        0        0     1864 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/data/transform.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.395067 delia-1.2.0/delia/transforms/physical_space/
--rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.2.0/delia/transforms/physical_space/__init__.py
--rw-rw-rw-   0        0        0     3360 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/matching_resample.py
--rw-rw-rw-   0        0        0     9808 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/pet_to_suv.py
--rw-rw-rw-   0        0        0     3694 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/resample.py
--rw-rw-rw-   0        0        0     2992 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/transform.py
--rw-rw-rw-   0        0        0     2403 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.403067 delia-1.2.0/delia/utils/
--rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.2.0/delia/utils/__init__.py
--rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.2.0/delia/utils/data_model.py
--rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.2.0/delia/utils/tools.py
--rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.2.0/delia/utils/transforms_history.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.319297 delia-1.2.0/delia.egg-info/
--rw-rw-rw-   0        0        0    15339 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2252 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.414692 delia-1.2.0/examples/
--rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.2.0/examples/__init__.py
--rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.2.0/examples/env_examples.py
--rw-rw-rw-   0        0        0     3440 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex01.py
--rw-rw-rw-   0        0        0     3085 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex02.py
--rw-rw-rw-   0        0        0     2726 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex03.py
--rw-rw-rw-   0        0        0     5348 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex04.py
--rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 15:28:16.416128 delia-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-06-20 15:27:44.000000 delia-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:30.027655 delia-1.2.1/
+-rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    15339 2023-06-21 13:09:30.026659 delia-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14707 2023-06-20 15:23:09.000000 delia-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.931163 delia-1.2.1/delia/
+-rw-rw-rw-   0        0        0      583 2023-06-21 13:08:38.000000 delia-1.2.1/delia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.938039 delia-1.2.1/delia/databases/
+-rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.2.1/delia/databases/__init__.py
+-rw-rw-rw-   0        0        0    13508 2023-06-21 12:58:00.000000 delia-1.2.1/delia/databases/patients_database.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.942345 delia-1.2.1/delia/extractors/
+-rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.2.1/delia/extractors/__init__.py
+-rw-rw-rw-   0        0        0    14578 2023-06-20 15:23:09.000000 delia-1.2.1/delia/extractors/patients_data_extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.946014 delia-1.2.1/delia/radiomics/
+-rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.2.1/delia/radiomics/__init__.py
+-rw-rw-rw-   0        0        0    11664 2023-06-20 15:23:09.000000 delia-1.2.1/delia/radiomics/radiomics_dataset.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.948051 delia-1.2.1/delia/readers/
+-rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.2.1/delia/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.950040 delia-1.2.1/delia/readers/image/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.1/delia/readers/image/__init__.py
+-rw-rw-rw-   0        0        0    11258 2023-06-20 15:23:09.000000 delia-1.2.1/delia/readers/image/dicom_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.956739 delia-1.2.1/delia/readers/patient_data/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.1/delia/readers/patient_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.961705 delia-1.2.1/delia/readers/patient_data/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.1/delia/readers/patient_data/factories/__init__.py
+-rw-rw-rw-   0        0        0     5110 2023-06-20 15:23:09.000000 delia-1.2.1/delia/readers/patient_data/factories/base_patient_data_factory.py
+-rw-rw-rw-   0        0        0     8114 2023-06-20 15:23:09.000000 delia-1.2.1/delia/readers/patient_data/factories/patient_data_factories.py
+-rw-rw-rw-   0        0        0     3974 2023-06-20 15:23:09.000000 delia-1.2.1/delia/readers/patient_data/patient_data_query_context.py
+-rw-rw-rw-   0        0        0      943 2023-06-20 15:23:09.000000 delia-1.2.1/delia/readers/patient_data/patient_data_query_strategy.py
+-rw-rw-rw-   0        0        0    10030 2023-06-20 15:23:09.000000 delia-1.2.1/delia/readers/patient_data/patient_data_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.967920 delia-1.2.1/delia/readers/segmentation/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.1/delia/readers/segmentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.976797 delia-1.2.1/delia/readers/segmentation/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.1/delia/readers/segmentation/factories/__init__.py
+-rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.2.1/delia/readers/segmentation/factories/base_segmentation_factory.py
+-rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.2.1/delia/readers/segmentation/factories/dicom_segmentation_factories.py
+-rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.2.1/delia/readers/segmentation/factories/segment.py
+-rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.2.1/delia/readers/segmentation/factories/segmentation.py
+-rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.2.1/delia/readers/segmentation/segmentation_context.py
+-rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.2.1/delia/readers/segmentation/segmentation_reader.py
+-rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.2.1/delia/readers/segmentation/segmentation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.983581 delia-1.2.1/delia/transforms/
+-rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.2.1/delia/transforms/__init__.py
+-rw-rw-rw-   0        0        0    13141 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/applications.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.992601 delia-1.2.1/delia/transforms/array_space/
+-rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.2.1/delia/transforms/array_space/__init__.py
+-rw-rw-rw-   0        0        0     5085 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/array_space/matching_centroid_spatial_crop.py
+-rw-rw-rw-   0        0        0     3096 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/array_space/matching_crop_foreground.py
+-rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.2.1/delia/transforms/array_space/tools.py
+-rw-rw-rw-   0        0        0     2544 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/array_space/transform.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.997455 delia-1.2.1/delia/transforms/data/
+-rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.2.1/delia/transforms/data/__init__.py
+-rw-rw-rw-   0        0        0     4558 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/data/copy_segmentations.py
+-rw-rw-rw-   0        0        0     1864 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/data/transform.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:30.006520 delia-1.2.1/delia/transforms/physical_space/
+-rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.2.1/delia/transforms/physical_space/__init__.py
+-rw-rw-rw-   0        0        0     3360 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/physical_space/matching_resample.py
+-rw-rw-rw-   0        0        0     9808 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/physical_space/pet_to_suv.py
+-rw-rw-rw-   0        0        0     3694 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/physical_space/resample.py
+-rw-rw-rw-   0        0        0     2992 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/physical_space/transform.py
+-rw-rw-rw-   0        0        0     2403 2023-06-20 15:23:09.000000 delia-1.2.1/delia/transforms/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:30.014111 delia-1.2.1/delia/utils/
+-rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.2.1/delia/utils/__init__.py
+-rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.2.1/delia/utils/data_model.py
+-rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.2.1/delia/utils/tools.py
+-rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.2.1/delia/utils/transforms_history.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:29.934453 delia-1.2.1/delia.egg-info/
+-rw-rw-rw-   0        0        0    15339 2023-06-21 13:09:29.000000 delia-1.2.1/delia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2252 2023-06-21 13:09:29.000000 delia-1.2.1/delia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:09:29.000000 delia-1.2.1/delia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-21 13:09:29.000000 delia-1.2.1/delia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 13:09:29.000000 delia-1.2.1/delia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 13:09:30.025636 delia-1.2.1/examples/
+-rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.2.1/examples/__init__.py
+-rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.2.1/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3440 2023-06-20 15:23:09.000000 delia-1.2.1/examples/ex01.py
+-rw-rw-rw-   0        0        0     3085 2023-06-20 15:23:09.000000 delia-1.2.1/examples/ex02.py
+-rw-rw-rw-   0        0        0     2726 2023-06-20 15:23:09.000000 delia-1.2.1/examples/ex03.py
+-rw-rw-rw-   0        0        0     5348 2023-06-20 15:23:09.000000 delia-1.2.1/examples/ex04.py
+-rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:09:30.027655 delia-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-06-21 13:08:38.000000 delia-1.2.1/setup.py
```

### Comparing `delia-1.2.0/LICENSE` & `delia-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/PKG-INFO` & `delia-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.2.0
+Version: 1.2.1
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.2.0/README.md` & `delia-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/__init__.py` & `delia-1.2.1/delia/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from .utils import PatientDataModel
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "Maxence Larose"
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __copyright__ = "Copyright 2022, Maxence Larose"
 __credits__ = ["Maxence Larose"]
 __license__ = "Apache License 2.0"
 __maintainer__ = "Maxence Larose"
 __email__ = "maxence.larose.1@ulaval.ca"
 __status__ = "Production"
```

### Comparing `delia-1.2.0/delia/databases/patients_database.py` & `delia-1.2.1/delia/databases/patients_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         ----------
         path_to_database : str
             Path to database.
         """
         self.path_to_database = path_to_database
 
         if os.path.exists(path_to_database):
-            self._file = h5py.File(path_to_database, mode="r+")
+            try:
+                self._file = h5py.File(path_to_database, mode="r+")
+            except OSError:
+                self._file = h5py.File(path_to_database, mode="r")
         else:
             self._file = None
 
     @property
     def path_to_database(self) -> str:
         """
         Path to database.
@@ -311,15 +314,18 @@
                     )
 
                 _logger.info(f"Progress : {patient_idx + 1}/{number_of_patients} patients added to database.")
 
             patients_data_extractor.close()
             patients_data_extractor.reset()
 
-        self._file = h5py.File(self.path_to_database, "r+")
+        try:
+            self._file = h5py.File(self.path_to_database, mode="r+")
+        except OSError:
+            self._file = h5py.File(self.path_to_database, mode="r")
 
         return patients_data_extractor.patients_who_failed
 
     def close(self):
         """
         Closes the hdf5 file database.
         """
```

### Comparing `delia-1.2.0/delia/extractors/patients_data_extractor.py` & `delia-1.2.1/delia/extractors/patients_data_extractor.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/radiomics/radiomics_dataset.py` & `delia-1.2.1/delia/radiomics/radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/image/dicom_reader.py` & `delia-1.2.1/delia/readers/image/dicom_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/patient_data/factories/base_patient_data_factory.py` & `delia-1.2.1/delia/readers/patient_data/factories/base_patient_data_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/patient_data/factories/patient_data_factories.py` & `delia-1.2.1/delia/readers/patient_data/factories/patient_data_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/patient_data/patient_data_query_context.py` & `delia-1.2.1/delia/readers/patient_data/patient_data_query_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/patient_data/patient_data_query_strategy.py` & `delia-1.2.1/delia/readers/patient_data/patient_data_query_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/patient_data/patient_data_reader.py` & `delia-1.2.1/delia/readers/patient_data/patient_data_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/segmentation/factories/base_segmentation_factory.py` & `delia-1.2.1/delia/readers/segmentation/factories/base_segmentation_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/segmentation/factories/dicom_segmentation_factories.py` & `delia-1.2.1/delia/readers/segmentation/factories/dicom_segmentation_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/segmentation/factories/segment.py` & `delia-1.2.1/delia/readers/segmentation/factories/segment.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/segmentation/factories/segmentation.py` & `delia-1.2.1/delia/readers/segmentation/factories/segmentation.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/segmentation/segmentation_context.py` & `delia-1.2.1/delia/readers/segmentation/segmentation_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/segmentation/segmentation_reader.py` & `delia-1.2.1/delia/readers/segmentation/segmentation_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/readers/segmentation/segmentation_strategy.py` & `delia-1.2.1/delia/readers/segmentation/segmentation_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/applications.py` & `delia-1.2.1/delia/transforms/applications.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/array_space/matching_centroid_spatial_crop.py` & `delia-1.2.1/delia/transforms/array_space/matching_centroid_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/array_space/matching_crop_foreground.py` & `delia-1.2.1/delia/transforms/array_space/matching_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/array_space/tools.py` & `delia-1.2.1/delia/transforms/array_space/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/array_space/transform.py` & `delia-1.2.1/delia/transforms/array_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/data/copy_segmentations.py` & `delia-1.2.1/delia/transforms/data/copy_segmentations.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/data/transform.py` & `delia-1.2.1/delia/transforms/data/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/physical_space/matching_resample.py` & `delia-1.2.1/delia/transforms/physical_space/matching_resample.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/physical_space/pet_to_suv.py` & `delia-1.2.1/delia/transforms/physical_space/pet_to_suv.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/physical_space/resample.py` & `delia-1.2.1/delia/transforms/physical_space/resample.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/physical_space/transform.py` & `delia-1.2.1/delia/transforms/physical_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/transforms/tools.py` & `delia-1.2.1/delia/transforms/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/utils/data_model.py` & `delia-1.2.1/delia/utils/data_model.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/utils/tools.py` & `delia-1.2.1/delia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia/utils/transforms_history.py` & `delia-1.2.1/delia/utils/transforms_history.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/delia.egg-info/PKG-INFO` & `delia-1.2.1/delia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.2.0
+Version: 1.2.1
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.2.0/delia.egg-info/SOURCES.txt` & `delia-1.2.1/delia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/examples/env_examples.py` & `delia-1.2.1/examples/env_examples.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/examples/ex01.py` & `delia-1.2.1/examples/ex01.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/examples/ex02.py` & `delia-1.2.1/examples/ex02.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/examples/ex03.py` & `delia-1.2.1/examples/ex03.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/examples/ex04.py` & `delia-1.2.1/examples/ex04.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.0/setup.py` & `delia-1.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="delia",
-    version="1.2.0",
+    version="1.2.1",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="DICOM Extraction for Large-scale Image Analysis (DELIA).",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/delia",
     license="Apache License 2.0",
```

