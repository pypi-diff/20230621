# Comparing `tmp/kaskada-0.4.0.tar.gz` & `tmp/kaskada-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.4.0.tar", max compression
+gzip compressed data, was "kaskada-0.4.1.tar", max compression
```

## Comparing `kaskada-0.4.0.tar` & `kaskada-0.4.1.tar`

### file list

```diff
@@ -1,73 +1,75 @@
--rw-r--r--   0        0        0     1646 2023-05-31 11:54:25.771904 kaskada-0.4.0/README.md
--rw-r--r--   0        0        0     3917 2023-05-31 11:54:25.771904 kaskada-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7656 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/fenlmagic/utils.py
--rw-r--r--   0        0        0       33 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/__init__.py
--rw-r--r--   0        0        0      569 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0        0 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/local_session/__init__.py
--rw-r--r--   0        0        0     3573 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/local_session/local_service.py
--rw-r--r--   0        0        0     3312 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/local_session/local_session_keep_alive.py
--rw-r--r--   0        0        0     6381 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/release.py
--rw-r--r--   0        0        0     1108 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/remote_session/__init__.py
--rw-r--r--   0        0        0    11294 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/session.py
--rw-r--r--   0        0        0    11972 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7337 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0    10325 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0        0 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/health_check_client.py
--rw-r--r--   0        0        0     4522 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/health_check_servicer.py
--rw-r--r--   0        0        0     2326 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/health_check_watcher.py
--rw-r--r--   0        0        0     7626 2023-05-31 11:54:26.287927 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.291927 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    12572 2023-05-31 11:54:26.319928 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0    12538 2023-05-31 11:54:26.315928 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     4489 2023-05-31 11:54:26.351930 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-05-31 11:54:26.367930 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     4191 2023-05-31 11:54:26.375931 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.411932 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     2718 2023-05-31 11:54:26.411932 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.447934 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     3976 2023-05-31 11:54:26.447934 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-05-31 11:54:26.471935 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0    10837 2023-05-31 11:54:26.471935 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-05-31 11:54:26.495936 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-05-31 11:54:26.503936 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.527938 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    13180 2023-05-31 11:54:26.531938 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.555939 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     3398 2023-05-31 11:54:26.559939 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-05-31 11:54:26.579940 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     2805 2023-05-31 11:54:26.587940 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.607941 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    11773 2023-05-31 11:54:26.619942 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-05-31 11:54:26.631942 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4018 2023-05-31 11:54:26.831951 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.667944 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-31 11:54:26.703945 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.731947 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2729 2023-05-31 11:54:26.767948 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.791949 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    11249 2023-05-31 11:54:26.819950 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-05-31 11:54:26.843952 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     5157 2023-05-31 11:54:26.855952 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-05-31 11:54:26.871953 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0     8140 2023-05-31 11:54:26.875953 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-05-31 11:54:26.891954 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    16491 2023-05-31 11:54:26.907954 kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-05-31 11:54:26.923955 kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8622 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9272 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10126 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/table.py
--rw-r--r--   0        0        0     7131 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/utils.py
--rw-r--r--   0        0        0     4543 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 kaskada-0.4.0/setup.py
--rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 kaskada-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-05-01 19:22:44.891724 kaskada-0.4.1/README.md
+-rw-r--r--   0        0        0     3917 2023-06-20 17:23:20.820629 kaskada-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7656 2023-06-06 17:35:42.987556 kaskada-0.4.1/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-05 20:07:05.230947 kaskada-0.4.1/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-05-01 19:22:44.892917 kaskada-0.4.1/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 15:20:54.673916 kaskada-0.4.1/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-23 16:27:30.619980 kaskada-0.4.1/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:27:30.620032 kaskada-0.4.1/src/kaskada/api/local_session/__init__.py
+-rw-r--r--   0        0        0     3573 2023-05-23 16:27:30.620441 kaskada-0.4.1/src/kaskada/api/local_session/local_service.py
+-rw-r--r--   0        0        0     3312 2023-05-24 15:28:38.424727 kaskada-0.4.1/src/kaskada/api/local_session/local_session_keep_alive.py
+-rw-r--r--   0        0        0     6381 2023-04-05 20:07:05.231172 kaskada-0.4.1/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     1108 2023-06-06 17:35:42.987905 kaskada-0.4.1/src/kaskada/api/remote_session/__init__.py
+-rw-r--r--   0        0        0    11294 2023-06-15 16:50:30.249227 kaskada-0.4.1/src/kaskada/api/session.py
+-rw-r--r--   0        0        0    11972 2023-06-06 17:35:42.988531 kaskada-0.4.1/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-04-05 20:07:05.231408 kaskada-0.4.1/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-04-05 20:07:05.231471 kaskada-0.4.1/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-04-05 20:07:05.231594 kaskada-0.4.1/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7337 2023-05-01 19:22:49.940266 kaskada-0.4.1/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0    10325 2023-05-30 23:13:08.825837 kaskada-0.4.1/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:27:30.621359 kaskada-0.4.1/src/kaskada/health/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-23 16:27:30.621683 kaskada-0.4.1/src/kaskada/health/health_check_client.py
+-rw-r--r--   0        0        0     4522 2023-05-23 16:27:30.621896 kaskada-0.4.1/src/kaskada/health/health_check_servicer.py
+-rw-r--r--   0        0        0     2326 2023-05-23 16:27:30.622083 kaskada-0.4.1/src/kaskada/health/health_check_watcher.py
+-rw-r--r--   0        0        0     7626 2023-06-16 14:06:27.521454 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.526292 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    13155 2023-06-16 14:06:27.520709 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0    12538 2023-06-16 14:06:27.530338 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4489 2023-06-16 14:06:27.527963 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-06-16 14:06:27.529640 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4191 2023-06-16 14:06:27.522431 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.526364 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     2718 2023-06-16 14:06:27.530593 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.531560 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     3976 2023-06-16 14:06:27.532320 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-06-16 14:06:27.533962 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1710 2023-05-15 22:34:43.474188 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/health_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-15 22:34:43.474353 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/health_pb2_grpc.py
+-rw-r--r--   0        0        0    10837 2023-06-16 14:06:27.534314 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-06-16 14:06:27.536488 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-06-16 14:06:27.536464 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.538548 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    13180 2023-06-16 14:06:27.541085 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.540976 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     3398 2023-06-16 14:06:27.541884 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-06-16 14:06:27.542461 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2805 2023-06-16 14:06:27.543469 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.543684 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    11773 2023-06-16 14:06:27.544769 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-06-16 14:06:27.545476 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4018 2023-06-16 14:06:27.545999 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.544085 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-06-16 14:06:27.546778 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.547035 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2729 2023-06-16 14:06:27.548973 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.549601 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    11249 2023-06-16 14:06:27.552866 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-06-16 14:06:27.553614 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5157 2023-06-16 14:06:27.554368 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 14:06:27.554353 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0     8140 2023-06-16 14:06:27.555880 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-06-16 14:06:27.556002 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16491 2023-06-16 14:06:27.555867 kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-06-16 14:06:27.556311 kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8622 2023-05-01 19:22:49.940570 kaskada-0.4.1/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9272 2023-05-01 19:22:49.940719 kaskada-0.4.1/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-04-05 20:07:05.232035 kaskada-0.4.1/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10286 2023-06-06 17:35:42.988703 kaskada-0.4.1/src/kaskada/table.py
+-rw-r--r--   0        0        0     7131 2023-05-08 21:01:05.018302 kaskada-0.4.1/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4543 2023-05-01 19:22:49.941272 kaskada-0.4.1/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-04-05 20:07:05.233220 kaskada-0.4.1/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-04-05 20:07:05.233314 kaskada-0.4.1/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-04-05 20:07:05.233416 kaskada-0.4.1/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-05 20:07:05.233487 kaskada-0.4.1/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 kaskada-0.4.1/setup.py
+-rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 kaskada-0.4.1/PKG-INFO
```

### Comparing `kaskada-0.4.0/README.md` & `kaskada-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/pyproject.toml` & `kaskada-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.4.0"
+version = "0.4.1"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
```

### Comparing `kaskada-0.4.0/src/fenlmagic/__init__.py` & `kaskada-0.4.1/src/fenlmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/api/api_utils.py` & `kaskada-0.4.1/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/api/local_session/local_service.py` & `kaskada-0.4.1/src/kaskada/api/local_session/local_service.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/api/local_session/local_session_keep_alive.py` & `kaskada-0.4.1/src/kaskada/api/local_session/local_session_keep_alive.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/api/release.py` & `kaskada-0.4.1/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/api/remote_session/__init__.py` & `kaskada-0.4.1/src/kaskada/api/remote_session/__init__.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/api/session.py` & `kaskada-0.4.1/src/kaskada/api/session.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/client.py` & `kaskada-0.4.1/src/kaskada/client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/formatters.css` & `kaskada-0.4.1/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/formatters.js` & `kaskada-0.4.1/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/formatters.py` & `kaskada-0.4.1/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/formatters_helpers.py` & `kaskada-0.4.1/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/formatters_shared.py` & `kaskada-0.4.1/src/kaskada/formatters_shared.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/health/health_check_client.py` & `kaskada-0.4.1/src/kaskada/health/health_check_client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/health/health_check_servicer.py` & `kaskada-0.4.1/src/kaskada/health/health_check_servicer.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/health/health_check_watcher.py` & `kaskada-0.4.1/src/kaskada/health/health_check_watcher.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/common_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
 from kaskada.kaskada.v1alpha import destinations_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_destinations__pb2
 from kaskada.kaskada.v1alpha import fenl_diagnostics_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_fenl__diagnostics__pb2
 from kaskada.kaskada.v1alpha import plan_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_plan__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-kaskada/kaskada/v1alpha/compute_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a*kaskada/kaskada/v1alpha/destinations.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a\"kaskada/kaskada/v1alpha/plan.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"`\n\nFeatureSet\x12<\n\x08\x66ormulas\x18\x01 \x03(\x0b\x32 .kaskada.kaskada.v1alpha.FormulaR\x08\x66ormulas\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\"`\n\x07\x46ormula\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07\x66ormula\x18\x02 \x01(\tR\x07\x66ormula\x12\'\n\x0fsource_location\x18\x03 \x01(\tR\x0esourceLocation\"\xf9\x02\n\x0c\x43omputeTable\x12<\n\x06\x63onfig\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.TableConfigR\x06\x63onfig\x12\x42\n\x08metadata\x18\x02 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\x08metadata\x12J\n\tfile_sets\x18\x03 \x03(\x0b\x32-.kaskada.kaskada.v1alpha.ComputeTable.FileSetR\x08\x66ileSets\x1a\x9a\x01\n\x07\x46ileSet\x12\x41\n\nslice_plan\x18\x01 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\x12L\n\x0eprepared_files\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.PreparedFileR\rpreparedFiles\"\x1e\n\x08PlanHash\x12\x12\n\x04hash\x18\x01 \x01(\x0cR\x04hash\"\xed\x02\n\x13ProgressInformation\x12(\n\x10total_input_rows\x18\x01 \x01(\x03R\x0etotalInputRows\x12\x30\n\x14processed_input_rows\x18\x02 \x01(\x03R\x12processedInputRows\x12#\n\rbuffered_rows\x18\x03 \x01(\x03R\x0c\x62ufferedRows\x12\x36\n\x17processed_buffered_rows\x18\x08 \x01(\x03R\x15processedBufferedRows\x12$\n\x0emin_event_time\x18\x04 \x01(\x03R\x0cminEventTime\x12$\n\x0emax_event_time\x18\x05 \x01(\x03R\x0cmaxEventTime\x12\x1f\n\x0boutput_time\x18\x06 \x01(\x03R\noutputTime\x12\x30\n\x14produced_output_rows\x18\x07 \x01(\x03R\x12producedOutputRows\"{\n\x15\x43omputeSnapshotConfig\x12#\n\routput_prefix\x18\x01 \x01(\tR\x0coutputPrefix\x12=\n\x0bresume_from\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nresumeFrom\"\xd2\x01\n\x0f\x43omputeSnapshot\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emax_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12>\n\tplan_hash\x18\x03 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\x12)\n\x10snapshot_version\x18\x04 \x01(\x05R\x0fsnapshotVersion\"\"\n GetCurrentSnapshotVersionRequest\"N\n!GetCurrentSnapshotVersionResponse\x12)\n\x10snapshot_version\x18\x01 \x01(\x05R\x0fsnapshotVersion\"\xb0\x04\n\x0e\x43ompileRequest\x12=\n\x06tables\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x44\n\x0b\x66\x65\x61ture_set\x18\x02 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.FeatureSetR\nfeatureSet\x12J\n\rslice_request\x18\x03 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x0csliceRequest\x12_\n\x0f\x65xpression_kind\x18\x04 \x01(\x0e\x32\x36.kaskada.kaskada.v1alpha.CompileRequest.ExpressionKindR\x0e\x65xpressionKind\x12\"\n\x0c\x65xperimental\x18\x05 \x01(\x08R\x0c\x65xperimental\x12Z\n\x13per_entity_behavior\x18\x06 \x01(\x0e\x32*.kaskada.kaskada.v1alpha.PerEntityBehaviorR\x11perEntityBehavior\"l\n\x0e\x45xpressionKind\x12\x1f\n\x1b\x45XPRESSION_KIND_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45XPRESSION_KIND_COMPLETE\x10\x01\x12\x1b\n\x17\x45XPRESSION_KIND_FORMULA\x10\x02\"\xe0\x03\n\x0f\x43ompileResponse\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x38\n\x04plan\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12\x42\n\x0bresult_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\nresultType\x12\x1d\n\nfree_names\x18\x05 \x03(\tR\tfreeNames\x12\x45\n\x0ctable_slices\x18\x06 \x03(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\x0btableSlices\x12/\n\x13incremental_enabled\x18\x07 \x01(\x08R\x12incrementalEnabled\x12>\n\tplan_hash\x18\x08 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\"\xb7\x04\n\x0e\x45xecuteRequest\x12\x38\n\x04plan\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x12\x46\n\x06limits\x18\x05 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ExecuteRequest.LimitsR\x06limits\x12\x66\n\x17\x63ompute_snapshot_config\x18\x06 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ComputeSnapshotConfigR\x15\x63omputeSnapshotConfig\x12?\n\rchanged_since\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x63hangedSince\x12\x46\n\x11\x66inal_result_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\x1a+\n\x06Limits\x12!\n\x0cpreview_rows\x18\x01 \x01(\x03R\x0bpreviewRows\"\xed\x03\n\x0f\x45xecuteResponse\x12=\n\x05state\x18\x01 \x01(\x0e\x32\'.kaskada.kaskada.v1alpha.LongQueryStateR\x05state\x12\"\n\ris_query_done\x18\x02 \x01(\x08R\x0bisQueryDone\x12H\n\x08progress\x18\x03 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.ProgressInformationR\x08progress\x12J\n\x12\x66light_record_path\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x10\x66lightRecordPath\x12\x42\n\x0eplan_yaml_path\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0cplanYamlPath\x12U\n\x11\x63ompute_snapshots\x18\x06 \x03(\x0b\x32(.kaskada.kaskada.v1alpha.ComputeSnapshotR\x10\x63omputeSnapshots\x12\x46\n\x0b\x64\x65stination\x18\x07 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\"\x8d\x02\n\x1bStartMaterializationRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\x12\x38\n\x04plan\x18\x02 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x03 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x04 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\"\x1e\n\x1cStartMaterializationResponse\"P\n\x1fGetMaterializationStatusRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\"l\n GetMaterializationStatusResponse\x12H\n\x08progress\x18\x01 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.ProgressInformationR\x08progress\"K\n\x1aStopMaterializationRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\"\x1d\n\x1bStopMaterializationResponse*\x8a\x01\n\x0eLongQueryState\x12 \n\x1cLONG_QUERY_STATE_UNSPECIFIED\x10\x00\x12\x1c\n\x18LONG_QUERY_STATE_INITIAL\x10\x01\x12\x1c\n\x18LONG_QUERY_STATE_RUNNING\x10\x02\x12\x1a\n\x16LONG_QUERY_STATE_FINAL\x10\x03\x32\xfe\x05\n\x0e\x43omputeService\x12\\\n\x07\x43ompile\x12\'.kaskada.kaskada.v1alpha.CompileRequest\x1a(.kaskada.kaskada.v1alpha.CompileResponse\x12^\n\x07\x45xecute\x12\'.kaskada.kaskada.v1alpha.ExecuteRequest\x1a(.kaskada.kaskada.v1alpha.ExecuteResponse0\x01\x12\x83\x01\n\x14StartMaterialization\x12\x34.kaskada.kaskada.v1alpha.StartMaterializationRequest\x1a\x35.kaskada.kaskada.v1alpha.StartMaterializationResponse\x12\x8f\x01\n\x18GetMaterializationStatus\x12\x38.kaskada.kaskada.v1alpha.GetMaterializationStatusRequest\x1a\x39.kaskada.kaskada.v1alpha.GetMaterializationStatusResponse\x12\x80\x01\n\x13StopMaterialization\x12\x33.kaskada.kaskada.v1alpha.StopMaterializationRequest\x1a\x34.kaskada.kaskada.v1alpha.StopMaterializationResponse\x12\x92\x01\n\x19GetCurrentSnapshotVersion\x12\x39.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionRequest\x1a:.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionResponseB\x83\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x13\x43omputeServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-kaskada/kaskada/v1alpha/compute_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a*kaskada/kaskada/v1alpha/destinations.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a\"kaskada/kaskada/v1alpha/plan.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"`\n\nFeatureSet\x12<\n\x08\x66ormulas\x18\x01 \x03(\x0b\x32 .kaskada.kaskada.v1alpha.FormulaR\x08\x66ormulas\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\"`\n\x07\x46ormula\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07\x66ormula\x18\x02 \x01(\tR\x07\x66ormula\x12\'\n\x0fsource_location\x18\x03 \x01(\tR\x0esourceLocation\"\xf9\x02\n\x0c\x43omputeTable\x12<\n\x06\x63onfig\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.TableConfigR\x06\x63onfig\x12\x42\n\x08metadata\x18\x02 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\x08metadata\x12J\n\tfile_sets\x18\x03 \x03(\x0b\x32-.kaskada.kaskada.v1alpha.ComputeTable.FileSetR\x08\x66ileSets\x1a\x9a\x01\n\x07\x46ileSet\x12\x41\n\nslice_plan\x18\x01 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\x12L\n\x0eprepared_files\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.PreparedFileR\rpreparedFiles\"\x1e\n\x08PlanHash\x12\x12\n\x04hash\x18\x01 \x01(\x0cR\x04hash\"\xed\x02\n\x13ProgressInformation\x12(\n\x10total_input_rows\x18\x01 \x01(\x03R\x0etotalInputRows\x12\x30\n\x14processed_input_rows\x18\x02 \x01(\x03R\x12processedInputRows\x12#\n\rbuffered_rows\x18\x03 \x01(\x03R\x0c\x62ufferedRows\x12\x36\n\x17processed_buffered_rows\x18\x08 \x01(\x03R\x15processedBufferedRows\x12$\n\x0emin_event_time\x18\x04 \x01(\x03R\x0cminEventTime\x12$\n\x0emax_event_time\x18\x05 \x01(\x03R\x0cmaxEventTime\x12\x1f\n\x0boutput_time\x18\x06 \x01(\x03R\noutputTime\x12\x30\n\x14produced_output_rows\x18\x07 \x01(\x03R\x12producedOutputRows\"{\n\x15\x43omputeSnapshotConfig\x12#\n\routput_prefix\x18\x01 \x01(\tR\x0coutputPrefix\x12=\n\x0bresume_from\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nresumeFrom\"\xd2\x01\n\x0f\x43omputeSnapshot\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emax_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12>\n\tplan_hash\x18\x03 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\x12)\n\x10snapshot_version\x18\x04 \x01(\x05R\x0fsnapshotVersion\"\"\n GetCurrentSnapshotVersionRequest\"N\n!GetCurrentSnapshotVersionResponse\x12)\n\x10snapshot_version\x18\x01 \x01(\x05R\x0fsnapshotVersion\"\xb0\x04\n\x0e\x43ompileRequest\x12=\n\x06tables\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x44\n\x0b\x66\x65\x61ture_set\x18\x02 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.FeatureSetR\nfeatureSet\x12J\n\rslice_request\x18\x03 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x0csliceRequest\x12_\n\x0f\x65xpression_kind\x18\x04 \x01(\x0e\x32\x36.kaskada.kaskada.v1alpha.CompileRequest.ExpressionKindR\x0e\x65xpressionKind\x12\"\n\x0c\x65xperimental\x18\x05 \x01(\x08R\x0c\x65xperimental\x12Z\n\x13per_entity_behavior\x18\x06 \x01(\x0e\x32*.kaskada.kaskada.v1alpha.PerEntityBehaviorR\x11perEntityBehavior\"l\n\x0e\x45xpressionKind\x12\x1f\n\x1b\x45XPRESSION_KIND_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45XPRESSION_KIND_COMPLETE\x10\x01\x12\x1b\n\x17\x45XPRESSION_KIND_FORMULA\x10\x02\"\xe0\x03\n\x0f\x43ompileResponse\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x38\n\x04plan\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12\x42\n\x0bresult_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\nresultType\x12\x1d\n\nfree_names\x18\x05 \x03(\tR\tfreeNames\x12\x45\n\x0ctable_slices\x18\x06 \x03(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\x0btableSlices\x12/\n\x13incremental_enabled\x18\x07 \x01(\x08R\x12incrementalEnabled\x12>\n\tplan_hash\x18\x08 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\"\xb7\x04\n\x0e\x45xecuteRequest\x12\x38\n\x04plan\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x12\x46\n\x06limits\x18\x05 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ExecuteRequest.LimitsR\x06limits\x12\x66\n\x17\x63ompute_snapshot_config\x18\x06 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ComputeSnapshotConfigR\x15\x63omputeSnapshotConfig\x12?\n\rchanged_since\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x63hangedSince\x12\x46\n\x11\x66inal_result_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\x1a+\n\x06Limits\x12!\n\x0cpreview_rows\x18\x01 \x01(\x03R\x0bpreviewRows\"\xed\x03\n\x0f\x45xecuteResponse\x12=\n\x05state\x18\x01 \x01(\x0e\x32\'.kaskada.kaskada.v1alpha.LongQueryStateR\x05state\x12\"\n\ris_query_done\x18\x02 \x01(\x08R\x0bisQueryDone\x12H\n\x08progress\x18\x03 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.ProgressInformationR\x08progress\x12J\n\x12\x66light_record_path\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x10\x66lightRecordPath\x12\x42\n\x0eplan_yaml_path\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0cplanYamlPath\x12U\n\x11\x63ompute_snapshots\x18\x06 \x03(\x0b\x32(.kaskada.kaskada.v1alpha.ComputeSnapshotR\x10\x63omputeSnapshots\x12\x46\n\x0b\x64\x65stination\x18\x07 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\"\x8d\x02\n\x1bStartMaterializationRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\x12\x38\n\x04plan\x18\x02 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x03 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x04 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\"\x1e\n\x1cStartMaterializationResponse\"P\n\x1fGetMaterializationStatusRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\"\xf9\x02\n GetMaterializationStatusResponse\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\x12U\n\x05state\x18\x02 \x01(\x0e\x32?.kaskada.kaskada.v1alpha.GetMaterializationStatusResponse.StateR\x05state\x12H\n\x08progress\x18\x03 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.ProgressInformationR\x08progress\x12\x14\n\x05\x65rror\x18\x04 \x01(\tR\x05\x65rror\"o\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x17\n\x13STATE_UNINITIALIZED\x10\x01\x12\x11\n\rSTATE_RUNNING\x10\x02\x12\x11\n\rSTATE_STOPPED\x10\x03\x12\x10\n\x0cSTATE_FAILED\x10\x04\"K\n\x1aStopMaterializationRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\"\x1d\n\x1bStopMaterializationResponse*\x8a\x01\n\x0eLongQueryState\x12 \n\x1cLONG_QUERY_STATE_UNSPECIFIED\x10\x00\x12\x1c\n\x18LONG_QUERY_STATE_INITIAL\x10\x01\x12\x1c\n\x18LONG_QUERY_STATE_RUNNING\x10\x02\x12\x1a\n\x16LONG_QUERY_STATE_FINAL\x10\x03\x32\xfe\x05\n\x0e\x43omputeService\x12\\\n\x07\x43ompile\x12\'.kaskada.kaskada.v1alpha.CompileRequest\x1a(.kaskada.kaskada.v1alpha.CompileResponse\x12^\n\x07\x45xecute\x12\'.kaskada.kaskada.v1alpha.ExecuteRequest\x1a(.kaskada.kaskada.v1alpha.ExecuteResponse0\x01\x12\x83\x01\n\x14StartMaterialization\x12\x34.kaskada.kaskada.v1alpha.StartMaterializationRequest\x1a\x35.kaskada.kaskada.v1alpha.StartMaterializationResponse\x12\x8f\x01\n\x18GetMaterializationStatus\x12\x38.kaskada.kaskada.v1alpha.GetMaterializationStatusRequest\x1a\x39.kaskada.kaskada.v1alpha.GetMaterializationStatusResponse\x12\x80\x01\n\x13StopMaterialization\x12\x33.kaskada.kaskada.v1alpha.StopMaterializationRequest\x1a\x34.kaskada.kaskada.v1alpha.StopMaterializationResponse\x12\x92\x01\n\x19GetCurrentSnapshotVersion\x12\x39.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionRequest\x1a:.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionResponseB\x83\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x13\x43omputeServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.compute_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\023ComputeServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_LONGQUERYSTATE']._serialized_start=4490
-  _globals['_LONGQUERYSTATE']._serialized_end=4628
+  _globals['_LONGQUERYSTATE']._serialized_start=4760
+  _globals['_LONGQUERYSTATE']._serialized_end=4898
   _globals['_FEATURESET']._serialized_start=343
   _globals['_FEATURESET']._serialized_end=439
   _globals['_FORMULA']._serialized_start=441
   _globals['_FORMULA']._serialized_end=537
   _globals['_COMPUTETABLE']._serialized_start=540
   _globals['_COMPUTETABLE']._serialized_end=917
   _globals['_COMPUTETABLE_FILESET']._serialized_start=763
@@ -65,16 +65,18 @@
   _globals['_EXECUTERESPONSE']._serialized_end=3883
   _globals['_STARTMATERIALIZATIONREQUEST']._serialized_start=3886
   _globals['_STARTMATERIALIZATIONREQUEST']._serialized_end=4155
   _globals['_STARTMATERIALIZATIONRESPONSE']._serialized_start=4157
   _globals['_STARTMATERIALIZATIONRESPONSE']._serialized_end=4187
   _globals['_GETMATERIALIZATIONSTATUSREQUEST']._serialized_start=4189
   _globals['_GETMATERIALIZATIONSTATUSREQUEST']._serialized_end=4269
-  _globals['_GETMATERIALIZATIONSTATUSRESPONSE']._serialized_start=4271
-  _globals['_GETMATERIALIZATIONSTATUSRESPONSE']._serialized_end=4379
-  _globals['_STOPMATERIALIZATIONREQUEST']._serialized_start=4381
-  _globals['_STOPMATERIALIZATIONREQUEST']._serialized_end=4456
-  _globals['_STOPMATERIALIZATIONRESPONSE']._serialized_start=4458
-  _globals['_STOPMATERIALIZATIONRESPONSE']._serialized_end=4487
-  _globals['_COMPUTESERVICE']._serialized_start=4631
-  _globals['_COMPUTESERVICE']._serialized_end=5397
+  _globals['_GETMATERIALIZATIONSTATUSRESPONSE']._serialized_start=4272
+  _globals['_GETMATERIALIZATIONSTATUSRESPONSE']._serialized_end=4649
+  _globals['_GETMATERIALIZATIONSTATUSRESPONSE_STATE']._serialized_start=4538
+  _globals['_GETMATERIALIZATIONSTATUSRESPONSE_STATE']._serialized_end=4649
+  _globals['_STOPMATERIALIZATIONREQUEST']._serialized_start=4651
+  _globals['_STOPMATERIALIZATIONREQUEST']._serialized_end=4726
+  _globals['_STOPMATERIALIZATIONRESPONSE']._serialized_start=4728
+  _globals['_STOPMATERIALIZATIONRESPONSE']._serialized_end=4757
+  _globals['_COMPUTESERVICE']._serialized_start=4901
+  _globals['_COMPUTESERVICE']._serialized_end=5667
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/destinations_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/plan_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/schema_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/sources_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/spec_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/test_cases_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py` & `kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py` & `kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/materialization.py` & `kaskada-0.4.1/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/query.py` & `kaskada-0.4.1/src/kaskada/query.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/slice_filters.py` & `kaskada-0.4.1/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/table.py` & `kaskada-0.4.1/src/kaskada/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,24 @@
     pass
 
 
 class PulsarTableSource(TableSource):
     def __init__(
         self,
         broker_service_url: str,
+        admin_service_url: str,
         auth_plugin: str,
         auth_params: str,
         tenant: str,
         namespace: str,
         topic_name: str,
     ):
         self._broker_service_url = broker_service_url
         self._auth_plugin = auth_plugin
+        self._admin_service_url = admin_service_url
         self._auth_params = auth_params
         self._tenant = tenant
         self._namespace = namespace
         self._topic_name = topic_name
 
 
 def get_table_name(
@@ -173,14 +175,15 @@
             )
         if source is not None:
             if isinstance(source, PulsarTableSource):
                 table_args["source"] = {
                     "pulsar": {
                         "config": {
                             "broker_service_url": source._broker_service_url,
+                            "admin_service_url": source._admin_service_url,
                             "auth_plugin": source._auth_plugin,
                             "auth_params": source._auth_params,
                             "tenant": source._tenant,
                             "namespace": source._namespace,
                             "topic_name": source._topic_name,
                         }
                     }
```

### Comparing `kaskada-0.4.0/src/kaskada/utils.py` & `kaskada-0.4.1/src/kaskada/utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/src/kaskada/view.py` & `kaskada-0.4.1/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/vendor/validate/validate.proto` & `kaskada-0.4.1/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/vendor/validate/validate_pb2.py` & `kaskada-0.4.1/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/vendor/validate/validate_pb2.pyi` & `kaskada-0.4.1/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.0/setup.py` & `kaskada-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n#### Generate documentation \nWe use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and \ngenerate an HTML formatted version of the codes documentation. \n\n* `poetry run poe docs` : generates and builds the docs \n* `poetry run poe docs-generate` : generates the docs (.rst files)\n* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)\n\nThe generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. \n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kaskada-0.4.0/PKG-INFO` & `kaskada-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.4.0
+Version: 0.4.1
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

