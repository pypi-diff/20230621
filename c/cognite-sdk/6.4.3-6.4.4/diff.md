# Comparing `tmp/cognite_sdk-6.4.3.tar.gz` & `tmp/cognite_sdk-6.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.4.3.tar", max compression
+gzip compressed data, was "cognite_sdk-6.4.4.tar", max compression
```

## Comparing `cognite_sdk-6.4.3.tar` & `cognite_sdk-6.4.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0    11349 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/README.md
--rw-r--r--   0        0        0      574 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     7867 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8393 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    24647 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6424 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7857 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11025 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17192 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41485 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45301 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49823 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-15 15:43:44.287009 cognite_sdk-6.4.3/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38099 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     3689 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    12373 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7267 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4019 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     5880 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    28798 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2543 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14642 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-15 15:43:44.291009 cognite_sdk-6.4.3/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6037 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7684 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-15 15:43:44.295009 cognite_sdk-6.4.3/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-15 15:43:44.299009 cognite_sdk-6.4.3/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/README.md
+-rw-r--r--   0        0        0      574 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     7857 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8393 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    24633 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6424 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7857 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11025 2023-06-21 11:06:44.805878 cognite_sdk-6.4.4/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17192 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41485 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45301 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49823 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38099 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-21 11:06:44.809878 cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     3629 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    12076 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7267 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4019 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     6238 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    28930 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2543 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14635 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6037 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-21 11:06:44.813879 cognite_sdk-6.4.4/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7684 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-21 11:06:44.817879 cognite_sdk-6.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.4/PKG-INFO
```

### Comparing `cognite_sdk-6.4.3/LICENSE` & `cognite_sdk-6.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/README.md` & `cognite_sdk-6.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/__init__.py` & `cognite_sdk-6.4.4/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/annotations.py` & `cognite_sdk-6.4.4/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/assets.py` & `cognite_sdk-6.4.4/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,11 +196,11 @@
         Examples:
 
             Create new containers:
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_classes.data_modeling as models
                 >>> c = CogniteClient()
-                >>> containers = [models.Container(space="mySpace",properties={"name": models.ContainerPropertyIdentifier(type=models.TextType, name="name")})]
+                >>> containers = [models.Container(space="mySpace",properties={"name": models.ContainerProperty(type=models.TextType, name="name")})]
                 >>> res = c.data_modeling.containers.create(containers)
         """
         return self._create_multiple(list_cls=ContainerList, resource_cls=Container, items=container)
```

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,28 +412,28 @@
                 ...                               dm.ViewId("mySpace", "ActorView", "v1"),
                 ...                               {"wonOscar": False,
                 ...                               # This is a one-to-one edge from actor to person
                 ...                                "person": {"space": "mySpace", "externalId": "person:arnold_schwarzenegger"}})
                 ... ])
                 >>> # This is one to many edge, in this case from Person to role
                 >>> # (a person can have multiple roles, in this model for example Actor and Director)
-                >>> person_to_actor = dm.EdgeApply.create(space="mySpace",
+                >>> person_to_actor = dm.EdgeApply(space="mySpace",
                 ...                                       external_id="relation:arnold_schwarzenegger:actor",
                 ...                                       type="Person.roles",
                 ...                                       start_node="person:arnold_schwarzenegger",
                 ...                                       end_node="actor:arnold_schwarzenegger",
                 ... )
                 >>> res = c.data_modeling.instances.apply([person, actor], [person_to_actor])
 
             Create new edge an automatically create end nodes.
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_modeling as dm
                 >>> c = CogniteClient()
-                >>> edge = dm.EdgeApply.create(space="mySpace",
+                >>> edge = dm.EdgeApply(space="mySpace",
                 ...                            external_id="relation:sylvester_stallone:actor",
                 ...                            type="Person.roles",
                 ...                            start_node="person:sylvester_stallone",
                 ...                            end_node="actor:sylvester_stallone",
                 ... )
                 >>> res = c.data_modeling.instances.apply(edges=edge, auto_create_start_nodes=True, auto_create_end_nodes=True)
```

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.4.4/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/data_sets.py` & `cognite_sdk-6.4.4/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.4.4/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/datapoints.py` & `cognite_sdk-6.4.4/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/diagrams.py` & `cognite_sdk-6.4.4/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.4.4/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/events.py` & `cognite_sdk-6.4.4/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.4.4/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/files.py` & `cognite_sdk-6.4.4/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/functions.py` & `cognite_sdk-6.4.4/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/geospatial.py` & `cognite_sdk-6.4.4/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/iam.py` & `cognite_sdk-6.4.4/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/labels.py` & `cognite_sdk-6.4.4/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/raw.py` & `cognite_sdk-6.4.4/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/relationships.py` & `cognite_sdk-6.4.4/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/sequences.py` & `cognite_sdk-6.4.4/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.4.4/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/templates.py` & `cognite_sdk-6.4.4/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/three_d.py` & `cognite_sdk-6.4.4/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/time_series.py` & `cognite_sdk-6.4.4/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.4.4/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.4.4/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.4.4/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.4.4/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.4.4/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api/vision.py` & `cognite_sdk-6.4.4/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_api_client.py` & `cognite_sdk-6.4.4/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_cognite_client.py` & `cognite_sdk-6.4.4/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_http_client.py` & `cognite_sdk-6.4.4/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.4/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.4.4/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.4.4/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.4.4/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/config.py` & `cognite_sdk-6.4.4/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/credentials.py` & `cognite_sdk-6.4.4/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/_base.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/assets.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from cognite.client.data_classes.data_modeling import filters
 from cognite.client.data_classes.data_modeling.containers import (
-    ConstraintIdentifier,
+    Constraint,
     Container,
     ContainerApply,
     ContainerApplyList,
     ContainerDirectRelation,
     ContainerFilter,
     ContainerList,
-    ContainerPropertyIdentifier,
-    IndexIdentifier,
+    ContainerProperty,
+    Index,
     RequiresConstraintDefinition,
     UniquenessConstraintDefinition,
 )
 from cognite.client.data_classes.data_modeling.data_models import (
     DataModel,
     DataModelApply,
     DataModelApplyList,
@@ -115,17 +115,17 @@
     "SpaceApplyList",
     "View",
     "ViewList",
     "Container",
     "ContainerList",
     "ContainerApply",
     "ContainerApplyList",
-    "IndexIdentifier",
-    "ConstraintIdentifier",
-    "ContainerPropertyIdentifier",
+    "Index",
+    "Constraint",
+    "ContainerProperty",
     "Primitive",
     "CDFExternalIdReference",
     "ContainerDirectRelation",
     "RequiresConstraintDefinition",
     "UniquenessConstraintDefinition",
     "ContainerId",
     "ViewId",
```

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/containers.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 
     Args:
         space (str): The workspace for the view, a unique identifier for the space.
         external_id (str): Combined with the space is the unique identifier of the view.
         description (str): Textual description of the view
         name (str): Human readable name for the view.
         used_for (Literal['node', 'edge', 'all']): Should this operation apply to nodes, edges or both.
-        properties (dict[str, ContainerPropertyIdentifier]): We index the property by a local unique identifier.
-        constraints (dict[str, ConstraintIdentifier]): Set of constraints to apply to the container
-        indexes (dict[str, IndexIdentifier]): Set of indexes to apply to the container.
+        properties (dict[str, ContainerProperty]): We index the property by a local unique identifier.
+        constraints (dict[str, Constraint]): Set of constraints to apply to the container
+        indexes (dict[str, Index]): Set of indexes to apply to the container.
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
-        properties: dict[str, ContainerPropertyIdentifier],
+        properties: dict[str, ContainerProperty],
         description: str = None,
         name: str = None,
         used_for: Literal["node", "edge", "all"] = None,
-        constraints: dict[str, ConstraintIdentifier] = None,
-        indexes: dict[str, IndexIdentifier] = None,
+        constraints: dict[str, Constraint] = None,
+        indexes: dict[str, Index] = None,
         **_: dict,
     ):
         validate_data_modeling_identifier(space, external_id)
         self.space = space
         self.external_id = external_id
         self.description = description
         self.name = name
@@ -56,60 +56,60 @@
         self.constraints = constraints
         self.indexes = indexes
 
     @classmethod
     def load(cls, resource: dict | str) -> ContainerCore:
         data = json.loads(resource) if isinstance(resource, str) else resource
         if "constraints" in data:
-            data["constraints"] = {k: ConstraintIdentifier.load(v) for k, v in data["constraints"].items()} or None
+            data["constraints"] = {k: Constraint.load(v) for k, v in data["constraints"].items()} or None
         if "indexes" in data:
-            data["indexes"] = {k: IndexIdentifier.load(v) for k, v in data["indexes"].items()} or None
+            data["indexes"] = {k: Index.load(v) for k, v in data["indexes"].items()} or None
         if "properties" in data:
-            data["properties"] = {k: ContainerPropertyIdentifier.load(v) for k, v in data["properties"].items()} or None
+            data["properties"] = {k: ContainerProperty.load(v) for k, v in data["properties"].items()} or None
         return cast(ContainerCore, super().load(data))
 
     def dump(self, camel_case: bool = False) -> dict[str, Any]:
         output = super().dump(camel_case)
         if self.constraints:
             output["constraints"] = {k: v.dump(camel_case) for k, v in self.constraints.items()}
         if self.indexes:
             output["indexes"] = {k: v.dump(camel_case) for k, v in self.indexes.items()}
         if self.properties:
             output["properties"] = {k: v.dump(camel_case) for k, v in self.properties.items()}
 
         return output
 
-    def as_reference(self) -> ContainerId:
+    def as_id(self) -> ContainerId:
         return ContainerId(self.space, self.external_id)
 
 
 class ContainerApply(ContainerCore):
     """Represent the physical storage of data. This is the write format of the container
 
     Args:
         space (str): The workspace for the view, a unique identifier for the space.
         external_id (str): Combined with the space is the unique identifier of the view.
         description (str): Textual description of the view
         name (str): Human readable name for the view.
         used_for (Literal['node', 'edge', 'all']): Should this operation apply to nodes, edges or both.
-        properties (dict[str, ContainerPropertyIdentifier]): We index the property by a local unique identifier.
-        constraints (dict[str, ConstraintIdentifier]): Set of constraints to apply to the container
-        indexes (dict[str, IndexIdentifier]): Set of indexes to apply to the container.
+        properties (dict[str, ContainerProperty]): We index the property by a local unique identifier.
+        constraints (dict[str, Constraint]): Set of constraints to apply to the container
+        indexes (dict[str, Index]): Set of indexes to apply to the container.
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
-        properties: dict[str, ContainerPropertyIdentifier],
+        properties: dict[str, ContainerProperty],
         description: str = None,
         name: str = None,
         used_for: Literal["node", "edge", "all"] = None,
-        constraints: dict[str, ConstraintIdentifier] = None,
-        indexes: dict[str, IndexIdentifier] = None,
+        constraints: dict[str, Constraint] = None,
+        indexes: dict[str, Index] = None,
         **_: dict,
     ):
         super().__init__(space, external_id, properties, description, name, used_for, constraints, indexes)
 
 
 class Container(ContainerCore):
     """Represent the physical storage of data. This is the read format of the container
@@ -117,34 +117,34 @@
     Args:
         space (str): The workspace for the view, a unique identifier for the space.
         external_id (str): Combined with the space is the unique identifier of the view.
         description (str): Textual description of the view
         name (str): Human readable name for the view.
         is_global (bool): Whether this is a global container, i.e., one of the out-of-the-box models.
         used_for (Literal['node', 'edge', 'all']): Should this operation apply to nodes, edges or both.
-        properties (dict[str, ContainerPropertyIdentifier]): We index the property by a local unique identifier.
-        constraints (dict[str, ConstraintIdentifier]): Set of constraints to apply to the container
-        indexes (dict[str, IndexIdentifier]): Set of indexes to apply to the container.
+        properties (dict[str, ContainerProperty]): We index the property by a local unique identifier.
+        constraints (dict[str, Constraint]): Set of constraints to apply to the container
+        indexes (dict[str, Index]): Set of indexes to apply to the container.
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
-        properties: dict[str, ContainerPropertyIdentifier],
+        properties: dict[str, ContainerProperty],
         is_global: bool,
         last_updated_time: int,
         created_time: int,
         description: str = None,
         name: str = None,
         used_for: Literal["node", "edge", "all"] = "node",
-        constraints: dict[str, ConstraintIdentifier] = None,
-        indexes: dict[str, IndexIdentifier] = None,
+        constraints: dict[str, Constraint] = None,
+        indexes: dict[str, Index] = None,
     ):
         super().__init__(space, external_id, properties, description, name, used_for, constraints, indexes)
         self.is_global = is_global
         self.last_updated_time = last_updated_time
         self.created_time = created_time
 
     def as_apply(self) -> ContainerApply:
@@ -204,24 +204,24 @@
         output = cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
         if isinstance(data.get("container"), dict):
             output.container = ContainerId.load(data["container"])
         return output
 
 
 @dataclass
-class ContainerPropertyIdentifier:
+class ContainerProperty:
     type: PropertyType | ContainerDirectRelation
     nullable: bool = True
     auto_increment: bool = False
     name: Optional[str] = None
     default_value: str | int | dict | None = None
     description: str | None = None
 
     @classmethod
-    def load(cls, data: dict[str, Any]) -> ContainerPropertyIdentifier:
+    def load(cls, data: dict[str, Any]) -> ContainerProperty:
         if "type" not in data:
             raise ValueError("Type not specified")
         if data["type"].get("type") == "direct":
             data["type"] = ContainerDirectRelation.load(data["type"])
         else:
             data["type"] = PropertyType.load(data["type"])
         return cls(**convert_all_keys_to_snake_case(data))
@@ -230,17 +230,17 @@
         output = asdict(self)
         if "type" in output and isinstance(output["type"], dict):
             output["type"] = self.type.dump(camel_case)
         return convert_all_keys_to_camel_case_recursive(output) if camel_case else output
 
 
 @dataclass
-class ConstraintIdentifier(ABC):
+class Constraint(ABC):
     @classmethod
-    def _load(cls, data: dict) -> ConstraintIdentifier:
+    def _load(cls, data: dict) -> Constraint:
         return cls(**convert_all_keys_to_snake_case(data))
 
     @classmethod
     def load(cls, data: dict) -> RequiresConstraintDefinition | UniquenessConstraintDefinition:
         if data["constraintType"] == "requires":
             return RequiresConstraintDefinition.load(data)
         elif data["constraintType"] == "uniqueness":
@@ -249,15 +249,15 @@
 
     def dump(self, camel_case: bool = False) -> dict[str, str | dict]:
         output = asdict(self)
         return convert_all_keys_to_camel_case_recursive(output) if camel_case else output
 
 
 @dataclass
-class RequiresConstraintDefinition(ConstraintIdentifier):
+class RequiresConstraintDefinition(Constraint):
     require: ContainerId
 
     @classmethod
     def load(cls, data: dict) -> RequiresConstraintDefinition:
         output = cast(
             RequiresConstraintDefinition, super()._load(rename_and_exclude_keys(data, exclude={"constraintType"}))
         )
@@ -271,15 +271,15 @@
             output["require"] = self.require.dump(camel_case)
         key = "constraintType" if camel_case else "constraint_type"
         output[key] = "requires"
         return output
 
 
 @dataclass
-class UniquenessConstraintDefinition(ConstraintIdentifier):
+class UniquenessConstraintDefinition(Constraint):
     properties: list[str]
 
     @classmethod
     def load(cls, data: dict) -> UniquenessConstraintDefinition:
         return cast(
             UniquenessConstraintDefinition, super()._load(rename_and_exclude_keys(data, exclude={"constraintType"}))
         )
@@ -288,18 +288,18 @@
         output = super().dump()
         key = "constraintType" if camel_case else "constraint_type"
         output[key] = "uniqueness"
         return output
 
 
 @dataclass
-class IndexIdentifier:
+class Index:
     properties: list[str]
     index_type: Literal["btree"] | str = "btree"
 
     @classmethod
-    def load(cls, data: dict[str, Any]) -> IndexIdentifier:
+    def load(cls, data: dict[str, Any]) -> Index:
         return cls(**convert_all_keys_to_snake_case(data))
 
     def dump(self, camel_case: bool = False) -> dict[str, str | dict]:
         output = asdict(self)
         return convert_all_keys_to_camel_case_recursive(output) if camel_case else output
```

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/ids.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import ClassVar, Literal, Optional, Sequence, Tuple, Type, TypeVar, Union, cast
 
 from cognite.client.utils._auxiliary import rename_and_exclude_keys
 from cognite.client.utils._identifier import DataModelingIdentifier, DataModelingIdentifierSequence
 from cognite.client.utils._text import convert_all_keys_recursive, convert_all_keys_to_snake_case
 
 
-@dataclass
+@dataclass(frozen=True)
 class DataModelingId:
     _type: ClassVar[str] = field(init=False)
     space: str
     external_id: str
 
     def as_tuple(self) -> tuple[str, str]:
         return self.space, self.external_id
@@ -33,15 +33,15 @@
             return cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
         raise ValueError(f"Cannot load {data} into {cls}, invalid type={type(data)}")
 
 
 T_DataModelingId = TypeVar("T_DataModelingId", bound=DataModelingId)
 
 
-@dataclass
+@dataclass(frozen=True)
 class VersionedDataModelingId:
     _type: ClassVar[str] = field(init=False)
     space: str
     external_id: str
     version: Optional[str] = None
 
     def as_tuple(self) -> tuple[str, str, Optional[str]]:
@@ -51,15 +51,16 @@
         output = asdict(self)
         if include_type:
             output["type"] = self._type
         return convert_all_keys_recursive(output, camel_case)
 
     @classmethod
     def load(
-        cls: Type[T_Versioned_DataModeling_Id], data: dict | T_Versioned_DataModeling_Id | tuple[str, str, str]
+        cls: Type[T_Versioned_DataModeling_Id],
+        data: dict | T_Versioned_DataModeling_Id | tuple[str, str, str] | tuple[str, str],
     ) -> T_Versioned_DataModeling_Id:
         if isinstance(data, cls):
             return data
         elif isinstance(data, tuple):
             return cls(*data)
         elif isinstance(data, dict):
             return cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
@@ -101,31 +102,37 @@
 
 
 @dataclass
 class EdgeId(InstanceId):
     _instance_type = "edge"  # type: ignore[assignment]
 
 
-@dataclass
+@dataclass(frozen=True)
 class ContainerId(DataModelingId):
     _type = "container"
 
     def as_source_identifier(self) -> str:
         return self.external_id
 
+    def as_property_ref(self, property: str) -> tuple[str, ...]:
+        return (self.space, self.as_source_identifier(), property)
 
-@dataclass
+
+@dataclass(frozen=True)
 class ViewId(VersionedDataModelingId):
     _type = "view"
 
     def as_source_identifier(self) -> str:
         return f"{self.external_id}/{self.version}"
 
+    def as_property_ref(self, property: str) -> tuple[str, ...]:
+        return (self.space, self.as_source_identifier(), property)
 
-@dataclass
+
+@dataclass(frozen=True)
 class DataModelId(VersionedDataModelingId):
     _type = "datamodel"
 
 
 ContainerIdentifier = Union[ContainerId, Tuple[str, str]]
 ViewIdentifier = Union[ViewId, Tuple[str, str], Tuple[str, str, str]]
 DataModelIdentifier = Union[DataModelId, Tuple[str, str], Tuple[str, str, str]]
```

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/instances.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,68 @@
 from __future__ import annotations
 
 import json
+from abc import abstractmethod
+from collections import defaultdict
 from dataclasses import asdict, dataclass
-from typing import Any, List, Literal, Type, TypeVar, Union, cast
+from typing import (
+    Any,
+    Dict,
+    ItemsView,
+    Iterator,
+    KeysView,
+    List,
+    Literal,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    ValuesView,
+    cast,
+    overload,
+)
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteResourceList,
 )
 from cognite.client.data_classes.data_modeling._core import DataModelingResource
 from cognite.client.data_classes.data_modeling._validation import validate_data_modeling_identifier
 from cognite.client.data_classes.data_modeling.data_types import (
     DirectRelationReference,
 )
-from cognite.client.data_classes.data_modeling.ids import ContainerId, EdgeId, NodeId, ViewId
+from cognite.client.data_classes.data_modeling.ids import (
+    ContainerId,
+    ContainerIdentifier,
+    EdgeId,
+    NodeId,
+    ViewId,
+    ViewIdentifier,
+)
 from cognite.client.utils._text import convert_all_keys_to_camel_case_recursive, convert_all_keys_to_snake_case
 
 PropertyValue = Union[str, int, float, bool, dict, List[str], List[int], List[float], List[bool], List[dict]]
 Space = str
 PropertyIdentifier = str
 
 
 @dataclass
 class NodeOrEdgeData:
     """This represents the data values of a node or edge.
 
     Args:
         source (ContainerId | ViewId): The container or view the node or edge property is in
-        properties (dict[str, PropertyValue]): The properties of the node or edge.
+        properties (Mapping[str, PropertyValue]): The properties of the node or edge.
     """
 
     source: ContainerId | ViewId
-    properties: dict[str, PropertyValue]
+    properties: Mapping[str, PropertyValue]
 
     @classmethod
     def load(cls, data: dict) -> NodeOrEdgeData:
         return cls(**convert_all_keys_to_snake_case(data))
 
     def dump(self, camel_case: bool = False) -> dict:
         output = asdict(self)
@@ -105,81 +132,145 @@
         if "sources" in data:
             instance.sources = [NodeOrEdgeData.load(source) for source in data["sources"]]
         return instance
 
 
 T_Instance_Apply = TypeVar("T_Instance_Apply", bound=InstanceApply)
 
+_T = TypeVar("_T")
+
+
+class Properties(MutableMapping[ViewIdentifier, MutableMapping[PropertyIdentifier, PropertyValue]]):
+    def __init__(self, properties: MutableMapping[ViewId, MutableMapping[PropertyIdentifier, PropertyValue]]):
+        self.data = properties
+
+    @classmethod
+    def load(
+        cls, data: MutableMapping[Space, MutableMapping[str, MutableMapping[PropertyIdentifier, PropertyValue]]]
+    ) -> Properties:
+        props: MutableMapping[ViewId, MutableMapping[PropertyIdentifier, PropertyValue]] = {}
+        for space, view_properties in data.items():
+            for view_id_str, properties in view_properties.items():
+                view_tuple = tuple(view_id_str.split("/", 1))
+                if len(view_tuple) != 2:
+                    raise ValueError("View id must be in the format <external_id>/<version>")
+                view_id = ViewId.load(cast(Tuple[str, str, str], (space, *view_tuple)))
+                props[view_id] = properties
+        return Properties(props)
+
+    def dump(self) -> dict[Space, dict[str, dict[PropertyIdentifier, PropertyValue]]]:
+        props: dict[Space, dict[str, dict[PropertyIdentifier, PropertyValue]]] = defaultdict(dict)
+        for view_id, properties in self.data.items():
+            view_id_str = f"{view_id.external_id}/{view_id.version}"
+            props[view_id.space][view_id_str] = cast(Dict[PropertyIdentifier, PropertyValue], properties)
+        return props
+
+    def items(self) -> ItemsView[ViewId, MutableMapping[PropertyIdentifier, PropertyValue]]:
+        return self.data.items()
+
+    def keys(self) -> KeysView[ViewId]:
+        return self.data.keys()
+
+    def values(self) -> ValuesView[MutableMapping[PropertyIdentifier, PropertyValue]]:
+        return self.data.values()
+
+    def __iter__(self) -> Iterator[ViewId]:
+        yield from self.keys()
+
+    def __getitem__(self, view: ViewIdentifier) -> MutableMapping[PropertyIdentifier, PropertyValue]:
+        view_id = ViewId.load(view)
+        return self.data.get(view_id, {})
+
+    def __contains__(self, item: Any) -> bool:
+        view_id = ViewId.load(item)
+        return view_id in self.data
+
+    @overload
+    def get(self, view: ViewIdentifier) -> Optional[MutableMapping[PropertyIdentifier, PropertyValue]]:
+        ...
+
+    @overload
+    def get(
+        self, view: ViewIdentifier, default: MutableMapping[PropertyIdentifier, PropertyValue] | _T
+    ) -> MutableMapping[PropertyIdentifier, PropertyValue] | _T:
+        ...
+
+    def get(
+        self, view: ViewIdentifier, default: Optional[MutableMapping[PropertyIdentifier, PropertyValue]] | _T = None
+    ) -> Optional[MutableMapping[PropertyIdentifier, PropertyValue]] | _T:
+        view_id = ViewId.load(view)
+        return self.data.get(view_id, default)
+
+    def __len__(self) -> int:
+        return len(self.data)
+
+    def __delitem__(self, view: ViewIdentifier) -> None:
+        view_id = ViewId.load(view)
+        del self.data[view_id]
+
+    def __setitem__(self, view: ViewIdentifier, properties: MutableMapping[PropertyIdentifier, PropertyValue]) -> None:
+        view_id = ViewId.load(view)
+        self.data[view_id] = properties
+
+
+T_Instance = TypeVar("T_Instance", bound="Instance")
+
 
 class Instance(InstanceCore):
     """A node or edge. This is the read version of the instance.
 
     Args:
         space (str): The workspace for the instance.a unique identifier for the space.
         external_id (str): Combined with the space is the unique identifier of the instance.
         version (str): DMS version.
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         deleted_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
                             Timestamp when the instance was soft deleted. Note that deleted instances are filtered out of query results, but present in sync results
         instance_type (Literal["node", "edge"]) The type of instance.
-        properties (dict[Space, dict[PropertyIdentifier, dict[str, PropertyValue]]]): Properties of the instance.
+        properties (Properties): Properties of the instance.
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         version: str,
         last_updated_time: int,
         created_time: int,
         instance_type: Literal["node", "edge"] = "node",
         deleted_time: int = None,
-        properties: dict[Space, dict[PropertyIdentifier, dict[str, PropertyValue]]] = None,
+        properties: Properties = None,
         **_: dict,
     ):
         super().__init__(space, external_id, instance_type)
         self.version = version
         self.last_updated_time = last_updated_time
         self.created_time = created_time
         self.deleted_time = deleted_time
-        self.properties = properties
-
-    def as_apply(self, source: ViewId | ContainerId, existing_version: int) -> InstanceApply:
-        """
-        This is a convenience function for converting the instance to an apply instance.
-
-        It makes the simplifying assumption that all properties are from the same view. Note that this
-        is not true in general.
+        self.properties: Properties = properties or Properties({})
 
-        Args:
-            source (ViewId | ContainerId): The view or container to with all the properties.
-            existing_version (int): Fail the ingestion request if the node's version is greater than or equal to this value.
-                                    If no existingVersion is specified, the ingestion will always overwrite any
-                                    existing data for the edge (for the specified container or instance). If existingVersion is
-                                    set to 0, the upsert will behave as an insert, so it will fail the bulk if the
-                                    item already exists. If skipOnVersionConflict is set on the ingestion request,
-                                    then the item will be skipped instead of failing the ingestion request.
-
-        Returns:
-            An InstanceApply.
-
-        """
-        return InstanceApply(
-            space=self.space,
-            external_id=self.external_id,
-            instance_type=self.instance_type,
-            existing_version=existing_version,
-            sources=[
-                NodeOrEdgeData(source=source, properties=space_properties)  # type: ignore[arg-type]
-                for space_properties in self.properties.values()
-            ]
-            if self.properties
-            else None,
-        )
+    @classmethod
+    def load(cls: Type[T_Instance], data: dict | str) -> T_Instance:
+        data = json.loads(data) if isinstance(data, str) else data
+        if "properties" in data:
+            data["properties"] = Properties.load(data["properties"])
+        res = super().load(data)
+        return res
+
+    def dump(self, camel_case: bool = False) -> Dict[str, Any]:
+        dumped = super().dump(camel_case)
+        if "properties" in dumped:
+            dumped["properties"] = self.properties.dump()
+        return dumped
+
+    @abstractmethod
+    def as_apply(self, source: ViewIdentifier | ContainerIdentifier, existing_version: int) -> InstanceApply:
+        """Convert the instance to an apply instance."""
+        raise NotImplementedError()
 
 
 class InstanceApplyResult(InstanceCore):
     """A node or edge. This represents the update on the instance.
 
     Args:
         instance_type (Literal["node", "edge"]) The type of instance.
@@ -256,28 +347,28 @@
         self,
         space: str,
         external_id: str,
         version: str,
         last_updated_time: int,
         created_time: int,
         deleted_time: int = None,
-        properties: dict[Space, dict[PropertyIdentifier, dict[str, PropertyValue]]] = None,
+        properties: Properties = None,
         **_: dict,
     ):
         super().__init__(space, external_id, version, last_updated_time, created_time, "node", deleted_time, properties)
 
-    def as_apply(self, source: ViewId | ContainerId, existing_version: int) -> NodeApply:
+    def as_apply(self, source: ViewIdentifier | ContainerIdentifier, existing_version: int) -> NodeApply:
         """
         This is a convenience function for converting the read to a write node.
 
         It makes the simplifying assumption that all properties are from the same view. Note that this
         is not true in general.
 
         Args:
-            source (ViewId | ContainerId): The view or container to with all the properties.
+            source (ViewIdentifier | ContainerIdentifier): The view or container to with all the properties.
             existing_version (int): Fail the ingestion request if the node's version is greater than or equal to this value.
                                     If no existingVersion is specified, the ingestion will always overwrite any
                                     existing data for the edge (for the specified container or instance). If existingVersion is
                                     set to 0, the upsert will behave as an insert, so it will fail the bulk if the
                                     item already exists. If skipOnVersionConflict is set on the ingestion request,
                                     then the item will be skipped instead of failing the ingestion request.
 
@@ -286,16 +377,15 @@
 
         """
         return NodeApply(
             space=self.space,
             external_id=self.external_id,
             existing_version=existing_version,
             sources=[
-                NodeOrEdgeData(source=source, properties=space_properties[source.as_source_identifier()])  # type: ignore[arg-type]
-                for space_properties in self.properties.values()
+                NodeOrEdgeData(source=view_id, properties=properties) for view_id, properties in self.properties.items()
             ]
             if self.properties
             else None,
         )
 
     def as_id(self) -> NodeId:
         return NodeId(space=self.space, external_id=self.external_id)
@@ -394,58 +484,14 @@
         instance = cast(EdgeApply, super().load(data))
 
         instance.type = DirectRelationReference.load(data["type"])
         instance.start_node = DirectRelationReference.load(data["startNode"])
         instance.end_node = DirectRelationReference.load(data["endNode"])
         return instance
 
-    @classmethod
-    def create(
-        cls,
-        space: str,
-        external_id: str,
-        type: str,
-        start_node: str,
-        end_node: str,
-        existing_version: int = None,
-        sources: list[NodeOrEdgeData] = None,
-    ) -> EdgeApply:
-        """
-        This is a convenience factory method for creating an edge for writing. It assumes that the edge and its
-        nodes are from the same space.
-
-
-        Args:
-            space (str): The workspace for the edge, a unique identifier for the space. This is also used for the start, end, and type.
-            external_id (str): Combined with the space is the unique identifier of the edge.
-            type (str): The external id of the type, typically on the format 'TypeName.typeField'. For example, Person.roles.
-            start_node (str): The external id of the start node. Space is assumed to be equal to the edge.
-            end_node (str): The external id of the end node. Space is assumed to be equal to the edge.
-            existing_version (int): Fail the ingestion request if the node's version is greater than or equal to this value.
-                                    If no existingVersion is specified, the ingestion will always overwrite any
-                                    existing data for the edge (for the specified container or edge). If existingVersion is
-                                    set to 0, the upsert will behave as an insert, so it will fail the bulk if the
-                                    item already exists. If skipOnVersionConflict is set on the ingestion request,
-                                    then the item will be skipped instead of failing the ingestion request.
-            sources (list[NodeOrEdgeData]): List of source properties to write. The properties are from the edge and/or
-                            container the container(s) making up this node.
-
-        Returns:
-            An ApplyEdge
-        """
-        return cls(
-            space,
-            external_id,
-            DirectRelationReference(space, type),
-            DirectRelationReference(space, start_node),
-            DirectRelationReference(space, end_node),
-            existing_version,
-            sources,
-        )
-
 
 class Edge(Instance):
     """An Edge.  This is the read version of the edge.
 
     Args:
         space (str): The workspace for the edge an unique identifier for the space.
         external_id (str): Combined with the space is the unique identifier of the edge.
@@ -466,52 +512,50 @@
         version: str,
         type: DirectRelationReference,
         last_updated_time: int,
         created_time: int,
         start_node: DirectRelationReference,
         end_node: DirectRelationReference,
         deleted_time: int = None,
-        properties: dict[str, dict] = None,
+        properties: Properties = None,
         **_: dict,
     ):
         super().__init__(space, external_id, version, last_updated_time, created_time, "edge", deleted_time, properties)
         self.type = type
         self.start_node = start_node
         self.end_node = end_node
 
-    def as_apply(self, source: ViewId | ContainerId, existing_version: int = None) -> EdgeApply:
+    def as_apply(self, source: ViewIdentifier | ContainerIdentifier, existing_version: int = None) -> EdgeApply:
         """
         This is a convenience function for converting the read to a write edge.
 
         It makes the simplifying assumption that all properties are from the same view. Note that this
         is not true in general.
 
         Args:
-            source (ViewId | ContainerId): The view or container to with all the properties.
+            source (ViewIdentifier | ContainerIdentifier): The view or container to with all the properties.
             existing_version (int): Fail the ingestion request if the node's version is greater than or equal to this value.
                                     If no existingVersion is specified, the ingestion will always overwrite any
                                     existing data for the edge (for the specified container or instance). If existingVersion is
                                     set to 0, the upsert will behave as an insert, so it will fail the bulk if the
                                     item already exists. If skipOnVersionConflict is set on the ingestion request,
                                     then the item will be skipped instead of failing the ingestion request.
 
         Returns:
             A write edge, EdgeApply
-
         """
         return EdgeApply(
             space=self.space,
             external_id=self.external_id,
             type=self.type,
             start_node=self.start_node,
             end_node=self.end_node,
             existing_version=existing_version or None,
             sources=[
-                NodeOrEdgeData(source=source, properties=space_properties[source.as_source_identifier()])  # type: ignore[arg-type]
-                for space_properties in self.properties.values()  # type: ignore[union-attr]
+                NodeOrEdgeData(source=view_id, properties=properties) for view_id, properties in self.properties.items()
             ]
             or None,
         )
 
     def as_id(self) -> EdgeId:
         return EdgeId(space=self.space, external_id=self.external_id)
 
@@ -599,15 +643,15 @@
     def as_ids(self) -> list[EdgeId]:
         return [edge.as_id() for edge in self]
 
 
 class InstanceSort(CogniteFilter):
     def __init__(
         self,
-        property: list[str],
+        property: list[str] | tuple[str, ...],
         direction: Literal["ascending", "descending"] = "ascending",
         nulls_first: bool = False,
     ):
         self.property = property
         self.direction = direction
         self.nulls_first = nulls_first
```

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_modeling/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         if self.implements:
             output["implements"] = [v.dump(camel_case) for v in self.implements]
         if self.filter:
             output["filter"] = self.filter.dump()
 
         return output
 
-    def as_reference(self) -> ViewId:
+    def as_id(self) -> ViewId:
         return ViewId(
             space=self.space,
             external_id=self.external_id,
             version=self.version,
         )
```

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/events.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/files.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/functions.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/iam.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/labels.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/raw.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/shared.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/templates.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.4.4/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/exceptions.py` & `cognite_sdk-6.4.4/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/testing.py` & `cognite_sdk-6.4.4/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/__init__.py` & `cognite_sdk-6.4.4/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.4.4/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.4.4/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_graph.py` & `cognite_sdk-6.4.4/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_identifier.py` & `cognite_sdk-6.4.4/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_logging.py` & `cognite_sdk-6.4.4/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.4.4/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.4.4/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.4.4/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_text.py` & `cognite_sdk-6.4.4/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_time.py` & `cognite_sdk-6.4.4/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_validation.py` & `cognite_sdk-6.4.4/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.4.4/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.3/pyproject.toml` & `cognite_sdk-6.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.4.3"
+version = "6.4.4"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.4.3/PKG-INFO` & `cognite_sdk-6.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.4.3
+Version: 6.4.4
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.3 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.4 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

