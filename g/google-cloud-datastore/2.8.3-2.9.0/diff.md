# Comparing `tmp/google-cloud-datastore-2.8.3.tar.gz` & `tmp/google-cloud-datastore-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-datastore-2.8.3.tar", last modified: Mon Oct 10 19:54:34 2022, max compression
+gzip compressed data, was "google-cloud-datastore-2.9.0.tar", last modified: Tue Oct 18 20:56:57 2022, max compression
```

## Comparing `google-cloud-datastore-2.8.3.tar` & `google-cloud-datastore-2.9.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.566072 google-cloud-datastore-2.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4900 2022-10-10 19:54:34.566072 google-cloud-datastore-2.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3933 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.534062 google-cloud-datastore-2.8.3/google/
--rw-rw-r--   0 root         (0)     1003      763 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.534062 google-cloud-datastore-2.8.3/google/cloud/
--rw-rw-r--   0 root         (0)     1003      763 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.534062 google-cloud-datastore-2.8.3/google/cloud/datastore/
--rw-rw-r--   0 root         (0)     1003     2503 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/__init__.py
--rw-rw-r--   0 root         (0)     1003      896 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/_app_engine_key.proto
--rw-rw-r--   0 root         (0)     1003     3099 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/_app_engine_key_pb2.py
--rw-rw-r--   0 root         (0)     1003     1751 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/_gapic.py
--rw-rw-r--   0 root         (0)     1003    13964 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/_http.py
--rw-rw-r--   0 root         (0)     1003    13716 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/batch.py
--rw-rw-r--   0 root         (0)     1003    34711 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/client.py
--rw-rw-r--   0 root         (0)     1003     7234 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/entity.py
--rw-rw-r--   0 root         (0)     1003    17987 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/helpers.py
--rw-rw-r--   0 root         (0)     1003    21504 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/key.py
--rw-rw-r--   0 root         (0)     1003       85 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/py.typed
--rw-rw-r--   0 root         (0)     1003    25575 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/query.py
--rw-rw-r--   0 root         (0)     1003    10450 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/transaction.py
--rw-rw-r--   0 root         (0)     1003      597 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.534062 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/
--rw-rw-r--   0 root         (0)     1003     2437 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1983 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       89 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.538063 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.538063 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/
--rw-rw-r--   0 root         (0)     1003      769 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003    39714 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003    47935 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/client.py
--rw-rw-r--   0 root         (0)     1003     5848 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.542065 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1194 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9174 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22695 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23148 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.542065 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/
--rw-rw-r--   0 root         (0)     1003     1738 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    18704 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/datastore_admin.py
--rw-rw-r--   0 root         (0)     1003     3349 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/index.py
--rw-rw-r--   0 root         (0)     1003     4764 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/migration.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.546066 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/
--rw-rw-r--   0 root         (0)     1003     2972 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2126 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.546066 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.546066 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/
--rw-rw-r--   0 root         (0)     1003      749 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/__init__.py
--rw-rw-r--   0 root         (0)     1003    37126 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/async_client.py
--rw-rw-r--   0 root         (0)     1003    45511 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.550067 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/
--rw-rw-r--   0 root         (0)     1003     1149 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9594 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18310 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18722 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.554068 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/
--rw-rw-r--   0 root         (0)     1003     2115 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    22164 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/datastore.py
--rw-rw-r--   0 root         (0)     1003    12174 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/entity.py
--rw-rw-r--   0 root         (0)     1003    17198 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/query.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.554068 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/
--rw-r--r--   0 root         (0)     1003     4900 2022-10-10 19:54:34.000000 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3655 2022-10-10 19:54:34.000000 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 19:54:34.000000 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 19:54:34.000000 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 19:54:34.000000 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      259 2022-10-10 19:54:34.000000 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 19:54:34.000000 google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.554068 google-cloud-datastore-2.8.3/scripts/
--rw-rw-r--   0 root         (0)     1003     6338 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/scripts/fixup_datastore_admin_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6369 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/scripts/fixup_datastore_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 19:54:34.566072 google-cloud-datastore-2.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3598 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.558069 google-cloud-datastore-2.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     3090 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/doctests.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.558069 google-cloud-datastore-2.8.3/tests/system/
--rw-rw-r--   0 root         (0)     1003        0 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     1283 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/_helpers.py
--rw-rw-r--   0 root         (0)     1003     1487 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/conftest.py
--rw-rw-r--   0 root         (0)     1003      314 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/index.yaml
--rw-rw-r--   0 root         (0)     1003     1978 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/test_allocate_reserve_ids.py
--rw-rw-r--   0 root         (0)     1003     5505 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/test_put.py
--rw-rw-r--   0 root         (0)     1003    10809 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/test_query.py
--rw-rw-r--   0 root         (0)     1003     3913 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/test_read_consistency.py
--rw-rw-r--   0 root         (0)     1003     3649 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/test_transaction.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.558069 google-cloud-datastore-2.8.3/tests/system/utils/
--rw-rw-r--   0 root         (0)     1003        0 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/utils/__init__.py
--rw-rw-r--   0 root         (0)     1003     2738 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/utils/clear_datastore.py
--rw-rw-r--   0 root         (0)     1003     6483 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/system/utils/populate_datastore.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.562070 google-cloud-datastore-2.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.562070 google-cloud-datastore-2.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.562070 google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_admin_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_admin_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    84518 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_admin_v1/test_datastore_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 19:54:34.562070 google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    93270 2022-10-10 19:51:32.000000 google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_v1/test_datastore.py
--rw-rw-r--   0 root         (0)     1003     3162 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test__gapic.py
--rw-rw-r--   0 root         (0)     1003    26762 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test__http.py
--rw-rw-r--   0 root         (0)     1003    15730 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test_batch.py
--rw-rw-r--   0 root         (0)     1003    52906 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003     6739 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test_entity.py
--rw-rw-r--   0 root         (0)     1003    37561 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test_helpers.py
--rw-rw-r--   0 root         (0)     1003    22852 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test_key.py
--rw-rw-r--   0 root         (0)     1003    28328 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test_query.py
--rw-rw-r--   0 root         (0)     1003    14227 2022-10-10 19:51:31.000000 google-cloud-datastore-2.8.3/tests/unit/test_transaction.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.482428 google-cloud-datastore-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4900 2022-10-18 20:56:57.482428 google-cloud-datastore-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3933 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.462414 google-cloud-datastore-2.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      763 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.462414 google-cloud-datastore-2.9.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      763 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.466417 google-cloud-datastore-2.9.0/google/cloud/datastore/
+-rw-rw-r--   0 root         (0)     1003     2503 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      896 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/_app_engine_key.proto
+-rw-rw-r--   0 root         (0)     1003     3099 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/_app_engine_key_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1751 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/_gapic.py
+-rw-rw-r--   0 root         (0)     1003    13964 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/_http.py
+-rw-rw-r--   0 root         (0)     1003    13716 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/batch.py
+-rw-rw-r--   0 root         (0)     1003    34711 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/client.py
+-rw-rw-r--   0 root         (0)     1003     7234 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/entity.py
+-rw-rw-r--   0 root         (0)     1003    17987 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/helpers.py
+-rw-rw-r--   0 root         (0)     1003    21504 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/key.py
+-rw-rw-r--   0 root         (0)     1003       85 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/py.typed
+-rw-rw-r--   0 root         (0)     1003    25575 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/query.py
+-rw-rw-r--   0 root         (0)     1003    10450 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/transaction.py
+-rw-rw-r--   0 root         (0)     1003      597 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.466417 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/
+-rw-rw-r--   0 root         (0)     1003     2437 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1983 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       89 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.466417 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.466417 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/
+-rw-rw-r--   0 root         (0)     1003      769 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44344 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003    52521 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/client.py
+-rw-rw-r--   0 root         (0)     1003     5848 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.466417 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1194 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9493 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22778 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23231 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.470420 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1738 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18713 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/datastore_admin.py
+-rw-rw-r--   0 root         (0)     1003     3349 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/index.py
+-rw-rw-r--   0 root         (0)     1003     4806 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/migration.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.470420 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/
+-rw-rw-r--   0 root         (0)     1003     3392 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2396 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       83 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.470420 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.470420 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/
+-rw-rw-r--   0 root         (0)     1003      749 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54266 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62328 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.470420 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/
+-rw-rw-r--   0 root         (0)     1003     1149 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11732 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22944 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23387 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.470420 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2437 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3233 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/aggregation_result.py
+-rw-rw-r--   0 root         (0)     1003    27266 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/datastore.py
+-rw-rw-r--   0 root         (0)     1003    12801 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/entity.py
+-rw-rw-r--   0 root         (0)     1003    21313 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/query.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.474423 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/
+-rw-r--r--   0 root         (0)     1003     4900 2022-10-18 20:56:57.000000 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3709 2022-10-18 20:56:57.000000 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-18 20:56:57.000000 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-18 20:56:57.000000 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-18 20:56:57.000000 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      291 2022-10-18 20:56:57.000000 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-18 20:56:57.000000 google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.474423 google-cloud-datastore-2.9.0/scripts/
+-rw-rw-r--   0 root         (0)     1003     6338 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/scripts/fixup_datastore_admin_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6591 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/scripts/fixup_datastore_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-18 20:56:57.482428 google-cloud-datastore-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3286 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.474423 google-cloud-datastore-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3090 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/doctests.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.474423 google-cloud-datastore-2.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003        0 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1283 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     1487 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/conftest.py
+-rw-rw-r--   0 root         (0)     1003      314 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/index.yaml
+-rw-rw-r--   0 root         (0)     1003     1978 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/test_allocate_reserve_ids.py
+-rw-rw-r--   0 root         (0)     1003     5505 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/test_put.py
+-rw-rw-r--   0 root         (0)     1003    10809 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/test_query.py
+-rw-rw-r--   0 root         (0)     1003     3913 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/test_read_consistency.py
+-rw-rw-r--   0 root         (0)     1003     3649 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/test_transaction.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.478425 google-cloud-datastore-2.9.0/tests/system/utils/
+-rw-rw-r--   0 root         (0)     1003        0 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/utils/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2738 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/utils/clear_datastore.py
+-rw-rw-r--   0 root         (0)     1003     6483 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/system/utils/populate_datastore.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.478425 google-cloud-datastore-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.478425 google-cloud-datastore-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.478425 google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_admin_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_admin_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    99741 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_admin_v1/test_datastore_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-18 20:56:57.478425 google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   136717 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_v1/test_datastore.py
+-rw-rw-r--   0 root         (0)     1003     3162 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test__gapic.py
+-rw-rw-r--   0 root         (0)     1003    26762 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test__http.py
+-rw-rw-r--   0 root         (0)     1003    15730 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test_batch.py
+-rw-rw-r--   0 root         (0)     1003    52906 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003     6739 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test_entity.py
+-rw-rw-r--   0 root         (0)     1003    37561 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003    22852 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test_key.py
+-rw-rw-r--   0 root         (0)     1003    28328 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test_query.py
+-rw-rw-r--   0 root         (0)     1003    14227 2022-10-18 20:53:27.000000 google-cloud-datastore-2.9.0/tests/unit/test_transaction.py
```

### Comparing `google-cloud-datastore-2.8.3/LICENSE` & `google-cloud-datastore-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/MANIFEST.in` & `google-cloud-datastore-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/PKG-INFO` & `google-cloud-datastore-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastore
-Version: 2.8.3
+Version: 2.9.0
 Summary: Google Cloud Datastore API client library
 Home-page: https://github.com/googleapis/python-datastore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datastore-2.8.3/README.rst` & `google-cloud-datastore-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/__init__.py` & `google-cloud-datastore-2.9.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/_app_engine_key.proto` & `google-cloud-datastore-2.9.0/google/cloud/datastore/_app_engine_key.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/_app_engine_key_pb2.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/_app_engine_key_pb2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/_gapic.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/_gapic.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/_http.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/_http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/batch.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/client.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/entity.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/entity.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/helpers.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/key.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/key.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/query.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/transaction.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore/version.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.8.3"
+__version__ = "2.9.0"
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/gapic_metadata.json` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/async_client.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -283,32 +283,39 @@
         of an export may only be used once the associated
         operation is done. If an export operation is cancelled
         before completion it may leave partial data behind in
         Google Cloud Storage.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
-            def sample_export_entities():
+            async def sample_export_entities():
                 # Create a client
-                client = datastore_admin_v1.DatastoreAdminClient()
+                client = datastore_admin_v1.DatastoreAdminAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_admin_v1.ExportEntitiesRequest(
                     project_id="project_id_value",
                     output_url_prefix="output_url_prefix_value",
                 )
 
                 # Make the request
                 operation = client.export_entities(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = operation.result()
+                response = await operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_admin_v1.types.ExportEntitiesRequest, dict]):
                 The request object. The request for
@@ -405,14 +412,22 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.export_entities,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -446,32 +461,39 @@
         monitored and managed via the Operation resource that is
         created. If an ImportEntities operation is cancelled, it
         is possible that a subset of the data has already been
         imported to Cloud Datastore.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
-            def sample_import_entities():
+            async def sample_import_entities():
                 # Create a client
-                client = datastore_admin_v1.DatastoreAdminClient()
+                client = datastore_admin_v1.DatastoreAdminAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_admin_v1.ImportEntitiesRequest(
                     project_id="project_id_value",
                     input_url="input_url_value",
                 )
 
                 # Make the request
                 operation = client.import_entities(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = operation.result()
+                response = await operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_admin_v1.types.ImportEntitiesRequest, dict]):
                 The request object. The request for
@@ -536,17 +558,14 @@
 
                       service Foo {
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
-                   The JSON representation for Empty is empty JSON
-                   object {}.
-
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([project_id, labels, input_url, entity_filter])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -572,14 +591,22 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.import_entities,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -617,30 +644,37 @@
         then re-creating the index with [create]
         [google.datastore.admin.v1.DatastoreAdmin.CreateIndex].
 
         Indexes with a single property cannot be created.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
-            def sample_create_index():
+            async def sample_create_index():
                 # Create a client
-                client = datastore_admin_v1.DatastoreAdminClient()
+                client = datastore_admin_v1.DatastoreAdminAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_admin_v1.CreateIndexRequest(
                 )
 
                 # Make the request
                 operation = client.create_index(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = operation.result()
+                response = await operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_admin_v1.types.CreateIndexRequest, dict]):
                 The request object. The request for
@@ -667,14 +701,22 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.create_index,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -711,30 +753,37 @@
         process can be recovered by fixing the data that caused the
         error, followed by calling
         [delete][google.datastore.admin.v1.DatastoreAdmin.DeleteIndex]
         again.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
-            def sample_delete_index():
+            async def sample_delete_index():
                 # Create a client
-                client = datastore_admin_v1.DatastoreAdminClient()
+                client = datastore_admin_v1.DatastoreAdminAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_admin_v1.DeleteIndexRequest(
                 )
 
                 # Make the request
                 operation = client.delete_index(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = operation.result()
+                response = await operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_admin_v1.types.DeleteIndexRequest, dict]):
                 The request object. The request for
@@ -761,14 +810,25 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.delete_index,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (
+                    ("project_id", request.project_id),
+                    ("index_id", request.index_id),
+                )
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -792,26 +852,33 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> index.Index:
         r"""Gets an index.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
-            def sample_get_index():
+            async def sample_get_index():
                 # Create a client
-                client = datastore_admin_v1.DatastoreAdminClient()
+                client = datastore_admin_v1.DatastoreAdminAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_admin_v1.GetIndexRequest(
                 )
 
                 # Make the request
-                response = client.get_index(request=request)
+                response = await client.get_index(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_admin_v1.types.GetIndexRequest, dict]):
                 The request object. The request for
@@ -843,14 +910,25 @@
                 ),
                 deadline=60.0,
             ),
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (
+                    ("project_id", request.project_id),
+                    ("index_id", request.index_id),
+                )
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -869,29 +947,36 @@
         r"""Lists the indexes that match the specified filters.
         Datastore uses an eventually consistent query to fetch
         the list of indexes and may occasionally return stale
         results.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
-            def sample_list_indexes():
+            async def sample_list_indexes():
                 # Create a client
-                client = datastore_admin_v1.DatastoreAdminClient()
+                client = datastore_admin_v1.DatastoreAdminAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_admin_v1.ListIndexesRequest(
                 )
 
                 # Make the request
                 page_result = client.list_indexes(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.datastore_admin_v1.types.ListIndexesRequest, dict]):
                 The request object. The request for
                 [google.datastore.admin.v1.DatastoreAdmin.ListIndexes][google.datastore.admin.v1.DatastoreAdmin.ListIndexes].
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -926,14 +1011,22 @@
                 ),
                 deadline=60.0,
             ),
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/client.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -457,14 +457,15 @@
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
                 quota_project_id=client_options.quota_project_id,
                 client_info=client_info,
                 always_use_jwt_access=True,
+                api_audience=client_options.api_audience,
             )
 
     def export_entities(
         self,
         request: Union[datastore_admin.ExportEntitiesRequest, dict] = None,
         *,
         project_id: str = None,
@@ -484,14 +485,21 @@
         of an export may only be used once the associated
         operation is done. If an export operation is cancelled
         before completion it may leave partial data behind in
         Google Cloud Storage.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
             def sample_export_entities():
                 # Create a client
                 client = datastore_admin_v1.DatastoreAdminClient()
 
                 # Initialize request argument(s)
@@ -605,14 +613,22 @@
             if output_url_prefix is not None:
                 request.output_url_prefix = output_url_prefix
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.export_entities]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -646,14 +662,21 @@
         monitored and managed via the Operation resource that is
         created. If an ImportEntities operation is cancelled, it
         is possible that a subset of the data has already been
         imported to Cloud Datastore.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
             def sample_import_entities():
                 # Create a client
                 client = datastore_admin_v1.DatastoreAdminClient()
 
                 # Initialize request argument(s)
@@ -736,17 +759,14 @@
 
                       service Foo {
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
-                   The JSON representation for Empty is empty JSON
-                   object {}.
-
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([project_id, labels, input_url, entity_filter])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -771,14 +791,22 @@
             if entity_filter is not None:
                 request.entity_filter = entity_filter
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.import_entities]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -816,14 +844,21 @@
         then re-creating the index with [create]
         [google.datastore.admin.v1.DatastoreAdmin.CreateIndex].
 
         Indexes with a single property cannot be created.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
             def sample_create_index():
                 # Create a client
                 client = datastore_admin_v1.DatastoreAdminClient()
 
                 # Initialize request argument(s)
@@ -867,14 +902,22 @@
         if not isinstance(request, datastore_admin.CreateIndexRequest):
             request = datastore_admin.CreateIndexRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.create_index]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -911,14 +954,21 @@
         process can be recovered by fixing the data that caused the
         error, followed by calling
         [delete][google.datastore.admin.v1.DatastoreAdmin.DeleteIndex]
         again.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
             def sample_delete_index():
                 # Create a client
                 client = datastore_admin_v1.DatastoreAdminClient()
 
                 # Initialize request argument(s)
@@ -962,14 +1012,25 @@
         if not isinstance(request, datastore_admin.DeleteIndexRequest):
             request = datastore_admin.DeleteIndexRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.delete_index]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (
+                    ("project_id", request.project_id),
+                    ("index_id", request.index_id),
+                )
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -993,14 +1054,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> index.Index:
         r"""Gets an index.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
             def sample_get_index():
                 # Create a client
                 client = datastore_admin_v1.DatastoreAdminClient()
 
                 # Initialize request argument(s)
@@ -1035,14 +1103,25 @@
         if not isinstance(request, datastore_admin.GetIndexRequest):
             request = datastore_admin.GetIndexRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.get_index]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (
+                    ("project_id", request.project_id),
+                    ("index_id", request.index_id),
+                )
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -1061,14 +1140,21 @@
         r"""Lists the indexes that match the specified filters.
         Datastore uses an eventually consistent query to fetch
         the list of indexes and may occasionally return stale
         results.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_admin_v1
 
             def sample_list_indexes():
                 # Create a client
                 client = datastore_admin_v1.DatastoreAdminClient()
 
                 # Initialize request argument(s)
@@ -1109,14 +1195,22 @@
         if not isinstance(request, datastore_admin.ListIndexesRequest):
             request = datastore_admin.ListIndexesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.list_indexes]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/pagers.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/base.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         host: str = DEFAULT_HOST,
         credentials: ga_credentials.Credentials = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
         **kwargs,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
@@ -83,19 +84,14 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
 
-        # Save the hostname. Default to port 443 (HTTPS) if none is specified.
-        if ":" not in host:
-            host += ":443"
-        self._host = host
-
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
         # Save the scopes.
         self._scopes = scopes
 
         # If no credentials are provided, then determine the appropriate
         # defaults.
@@ -108,26 +104,36 @@
             credentials, _ = google.auth.load_credentials_from_file(
                 credentials_file, **scopes_kwargs, quota_project_id=quota_project_id
             )
         elif credentials is None:
             credentials, _ = google.auth.default(
                 **scopes_kwargs, quota_project_id=quota_project_id
             )
+            # Don't apply audience if the credentials file passed from user.
+            if hasattr(credentials, "with_gdch_audience"):
+                credentials = credentials.with_gdch_audience(
+                    api_audience if api_audience else host
+                )
 
         # If the credentials are service account credentials, then always try to use self signed JWT.
         if (
             always_use_jwt_access
             and isinstance(credentials, service_account.Credentials)
             and hasattr(service_account.Credentials, "with_always_use_jwt_access")
         ):
             credentials = credentials.with_always_use_jwt_access(True)
 
         # Save the credentials.
         self._credentials = credentials
 
+        # Save the hostname. Default to port 443 (HTTPS) if none is specified.
+        if ":" not in host:
+            host += ":443"
+        self._host = host
+
     def _prep_wrapped_messages(self, client_info):
         # Precompute the wrapped methods.
         self._wrapped_methods = {
             self.export_entities: gapic_v1.method.wrap_method(
                 self.export_entities,
                 default_timeout=60.0,
                 client_info=client_info,
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         api_mtls_endpoint: str = None,
         client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
         ssl_channel_credentials: grpc.ChannelCredentials = None,
         client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
             credentials (Optional[google.auth.credentials.Credentials]): The
@@ -210,14 +211,15 @@
             host=host,
             credentials=credentials,
             credentials_file=credentials_file,
             scopes=scopes,
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
+            api_audience=api_audience,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc_asyncio.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/services/datastore_admin/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         api_mtls_endpoint: str = None,
         client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
         ssl_channel_credentials: grpc.ChannelCredentials = None,
         client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
         quota_project_id=None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
             credentials (Optional[google.auth.credentials.Credentials]): The
@@ -255,14 +256,15 @@
             host=host,
             credentials=credentials,
             credentials_file=credentials_file,
             scopes=scopes,
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
+            api_audience=api_audience,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/datastore_admin.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/datastore_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
     r"""Metadata for Datastore to Firestore migration operations.
 
     The DatastoreFirestoreMigration operation is not started by the
     end-user via an explicit "creation" method. This is an intentional
     deviation from the LRO design pattern.
 
     This singleton resource can be accessed at:
-    ``projects/{project_id}/datastore-firestore-migration``
+    "projects/{project_id}/operations/datastore-firestore-migration"
 
     Attributes:
         migration_state (google.cloud.datastore_admin_v1.types.MigrationState):
             The current state of migration from Cloud
             Datastore to Cloud Firestore in Datastore mode.
         migration_step (google.cloud.datastore_admin_v1.types.MigrationStep):
             The current step of migration from Cloud
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/index.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/index.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_admin_v1/types/migration.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_admin_v1/types/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     """
 
     class ConcurrencyMode(proto.Enum):
         r"""Concurrency modes for transactions in Cloud Firestore."""
         CONCURRENCY_MODE_UNSPECIFIED = 0
         PESSIMISTIC = 1
         OPTIMISTIC = 2
+        OPTIMISTIC_WITH_ENTITY_GROUPS = 3
 
     class PrepareStepDetails(proto.Message):
         r"""Details for the ``PREPARE`` step.
 
         Attributes:
             concurrency_mode (google.cloud.datastore_admin_v1.types.MigrationProgressEvent.ConcurrencyMode):
                 The concurrency mode this database will use when it reaches
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from .services.datastore import DatastoreClient
 from .services.datastore import DatastoreAsyncClient
 
+from .types.aggregation_result import AggregationResult
+from .types.aggregation_result import AggregationResultBatch
 from .types.datastore import AllocateIdsRequest
 from .types.datastore import AllocateIdsResponse
 from .types.datastore import BeginTransactionRequest
 from .types.datastore import BeginTransactionResponse
 from .types.datastore import CommitRequest
 from .types.datastore import CommitResponse
 from .types.datastore import LookupRequest
@@ -28,22 +30,25 @@
 from .types.datastore import Mutation
 from .types.datastore import MutationResult
 from .types.datastore import ReadOptions
 from .types.datastore import ReserveIdsRequest
 from .types.datastore import ReserveIdsResponse
 from .types.datastore import RollbackRequest
 from .types.datastore import RollbackResponse
+from .types.datastore import RunAggregationQueryRequest
+from .types.datastore import RunAggregationQueryResponse
 from .types.datastore import RunQueryRequest
 from .types.datastore import RunQueryResponse
 from .types.datastore import TransactionOptions
 from .types.entity import ArrayValue
 from .types.entity import Entity
 from .types.entity import Key
 from .types.entity import PartitionId
 from .types.entity import Value
+from .types.query import AggregationQuery
 from .types.query import CompositeFilter
 from .types.query import EntityResult
 from .types.query import Filter
 from .types.query import GqlQuery
 from .types.query import GqlQueryParameter
 from .types.query import KindExpression
 from .types.query import Projection
@@ -51,14 +56,17 @@
 from .types.query import PropertyOrder
 from .types.query import PropertyReference
 from .types.query import Query
 from .types.query import QueryResultBatch
 
 __all__ = (
     "DatastoreAsyncClient",
+    "AggregationQuery",
+    "AggregationResult",
+    "AggregationResultBatch",
     "AllocateIdsRequest",
     "AllocateIdsResponse",
     "ArrayValue",
     "BeginTransactionRequest",
     "BeginTransactionResponse",
     "CommitRequest",
     "CommitResponse",
@@ -83,12 +91,14 @@
     "Query",
     "QueryResultBatch",
     "ReadOptions",
     "ReserveIdsRequest",
     "ReserveIdsResponse",
     "RollbackRequest",
     "RollbackResponse",
+    "RunAggregationQueryRequest",
+    "RunAggregationQueryResponse",
     "RunQueryRequest",
     "RunQueryResponse",
     "TransactionOptions",
     "Value",
 )
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/gapic_metadata.json` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/gapic_metadata.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996744791666666%*

 * *Differences: {"'services'": "{'Datastore': {'clients': {'grpc': {'rpcs': {'RunAggregationQuery': "*

 * *               "OrderedDict([('methods', ['run_aggregation_query'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'RunAggregationQuery': OrderedDict([('methods', ['run_aggregation_query'])])}}}}}"}*

```diff
@@ -36,14 +36,19 @@
                             ]
                         },
                         "Rollback": {
                             "methods": [
                                 "rollback"
                             ]
                         },
+                        "RunAggregationQuery": {
+                            "methods": [
+                                "run_aggregation_query"
+                            ]
+                        },
                         "RunQuery": {
                             "methods": [
                                 "run_query"
                             ]
                         }
                     }
                 },
@@ -76,14 +81,19 @@
                             ]
                         },
                         "Rollback": {
                             "methods": [
                                 "rollback"
                             ]
                         },
+                        "RunAggregationQuery": {
+                            "methods": [
+                                "run_aggregation_query"
+                            ]
+                        },
                         "RunQuery": {
                             "methods": [
                                 "run_query"
                             ]
                         }
                     }
                 }
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/async_client.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/async_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 from google.oauth2 import service_account  # type: ignore
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.datastore_v1.types import aggregation_result
 from google.cloud.datastore_v1.types import datastore
 from google.cloud.datastore_v1.types import entity
 from google.cloud.datastore_v1.types import query
+from google.longrunning import operations_pb2
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import DatastoreTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import DatastoreGrpcAsyncIOTransport
 from .client import DatastoreClient
 
 
 class DatastoreAsyncClient:
@@ -214,27 +216,34 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.LookupResponse:
         r"""Looks up entities by key.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
-            def sample_lookup():
+            async def sample_lookup():
                 # Create a client
-                client = datastore_v1.DatastoreClient()
+                client = datastore_v1.DatastoreAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_v1.LookupRequest(
                     project_id="project_id_value",
                 )
 
                 # Make the request
-                response = client.lookup(request=request)
+                response = await client.lookup(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_v1.types.LookupRequest, dict]):
                 The request object. The request for
@@ -305,14 +314,22 @@
                 ),
                 deadline=60.0,
             ),
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -328,27 +345,34 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.RunQueryResponse:
         r"""Queries for entities.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
-            def sample_run_query():
+            async def sample_run_query():
                 # Create a client
-                client = datastore_v1.DatastoreClient()
+                client = datastore_v1.DatastoreAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_v1.RunQueryRequest(
                     project_id="project_id_value",
                 )
 
                 # Make the request
-                response = client.run_query(request=request)
+                response = await client.run_query(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_v1.types.RunQueryRequest, dict]):
                 The request object. The request for
@@ -382,14 +406,114 @@
                 ),
                 deadline=60.0,
             ),
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def run_aggregation_query(
+        self,
+        request: Union[datastore.RunAggregationQueryRequest, dict] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> datastore.RunAggregationQueryResponse:
+        r"""Runs an aggregation query.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import datastore_v1
+
+            async def sample_run_aggregation_query():
+                # Create a client
+                client = datastore_v1.DatastoreAsyncClient()
+
+                # Initialize request argument(s)
+                request = datastore_v1.RunAggregationQueryRequest(
+                    project_id="project_id_value",
+                )
+
+                # Make the request
+                response = await client.run_aggregation_query(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.datastore_v1.types.RunAggregationQueryRequest, dict]):
+                The request object. The request for
+                [Datastore.RunAggregationQuery][google.datastore.v1.Datastore.RunAggregationQuery].
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.datastore_v1.types.RunAggregationQueryResponse:
+                The response for
+                [Datastore.RunAggregationQuery][google.datastore.v1.Datastore.RunAggregationQuery].
+
+        """
+        # Create or coerce a protobuf request object.
+        request = datastore.RunAggregationQueryRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.run_aggregation_query,
+            default_retry=retries.Retry(
+                initial=0.1,
+                maximum=60.0,
+                multiplier=1.3,
+                predicate=retries.if_exception_type(
+                    core_exceptions.DeadlineExceeded,
+                    core_exceptions.ServiceUnavailable,
+                ),
+                deadline=60.0,
+            ),
+            default_timeout=60.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -406,27 +530,34 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.BeginTransactionResponse:
         r"""Begins a new transaction.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
-            def sample_begin_transaction():
+            async def sample_begin_transaction():
                 # Create a client
-                client = datastore_v1.DatastoreClient()
+                client = datastore_v1.DatastoreAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_v1.BeginTransactionRequest(
                     project_id="project_id_value",
                 )
 
                 # Make the request
-                response = client.begin_transaction(request=request)
+                response = await client.begin_transaction(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_v1.types.BeginTransactionRequest, dict]):
                 The request object. The request for
@@ -471,14 +602,22 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.begin_transaction,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -499,28 +638,35 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.CommitResponse:
         r"""Commits a transaction, optionally creating, deleting
         or modifying some entities.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
-            def sample_commit():
+            async def sample_commit():
                 # Create a client
-                client = datastore_v1.DatastoreClient()
+                client = datastore_v1.DatastoreAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_v1.CommitRequest(
                     transaction=b'transaction_blob',
                     project_id="project_id_value",
                 )
 
                 # Make the request
-                response = client.commit(request=request)
+                response = await client.commit(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_v1.types.CommitRequest, dict]):
                 The request object. The request for
@@ -606,14 +752,22 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.commit,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -631,28 +785,35 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.RollbackResponse:
         r"""Rolls back a transaction.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
-            def sample_rollback():
+            async def sample_rollback():
                 # Create a client
-                client = datastore_v1.DatastoreClient()
+                client = datastore_v1.DatastoreAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_v1.RollbackRequest(
                     project_id="project_id_value",
                     transaction=b'transaction_blob',
                 )
 
                 # Make the request
-                response = client.rollback(request=request)
+                response = await client.rollback(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_v1.types.RollbackRequest, dict]):
                 The request object. The request for
@@ -707,14 +868,22 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.rollback,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -733,27 +902,34 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.AllocateIdsResponse:
         r"""Allocates IDs for the given keys, which is useful for
         referencing an entity before it is inserted.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
-            def sample_allocate_ids():
+            async def sample_allocate_ids():
                 # Create a client
-                client = datastore_v1.DatastoreClient()
+                client = datastore_v1.DatastoreAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_v1.AllocateIdsRequest(
                     project_id="project_id_value",
                 )
 
                 # Make the request
-                response = client.allocate_ids(request=request)
+                response = await client.allocate_ids(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_v1.types.AllocateIdsRequest, dict]):
                 The request object. The request for
@@ -809,14 +985,22 @@
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.allocate_ids,
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -835,27 +1019,34 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.ReserveIdsResponse:
         r"""Prevents the supplied keys' IDs from being
         auto-allocated by Cloud Datastore.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
-            def sample_reserve_ids():
+            async def sample_reserve_ids():
                 # Create a client
-                client = datastore_v1.DatastoreClient()
+                client = datastore_v1.DatastoreAsyncClient()
 
                 # Initialize request argument(s)
                 request = datastore_v1.ReserveIdsRequest(
                     project_id="project_id_value",
                 )
 
                 # Make the request
-                response = client.reserve_ids(request=request)
+                response = await client.reserve_ids(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.datastore_v1.types.ReserveIdsRequest, dict]):
                 The request object. The request for
@@ -920,25 +1111,250 @@
                 ),
                 deadline=60.0,
             ),
             default_timeout=60.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    async def list_operations(
+        self,
+        request: operations_pb2.ListOperationsRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.ListOperationsResponse:
+        r"""Lists operations that match the specified filter in the request.
+
+        Args:
+            request (:class:`~.operations_pb2.ListOperationsRequest`):
+                The request object. Request message for
+                `ListOperations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.ListOperationsResponse:
+                Response message for ``ListOperations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.ListOperationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_operations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_operation(
+        self,
+        request: operations_pb2.GetOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.Operation:
+        r"""Gets the latest state of a long-running operation.
+
+        Args:
+            request (:class:`~.operations_pb2.GetOperationRequest`):
+                The request object. Request message for
+                `GetOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.Operation:
+                An ``Operation`` object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.GetOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def delete_operation(
+        self,
+        request: operations_pb2.DeleteOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Deletes a long-running operation.
+
+        This method indicates that the client is no longer interested
+        in the operation result. It does not cancel the operation.
+        If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.DeleteOperationRequest`):
+                The request object. Request message for
+                `DeleteOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.DeleteOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.delete_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    async def cancel_operation(
+        self,
+        request: operations_pb2.CancelOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Starts asynchronous cancellation on a long-running operation.
+
+        The server makes a best effort to cancel the operation, but success
+        is not guaranteed.  If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.CancelOperationRequest`):
+                The request object. Request message for
+                `CancelOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.CancelOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.cancel_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/client.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 from google.oauth2 import service_account  # type: ignore
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.datastore_v1.types import aggregation_result
 from google.cloud.datastore_v1.types import datastore
 from google.cloud.datastore_v1.types import entity
 from google.cloud.datastore_v1.types import query
+from google.longrunning import operations_pb2
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import DatastoreTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import DatastoreGrpcTransport
 from .transports.grpc_asyncio import DatastoreGrpcAsyncIOTransport
 
 
 class DatastoreClientMeta(type):
@@ -405,14 +407,15 @@
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
                 quota_project_id=client_options.quota_project_id,
                 client_info=client_info,
                 always_use_jwt_access=True,
+                api_audience=client_options.api_audience,
             )
 
     def lookup(
         self,
         request: Union[datastore.LookupRequest, dict] = None,
         *,
         project_id: str = None,
@@ -422,14 +425,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.LookupResponse:
         r"""Looks up entities by key.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
             def sample_lookup():
                 # Create a client
                 client = datastore_v1.DatastoreClient()
 
                 # Initialize request argument(s)
@@ -503,14 +513,22 @@
             if keys is not None:
                 request.keys = keys
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.lookup]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -526,14 +544,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.RunQueryResponse:
         r"""Queries for entities.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
             def sample_run_query():
                 # Create a client
                 client = datastore_v1.DatastoreClient()
 
                 # Initialize request argument(s)
@@ -571,14 +596,105 @@
         if not isinstance(request, datastore.RunQueryRequest):
             request = datastore.RunQueryRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.run_query]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def run_aggregation_query(
+        self,
+        request: Union[datastore.RunAggregationQueryRequest, dict] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> datastore.RunAggregationQueryResponse:
+        r"""Runs an aggregation query.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import datastore_v1
+
+            def sample_run_aggregation_query():
+                # Create a client
+                client = datastore_v1.DatastoreClient()
+
+                # Initialize request argument(s)
+                request = datastore_v1.RunAggregationQueryRequest(
+                    project_id="project_id_value",
+                )
+
+                # Make the request
+                response = client.run_aggregation_query(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.datastore_v1.types.RunAggregationQueryRequest, dict]):
+                The request object. The request for
+                [Datastore.RunAggregationQuery][google.datastore.v1.Datastore.RunAggregationQuery].
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.datastore_v1.types.RunAggregationQueryResponse:
+                The response for
+                [Datastore.RunAggregationQuery][google.datastore.v1.Datastore.RunAggregationQuery].
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a datastore.RunAggregationQueryRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, datastore.RunAggregationQueryRequest):
+            request = datastore.RunAggregationQueryRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.run_aggregation_query]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -595,14 +711,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.BeginTransactionResponse:
         r"""Begins a new transaction.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
             def sample_begin_transaction():
                 # Create a client
                 client = datastore_v1.DatastoreClient()
 
                 # Initialize request argument(s)
@@ -660,14 +783,22 @@
             if project_id is not None:
                 request.project_id = project_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.begin_transaction]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -688,14 +819,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.CommitResponse:
         r"""Commits a transaction, optionally creating, deleting
         or modifying some entities.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
             def sample_commit():
                 # Create a client
                 client = datastore_v1.DatastoreClient()
 
                 # Initialize request argument(s)
@@ -795,14 +933,22 @@
             if mutations is not None:
                 request.mutations = mutations
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.commit]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -820,14 +966,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.RollbackResponse:
         r"""Rolls back a transaction.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
             def sample_rollback():
                 # Create a client
                 client = datastore_v1.DatastoreClient()
 
                 # Initialize request argument(s)
@@ -896,14 +1049,22 @@
             if transaction is not None:
                 request.transaction = transaction
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.rollback]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -922,14 +1083,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.AllocateIdsResponse:
         r"""Allocates IDs for the given keys, which is useful for
         referencing an entity before it is inserted.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
             def sample_allocate_ids():
                 # Create a client
                 client = datastore_v1.DatastoreClient()
 
                 # Initialize request argument(s)
@@ -998,14 +1166,22 @@
             if keys is not None:
                 request.keys = keys
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.allocate_ids]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -1024,14 +1200,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> datastore.ReserveIdsResponse:
         r"""Prevents the supplied keys' IDs from being
         auto-allocated by Cloud Datastore.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import datastore_v1
 
             def sample_reserve_ids():
                 # Create a client
                 client = datastore_v1.DatastoreClient()
 
                 # Initialize request argument(s)
@@ -1099,14 +1282,22 @@
             if keys is not None:
                 request.keys = keys
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.reserve_ids]
 
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("project_id", request.project_id),)
+            ),
+        )
+
         # Send the request.
         response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
@@ -1123,14 +1314,231 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def list_operations(
+        self,
+        request: operations_pb2.ListOperationsRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.ListOperationsResponse:
+        r"""Lists operations that match the specified filter in the request.
+
+        Args:
+            request (:class:`~.operations_pb2.ListOperationsRequest`):
+                The request object. Request message for
+                `ListOperations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.ListOperationsResponse:
+                Response message for ``ListOperations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.ListOperationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_operations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def get_operation(
+        self,
+        request: operations_pb2.GetOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.Operation:
+        r"""Gets the latest state of a long-running operation.
+
+        Args:
+            request (:class:`~.operations_pb2.GetOperationRequest`):
+                The request object. Request message for
+                `GetOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.Operation:
+                An ``Operation`` object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.GetOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def delete_operation(
+        self,
+        request: operations_pb2.DeleteOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Deletes a long-running operation.
+
+        This method indicates that the client is no longer interested
+        in the operation result. It does not cancel the operation.
+        If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.DeleteOperationRequest`):
+                The request object. Request message for
+                `DeleteOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.DeleteOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.delete_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    def cancel_operation(
+        self,
+        request: operations_pb2.CancelOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Starts asynchronous cancellation on a long-running operation.
+
+        The server makes a best effort to cancel the operation, but success
+        is not guaranteed.  If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.CancelOperationRequest`):
+                The request object. Request message for
+                `CancelOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.CancelOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.cancel_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
 
 try:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
         gapic_version=pkg_resources.get_distribution(
             "google-cloud-datastore",
         ).version,
     )
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/base.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.datastore_v1.types import datastore
+from google.longrunning import operations_pb2
 
 try:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
         gapic_version=pkg_resources.get_distribution(
             "google-cloud-datastore",
         ).version,
     )
@@ -53,14 +54,15 @@
         host: str = DEFAULT_HOST,
         credentials: ga_credentials.Credentials = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
         **kwargs,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
@@ -80,19 +82,14 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
 
-        # Save the hostname. Default to port 443 (HTTPS) if none is specified.
-        if ":" not in host:
-            host += ":443"
-        self._host = host
-
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
         # Save the scopes.
         self._scopes = scopes
 
         # If no credentials are provided, then determine the appropriate
         # defaults.
@@ -105,26 +102,36 @@
             credentials, _ = google.auth.load_credentials_from_file(
                 credentials_file, **scopes_kwargs, quota_project_id=quota_project_id
             )
         elif credentials is None:
             credentials, _ = google.auth.default(
                 **scopes_kwargs, quota_project_id=quota_project_id
             )
+            # Don't apply audience if the credentials file passed from user.
+            if hasattr(credentials, "with_gdch_audience"):
+                credentials = credentials.with_gdch_audience(
+                    api_audience if api_audience else host
+                )
 
         # If the credentials are service account credentials, then always try to use self signed JWT.
         if (
             always_use_jwt_access
             and isinstance(credentials, service_account.Credentials)
             and hasattr(service_account.Credentials, "with_always_use_jwt_access")
         ):
             credentials = credentials.with_always_use_jwt_access(True)
 
         # Save the credentials.
         self._credentials = credentials
 
+        # Save the hostname. Default to port 443 (HTTPS) if none is specified.
+        if ":" not in host:
+            host += ":443"
+        self._host = host
+
     def _prep_wrapped_messages(self, client_info):
         # Precompute the wrapped methods.
         self._wrapped_methods = {
             self.lookup: gapic_v1.method.wrap_method(
                 self.lookup,
                 default_retry=retries.Retry(
                     initial=0.1,
@@ -150,14 +157,29 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=60.0,
                 ),
                 default_timeout=60.0,
                 client_info=client_info,
             ),
+            self.run_aggregation_query: gapic_v1.method.wrap_method(
+                self.run_aggregation_query,
+                default_retry=retries.Retry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
             self.begin_transaction: gapic_v1.method.wrap_method(
                 self.begin_transaction,
                 default_timeout=60.0,
                 client_info=client_info,
             ),
             self.commit: gapic_v1.method.wrap_method(
                 self.commit,
@@ -215,14 +237,26 @@
     ) -> Callable[
         [datastore.RunQueryRequest],
         Union[datastore.RunQueryResponse, Awaitable[datastore.RunQueryResponse]],
     ]:
         raise NotImplementedError()
 
     @property
+    def run_aggregation_query(
+        self,
+    ) -> Callable[
+        [datastore.RunAggregationQueryRequest],
+        Union[
+            datastore.RunAggregationQueryResponse,
+            Awaitable[datastore.RunAggregationQueryResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def begin_transaction(
         self,
     ) -> Callable[
         [datastore.BeginTransactionRequest],
         Union[
             datastore.BeginTransactionResponse,
             Awaitable[datastore.BeginTransactionResponse],
@@ -263,12 +297,45 @@
     ) -> Callable[
         [datastore.ReserveIdsRequest],
         Union[datastore.ReserveIdsResponse, Awaitable[datastore.ReserveIdsResponse]],
     ]:
         raise NotImplementedError()
 
     @property
+    def list_operations(
+        self,
+    ) -> Callable[
+        [operations_pb2.ListOperationsRequest],
+        Union[
+            operations_pb2.ListOperationsResponse,
+            Awaitable[operations_pb2.ListOperationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def get_operation(
+        self,
+    ) -> Callable[
+        [operations_pb2.GetOperationRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def cancel_operation(
+        self,
+    ) -> Callable[[operations_pb2.CancelOperationRequest], None,]:
+        raise NotImplementedError()
+
+    @property
+    def delete_operation(
+        self,
+    ) -> Callable[[operations_pb2.DeleteOperationRequest], None,]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("DatastoreTransport",)
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/grpc.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/grpc.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.datastore_v1.types import datastore
+from google.longrunning import operations_pb2
 from .base import DatastoreTransport, DEFAULT_CLIENT_INFO
 
 
 class DatastoreGrpcTransport(DatastoreTransport):
     """gRPC backend transport for Datastore.
 
     Each RPC normalizes the partition IDs of the keys in its
@@ -60,14 +61,15 @@
         api_mtls_endpoint: str = None,
         client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
         ssl_channel_credentials: grpc.ChannelCredentials = None,
         client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
             credentials (Optional[google.auth.credentials.Credentials]): The
@@ -155,14 +157,15 @@
             host=host,
             credentials=credentials,
             credentials_file=credentials_file,
             scopes=scopes,
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
+            api_audience=api_audience,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
@@ -280,14 +283,42 @@
                 "/google.datastore.v1.Datastore/RunQuery",
                 request_serializer=datastore.RunQueryRequest.serialize,
                 response_deserializer=datastore.RunQueryResponse.deserialize,
             )
         return self._stubs["run_query"]
 
     @property
+    def run_aggregation_query(
+        self,
+    ) -> Callable[
+        [datastore.RunAggregationQueryRequest], datastore.RunAggregationQueryResponse
+    ]:
+        r"""Return a callable for the run aggregation query method over gRPC.
+
+        Runs an aggregation query.
+
+        Returns:
+            Callable[[~.RunAggregationQueryRequest],
+                    ~.RunAggregationQueryResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "run_aggregation_query" not in self._stubs:
+            self._stubs["run_aggregation_query"] = self.grpc_channel.unary_unary(
+                "/google.datastore.v1.Datastore/RunAggregationQuery",
+                request_serializer=datastore.RunAggregationQueryRequest.serialize,
+                response_deserializer=datastore.RunAggregationQueryResponse.deserialize,
+            )
+        return self._stubs["run_aggregation_query"]
+
+    @property
     def begin_transaction(
         self,
     ) -> Callable[
         [datastore.BeginTransactionRequest], datastore.BeginTransactionResponse
     ]:
         r"""Return a callable for the begin transaction method over gRPC.
 
@@ -416,12 +447,82 @@
             )
         return self._stubs["reserve_ids"]
 
     def close(self):
         self.grpc_channel.close()
 
     @property
+    def delete_operation(
+        self,
+    ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
+        r"""Return a callable for the delete_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_operation" not in self._stubs:
+            self._stubs["delete_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/DeleteOperation",
+                request_serializer=operations_pb2.DeleteOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["delete_operation"]
+
+    @property
+    def cancel_operation(
+        self,
+    ) -> Callable[[operations_pb2.CancelOperationRequest], None]:
+        r"""Return a callable for the cancel_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "cancel_operation" not in self._stubs:
+            self._stubs["cancel_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/CancelOperation",
+                request_serializer=operations_pb2.CancelOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["cancel_operation"]
+
+    @property
+    def get_operation(
+        self,
+    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
+        r"""Return a callable for the get_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_operation" not in self._stubs:
+            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/GetOperation",
+                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["get_operation"]
+
+    @property
+    def list_operations(
+        self,
+    ) -> Callable[
+        [operations_pb2.ListOperationsRequest], operations_pb2.ListOperationsResponse
+    ]:
+        r"""Return a callable for the list_operations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_operations" not in self._stubs:
+            self._stubs["list_operations"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/ListOperations",
+                request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
+                response_deserializer=operations_pb2.ListOperationsResponse.FromString,
+            )
+        return self._stubs["list_operations"]
+
+    @property
     def kind(self) -> str:
         return "grpc"
 
 
 __all__ = ("DatastoreGrpcTransport",)
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/services/datastore/transports/grpc_asyncio.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/services/datastore/transports/grpc_asyncio.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.datastore_v1.types import datastore
+from google.longrunning import operations_pb2
 from .base import DatastoreTransport, DEFAULT_CLIENT_INFO
 from .grpc import DatastoreGrpcTransport
 
 
 class DatastoreGrpcAsyncIOTransport(DatastoreTransport):
     """gRPC AsyncIO backend transport for Datastore.
 
@@ -105,14 +106,15 @@
         api_mtls_endpoint: str = None,
         client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
         ssl_channel_credentials: grpc.ChannelCredentials = None,
         client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
         quota_project_id=None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
             credentials (Optional[google.auth.credentials.Credentials]): The
@@ -200,14 +202,15 @@
             host=host,
             credentials=credentials,
             credentials_file=credentials_file,
             scopes=scopes,
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
+            api_audience=api_audience,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
@@ -285,14 +288,43 @@
                 "/google.datastore.v1.Datastore/RunQuery",
                 request_serializer=datastore.RunQueryRequest.serialize,
                 response_deserializer=datastore.RunQueryResponse.deserialize,
             )
         return self._stubs["run_query"]
 
     @property
+    def run_aggregation_query(
+        self,
+    ) -> Callable[
+        [datastore.RunAggregationQueryRequest],
+        Awaitable[datastore.RunAggregationQueryResponse],
+    ]:
+        r"""Return a callable for the run aggregation query method over gRPC.
+
+        Runs an aggregation query.
+
+        Returns:
+            Callable[[~.RunAggregationQueryRequest],
+                    Awaitable[~.RunAggregationQueryResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "run_aggregation_query" not in self._stubs:
+            self._stubs["run_aggregation_query"] = self.grpc_channel.unary_unary(
+                "/google.datastore.v1.Datastore/RunAggregationQuery",
+                request_serializer=datastore.RunAggregationQueryRequest.serialize,
+                response_deserializer=datastore.RunAggregationQueryResponse.deserialize,
+            )
+        return self._stubs["run_aggregation_query"]
+
+    @property
     def begin_transaction(
         self,
     ) -> Callable[
         [datastore.BeginTransactionRequest],
         Awaitable[datastore.BeginTransactionResponse],
     ]:
         r"""Return a callable for the begin transaction method over gRPC.
@@ -427,9 +459,79 @@
                 response_deserializer=datastore.ReserveIdsResponse.deserialize,
             )
         return self._stubs["reserve_ids"]
 
     def close(self):
         return self.grpc_channel.close()
 
+    @property
+    def delete_operation(
+        self,
+    ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
+        r"""Return a callable for the delete_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_operation" not in self._stubs:
+            self._stubs["delete_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/DeleteOperation",
+                request_serializer=operations_pb2.DeleteOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["delete_operation"]
+
+    @property
+    def cancel_operation(
+        self,
+    ) -> Callable[[operations_pb2.CancelOperationRequest], None]:
+        r"""Return a callable for the cancel_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "cancel_operation" not in self._stubs:
+            self._stubs["cancel_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/CancelOperation",
+                request_serializer=operations_pb2.CancelOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["cancel_operation"]
+
+    @property
+    def get_operation(
+        self,
+    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
+        r"""Return a callable for the get_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_operation" not in self._stubs:
+            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/GetOperation",
+                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["get_operation"]
+
+    @property
+    def list_operations(
+        self,
+    ) -> Callable[
+        [operations_pb2.ListOperationsRequest], operations_pb2.ListOperationsResponse
+    ]:
+        r"""Return a callable for the list_operations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_operations" not in self._stubs:
+            self._stubs["list_operations"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/ListOperations",
+                request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
+                response_deserializer=operations_pb2.ListOperationsResponse.FromString,
+            )
+        return self._stubs["list_operations"]
+
 
 __all__ = ("DatastoreGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/__init__.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from .aggregation_result import (
+    AggregationResult,
+    AggregationResultBatch,
+)
 from .datastore import (
     AllocateIdsRequest,
     AllocateIdsResponse,
     BeginTransactionRequest,
     BeginTransactionResponse,
     CommitRequest,
     CommitResponse,
@@ -25,26 +29,29 @@
     Mutation,
     MutationResult,
     ReadOptions,
     ReserveIdsRequest,
     ReserveIdsResponse,
     RollbackRequest,
     RollbackResponse,
+    RunAggregationQueryRequest,
+    RunAggregationQueryResponse,
     RunQueryRequest,
     RunQueryResponse,
     TransactionOptions,
 )
 from .entity import (
     ArrayValue,
     Entity,
     Key,
     PartitionId,
     Value,
 )
 from .query import (
+    AggregationQuery,
     CompositeFilter,
     EntityResult,
     Filter,
     GqlQuery,
     GqlQueryParameter,
     KindExpression,
     Projection,
@@ -52,14 +59,16 @@
     PropertyOrder,
     PropertyReference,
     Query,
     QueryResultBatch,
 )
 
 __all__ = (
+    "AggregationResult",
+    "AggregationResultBatch",
     "AllocateIdsRequest",
     "AllocateIdsResponse",
     "BeginTransactionRequest",
     "BeginTransactionResponse",
     "CommitRequest",
     "CommitResponse",
     "LookupRequest",
@@ -67,22 +76,25 @@
     "Mutation",
     "MutationResult",
     "ReadOptions",
     "ReserveIdsRequest",
     "ReserveIdsResponse",
     "RollbackRequest",
     "RollbackResponse",
+    "RunAggregationQueryRequest",
+    "RunAggregationQueryResponse",
     "RunQueryRequest",
     "RunQueryResponse",
     "TransactionOptions",
     "ArrayValue",
     "Entity",
     "Key",
     "PartitionId",
     "Value",
+    "AggregationQuery",
     "CompositeFilter",
     "EntityResult",
     "Filter",
     "GqlQuery",
     "GqlQueryParameter",
     "KindExpression",
     "Projection",
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/datastore.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/datastore.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import proto  # type: ignore
 
+from google.cloud.datastore_v1.types import aggregation_result
 from google.cloud.datastore_v1.types import entity
 from google.cloud.datastore_v1.types import query as gd_query
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.datastore.v1",
     manifest={
         "LookupRequest",
         "LookupResponse",
         "RunQueryRequest",
         "RunQueryResponse",
+        "RunAggregationQueryRequest",
+        "RunAggregationQueryResponse",
         "BeginTransactionRequest",
         "BeginTransactionResponse",
         "RollbackRequest",
         "RollbackResponse",
         "CommitRequest",
         "CommitResponse",
         "AllocateIdsRequest",
@@ -49,24 +52,33 @@
     r"""The request for
     [Datastore.Lookup][google.datastore.v1.Datastore.Lookup].
 
     Attributes:
         project_id (str):
             Required. The ID of the project against which
             to make the request.
+        database_id (str):
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
         read_options (google.cloud.datastore_v1.types.ReadOptions):
             The options for this lookup request.
         keys (Sequence[google.cloud.datastore_v1.types.Key]):
             Required. Keys of entities to look up.
     """
 
     project_id = proto.Field(
         proto.STRING,
         number=8,
     )
+    database_id = proto.Field(
+        proto.STRING,
+        number=9,
+    )
     read_options = proto.Field(
         proto.MESSAGE,
         number=1,
         message="ReadOptions",
     )
     keys = proto.RepeatedField(
         proto.MESSAGE,
@@ -131,36 +143,46 @@
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         project_id (str):
             Required. The ID of the project against which
             to make the request.
+        database_id (str):
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
         partition_id (google.cloud.datastore_v1.types.PartitionId):
             Entities are partitioned into subsets,
             identified by a partition ID. Queries are scoped
             to a single partition. This partition ID is
             normalized with the standard default context
             partition ID.
         read_options (google.cloud.datastore_v1.types.ReadOptions):
             The options for this query.
         query (google.cloud.datastore_v1.types.Query):
             The query to run.
 
             This field is a member of `oneof`_ ``query_type``.
         gql_query (google.cloud.datastore_v1.types.GqlQuery):
-            The GQL query to run.
+            The GQL query to run. This query must be a
+            non-aggregation query.
 
             This field is a member of `oneof`_ ``query_type``.
     """
 
     project_id = proto.Field(
         proto.STRING,
         number=8,
     )
+    database_id = proto.Field(
+        proto.STRING,
+        number=9,
+    )
     partition_id = proto.Field(
         proto.MESSAGE,
         number=2,
         message=entity.PartitionId,
     )
     read_options = proto.Field(
         proto.MESSAGE,
@@ -201,30 +223,135 @@
     query = proto.Field(
         proto.MESSAGE,
         number=2,
         message=gd_query.Query,
     )
 
 
+class RunAggregationQueryRequest(proto.Message):
+    r"""The request for
+    [Datastore.RunAggregationQuery][google.datastore.v1.Datastore.RunAggregationQuery].
+
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        project_id (str):
+            Required. The ID of the project against which
+            to make the request.
+        database_id (str):
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
+        partition_id (google.cloud.datastore_v1.types.PartitionId):
+            Entities are partitioned into subsets,
+            identified by a partition ID. Queries are scoped
+            to a single partition. This partition ID is
+            normalized with the standard default context
+            partition ID.
+        read_options (google.cloud.datastore_v1.types.ReadOptions):
+            The options for this query.
+        aggregation_query (google.cloud.datastore_v1.types.AggregationQuery):
+            The query to run.
+
+            This field is a member of `oneof`_ ``query_type``.
+        gql_query (google.cloud.datastore_v1.types.GqlQuery):
+            The GQL query to run. This query must be an
+            aggregation query.
+
+            This field is a member of `oneof`_ ``query_type``.
+    """
+
+    project_id = proto.Field(
+        proto.STRING,
+        number=8,
+    )
+    database_id = proto.Field(
+        proto.STRING,
+        number=9,
+    )
+    partition_id = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=entity.PartitionId,
+    )
+    read_options = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message="ReadOptions",
+    )
+    aggregation_query = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        oneof="query_type",
+        message=gd_query.AggregationQuery,
+    )
+    gql_query = proto.Field(
+        proto.MESSAGE,
+        number=7,
+        oneof="query_type",
+        message=gd_query.GqlQuery,
+    )
+
+
+class RunAggregationQueryResponse(proto.Message):
+    r"""The response for
+    [Datastore.RunAggregationQuery][google.datastore.v1.Datastore.RunAggregationQuery].
+
+    Attributes:
+        batch (google.cloud.datastore_v1.types.AggregationResultBatch):
+            A batch of aggregation results. Always
+            present.
+        query (google.cloud.datastore_v1.types.AggregationQuery):
+            The parsed form of the ``GqlQuery`` from the request, if it
+            was set.
+    """
+
+    batch = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=aggregation_result.AggregationResultBatch,
+    )
+    query = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=gd_query.AggregationQuery,
+    )
+
+
 class BeginTransactionRequest(proto.Message):
     r"""The request for
     [Datastore.BeginTransaction][google.datastore.v1.Datastore.BeginTransaction].
 
     Attributes:
         project_id (str):
             Required. The ID of the project against which
             to make the request.
+        database_id (str):
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
         transaction_options (google.cloud.datastore_v1.types.TransactionOptions):
             Options for a new transaction.
     """
 
     project_id = proto.Field(
         proto.STRING,
         number=8,
     )
+    database_id = proto.Field(
+        proto.STRING,
+        number=9,
+    )
     transaction_options = proto.Field(
         proto.MESSAGE,
         number=10,
         message="TransactionOptions",
     )
 
 
@@ -247,23 +374,32 @@
     r"""The request for
     [Datastore.Rollback][google.datastore.v1.Datastore.Rollback].
 
     Attributes:
         project_id (str):
             Required. The ID of the project against which
             to make the request.
+        database_id (str):
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
         transaction (bytes):
             Required. The transaction identifier, returned by a call to
             [Datastore.BeginTransaction][google.datastore.v1.Datastore.BeginTransaction].
     """
 
     project_id = proto.Field(
         proto.STRING,
         number=8,
     )
+    database_id = proto.Field(
+        proto.STRING,
+        number=9,
+    )
     transaction = proto.Field(
         proto.BYTES,
         number=1,
     )
 
 
 class RollbackResponse(proto.Message):
@@ -281,14 +417,19 @@
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         project_id (str):
             Required. The ID of the project against which
             to make the request.
+        database_id (str):
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
         mode (google.cloud.datastore_v1.types.CommitRequest.Mode):
             The type of commit to perform. Defaults to
             ``TRANSACTIONAL``.
         transaction (bytes):
             The identifier of the transaction associated with the
             commit. A transaction identifier is returned by a call to
             [Datastore.BeginTransaction][google.datastore.v1.Datastore.BeginTransaction].
@@ -317,14 +458,18 @@
         TRANSACTIONAL = 1
         NON_TRANSACTIONAL = 2
 
     project_id = proto.Field(
         proto.STRING,
         number=8,
     )
+    database_id = proto.Field(
+        proto.STRING,
+        number=9,
+    )
     mode = proto.Field(
         proto.ENUM,
         number=5,
         enum=Mode,
     )
     transaction = proto.Field(
         proto.BYTES,
@@ -375,24 +520,33 @@
     r"""The request for
     [Datastore.AllocateIds][google.datastore.v1.Datastore.AllocateIds].
 
     Attributes:
         project_id (str):
             Required. The ID of the project against which
             to make the request.
+        database_id (str):
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
         keys (Sequence[google.cloud.datastore_v1.types.Key]):
             Required. A list of keys with incomplete key
             paths for which to allocate IDs. No key may be
             reserved/read-only.
     """
 
     project_id = proto.Field(
         proto.STRING,
         number=8,
     )
+    database_id = proto.Field(
+        proto.STRING,
+        number=9,
+    )
     keys = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=entity.Key,
     )
 
 
@@ -419,16 +573,18 @@
     [Datastore.ReserveIds][google.datastore.v1.Datastore.ReserveIds].
 
     Attributes:
         project_id (str):
             Required. The ID of the project against which
             to make the request.
         database_id (str):
-            If not empty, the ID of the database against
-            which to make the request.
+            The ID of the database against which to make
+            the request.
+            '(default)' is not allowed; please use empty
+            string '' to refer the default database.
         keys (Sequence[google.cloud.datastore_v1.types.Key]):
             Required. A list of keys with complete key
             paths whose numeric IDs should not be
             auto-allocated.
     """
 
     project_id = proto.Field(
@@ -598,16 +754,16 @@
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         read_consistency (google.cloud.datastore_v1.types.ReadOptions.ReadConsistency):
-            The non-transactional read consistency to use. Cannot be set
-            to ``STRONG`` for global queries.
+            The non-transactional read consistency to
+            use.
 
             This field is a member of `oneof`_ ``consistency_type``.
         transaction (bytes):
             The identifier of the transaction in which to read. A
             transaction identifier is returned by a call to
             [Datastore.BeginTransaction][google.datastore.v1.Datastore.BeginTransaction].
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/entity.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,23 +53,30 @@
     context project ID ) are discouraged. Reads and writes of foreign
     partition IDs may fail if the project is not in an active state.
 
     Attributes:
         project_id (str):
             The ID of the project to which the entities
             belong.
+        database_id (str):
+            If not empty, the ID of the database to which
+            the entities belong.
         namespace_id (str):
             If not empty, the ID of the namespace to
             which the entities belong.
     """
 
     project_id = proto.Field(
         proto.STRING,
         number=2,
     )
+    database_id = proto.Field(
+        proto.STRING,
+        number=3,
+    )
     namespace_id = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class Key(proto.Message):
@@ -117,28 +124,40 @@
         Setting any member of the oneof automatically clears all other
         members.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
             kind (str):
-                The kind of the entity. A kind matching regex ``__.*__`` is
-                reserved/read-only. A kind must not contain more than 1500
-                bytes when UTF-8 encoded. Cannot be ``""``.
+                The kind of the entity.
+
+                A kind matching regex ``__.*__`` is reserved/read-only. A
+                kind must not contain more than 1500 bytes when UTF-8
+                encoded. Cannot be ``""``.
+
+                Must be valid UTF-8 bytes. Legacy values that are not valid
+                UTF-8 are encoded as ``__bytes<X>__`` where ``<X>`` is the
+                base-64 encoding of the bytes.
             id (int):
                 The auto-allocated ID of the entity.
                 Never equal to zero. Values less than zero are
                 discouraged and may not be supported in the
                 future.
 
                 This field is a member of `oneof`_ ``id_type``.
             name (str):
-                The name of the entity. A name matching regex ``__.*__`` is
-                reserved/read-only. A name must not be more than 1500 bytes
-                when UTF-8 encoded. Cannot be ``""``.
+                The name of the entity.
+
+                A name matching regex ``__.*__`` is reserved/read-only. A
+                name must not be more than 1500 bytes when UTF-8 encoded.
+                Cannot be ``""``.
+
+                Must be valid UTF-8 bytes. Legacy values that are not valid
+                UTF-8 are encoded as ``__bytes<X>__`` where ``<X>`` is the
+                base-64 encoding of the bytes.
 
                 This field is a member of `oneof`_ ``id_type``.
         """
 
         kind = proto.Field(
             proto.STRING,
             number=1,
```

### Comparing `google-cloud-datastore-2.8.3/google/cloud/datastore_v1/types/query.py` & `google-cloud-datastore-2.9.0/google/cloud/datastore_v1/types/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 __protobuf__ = proto.module(
     package="google.datastore.v1",
     manifest={
         "EntityResult",
         "Query",
+        "AggregationQuery",
         "KindExpression",
         "PropertyReference",
         "Projection",
         "PropertyOrder",
         "Filter",
         "CompositeFilter",
         "PropertyFilter",
@@ -184,14 +185,145 @@
     limit = proto.Field(
         proto.MESSAGE,
         number=12,
         message=wrappers_pb2.Int32Value,
     )
 
 
+class AggregationQuery(proto.Message):
+    r"""Datastore query for running an aggregation over a
+    [Query][google.datastore.v1.Query].
+
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        nested_query (google.cloud.datastore_v1.types.Query):
+            Nested query for aggregation
+
+            This field is a member of `oneof`_ ``query_type``.
+        aggregations (Sequence[google.cloud.datastore_v1.types.AggregationQuery.Aggregation]):
+            Optional. Series of aggregations to apply over the results
+            of the ``nested_query``.
+
+            Requires:
+
+            -  A minimum of one and maximum of five aggregations per
+               query.
+    """
+
+    class Aggregation(proto.Message):
+        r"""Defines a aggregation that produces a single result.
+
+        .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+        Attributes:
+            count (google.cloud.datastore_v1.types.AggregationQuery.Aggregation.Count):
+                Count aggregator.
+
+                This field is a member of `oneof`_ ``operator``.
+            alias (str):
+                Optional. Optional name of the property to store the result
+                of the aggregation.
+
+                If not provided, Datastore will pick a default name
+                following the format ``property_<incremental_id++>``. For
+                example:
+
+                ::
+
+                   AGGREGATE
+                     COUNT_UP_TO(1) AS count_up_to_1,
+                     COUNT_UP_TO(2),
+                     COUNT_UP_TO(3) AS count_up_to_3,
+                     COUNT_UP_TO(4)
+                   OVER (
+                     ...
+                   );
+
+                becomes:
+
+                ::
+
+                   AGGREGATE
+                     COUNT_UP_TO(1) AS count_up_to_1,
+                     COUNT_UP_TO(2) AS property_1,
+                     COUNT_UP_TO(3) AS count_up_to_3,
+                     COUNT_UP_TO(4) AS property_2
+                   OVER (
+                     ...
+                   );
+
+                Requires:
+
+                -  Must be unique across all aggregation aliases.
+                -  Conform to [entity property
+                   name][google.datastore.v1.Entity.properties] limitations.
+        """
+
+        class Count(proto.Message):
+            r"""Count of entities that match the query.
+
+            The ``COUNT(*)`` aggregation function operates on the entire entity
+            so it does not require a field reference.
+
+            Attributes:
+                up_to (google.protobuf.wrappers_pb2.Int64Value):
+                    Optional. Optional constraint on the maximum number of
+                    entities to count.
+
+                    This provides a way to set an upper bound on the number of
+                    entities to scan, limiting latency and cost.
+
+                    Unspecified is interpreted as no bound.
+
+                    If a zero value is provided, a count result of zero should
+                    always be expected.
+
+                    High-Level Example:
+
+                    ::
+
+                       AGGREGATE COUNT_UP_TO(1000) OVER ( SELECT * FROM k );
+
+                    Requires:
+
+                    -  Must be non-negative when present.
+            """
+
+            up_to = proto.Field(
+                proto.MESSAGE,
+                number=1,
+                message=wrappers_pb2.Int64Value,
+            )
+
+        count = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            oneof="operator",
+            message="AggregationQuery.Aggregation.Count",
+        )
+        alias = proto.Field(
+            proto.STRING,
+            number=7,
+        )
+
+    nested_query = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        oneof="query_type",
+        message="Query",
+    )
+    aggregations = proto.RepeatedField(
+        proto.MESSAGE,
+        number=3,
+        message=Aggregation,
+    )
+
+
 class KindExpression(proto.Message):
     r"""A representation of a kind.
 
     Attributes:
         name (str):
             The name of the kind.
     """
@@ -301,15 +433,18 @@
     operator.
 
     Attributes:
         op (google.cloud.datastore_v1.types.CompositeFilter.Operator):
             The operator for combining multiple filters.
         filters (Sequence[google.cloud.datastore_v1.types.Filter]):
             The list of filters to combine.
-            Must contain at least one filter.
+
+            Requires:
+
+            -  At least one filter is present.
     """
 
     class Operator(proto.Enum):
         r"""A composite filter operator."""
         OPERATOR_UNSPECIFIED = 0
         AND = 1
```

### Comparing `google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/PKG-INFO` & `google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastore
-Version: 2.8.3
+Version: 2.9.0
 Summary: Google Cloud Datastore API client library
 Home-page: https://github.com/googleapis/python-datastore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datastore-2.8.3/google_cloud_datastore.egg-info/SOURCES.txt` & `google-cloud-datastore-2.9.0/google_cloud_datastore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 google/cloud/datastore_v1/services/datastore/async_client.py
 google/cloud/datastore_v1/services/datastore/client.py
 google/cloud/datastore_v1/services/datastore/transports/__init__.py
 google/cloud/datastore_v1/services/datastore/transports/base.py
 google/cloud/datastore_v1/services/datastore/transports/grpc.py
 google/cloud/datastore_v1/services/datastore/transports/grpc_asyncio.py
 google/cloud/datastore_v1/types/__init__.py
+google/cloud/datastore_v1/types/aggregation_result.py
 google/cloud/datastore_v1/types/datastore.py
 google/cloud/datastore_v1/types/entity.py
 google/cloud/datastore_v1/types/query.py
 google_cloud_datastore.egg-info/PKG-INFO
 google_cloud_datastore.egg-info/SOURCES.txt
 google_cloud_datastore.egg-info/dependency_links.txt
 google_cloud_datastore.egg-info/namespace_packages.txt
```

### Comparing `google-cloud-datastore-2.8.3/scripts/fixup_datastore_admin_v1_keywords.py` & `google-cloud-datastore-2.9.0/scripts/fixup_datastore_admin_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/scripts/fixup_datastore_v1_keywords.py` & `google-cloud-datastore-2.9.0/scripts/fixup_datastore_v1_keywords.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,21 +35,22 @@
     # Returns trueList, falseList
     return results[1], results[0]
 
 
 class datastoreCallTransformer(cst.CSTTransformer):
     CTRL_PARAMS: Tuple[str] = ('retry', 'timeout', 'metadata')
     METHOD_TO_PARAMS: Dict[str, Tuple[str]] = {
-        'allocate_ids': ('project_id', 'keys', ),
-        'begin_transaction': ('project_id', 'transaction_options', ),
-        'commit': ('project_id', 'mode', 'transaction', 'mutations', ),
-        'lookup': ('project_id', 'keys', 'read_options', ),
+        'allocate_ids': ('project_id', 'keys', 'database_id', ),
+        'begin_transaction': ('project_id', 'database_id', 'transaction_options', ),
+        'commit': ('project_id', 'database_id', 'mode', 'transaction', 'mutations', ),
+        'lookup': ('project_id', 'keys', 'database_id', 'read_options', ),
         'reserve_ids': ('project_id', 'keys', 'database_id', ),
-        'rollback': ('project_id', 'transaction', ),
-        'run_query': ('project_id', 'partition_id', 'read_options', 'query', 'gql_query', ),
+        'rollback': ('project_id', 'transaction', 'database_id', ),
+        'run_aggregation_query': ('project_id', 'database_id', 'partition_id', 'read_options', 'aggregation_query', 'gql_query', ),
+        'run_query': ('project_id', 'database_id', 'partition_id', 'read_options', 'query', 'gql_query', ),
     }
 
     def leave_Call(self, original: cst.Call, updated: cst.Call) -> cst.CSTNode:
         try:
             key = original.func.attr.value
             kword_params = self.METHOD_TO_PARAMS[key]
         except (AttributeError, KeyError):
```

### Comparing `google-cloud-datastore-2.8.3/setup.py` & `google-cloud-datastore-2.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,21 +25,15 @@
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
-    # NOTE: Maintainers, please do not require google-api-core>=2.x.x
-    # Until this issue is closed
-    # https://github.com/googleapis/google-cloud-python/issues/10566
-    "google-api-core[grpc] >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
-    # NOTE: Maintainers, please do not require google-api-core>=2.x.x
-    # Until this issue is closed
-    # https://github.com/googleapis/google-cloud-python/issues/10566
+    "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "google-cloud-core >= 1.4.0, <3.0.0dev",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 extras = {"libcst": "libcst >= 0.2.5"}
```

### Comparing `google-cloud-datastore-2.8.3/tests/__init__.py` & `google-cloud-datastore-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/doctests.py` & `google-cloud-datastore-2.9.0/tests/doctests.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/_helpers.py` & `google-cloud-datastore-2.9.0/tests/system/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/conftest.py` & `google-cloud-datastore-2.9.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/test_allocate_reserve_ids.py` & `google-cloud-datastore-2.9.0/tests/system/test_allocate_reserve_ids.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/test_put.py` & `google-cloud-datastore-2.9.0/tests/system/test_put.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/test_query.py` & `google-cloud-datastore-2.9.0/tests/system/test_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/test_read_consistency.py` & `google-cloud-datastore-2.9.0/tests/system/test_read_consistency.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/test_transaction.py` & `google-cloud-datastore-2.9.0/tests/system/test_transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/utils/clear_datastore.py` & `google-cloud-datastore-2.9.0/tests/system/utils/clear_datastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/system/utils/populate_datastore.py` & `google-cloud-datastore-2.9.0/tests/system/utils/populate_datastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/__init__.py` & `google-cloud-datastore-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/gapic/__init__.py` & `google-cloud-datastore-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_admin_v1/__init__.py` & `google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_admin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_admin_v1/test_datastore_admin.py` & `google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_admin_v1/test_datastore_admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,22 +10,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock  # pragma: NO COVER
+except ImportError:  # pragma: NO COVER
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
-
+from proto.marshal.rules import wrappers
 
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import future
 from google.api_core import gapic_v1
 from google.api_core import grpc_helpers
 from google.api_core import grpc_helpers_async
@@ -224,14 +230,15 @@
             credentials_file=None,
             host="squid.clam.whelk",
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT is
     # "never".
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "never"}):
         with mock.patch.object(transport_class, "__init__") as patched:
             patched.return_value = None
@@ -241,14 +248,15 @@
                 credentials_file=None,
                 host=client.DEFAULT_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT is
     # "always".
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "always"}):
         with mock.patch.object(transport_class, "__init__") as patched:
             patched.return_value = None
@@ -258,14 +266,15 @@
                 credentials_file=None,
                 host=client.DEFAULT_MTLS_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT has
     # unsupported value.
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "Unsupported"}):
         with pytest.raises(MutualTLSChannelError):
             client = client_class(transport=transport_name)
@@ -287,14 +296,33 @@
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id="octopus",
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
+        )
+    # Check the case api_endpoint is provided
+    options = client_options.ClientOptions(
+        api_audience="https://language.googleapis.com"
+    )
+    with mock.patch.object(transport_class, "__init__") as patched:
+        patched.return_value = None
+        client = client_class(client_options=options, transport=transport_name)
+        patched.assert_called_once_with(
+            credentials=None,
+            credentials_file=None,
+            host=client.DEFAULT_ENDPOINT,
+            scopes=None,
+            client_cert_source_for_mtls=None,
+            quota_project_id=None,
+            client_info=transports.base.DEFAULT_CLIENT_INFO,
+            always_use_jwt_access=True,
+            api_audience="https://language.googleapis.com",
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,use_client_cert_env",
     [
         (DatastoreAdminClient, transports.DatastoreAdminGrpcTransport, "grpc", "true"),
@@ -354,14 +382,15 @@
                 credentials_file=None,
                 host=expected_host,
                 scopes=None,
                 client_cert_source_for_mtls=expected_client_cert_source,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case ADC client cert is provided. Whether client cert is used depends on
     # GOOGLE_API_USE_CLIENT_CERTIFICATE value.
     with mock.patch.dict(
         os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": use_client_cert_env}
     ):
@@ -388,14 +417,15 @@
                         credentials_file=None,
                         host=expected_host,
                         scopes=None,
                         client_cert_source_for_mtls=expected_client_cert_source,
                         quota_project_id=None,
                         client_info=transports.base.DEFAULT_CLIENT_INFO,
                         always_use_jwt_access=True,
+                        api_audience=None,
                     )
 
     # Check the case client_cert_source and ADC client cert are not provided.
     with mock.patch.dict(
         os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": use_client_cert_env}
     ):
         with mock.patch.object(transport_class, "__init__") as patched:
@@ -410,14 +440,15 @@
                     credentials_file=None,
                     host=client.DEFAULT_ENDPOINT,
                     scopes=None,
                     client_cert_source_for_mtls=None,
                     quota_project_id=None,
                     client_info=transports.base.DEFAULT_CLIENT_INFO,
                     always_use_jwt_access=True,
+                    api_audience=None,
                 )
 
 
 @pytest.mark.parametrize(
     "client_class", [DatastoreAdminClient, DatastoreAdminAsyncClient]
 )
 @mock.patch.object(
@@ -524,14 +555,15 @@
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
             scopes=["1", "2"],
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,grpc_helpers",
     [
         (
@@ -562,14 +594,15 @@
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 def test_datastore_admin_client_client_options_from_dict():
     with mock.patch(
         "google.cloud.datastore_admin_v1.services.datastore_admin.transports.DatastoreAdminGrpcTransport.__init__"
     ) as grpc_transport:
@@ -582,14 +615,15 @@
             credentials_file=None,
             host="squid.clam.whelk",
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,grpc_helpers",
     [
         (
@@ -620,14 +654,15 @@
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
     # test that the credentials from file are saved and used as the credentials.
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch.object(
         google.auth, "default", autospec=True
@@ -737,14 +772,75 @@
 
 
 @pytest.mark.asyncio
 async def test_export_entities_async_from_dict():
     await test_export_entities_async(request_type=dict)
 
 
+def test_export_entities_field_headers():
+    client = DatastoreAdminClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.ExportEntitiesRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_entities), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.export_entities(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_export_entities_field_headers_async():
+    client = DatastoreAdminAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.ExportEntitiesRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_entities), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.export_entities(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_export_entities_flattened():
     client = DatastoreAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.export_entities), "__call__") as call:
@@ -932,14 +1028,75 @@
 
 
 @pytest.mark.asyncio
 async def test_import_entities_async_from_dict():
     await test_import_entities_async(request_type=dict)
 
 
+def test_import_entities_field_headers():
+    client = DatastoreAdminClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.ImportEntitiesRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_entities), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.import_entities(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_import_entities_field_headers_async():
+    client = DatastoreAdminAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.ImportEntitiesRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_entities), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.import_entities(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_import_entities_flattened():
     client = DatastoreAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.import_entities), "__call__") as call:
@@ -1127,14 +1284,75 @@
 
 
 @pytest.mark.asyncio
 async def test_create_index_async_from_dict():
     await test_create_index_async(request_type=dict)
 
 
+def test_create_index_field_headers():
+    client = DatastoreAdminClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.CreateIndexRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_index), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.create_index(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_create_index_field_headers_async():
+    client = DatastoreAdminAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.CreateIndexRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_index), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.create_index(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 @pytest.mark.parametrize(
     "request_type",
     [
         datastore_admin.DeleteIndexRequest,
         dict,
     ],
 )
@@ -1210,14 +1428,77 @@
 
 
 @pytest.mark.asyncio
 async def test_delete_index_async_from_dict():
     await test_delete_index_async(request_type=dict)
 
 
+def test_delete_index_field_headers():
+    client = DatastoreAdminClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.DeleteIndexRequest()
+
+    request.project_id = "project_id_value"
+    request.index_id = "index_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_index), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.delete_index(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value&index_id=index_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_delete_index_field_headers_async():
+    client = DatastoreAdminAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.DeleteIndexRequest()
+
+    request.project_id = "project_id_value"
+    request.index_id = "index_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_index), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.delete_index(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value&index_id=index_id_value",
+    ) in kw["metadata"]
+
+
 @pytest.mark.parametrize(
     "request_type",
     [
         datastore_admin.GetIndexRequest,
         dict,
     ],
 )
@@ -1315,14 +1596,75 @@
 
 
 @pytest.mark.asyncio
 async def test_get_index_async_from_dict():
     await test_get_index_async(request_type=dict)
 
 
+def test_get_index_field_headers():
+    client = DatastoreAdminClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.GetIndexRequest()
+
+    request.project_id = "project_id_value"
+    request.index_id = "index_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_index), "__call__") as call:
+        call.return_value = index.Index()
+        client.get_index(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value&index_id=index_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_index_field_headers_async():
+    client = DatastoreAdminAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.GetIndexRequest()
+
+    request.project_id = "project_id_value"
+    request.index_id = "index_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_index), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(index.Index())
+        await client.get_index(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value&index_id=index_id_value",
+    ) in kw["metadata"]
+
+
 @pytest.mark.parametrize(
     "request_type",
     [
         datastore_admin.ListIndexesRequest,
         dict,
     ],
 )
@@ -1404,14 +1746,75 @@
 
 
 @pytest.mark.asyncio
 async def test_list_indexes_async_from_dict():
     await test_list_indexes_async(request_type=dict)
 
 
+def test_list_indexes_field_headers():
+    client = DatastoreAdminClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.ListIndexesRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_indexes), "__call__") as call:
+        call.return_value = datastore_admin.ListIndexesResponse()
+        client.list_indexes(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_indexes_field_headers_async():
+    client = DatastoreAdminAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore_admin.ListIndexesRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_indexes), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore_admin.ListIndexesResponse()
+        )
+        await client.list_indexes(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_list_indexes_pager(transport_name: str = "grpc"):
     client = DatastoreAdminClient(
         credentials=ga_credentials.AnonymousCredentials,
         transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1442,19 +1845,22 @@
                     index.Index(),
                 ],
             ),
             RuntimeError,
         )
 
         metadata = ()
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("project_id", ""),)),
+        )
         pager = client.list_indexes(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, index.Index) for i in results)
 
 
 def test_list_indexes_pages(transport_name: str = "grpc"):
     client = DatastoreAdminClient(
         credentials=ga_credentials.AnonymousCredentials,
@@ -1828,14 +2234,36 @@
                 "https://www.googleapis.com/auth/datastore",
             ),
             quota_project_id="octopus",
         )
 
 
 @pytest.mark.parametrize(
+    "transport_class",
+    [
+        transports.DatastoreAdminGrpcTransport,
+        transports.DatastoreAdminGrpcAsyncIOTransport,
+    ],
+)
+def test_datastore_admin_transport_auth_gdch_credentials(transport_class):
+    host = "https://language.com"
+    api_audience_tests = [None, "https://language2.com"]
+    api_audience_expect = [host, "https://language2.com"]
+    for t, e in zip(api_audience_tests, api_audience_expect):
+        with mock.patch.object(google.auth, "default", autospec=True) as adc:
+            gdch_mock = mock.MagicMock()
+            type(gdch_mock).with_gdch_audience = mock.PropertyMock(
+                return_value=gdch_mock
+            )
+            adc.return_value = (gdch_mock, None)
+            transport_class(host=host, api_audience=t)
+            gdch_mock.with_gdch_audience.assert_called_once_with(e)
+
+
+@pytest.mark.parametrize(
     "transport_class,grpc_helpers",
     [
         (transports.DatastoreAdminGrpcTransport, grpc_helpers),
         (transports.DatastoreAdminGrpcAsyncIOTransport, grpc_helpers_async),
     ],
 )
 def test_datastore_admin_transport_create_channel(transport_class, grpc_helpers):
@@ -2306,8 +2734,9 @@
                 credentials_file=None,
                 host=client.DEFAULT_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
```

### Comparing `google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_v1/__init__.py` & `google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/gapic/datastore_v1/test_datastore.py` & `google-cloud-datastore-2.9.0/tests/unit/gapic/datastore_v1/test_datastore.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,37 +10,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock  # pragma: NO COVER
+except ImportError:  # pragma: NO COVER
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
-
+from proto.marshal.rules import wrappers
 
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import grpc_helpers
 from google.api_core import grpc_helpers_async
 from google.api_core import path_template
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.datastore_v1.services.datastore import DatastoreAsyncClient
 from google.cloud.datastore_v1.services.datastore import DatastoreClient
 from google.cloud.datastore_v1.services.datastore import transports
+from google.cloud.datastore_v1.types import aggregation_result
 from google.cloud.datastore_v1.types import datastore
 from google.cloud.datastore_v1.types import entity
 from google.cloud.datastore_v1.types import query
+from google.longrunning import operations_pb2
 from google.oauth2 import service_account
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
 from google.type import latlng_pb2  # type: ignore
 import google.auth
 
@@ -210,14 +218,15 @@
             credentials_file=None,
             host="squid.clam.whelk",
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT is
     # "never".
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "never"}):
         with mock.patch.object(transport_class, "__init__") as patched:
             patched.return_value = None
@@ -227,14 +236,15 @@
                 credentials_file=None,
                 host=client.DEFAULT_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT is
     # "always".
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "always"}):
         with mock.patch.object(transport_class, "__init__") as patched:
             patched.return_value = None
@@ -244,14 +254,15 @@
                 credentials_file=None,
                 host=client.DEFAULT_MTLS_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT has
     # unsupported value.
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "Unsupported"}):
         with pytest.raises(MutualTLSChannelError):
             client = client_class(transport=transport_name)
@@ -273,14 +284,33 @@
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id="octopus",
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
+        )
+    # Check the case api_endpoint is provided
+    options = client_options.ClientOptions(
+        api_audience="https://language.googleapis.com"
+    )
+    with mock.patch.object(transport_class, "__init__") as patched:
+        patched.return_value = None
+        client = client_class(client_options=options, transport=transport_name)
+        patched.assert_called_once_with(
+            credentials=None,
+            credentials_file=None,
+            host=client.DEFAULT_ENDPOINT,
+            scopes=None,
+            client_cert_source_for_mtls=None,
+            quota_project_id=None,
+            client_info=transports.base.DEFAULT_CLIENT_INFO,
+            always_use_jwt_access=True,
+            api_audience="https://language.googleapis.com",
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,use_client_cert_env",
     [
         (DatastoreClient, transports.DatastoreGrpcTransport, "grpc", "true"),
@@ -338,14 +368,15 @@
                 credentials_file=None,
                 host=expected_host,
                 scopes=None,
                 client_cert_source_for_mtls=expected_client_cert_source,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case ADC client cert is provided. Whether client cert is used depends on
     # GOOGLE_API_USE_CLIENT_CERTIFICATE value.
     with mock.patch.dict(
         os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": use_client_cert_env}
     ):
@@ -372,14 +403,15 @@
                         credentials_file=None,
                         host=expected_host,
                         scopes=None,
                         client_cert_source_for_mtls=expected_client_cert_source,
                         quota_project_id=None,
                         client_info=transports.base.DEFAULT_CLIENT_INFO,
                         always_use_jwt_access=True,
+                        api_audience=None,
                     )
 
     # Check the case client_cert_source and ADC client cert are not provided.
     with mock.patch.dict(
         os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": use_client_cert_env}
     ):
         with mock.patch.object(transport_class, "__init__") as patched:
@@ -394,14 +426,15 @@
                     credentials_file=None,
                     host=client.DEFAULT_ENDPOINT,
                     scopes=None,
                     client_cert_source_for_mtls=None,
                     quota_project_id=None,
                     client_info=transports.base.DEFAULT_CLIENT_INFO,
                     always_use_jwt_access=True,
+                    api_audience=None,
                 )
 
 
 @pytest.mark.parametrize("client_class", [DatastoreClient, DatastoreAsyncClient])
 @mock.patch.object(
     DatastoreClient, "DEFAULT_ENDPOINT", modify_default_endpoint(DatastoreClient)
 )
@@ -504,14 +537,15 @@
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
             scopes=["1", "2"],
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,grpc_helpers",
     [
         (DatastoreClient, transports.DatastoreGrpcTransport, "grpc", grpc_helpers),
@@ -537,14 +571,15 @@
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 def test_datastore_client_client_options_from_dict():
     with mock.patch(
         "google.cloud.datastore_v1.services.datastore.transports.DatastoreGrpcTransport.__init__"
     ) as grpc_transport:
@@ -555,14 +590,15 @@
             credentials_file=None,
             host="squid.clam.whelk",
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,grpc_helpers",
     [
         (DatastoreClient, transports.DatastoreGrpcTransport, "grpc", grpc_helpers),
@@ -588,14 +624,15 @@
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
     # test that the credentials from file are saved and used as the credentials.
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch.object(
         google.auth, "default", autospec=True
@@ -705,14 +742,75 @@
 
 
 @pytest.mark.asyncio
 async def test_lookup_async_from_dict():
     await test_lookup_async(request_type=dict)
 
 
+def test_lookup_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.LookupRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.lookup), "__call__") as call:
+        call.return_value = datastore.LookupResponse()
+        client.lookup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_lookup_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.LookupRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.lookup), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.LookupResponse()
+        )
+        await client.lookup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_lookup_flattened():
     client = DatastoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.lookup), "__call__") as call:
@@ -922,14 +1020,229 @@
 
 
 @pytest.mark.asyncio
 async def test_run_query_async_from_dict():
     await test_run_query_async(request_type=dict)
 
 
+def test_run_query_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.RunQueryRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_query), "__call__") as call:
+        call.return_value = datastore.RunQueryResponse()
+        client.run_query(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_run_query_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.RunQueryRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_query), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.RunQueryResponse()
+        )
+        await client.run_query(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        datastore.RunAggregationQueryRequest,
+        dict,
+    ],
+)
+def test_run_aggregation_query(request_type, transport: str = "grpc"):
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.run_aggregation_query), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = datastore.RunAggregationQueryResponse()
+        response = client.run_aggregation_query(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == datastore.RunAggregationQueryRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, datastore.RunAggregationQueryResponse)
+
+
+def test_run_aggregation_query_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.run_aggregation_query), "__call__"
+    ) as call:
+        client.run_aggregation_query()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == datastore.RunAggregationQueryRequest()
+
+
+@pytest.mark.asyncio
+async def test_run_aggregation_query_async(
+    transport: str = "grpc_asyncio", request_type=datastore.RunAggregationQueryRequest
+):
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.run_aggregation_query), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.RunAggregationQueryResponse()
+        )
+        response = await client.run_aggregation_query(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == datastore.RunAggregationQueryRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, datastore.RunAggregationQueryResponse)
+
+
+@pytest.mark.asyncio
+async def test_run_aggregation_query_async_from_dict():
+    await test_run_aggregation_query_async(request_type=dict)
+
+
+def test_run_aggregation_query_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.RunAggregationQueryRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.run_aggregation_query), "__call__"
+    ) as call:
+        call.return_value = datastore.RunAggregationQueryResponse()
+        client.run_aggregation_query(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_run_aggregation_query_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.RunAggregationQueryRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.run_aggregation_query), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.RunAggregationQueryResponse()
+        )
+        await client.run_aggregation_query(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 @pytest.mark.parametrize(
     "request_type",
     [
         datastore.BeginTransactionRequest,
         dict,
     ],
 )
@@ -1017,14 +1330,79 @@
 
 
 @pytest.mark.asyncio
 async def test_begin_transaction_async_from_dict():
     await test_begin_transaction_async(request_type=dict)
 
 
+def test_begin_transaction_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.BeginTransactionRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.begin_transaction), "__call__"
+    ) as call:
+        call.return_value = datastore.BeginTransactionResponse()
+        client.begin_transaction(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_begin_transaction_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.BeginTransactionRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.begin_transaction), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.BeginTransactionResponse()
+        )
+        await client.begin_transaction(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_begin_transaction_flattened():
     client = DatastoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
@@ -1192,14 +1570,75 @@
 
 
 @pytest.mark.asyncio
 async def test_commit_async_from_dict():
     await test_commit_async(request_type=dict)
 
 
+def test_commit_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.CommitRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.commit), "__call__") as call:
+        call.return_value = datastore.CommitResponse()
+        client.commit(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_commit_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.CommitRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.commit), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.CommitResponse()
+        )
+        await client.commit(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_commit_flattened():
     client = DatastoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.commit), "__call__") as call:
@@ -1439,14 +1878,75 @@
 
 
 @pytest.mark.asyncio
 async def test_rollback_async_from_dict():
     await test_rollback_async(request_type=dict)
 
 
+def test_rollback_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.RollbackRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.rollback), "__call__") as call:
+        call.return_value = datastore.RollbackResponse()
+        client.rollback(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_rollback_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.RollbackRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.rollback), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.RollbackResponse()
+        )
+        await client.rollback(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_rollback_flattened():
     client = DatastoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.rollback), "__call__") as call:
@@ -1614,14 +2114,75 @@
 
 
 @pytest.mark.asyncio
 async def test_allocate_ids_async_from_dict():
     await test_allocate_ids_async(request_type=dict)
 
 
+def test_allocate_ids_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.AllocateIdsRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.allocate_ids), "__call__") as call:
+        call.return_value = datastore.AllocateIdsResponse()
+        client.allocate_ids(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_allocate_ids_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.AllocateIdsRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.allocate_ids), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.AllocateIdsResponse()
+        )
+        await client.allocate_ids(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_allocate_ids_flattened():
     client = DatastoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.allocate_ids), "__call__") as call:
@@ -1809,14 +2370,75 @@
 
 
 @pytest.mark.asyncio
 async def test_reserve_ids_async_from_dict():
     await test_reserve_ids_async(request_type=dict)
 
 
+def test_reserve_ids_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.ReserveIdsRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.reserve_ids), "__call__") as call:
+        call.return_value = datastore.ReserveIdsResponse()
+        client.reserve_ids(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_reserve_ids_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = datastore.ReserveIdsRequest()
+
+    request.project_id = "project_id_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.reserve_ids), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            datastore.ReserveIdsResponse()
+        )
+        await client.reserve_ids(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "project_id=project_id_value",
+    ) in kw["metadata"]
+
+
 def test_reserve_ids_flattened():
     client = DatastoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.reserve_ids), "__call__") as call:
@@ -2060,19 +2682,24 @@
         )
 
     # Every method on the transport should just blindly
     # raise NotImplementedError.
     methods = (
         "lookup",
         "run_query",
+        "run_aggregation_query",
         "begin_transaction",
         "commit",
         "rollback",
         "allocate_ids",
         "reserve_ids",
+        "get_operation",
+        "cancel_operation",
+        "delete_operation",
+        "list_operations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -2156,14 +2783,36 @@
                 "https://www.googleapis.com/auth/datastore",
             ),
             quota_project_id="octopus",
         )
 
 
 @pytest.mark.parametrize(
+    "transport_class",
+    [
+        transports.DatastoreGrpcTransport,
+        transports.DatastoreGrpcAsyncIOTransport,
+    ],
+)
+def test_datastore_transport_auth_gdch_credentials(transport_class):
+    host = "https://language.com"
+    api_audience_tests = [None, "https://language2.com"]
+    api_audience_expect = [host, "https://language2.com"]
+    for t, e in zip(api_audience_tests, api_audience_expect):
+        with mock.patch.object(google.auth, "default", autospec=True) as adc:
+            gdch_mock = mock.MagicMock()
+            type(gdch_mock).with_gdch_audience = mock.PropertyMock(
+                return_value=gdch_mock
+            )
+            adc.return_value = (gdch_mock, None)
+            transport_class(host=host, api_audience=t)
+            gdch_mock.with_gdch_audience.assert_called_once_with(e)
+
+
+@pytest.mark.parametrize(
     "transport_class,grpc_helpers",
     [
         (transports.DatastoreGrpcTransport, grpc_helpers),
         (transports.DatastoreGrpcAsyncIOTransport, grpc_helpers_async),
     ],
 )
 def test_datastore_transport_create_channel(transport_class, grpc_helpers):
@@ -2529,14 +3178,582 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_delete_operation(transport: str = "grpc"):
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.DeleteOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+        response = client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+@pytest.mark.asyncio
+async def test_delete_operation_async(transport: str = "grpc"):
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.DeleteOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+def test_delete_operation_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.DeleteOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        call.return_value = None
+
+        client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_delete_operation_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.DeleteOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        await client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_delete_operation_from_dict():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+
+        response = client.delete_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_delete_operation_from_dict_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_cancel_operation(transport: str = "grpc"):
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.CancelOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+        response = client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+@pytest.mark.asyncio
+async def test_cancel_operation_async(transport: str = "grpc"):
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.CancelOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+def test_cancel_operation_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.CancelOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        call.return_value = None
+
+        client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_cancel_operation_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.CancelOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        await client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_cancel_operation_from_dict():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+
+        response = client.cancel_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_cancel_operation_from_dict_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.cancel_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_operation(transport: str = "grpc"):
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.GetOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation()
+        response = client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.Operation)
+
+
+@pytest.mark.asyncio
+async def test_get_operation_async(transport: str = "grpc"):
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.GetOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        response = await client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.Operation)
+
+
+def test_get_operation_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.GetOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        call.return_value = operations_pb2.Operation()
+
+        client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_operation_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.GetOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        await client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_get_operation_from_dict():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation()
+
+        response = client.get_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_operation_from_dict_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        response = await client.get_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_list_operations(transport: str = "grpc"):
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.ListOperationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.ListOperationsResponse()
+        response = client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.ListOperationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_operations_async(transport: str = "grpc"):
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.ListOperationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.ListOperationsResponse()
+        )
+        response = await client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.ListOperationsResponse)
+
+
+def test_list_operations_field_headers():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.ListOperationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        call.return_value = operations_pb2.ListOperationsResponse()
+
+        client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_operations_field_headers_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.ListOperationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.ListOperationsResponse()
+        )
+        await client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_operations_from_dict():
+    client = DatastoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.ListOperationsResponse()
+
+        response = client.list_operations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_operations_from_dict_async():
+    client = DatastoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.ListOperationsResponse()
+        )
+        response = await client.list_operations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
         client = DatastoreClient(
@@ -2589,8 +3806,9 @@
                 credentials_file=None,
                 host=client.DEFAULT_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
```

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test__gapic.py` & `google-cloud-datastore-2.9.0/tests/unit/test__gapic.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test__http.py` & `google-cloud-datastore-2.9.0/tests/unit/test__http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test_batch.py` & `google-cloud-datastore-2.9.0/tests/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test_client.py` & `google-cloud-datastore-2.9.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test_entity.py` & `google-cloud-datastore-2.9.0/tests/unit/test_entity.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test_helpers.py` & `google-cloud-datastore-2.9.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test_key.py` & `google-cloud-datastore-2.9.0/tests/unit/test_key.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test_query.py` & `google-cloud-datastore-2.9.0/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastore-2.8.3/tests/unit/test_transaction.py` & `google-cloud-datastore-2.9.0/tests/unit/test_transaction.py`

 * *Files identical despite different names*

