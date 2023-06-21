# Comparing `tmp/sparrow-order-lib-0.2.0.tar.gz` & `tmp/sparrow-order-lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/liaojessica/Documents/git/sparrow_order_lib/dist/.tmp-nqu56xcq/sparrow-order-lib-0.2.0.tar", last modified: Tue Jun 20 08:33:07 2023, max compression
+gzip compressed data, was "/Users/liaojessica/Documents/git/sparrow_order_lib/dist/.tmp-gxv7y5wh/sparrow-order-lib-0.2.1.tar", last modified: Wed Jun 21 01:19:44 2023, max compression
```

## Comparing `sparrow-order-lib-0.2.0.tar` & `sparrow-order-lib-0.2.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/
--rw-r--r--   0 liaojessica   (501) staff       (20)     1073 2021-11-09 03:23:03.000000 sparrow-order-lib-0.2.0/LICENSE
--rw-r--r--   0 liaojessica   (501) staff       (20)     9127 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/PKG-INFO
--rw-r--r--   0 liaojessica   (501) staff       (20)     8590 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.0/README.md
--rw-r--r--   0 liaojessica   (501) staff       (20)      103 2021-11-09 03:17:41.000000 sparrow-order-lib-0.2.0/pyproject.toml
--rw-r--r--   0 liaojessica   (501) staff       (20)      723 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/setup.cfg
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/
--rw-r--r--   0 liaojessica   (501) staff       (20)       76 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/__init__.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/
--rw-r--r--   0 liaojessica   (501) staff       (20)      912 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2014 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/base_models.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      704 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/common_utils.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     5712 2023-05-06 04:21:47.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1592 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/datastructures.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1353 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/decorators.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    12853 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/dt_utils.py
--rw-r--r--   0 liaojessica   (501) staff       (20)       90 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/formats.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      714 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/model_function.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      251 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/numbers.py
--rw-r--r--   0 liaojessica   (501) staff       (20)        0 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/text.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1415 2022-10-25 02:16:51.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/xls_util.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/db_tool/
--rw-r--r--   0 liaojessica   (501) staff       (20)        0 2021-11-13 15:05:09.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/db_tool/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      848 2022-10-25 02:16:51.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/db_tool/query.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/
--rw-r--r--   0 liaojessica   (501) staff       (20)     1359 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      422 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/constants.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/
--rw-r--r--   0 liaojessica   (501) staff       (20)       56 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     7841 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/base.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1092 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/client.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1228 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3661 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_builder.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3091 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_door.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     5145 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_param.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3620 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_query_util.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1223 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/exceptions.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2207 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/field.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      381 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/in_query_param.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      163 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/index.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      241 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/mock.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3137 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/operators.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/
--rw-r--r--   0 liaojessica   (501) staff       (20)     1619 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1782 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_base.py
--rw-r--r--   0 liaojessica   (501) staff       (20)       64 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_client.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2455 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3294 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3947 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2500 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2310 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_field.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      515 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      373 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_mock.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2203 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_operators.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     7542 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/mapping_constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3086 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/query_mapping_constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3490 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/test_order_doc_type.py
--rw-r--r--   0 liaojessica   (501) staff       (20)       42 2021-11-09 03:18:09.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/example.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/
--rw-r--r--   0 liaojessica   (501) staff       (20)        0 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1406 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_api_path.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      815 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_core.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     5271 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_core_go.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2778 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     4706 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_product.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      383 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/svc_config.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/
--rw-r--r--   0 liaojessica   (501) staff       (20)       31 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3239 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     2974 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/models.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1164 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      539 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/utils.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/
--rw-r--r--   0 liaojessica   (501) staff       (20)       33 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     8626 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    32383 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    71783 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/models.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/
--rw-r--r--   0 liaojessica   (501) staff       (20)       34 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     7206 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1892 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/disstorage.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    15398 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/models.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      550 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      390 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/serializers.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      514 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/utils.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/
--rw-r--r--   0 liaojessica   (501) staff       (20)       34 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    57678 2023-06-20 08:31:47.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    32810 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/models.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     7952 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/serializer_data.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     4095 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/serializers.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_exchange/
--rw-r--r--   0 liaojessica   (501) staff       (20)      155 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_exchange/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    15287 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_exchange/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    17612 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_exchange/models.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_inparcel/
--rw-r--r--   0 liaojessica   (501) staff       (20)       32 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_inparcel/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     8197 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_inparcel/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    11201 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_inparcel/models.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_orders/
--rw-r--r--   0 liaojessica   (501) staff       (20)       68 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_orders/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)    10215 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_orders/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)   108809 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_orders/models.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_parcel/
--rw-r--r--   0 liaojessica   (501) staff       (20)       30 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_parcel/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     4434 2022-11-08 11:01:56.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_parcel/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)      455 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_parcel/exceptions.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     7599 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_parcel/models.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_promotions/
--rw-r--r--   0 liaojessica   (501) staff       (20)       34 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_promotions/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     1979 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_promotions/models.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_shipping/
--rw-r--r--   0 liaojessica   (501) staff       (20)       32 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_shipping/__init__.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     3236 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_shipping/constants.py
--rw-r--r--   0 liaojessica   (501) staff       (20)     9065 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_shipping/models.py
-drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/
--rw-r--r--   0 liaojessica   (501) staff       (20)     9127 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/PKG-INFO
--rw-r--r--   0 liaojessica   (501) staff       (20)     4741 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/SOURCES.txt
--rw-r--r--   0 liaojessica   (501) staff       (20)        1 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/dependency_links.txt
--rw-r--r--   0 liaojessica   (501) staff       (20)       39 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/requires.txt
--rw-r--r--   0 liaojessica   (501) staff       (20)       18 2023-06-20 08:33:07.000000 sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/top_level.txt
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1073 2021-11-09 03:23:03.000000 sparrow-order-lib-0.2.1/LICENSE
+-rw-r--r--   0 liaojessica   (501) staff       (20)     9127 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/PKG-INFO
+-rw-r--r--   0 liaojessica   (501) staff       (20)     8590 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.1/README.md
+-rw-r--r--   0 liaojessica   (501) staff       (20)      103 2021-11-09 03:17:41.000000 sparrow-order-lib-0.2.1/pyproject.toml
+-rw-r--r--   0 liaojessica   (501) staff       (20)      723 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/setup.cfg
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       76 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/__init__.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/
+-rw-r--r--   0 liaojessica   (501) staff       (20)      912 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2014 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/base_models.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      704 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/common_utils.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     5712 2023-05-06 04:21:47.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1592 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/datastructures.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1353 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/decorators.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    12853 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/dt_utils.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)       90 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/formats.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      714 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/model_function.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      251 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/numbers.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)        0 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/text.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1415 2022-10-25 02:16:51.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/xls_util.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/db_tool/
+-rw-r--r--   0 liaojessica   (501) staff       (20)        0 2021-11-13 15:05:09.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/db_tool/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      848 2022-10-25 02:16:51.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/db_tool/query.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1359 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      422 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/constants.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       56 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     7841 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/base.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1092 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/client.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1228 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3661 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_builder.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3091 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_door.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     5145 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_param.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3620 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_query_util.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1223 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/exceptions.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2207 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/field.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      381 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/in_query_param.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      163 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/index.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      241 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/mock.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3137 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/operators.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1619 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1782 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_base.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)       64 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_client.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2455 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3294 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3947 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2500 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2310 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_field.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      515 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      373 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_mock.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2203 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_operators.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     7542 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/mapping_constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3086 2022-10-13 06:21:54.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/query_mapping_constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3490 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/test_order_doc_type.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)       42 2021-11-09 03:18:09.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/example.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/
+-rw-r--r--   0 liaojessica   (501) staff       (20)        0 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1406 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_api_path.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      815 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_core.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     5271 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_core_go.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2778 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     4706 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_product.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      383 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/svc_config.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       31 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3239 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     2974 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/models.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1164 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      539 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/utils.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       33 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     8626 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    32383 2023-06-20 08:31:28.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    71783 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/models.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       34 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     7206 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1892 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/disstorage.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    15398 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/models.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      550 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      390 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/serializers.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      514 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/utils.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       34 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    57677 2023-06-21 01:18:38.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    32810 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/models.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     7952 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/serializer_data.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     4095 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/serializers.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_exchange/
+-rw-r--r--   0 liaojessica   (501) staff       (20)      155 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_exchange/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    15287 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_exchange/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    17612 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_exchange/models.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_inparcel/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       32 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_inparcel/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     8197 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_inparcel/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    11201 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_inparcel/models.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_orders/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       68 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_orders/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)    10215 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_orders/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)   108809 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_orders/models.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_parcel/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       30 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_parcel/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     4434 2022-11-08 11:01:56.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_parcel/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)      455 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_parcel/exceptions.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     7599 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_parcel/models.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_promotions/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       34 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_promotions/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     1979 2021-12-21 01:24:43.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_promotions/models.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_shipping/
+-rw-r--r--   0 liaojessica   (501) staff       (20)       32 2022-07-01 02:39:05.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_shipping/__init__.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     3236 2023-03-13 09:19:37.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_shipping/constants.py
+-rw-r--r--   0 liaojessica   (501) staff       (20)     9065 2022-03-14 08:31:01.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_shipping/models.py
+drwxr-xr-x   0 liaojessica   (501) staff       (20)        0 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/
+-rw-r--r--   0 liaojessica   (501) staff       (20)     9127 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/PKG-INFO
+-rw-r--r--   0 liaojessica   (501) staff       (20)     4741 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 liaojessica   (501) staff       (20)        1 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 liaojessica   (501) staff       (20)       39 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/requires.txt
+-rw-r--r--   0 liaojessica   (501) staff       (20)       18 2023-06-21 01:19:44.000000 sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/top_level.txt
```

### Comparing `sparrow-order-lib-0.2.0/LICENSE` & `sparrow-order-lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/PKG-INFO` & `sparrow-order-lib-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-order-lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: This is a lib for sparrow order projects.
 Home-page: https://gitee.com/sparrow614/sparrow-order-lib
 Author: Jessica Liao
 Author-email: 18610193367@sina.cn
 Project-URL: Bug Tracker, https://gitee.com/sparrow614/sparrow-order-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparrow-order-lib-0.2.0/README.md` & `sparrow-order-lib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/setup.cfg` & `sparrow-order-lib-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sparrow-order-lib
-version = 0.2.0
+version = 0.2.1
 author = Jessica Liao
 author_email = 18610193367@sina.cn
 description = This is a lib for sparrow order projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitee.com/sparrow614/sparrow-order-lib
 project_urls =
```

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/__init__.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/base_models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/base_models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/common_utils.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/common_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/datastructures.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/decorators.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/dt_utils.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/dt_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/model_function.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/model_function.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/core/xls_util.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/core/xls_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/db_tool/query.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/db_tool/query.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/__init__.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/base.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/client.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/client.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_builder.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_door.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_param.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/es_query_util.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/exceptions.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/field.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/operators.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/__init__.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_base.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_door.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_param.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_field.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/es_util/tests/test_operators.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/es_util/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/mapping_constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/query_mapping_constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/query_mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/es/test_order_doc_type.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/es/test_order_doc_type.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_api_path.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_api_path.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_core.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_core.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_core_go.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_core_go.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_lanyue.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_lanyue.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/remote_call/sparrow_product.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/remote_call/sparrow_product.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_afsplus/utils.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_afsplus/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_aftersale/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_aftersale/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/disstorage.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/disstorage.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_disstorage/utils.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_disstorage/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1347,15 +1347,15 @@
 
 
 # 欧莱雅集团可同步专柜列表
 OLAY_SHOP_DICT_CONST = {
     "108030": "01",
     "108048": "45",
     "108063": "15",
-    "108066": "V45" 
+    "108066": "83" 
 }
 
 class AddressGroupStatus(object):
     """
     可合-已齐、可合-未齐、无可合、已合单、在库已合、单单、无在库、其他
     """
     # 可合-已齐（多单在库、未合、无其他状态）
```

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/serializer_data.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/serializer_data.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_distribute/serializers.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_distribute/serializers.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_exchange/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_exchange/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_exchange/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_exchange/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_inparcel/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_inparcel/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_inparcel/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_inparcel/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_orders/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_orders/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_orders/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_orders/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_parcel/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_parcel/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_parcel/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_parcel/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_promotions/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_promotions/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_shipping/constants.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_shipping/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib/sparrow_shipping/models.py` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib/sparrow_shipping/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/PKG-INFO` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-order-lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: This is a lib for sparrow order projects.
 Home-page: https://gitee.com/sparrow614/sparrow-order-lib
 Author: Jessica Liao
 Author-email: 18610193367@sina.cn
 Project-URL: Bug Tracker, https://gitee.com/sparrow614/sparrow-order-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparrow-order-lib-0.2.0/src/sparrow_order_lib.egg-info/SOURCES.txt` & `sparrow-order-lib-0.2.1/src/sparrow_order_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

