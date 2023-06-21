# Comparing `tmp/cognite_sdk-6.4.4.tar.gz` & `tmp/cognite_sdk-6.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.4.4.tar", max compression
+gzip compressed data, was "cognite_sdk-6.4.5.tar", max compression
```

## Comparing `cognite_sdk-6.4.4.tar` & `cognite_sdk-6.4.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0    11349 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/README.md
--rw-r--r--   0        0        0      574 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     7857 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8393 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    24633 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6424 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7857 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11025 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17192 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41485 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45301 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49823 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38099 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     3629 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    12076 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7267 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4019 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     6238 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    28930 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2543 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14635 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6037 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7684 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/README.md
+-rw-r--r--   0        0        0      574 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     7857 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8393 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    26302 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6424 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7857 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11025 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17192 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41485 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45301 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49823 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38099 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     3629 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    12076 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7267 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4019 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     6238 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    28930 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2543 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14855 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6037 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7684 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.5/PKG-INFO
```

### Comparing `cognite_sdk-6.4.4/LICENSE` & `cognite_sdk-6.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/README.md` & `cognite_sdk-6.4.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/__init__.py` & `cognite_sdk-6.4.5/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/annotations.py` & `cognite_sdk-6.4.5/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/assets.py` & `cognite_sdk-6.4.5/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from cognite.client._constants import INSTANCES_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes._base import CogniteResourceList
 from cognite.client.data_classes.data_modeling.filters import Filter
 from cognite.client.data_classes.data_modeling.ids import (
     EdgeId,
     NodeId,
     ViewId,
+    ViewIdentifier,
     _load_identifier,
 )
 from cognite.client.data_classes.data_modeling.instances import (
     Edge,
     EdgeApply,
     EdgeApplyResult,
     EdgeApplyResultList,
@@ -25,14 +26,15 @@
     InstancesResult,
     Node,
     NodeApply,
     NodeApplyResult,
     NodeApplyResultList,
     NodeList,
 )
+from cognite.client.data_classes.data_modeling.views import View
 from cognite.client.utils._identifier import DataModelingIdentifierSequence
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
 
 class _NodeOrEdgeList(CogniteResourceList):
@@ -209,43 +211,58 @@
         """
         return cast(Iterator[Node], self(None, "node"))
 
     def retrieve(
         self,
         nodes: NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None = None,
         edges: EdgeId | Sequence[EdgeId] | tuple[str, str] | Sequence[tuple[str, str]] | None = None,
-        sources: list[ViewId] | ViewId | None = None,
+        sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         include_typing: bool = False,
     ) -> InstancesResult:
         """`Retrieve one or more instance by id(s). <https://docs.cognite.com/api/v1/#tag/Instances/operation/byExternalIdsInstances>`_
 
         Args:
             nodes (NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None): Node ids
             edges (EdgeId | Sequence[EdgeId] | tuple[str, str] | Sequence[tuple[str, str]] | None): Edge ids
-            sources (list[ViewId] | None): Retrieve properties from the listed - by reference - views.
+            sources (ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence(View) None): Retrieve properties from the listed - by reference - views.
             include_typing (bool): Whether to return property type information as part of the result.
 
         Returns:
             InstancesResult: Requested instances.
 
         Examples:
 
-            Delete instances by id:
+            Retrieve instances by id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
-                >>> res = c.data_modeling.instances.retrieve(('mySpace', 'myNode'))
+                >>> res = c.data_modeling.instances.retrieve(nodes=("mySpace", "myNodeExternalId"),
+                ...                                          edges=("mySpace", "myEdgeExternalId"),
+                ...                                          sources=("mySpace", "myViewExternalId", "myViewVersion")
+                ...                                         )
+
+            Retrieve nodes an edges using the built in data class
+
+                >>> from cognite.client import CogniteClient
+                >>> import cognite.client.data_modeling as dm
+                >>> c = CogniteClient()
+                >>> res = c.data_modeling.instances.retrieve(dm.NodeId("mySpace", "myNode"),
+                ...                                          dm.EdgeId("mySpace", "myEdge"),
+                ...                                          dm.ViewId("mySpace", "myViewExternalId", "myViewVersion")
+                ...                                         )
 
-            Delete nodes an edger using the built in data class
+            Retrieve nodes an edges using the the view object as source
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_modeling as dm
                 >>> c = CogniteClient()
-                >>> c.data_modeling.instances.retrieve(dm.NodeId("mySpace", "myNode"),
-                ...                                    dm.EdgeId("mySpace", "myEdge"))
+                >>> res = c.data_modeling.instances.retrieve(dm.NodeId("mySpace", "myNode"),
+                ...                                          dm.EdgeId("mySpace", "myEdge"),
+                ...                                          sources='myView')
+                ...                                         )
         """
         identifiers = self._load_node_and_edge_ids(nodes, edges)
         other_params = self._create_other_params(
             include_typing=include_typing,
             sources=sources,
             sort=None,
             instance_type=None,
@@ -325,15 +342,15 @@
 
     @classmethod
     def _create_other_params(
         cls,
         *,
         include_typing: bool,
         sort: list[InstanceSort | dict] | InstanceSort | dict | None,
-        sources: ViewId | Sequence[ViewId] | None,
+        sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None,
         instance_type: Literal["node", "edge"] | None,
     ) -> dict[str, Any]:
         other_params: dict[str, Any] = {"includeTyping": include_typing}
         if sources:
             other_params["sources"] = (
                 [cls._dump_instance_source(source) for source in sources]
                 if isinstance(sources, Sequence)
@@ -345,16 +362,21 @@
             else:
                 other_params["sort"] = [cls._dump_instance_sort(s) for s in sort]
         if instance_type:
             other_params["instanceType"] = instance_type
         return other_params
 
     @classmethod
-    def _dump_instance_source(cls, source: ViewId) -> dict:
-        return {"source": source.dump(camel_case=True)}
+    def _dump_instance_source(cls, source: ViewIdentifier | View) -> dict:
+        instance_source: ViewIdentifier
+        if isinstance(source, View):
+            instance_source = source.as_id()
+        else:
+            instance_source = source
+        return {"source": ViewId.load(instance_source).dump(camel_case=True)}
 
     @classmethod
     def _dump_instance_sort(cls, sort: InstanceSort | dict) -> dict:
         return sort.dump(camel_case=True) if isinstance(sort, InstanceSort) else sort
 
     def apply(
         self,
@@ -464,52 +486,52 @@
         )
 
     @overload
     def list(
         self,
         instance_type: Literal["node"] = "node",
         include_typing: bool = False,
-        sources: list[ViewId] | ViewId | None = None,
+        sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
         sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> NodeList:
         ...
 
     @overload
     def list(
         self,
         instance_type: Literal["edge"],
         include_typing: bool = False,
-        sources: list[ViewId] | ViewId | None = None,
+        sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
         sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> EdgeList:
         ...
 
     def list(
         self,
         instance_type: Literal["node", "edge"] = "node",
         include_typing: bool = False,
-        sources: list[ViewId] | ViewId | None = None,
+        sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
         sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> NodeList | EdgeList:
         """`List instances <https://docs.cognite.com/api/v1/#tag/Instances/operation/advancedListInstance>`_
 
         Args:
             instance_type(Literal["node", "edge"]): Whether to query for nodes or edges.
             include_typing (bool): Whether to return property type information as part of the result.
-            sources (list[ViewId] | ViewId): Views to retrieve properties from.
+            sources (ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence(View) | None): Views to retrieve properties from.
             limit (int, optional): Maximum number of instances to return. Default to 1000. Set to -1, float("inf") or None
                 to return all items.
             sort (list[InstanceSost] | InstanceSort | dict): How you want the listed instances information ordered.
-            filter (dict | Filter): Advnanced filtering of instances.
+            filter (dict | Filter): Advanced filtering of instances.
 
         Returns:
             Union[EdgeList, NodeList]: List of requested instances
 
         Examples:
 
             List instances and limit to 5:
```

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/data_sets.py` & `cognite_sdk-6.4.5/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.4.5/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/datapoints.py` & `cognite_sdk-6.4.5/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/diagrams.py` & `cognite_sdk-6.4.5/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.4.5/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/events.py` & `cognite_sdk-6.4.5/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.4.5/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/files.py` & `cognite_sdk-6.4.5/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/functions.py` & `cognite_sdk-6.4.5/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/geospatial.py` & `cognite_sdk-6.4.5/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/iam.py` & `cognite_sdk-6.4.5/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/labels.py` & `cognite_sdk-6.4.5/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/raw.py` & `cognite_sdk-6.4.5/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/relationships.py` & `cognite_sdk-6.4.5/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/sequences.py` & `cognite_sdk-6.4.5/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.4.5/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/templates.py` & `cognite_sdk-6.4.5/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/three_d.py` & `cognite_sdk-6.4.5/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/time_series.py` & `cognite_sdk-6.4.5/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.4.5/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.4.5/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.4.5/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.4.5/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.4.5/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api/vision.py` & `cognite_sdk-6.4.5/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_api_client.py` & `cognite_sdk-6.4.5/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_cognite_client.py` & `cognite_sdk-6.4.5/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_http_client.py` & `cognite_sdk-6.4.5/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.4.5/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/config.py` & `cognite_sdk-6.4.5/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/credentials.py` & `cognite_sdk-6.4.5/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/_base.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/assets.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if include_type:
             output["type"] = self._type
         return convert_all_keys_recursive(output, camel_case)
 
     @classmethod
     def load(
         cls: Type[T_Versioned_DataModeling_Id],
-        data: dict | T_Versioned_DataModeling_Id | tuple[str, str, str] | tuple[str, str],
+        data: dict | T_Versioned_DataModeling_Id | tuple[str, str] | tuple[str, str, str],
     ) -> T_Versioned_DataModeling_Id:
         if isinstance(data, cls):
             return data
         elif isinstance(data, tuple):
             return cls(*data)
         elif isinstance(data, dict):
             return cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
```

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,22 @@
             description=self.description,
             name=self.name,
             filter=self.filter,
             implements=self.implements,
             properties=properties,
         )
 
+    def as_id(self) -> ViewId:
+        """Convert to a view id.
+
+        Returns:
+            ViewId: The view id.
+        """
+        return ViewId(space=self.space, external_id=self.external_id, version=self.version)
+
 
 class ViewList(CogniteResourceList[View]):
     _RESOURCE = View
 
     def to_view_apply(self) -> ViewApplyList:
         """Convert to a view an apply list.
```

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/events.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/files.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/functions.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/iam.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/labels.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/raw.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/shared.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/templates.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/exceptions.py` & `cognite_sdk-6.4.5/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/testing.py` & `cognite_sdk-6.4.5/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/__init__.py` & `cognite_sdk-6.4.5/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.4.5/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.4.5/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_graph.py` & `cognite_sdk-6.4.5/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_identifier.py` & `cognite_sdk-6.4.5/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_logging.py` & `cognite_sdk-6.4.5/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.4.5/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.4.5/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.4.5/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_text.py` & `cognite_sdk-6.4.5/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_time.py` & `cognite_sdk-6.4.5/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_validation.py` & `cognite_sdk-6.4.5/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.4.5/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.4/pyproject.toml` & `cognite_sdk-6.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.4.4"
+version = "6.4.5"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.4.4/PKG-INFO` & `cognite_sdk-6.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.4.4
+Version: 6.4.5
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.4 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.5 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

