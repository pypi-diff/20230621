# Comparing `tmp/pds.api-client-1.2.0.tar.gz` & `tmp/pds.api-client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pds.api-client-1.2.0.tar", last modified: Wed Jan 18 21:17:39 2023, max compression
+gzip compressed data, was "pds.api-client-1.3.0.tar", last modified: Wed Jun 21 18:43:07 2023, max compression
```

## Comparing `pds.api-client-1.2.0.tar` & `pds.api-client-1.3.0.tar`

### file list

```diff
@@ -1,392 +1,84 @@
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.460268 pds.api-client-1.2.0/
--rw-r--r--   0 loubrieu   (502) staff       (20)    11331 2021-10-14 21:02:12.000000 pds.api-client-1.2.0/LICENSE.txt
--rw-r--r--   0 loubrieu   (502) staff       (20)       57 2021-03-04 22:56:04.000000 pds.api-client-1.2.0/MANIFEST.in
--rw-r--r--   0 loubrieu   (502) staff       (20)     1599 2021-10-14 21:02:12.000000 pds.api-client-1.2.0/NOTICE.txt
--rw-r--r--   0 loubrieu   (502) staff       (20)      766 2023-01-18 21:17:39.460431 pds.api-client-1.2.0/PKG-INFO
--rw-r--r--   0 loubrieu   (502) staff       (20)    29968 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/README.md
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.296393 pds.api-client-1.2.0/pds/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/__init__.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.301708 pds.api-client-1.2.0/pds/api_client/
--rw-r--r--   0 loubrieu   (502) staff       (20)     1122 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    58860 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/api_client.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.304861 pds.api-client-1.2.0/pds/api_client/apis/
--rw-r--r--   0 loubrieu   (502) staff       (20)      214 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/apis/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    11659 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/path_to_api.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.331947 pds.api-client-1.2.0/pds/api_client/apis/paths/
--rw-r--r--   0 loubrieu   (502) staff       (20)      241 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)       99 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      120 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles_identifier.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      127 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles_identifier_all.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      143 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles_identifier_collections.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      150 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles_identifier_collections_all.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      156 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles_identifier_collections_latest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      133 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles_identifier_latest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      137 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/bundles_identifier_products.py
--rw-r--r--   0 loubrieu   (502) staff       (20)       99 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      110 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      149 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_member_of.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      167 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_member_of_member_of.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      184 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_member_of_member_of_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      166 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_member_of_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      146 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_members.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      161 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_members_members.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      178 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_members_members_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      163 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/classes_class_identifier_members_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      107 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      128 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections_identifier.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      135 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections_identifier_all.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      143 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections_identifier_bundles.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      141 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections_identifier_latest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      145 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections_identifier_products.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      152 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections_identifier_products_all.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      158 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/collections_identifier_products_latest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      101 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      122 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      129 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_all.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      137 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_bundles.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      144 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_bundles_all.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      150 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_bundles_latest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      145 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_collections.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      152 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_collections_all.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      158 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_collections_latest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      135 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_latest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      140 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_member_of.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      158 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_member_of_member_of.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      175 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_member_of_member_of_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      157 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_member_of_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      137 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_members.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      152 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_members_members.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      169 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_members_members_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      154 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/paths/products_identifier_members_versions.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      776 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/tag_to_api.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.334912 pds.api-client-1.2.0/pds/api_client/apis/tags/
--rw-r--r--   0 loubrieu   (502) staff       (20)      397 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/tags/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      923 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/pds/api_client/apis/tags/classes_api.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     3390 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/apis/tags/deprecated_api.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1162 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/apis/tags/products_api.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     2704 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/apis/tags/references_api.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    16360 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/configuration.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     4801 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/exceptions.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.342401 pds.api-client-1.2.0/pds/api_client/model/
--rw-r--r--   0 loubrieu   (502) staff       (20)      348 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/model/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     3375 2023-01-18 21:13:32.000000 pds.api-client-1.2.0/pds/api_client/model/error_message.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     5279 2023-01-18 21:13:32.000000 pds.api-client-1.2.0/pds/api_client/model/metadata.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    17300 2023-01-18 21:13:32.000000 pds.api-client-1.2.0/pds/api_client/model/pds4_metadata.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     4012 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/pds/api_client/model/pds4_product.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     4275 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/pds/api_client/model/pds4_products.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    12614 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/pds/api_client/model/pds_product.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     4266 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/pds/api_client/model/pds_products.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1670 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/pds/api_client/model/property_array_values.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     4907 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/pds/api_client/model/reference.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     7360 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/pds/api_client/model/summary.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     7246 2023-01-18 21:13:34.000000 pds.api-client-1.2.0/pds/api_client/model/wyriwyg_product.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     4302 2023-01-18 21:13:34.000000 pds.api-client-1.2.0/pds/api_client/model/wyriwyg_products.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.342839 pds.api-client-1.2.0/pds/api_client/models/
--rw-r--r--   0 loubrieu   (502) staff       (20)     1098 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/models/__init__.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.343232 pds.api-client-1.2.0/pds/api_client/paths/
--rw-r--r--   0 loubrieu   (502) staff       (20)     3566 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/__init__.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.344281 pds.api-client-1.2.0/pds/api_client/paths/bundles/
--rw-r--r--   0 loubrieu   (502) staff       (20)      301 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25604 2023-01-18 21:13:36.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.345541 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier/
--rw-r--r--   0 loubrieu   (502) staff       (20)      323 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25036 2023-01-18 21:13:36.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.346765 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)      331 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26606 2023-01-18 21:13:37.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_all/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.347971 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections/
--rw-r--r--   0 loubrieu   (502) staff       (20)      347 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26694 2023-01-18 21:13:37.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.351372 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)      355 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26737 2023-01-18 21:13:38.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections_all/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.353219 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)      361 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26770 2023-01-18 21:13:38.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_collections_latest/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.355029 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)      337 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25112 2023-01-18 21:13:39.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_latest/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.356419 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_products/
--rw-r--r--   0 loubrieu   (502) staff       (20)      341 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_products/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26661 2023-01-18 21:13:39.000000 pds.api-client-1.2.0/pds/api_client/paths/bundles_identifier_products/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.358163 pds.api-client-1.2.0/pds/api_client/paths/classes/
--rw-r--r--   0 loubrieu   (502) staff       (20)      301 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/pds/api_client/paths/classes/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    18704 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/pds/api_client/paths/classes/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.359379 pds.api-client-1.2.0/pds/api_client/paths/classes_class/
--rw-r--r--   0 loubrieu   (502) staff       (20)      313 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    28507 2023-01-18 21:13:34.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.360983 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)      354 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27795 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.362891 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)      373 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27842 2023-01-18 21:13:52.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_member_of/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.364456 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      391 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    28501 2023-01-18 21:13:52.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_member_of_versions/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.366501 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      372 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    28454 2023-01-18 21:13:53.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_member_of_versions/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.367937 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)      351 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27772 2023-01-18 21:13:54.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.369588 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)      367 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27878 2023-01-18 21:13:54.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_members/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.371155 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      385 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    28537 2023-01-18 21:13:55.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_members_versions/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.372655 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      369 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    28431 2023-01-18 21:13:55.000000 pds.api-client-1.2.0/pds/api_client/paths/classes_class_identifier_members_versions/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.373957 pds.api-client-1.2.0/pds/api_client/paths/collections/
--rw-r--r--   0 loubrieu   (502) staff       (20)      309 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25648 2023-01-18 21:13:40.000000 pds.api-client-1.2.0/pds/api_client/paths/collections/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.375111 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier/
--rw-r--r--   0 loubrieu   (502) staff       (20)      331 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25080 2023-01-18 21:13:40.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.376399 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)      339 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26650 2023-01-18 21:13:41.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_all/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.377817 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_bundles/
--rw-r--r--   0 loubrieu   (502) staff       (20)      347 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_bundles/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26694 2023-01-18 21:13:41.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_bundles/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.379078 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)      345 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25156 2023-01-18 21:13:42.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_latest/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.380605 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products/
--rw-r--r--   0 loubrieu   (502) staff       (20)      349 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26705 2023-01-18 21:13:42.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.382139 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)      357 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26748 2023-01-18 21:13:43.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products_all/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.383781 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)      363 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26781 2023-01-18 21:13:43.000000 pds.api-client-1.2.0/pds/api_client/paths/collections_identifier_products_latest/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.384839 pds.api-client-1.2.0/pds/api_client/paths/products/
--rw-r--r--   0 loubrieu   (502) staff       (20)      303 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/paths/products/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25751 2023-01-18 21:13:49.000000 pds.api-client-1.2.0/pds/api_client/paths/products/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.386238 pds.api-client-1.2.0/pds/api_client/paths/products_identifier/
--rw-r--r--   0 loubrieu   (502) staff       (20)      325 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25278 2023-01-18 21:13:49.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.387602 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)      333 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26827 2023-01-18 21:13:50.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_all/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.388585 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles/
--rw-r--r--   0 loubrieu   (502) staff       (20)      341 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26661 2023-01-18 21:13:44.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.389924 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)      349 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26715 2023-01-18 21:13:44.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles_all/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.390848 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)      355 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26737 2023-01-18 21:13:45.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_bundles_latest/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.391863 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections/
--rw-r--r--   0 loubrieu   (502) staff       (20)      349 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26705 2023-01-18 21:13:45.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.393195 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)      357 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26748 2023-01-18 21:13:46.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections_all/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.394595 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)      363 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26781 2023-01-18 21:13:46.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_collections_latest/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.395578 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)      339 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    25265 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_latest/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.396567 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)      344 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26666 2023-01-18 21:13:56.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.397483 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)      363 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26713 2023-01-18 21:13:56.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_member_of/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.398847 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      381 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27372 2023-01-18 21:13:57.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_member_of_versions/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.400199 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      362 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27325 2023-01-18 21:13:57.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_member_of_versions/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.401353 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)      341 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26615 2023-01-18 21:13:58.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.403066 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)      357 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    26717 2023-01-18 21:13:58.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_members/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.404806 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      375 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27376 2023-01-18 21:13:59.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_members_versions/get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.406276 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)      359 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    27274 2023-01-18 21:13:59.000000 pds.api-client-1.2.0/pds/api_client/paths/products_identifier_members_versions/get.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    10913 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/rest.py
--rw-r--r--   0 loubrieu   (502) staff       (20)    97249 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/pds/api_client/schemas.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.297995 pds.api-client-1.2.0/pds.api_client.egg-info/
--rw-r--r--   0 loubrieu   (502) staff       (20)      766 2023-01-18 21:17:39.000000 pds.api-client-1.2.0/pds.api_client.egg-info/PKG-INFO
--rw-r--r--   0 loubrieu   (502) staff       (20)    16012 2023-01-18 21:17:39.000000 pds.api-client-1.2.0/pds.api_client.egg-info/SOURCES.txt
--rw-r--r--   0 loubrieu   (502) staff       (20)        1 2023-01-18 21:17:39.000000 pds.api-client-1.2.0/pds.api_client.egg-info/dependency_links.txt
--rw-r--r--   0 loubrieu   (502) staff       (20)      118 2023-01-18 21:17:39.000000 pds.api-client-1.2.0/pds.api_client.egg-info/requires.txt
--rw-r--r--   0 loubrieu   (502) staff       (20)       13 2023-01-18 21:17:39.000000 pds.api-client-1.2.0/pds.api_client.egg-info/top_level.txt
--rw-r--r--   0 loubrieu   (502) staff       (20)       69 2023-01-18 21:17:39.461063 pds.api-client-1.2.0/setup.cfg
--rw-r--r--   0 loubrieu   (502) staff       (20)     1902 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/setup.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.407057 pds.api-client-1.2.0/src/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2022-11-10 15:57:53.000000 pds.api-client-1.2.0/src/__init__.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.407347 pds.api-client-1.2.0/src/pds/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2022-11-10 15:57:53.000000 pds.api-client-1.2.0/src/pds/__init__.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.408090 pds.api-client-1.2.0/src/pds/api_client/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2022-11-10 15:57:53.000000 pds.api-client-1.2.0/src/pds/api_client/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      451 2022-11-10 15:57:53.000000 pds.api-client-1.2.0/src/pds/api_client/preprocess_openapi.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.408817 pds.api-client-1.2.0/src/pds/api_client/test/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2022-11-10 15:57:53.000000 pds.api-client-1.2.0/src/pds/api_client/test/__init__.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.410846 pds.api-client-1.2.0/src/pds/api_client/test/integration/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2022-11-10 15:57:53.000000 pds.api-client-1.2.0/src/pds/api_client/test/integration/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     2586 2023-01-18 21:11:55.000000 pds.api-client-1.2.0/src/pds/api_client/test/integration/test_bundles.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      892 2023-01-18 21:11:55.000000 pds.api-client-1.2.0/src/pds/api_client/test/integration/test_classes.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     3681 2023-01-18 21:11:55.000000 pds.api-client-1.2.0/src/pds/api_client/test/integration/test_collections.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.285426 pds.api-client-1.2.0/test/
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.418557 pds.api-client-1.2.0/test/test_models/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:01.000000 pds.api-client-1.2.0/test/test_models/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      925 2023-01-18 21:13:32.000000 pds.api-client-1.2.0/test/test_models/test_error_message.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      908 2023-01-18 21:13:32.000000 pds.api-client-1.2.0/test/test_models/test_metadata.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      925 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_pds4_metadata.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      921 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_pds4_product.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      925 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_pds4_products.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      917 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_pds_product.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      921 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_pds_products.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      954 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_property_array_values.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      912 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_reference.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      904 2023-01-18 21:13:33.000000 pds.api-client-1.2.0/test/test_models/test_summary.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      933 2023-01-18 21:13:34.000000 pds.api-client-1.2.0/test/test_models/test_wyriwyg_product.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      937 2023-01-18 21:13:34.000000 pds.api-client-1.2.0/test/test_models/test_wyriwyg_products.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.419199 pds.api-client-1.2.0/test/test_paths/
--rw-r--r--   0 loubrieu   (502) staff       (20)     1995 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/__init__.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.420346 pds.api-client-1.2.0/test/test_paths/test_bundles/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      811 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.421177 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      842 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.422088 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      852 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_all/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.422973 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      876 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.424221 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      886 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections_all/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.425197 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      895 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_collections_latest/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.426027 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      861 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_latest/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.427075 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_products/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_products/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      867 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_bundles_identifier_products/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.428164 pds.api-client-1.2.0/test/test_paths/test_classes/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/test/test_paths/test_classes/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      985 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/test/test_paths/test_classes/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.429223 pds.api-client-1.2.0/test/test_paths/test_classes_class/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      906 2023-01-18 21:13:35.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.430009 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      973 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.430926 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1014 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_member_of/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.431932 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1039 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_member_of_versions/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.432735 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      998 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_member_of_versions/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.433992 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      967 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.435007 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1008 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_members/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.435984 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1033 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_members_versions/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.437033 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      992 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_classes_class_identifier_members_versions/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.438123 pds.api-client-1.2.0/test/test_paths/test_collections/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      823 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.439137 pds.api-client-1.2.0/test/test_paths/test_collections_identifier/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      854 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.439926 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      864 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_all/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.440823 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_bundles/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_bundles/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      876 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_bundles/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.441610 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      873 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_latest/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.442367 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      879 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.443047 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      889 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products_all/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.443987 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      898 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_collections_identifier_products_latest/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.444870 pds.api-client-1.2.0/test/test_paths/test_products/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      950 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.445681 pds.api-client-1.2.0/test/test_paths/test_products_identifier/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1066 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.446594 pds.api-client-1.2.0/test/test_paths/test_products_identifier_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1055 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_all/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.447374 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      867 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.448236 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      877 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles_all/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.448946 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      886 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_bundles_latest/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.449675 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      879 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.450459 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections_all/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections_all/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      889 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections_all/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.451202 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      898 2023-01-18 21:13:47.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_collections_latest/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.451948 pds.api-client-1.2.0/test/test_paths/test_products_identifier_latest/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_latest/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      996 2023-01-18 21:13:51.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_latest/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.453113 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      942 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.454146 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_member_of/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_member_of/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      983 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_member_of/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.455025 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)     1008 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_member_of_versions/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.455967 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      967 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_member_of_versions/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.456941 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      908 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.457852 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_members/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_members/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      945 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_members/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.458846 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      970 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_members_versions/test_get.py
-drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:17:39.459663 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_versions/
--rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_versions/__init__.py
--rw-r--r--   0 loubrieu   (502) staff       (20)      933 2023-01-18 21:14:00.000000 pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_versions/test_get.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.304291 pds.api-client-1.3.0/
+-rw-r--r--   0 loubrieu   (502) staff       (20)    11331 2023-03-02 23:53:30.000000 pds.api-client-1.3.0/LICENSE.txt
+-rw-r--r--   0 loubrieu   (502) staff       (20)       57 2021-03-04 22:56:04.000000 pds.api-client-1.3.0/MANIFEST.in
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1599 2023-03-02 23:53:30.000000 pds.api-client-1.3.0/NOTICE.txt
+-rw-r--r--   0 loubrieu   (502) staff       (20)      717 2023-06-21 18:43:07.304558 pds.api-client-1.3.0/PKG-INFO
+-rw-r--r--   0 loubrieu   (502) staff       (20)    14322 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/README.md
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.251532 pds.api-client-1.3.0/pds/
+-rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/__init__.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.260306 pds.api-client-1.3.0/pds/api_client/
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2411 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/__init__.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.267310 pds.api-client-1.3.0/pds/api_client/api/
+-rw-r--r--   0 loubrieu   (502) staff       (20)      320 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/api/__init__.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)    57782 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/api/all_products_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)    22371 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/api/by_product_classes_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)   456886 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/api/deprecated_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)   126876 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/api/product_references_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)    29914 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/api_client.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)    14568 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/configuration.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     5425 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/exceptions.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.280136 pds.api-client-1.3.0/pds/api_client/models/
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1648 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/__init__.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2199 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/error_message.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2603 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/metadata.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     4067 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds4_metadata.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     3061 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds4_metadata_ops_data_file.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2955 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds4_metadata_ops_label_file_info.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2358 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds4_metadata_ops_tracking_meta.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2788 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds4_product.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2932 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds4_products.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     5550 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds_product.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2920 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/pds_products.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     3061 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/reference.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2860 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/summary.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2865 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/wyriwyg_product.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2336 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/wyriwyg_product_key_value_pair.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2968 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/models/wyriwyg_products.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)    12945 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pds/api_client/rest.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.255217 pds.api-client-1.3.0/pds.api_client.egg-info/
+-rw-r--r--   0 loubrieu   (502) staff       (20)      717 2023-06-21 18:43:07.000000 pds.api-client-1.3.0/pds.api_client.egg-info/PKG-INFO
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2381 2023-06-21 18:43:07.000000 pds.api-client-1.3.0/pds.api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 loubrieu   (502) staff       (20)        1 2023-06-21 18:43:07.000000 pds.api-client-1.3.0/pds.api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 loubrieu   (502) staff       (20)       47 2023-06-21 18:43:07.000000 pds.api-client-1.3.0/pds.api_client.egg-info/requires.txt
+-rw-r--r--   0 loubrieu   (502) staff       (20)        8 2023-06-21 18:43:07.000000 pds.api-client-1.3.0/pds.api_client.egg-info/top_level.txt
+-rw-r--r--   0 loubrieu   (502) staff       (20)      614 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/pyproject.toml
+-rw-r--r--   0 loubrieu   (502) staff       (20)       69 2023-06-21 18:43:07.305742 pds.api-client-1.3.0/setup.cfg
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1769 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/setup.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.281138 pds.api-client-1.3.0/src/
+-rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-03-02 23:53:30.000000 pds.api-client-1.3.0/src/__init__.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.281682 pds.api-client-1.3.0/src/pds/
+-rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-03-02 23:53:30.000000 pds.api-client-1.3.0/src/pds/__init__.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.283110 pds.api-client-1.3.0/src/pds/api_client/
+-rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-03-02 23:53:30.000000 pds.api-client-1.3.0/src/pds/api_client/__init__.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.285816 pds.api-client-1.3.0/src/pds/api_client/demo/
+-rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-06-09 16:52:26.000000 pds.api-client-1.3.0/src/pds/api_client/demo/__init__.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)      901 2023-06-16 20:48:21.000000 pds.api-client-1.3.0/src/pds/api_client/demo/client-demo.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)      836 2023-06-09 17:54:41.000000 pds.api-client-1.3.0/src/pds/api_client/demo/get_messenger_mdis_products.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2116 2023-06-21 18:40:00.000000 pds.api-client-1.3.0/src/pds/api_client/preprocess_openapi.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.286869 pds.api-client-1.3.0/src/pds/api_client/test/
+-rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-03-02 23:53:30.000000 pds.api-client-1.3.0/src/pds/api_client/test/__init__.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.289323 pds.api-client-1.3.0/src/pds/api_client/test/integration/
+-rw-r--r--   0 loubrieu   (502) staff       (20)        0 2023-03-02 23:53:30.000000 pds.api-client-1.3.0/src/pds/api_client/test/integration/__init__.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     3042 2023-06-20 21:49:18.000000 pds.api-client-1.3.0/src/pds/api_client/test/integration/test_collections.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2472 2023-06-20 21:41:18.000000 pds.api-client-1.3.0/src/pds/api_client/test/integration/test_collections_of_bundle.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)      706 2023-06-20 21:40:33.000000 pds.api-client-1.3.0/src/pds/api_client/test/integration/test_products.py
+drwxr-xr-x   0 loubrieu   (502) staff       (20)        0 2023-06-21 18:43:07.303348 pds.api-client-1.3.0/test/
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2256 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_all_products_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1580 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_by_product_classes_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     6403 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_deprecated_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1847 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_error_message.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1891 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_metadata.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2706 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds4_metadata.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2085 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds4_metadata_ops_data_file.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2111 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds4_metadata_ops_label_file_info.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1952 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds4_metadata_ops_tracking_meta.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2927 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds4_product.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     5533 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds4_products.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     3541 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds_product.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     5945 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_pds_products.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2767 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_product_references_api.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1858 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_reference.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1952 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_summary.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     2224 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_wyriwyg_product.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     1955 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_wyriwyg_product_key_value_pair.py
+-rw-r--r--   0 loubrieu   (502) staff       (20)     3365 2023-06-21 18:42:12.000000 pds.api-client-1.3.0/test/test_wyriwyg_products.py
```

### Comparing `pds.api-client-1.2.0/LICENSE.txt` & `pds.api-client-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pds.api-client-1.2.0/NOTICE.txt` & `pds.api-client-1.3.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `pds.api-client-1.2.0/PKG-INFO` & `pds.api-client-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pds.api-client
-Version: 1.2.0
-Summary: Registry API
+Version: 1.3.0
+Summary: PDS Registry Search API
 Home-page: UNKNOWN
 Author: OpenAPI Generator community
 Author-email: pds-operator@jpl.nasa.gov
 License: Apache 2.0
-Keywords: OpenAPI,OpenAPI-Generator,Registry API
+Keywords: OpenAPI,OpenAPI-Generator,PDS Registry Search API
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
-    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product). The detailed syntax for querying the end-point is given in the reference documentation.   # noqa: E501
+    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product).   # noqa: E501
```

### Comparing `pds.api-client-1.2.0/pds/api_client/__init__.py` & `pds.api-client-1.3.0/pds/api_client/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
-    Registry API
+    PDS Registry Search API
 
-    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product). The detailed syntax for querying the end-point is given in the reference documentation.   # noqa: E501
+    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product).   # noqa: E501
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: pds-operator@jpl.nasa.gov
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-__version__ = "1.2.0"
-
-# import ApiClient
-from pds.api_client.api_client import ApiClient
+    Do not edit the class manually.
+"""
 
-# import Configuration
-from pds.api_client.configuration import Configuration
 
-# import exceptions
-from pds.api_client.exceptions import OpenApiException
-from pds.api_client.exceptions import ApiAttributeError
-from pds.api_client.exceptions import ApiTypeError
-from pds.api_client.exceptions import ApiValueError
-from pds.api_client.exceptions import ApiKeyError
-from pds.api_client.exceptions import ApiException
+# import models into model package
+from pds.api_client.models.error_message import ErrorMessage
+from pds.api_client.models.metadata import Metadata
+from pds.api_client.models.pds4_metadata import Pds4Metadata
+from pds.api_client.models.pds4_metadata_ops_data_file import Pds4MetadataOpsDataFile
+from pds.api_client.models.pds4_metadata_ops_label_file_info import Pds4MetadataOpsLabelFileInfo
+from pds.api_client.models.pds4_metadata_ops_tracking_meta import Pds4MetadataOpsTrackingMeta
+from pds.api_client.models.pds4_product import Pds4Product
+from pds.api_client.models.pds4_products import Pds4Products
+from pds.api_client.models.pds_product import PdsProduct
+from pds.api_client.models.pds_products import PdsProducts
+from pds.api_client.models.reference import Reference
+from pds.api_client.models.summary import Summary
+from pds.api_client.models.wyriwyg_product import WyriwygProduct
+from pds.api_client.models.wyriwyg_product_key_value_pair import WyriwygProductKeyValuePair
+from pds.api_client.models.wyriwyg_products import WyriwygProducts
```

### Comparing `pds.api-client-1.2.0/pds/api_client/configuration.py` & `pds.api-client-1.3.0/pds/api_client/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,101 +1,78 @@
 # coding: utf-8
 
 """
-    Registry API
+    PDS Registry Search API
 
-    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product). The detailed syntax for querying the end-point is given in the reference documentation.   # noqa: E501
+    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product).   # noqa: E501
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: pds-operator@jpl.nasa.gov
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
+import http.client as httplib
 from pds.api_client.exceptions import ApiValueError
 
-
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems',
-    'uniqueItems', 'maxProperties', 'minProperties',
+    'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """This class contains various settings of the API client.
 
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
-
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format.
 
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
-                 discard_unknown_keys=False,
-                 disabled_client_side_validations="",
+                 access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
+                 ssl_ca_cert=None,
                  ):
         """Constructor
         """
-        self._base_path = "https://pds.nasa.gov/api/registry/1.0" if host is None else host
+        self._base_path = "https://pds.nasa.gov/api/registry/1" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -121,16 +98,17 @@
         """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
-        self.discard_unknown_keys = discard_unknown_keys
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("pds.api_client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -149,15 +127,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = None
+        self.ssl_ca_cert = ssl_ca_cert
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -185,16 +163,25 @@
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -204,46 +191,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -289,23 +279,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -370,26 +360,26 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.1\n"\
-               "SDK Package Version: 1.2.0".\
+               "Version of the API: 1.1.1\n"\
+               "SDK Package Version: 1.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://pds.nasa.gov/api/registry/1.0",
+                'url': "https://pds.nasa.gov/api/registry/1",
                 'description': "production server",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `pds.api-client-1.2.0/pds/api_client/exceptions.py` & `pds.api-client-1.3.0/pds/api_client/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # coding: utf-8
 
 """
-    Registry API
+    PDS Registry Search API
 
-    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product). The detailed syntax for querying the end-point is given in the reference documentation.   # noqa: E501
+    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product).   # noqa: E501
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: pds-operator@jpl.nasa.gov
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
@@ -96,20 +98,20 @@
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
 class ApiException(OpenApiException):
 
-    def __init__(self, status=None, reason=None, api_response: 'pds.api_client.api_client.ApiResponse' = None):
-        if api_response:
-            self.status = api_response.response.status
-            self.reason = api_response.response.reason
-            self.body = api_response.response.data
-            self.headers = api_response.response.getheaders()
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
 
     def __str__(self):
@@ -122,14 +124,38 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
+
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `pds.api-client-1.2.0/pds.api_client.egg-info/PKG-INFO` & `pds.api-client-1.3.0/pds.api_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pds.api-client
-Version: 1.2.0
-Summary: Registry API
+Version: 1.3.0
+Summary: PDS Registry Search API
 Home-page: UNKNOWN
 Author: OpenAPI Generator community
 Author-email: pds-operator@jpl.nasa.gov
 License: Apache 2.0
-Keywords: OpenAPI,OpenAPI-Generator,Registry API
+Keywords: OpenAPI,OpenAPI-Generator,PDS Registry Search API
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
-    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product). The detailed syntax for querying the end-point is given in the reference documentation.   # noqa: E501
+    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product).   # noqa: E501
```

### Comparing `pds.api-client-1.2.0/setup.py` & `pds.api-client-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # coding: utf-8
 
 """
-    Registry API
+    PDS Registry Search API
 
-    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product). The detailed syntax for querying the end-point is given in the reference documentation.   # noqa: E501
+    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product).   # noqa: E501
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: pds-operator@jpl.nasa.gov
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 from setuptools import setup, find_packages  # noqa: H301
 
-NAME = "pds.api-client"
-VERSION = "1.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
-
+NAME = "pds.api-client"
+VERSION = "1.3.0"
+PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
-    "certifi >= 14.5.14",
-    "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
-    "setuptools >= 21.0.0",
-    "typing_extensions ~= 4.3.0",
-    "urllib3 ~= 1.26.7",
+    "urllib3 >= 1.25.3",
+    "python-dateutil",
+    "pydantic",
+    "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
-    description="Registry API",
+    description="PDS Registry Search API",
     author="OpenAPI Generator community",
     author_email="pds-operator@jpl.nasa.gov",
     url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Registry API"],
-    python_requires=">=3.7",
+    keywords=["OpenAPI", "OpenAPI-Generator", "PDS Registry Search API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Apache 2.0",
+    long_description_content_type='text/markdown',
     long_description="""\
-    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product). The detailed syntax for querying the end-point is given in the reference documentation.   # noqa: E501
+    Registry API enabling advanced search on PDS data and metadata. The API provides end-points to search for bundles, collections and any PDS products with advanced search queries. It also enables to browse the archive hierarchically downward (e.g. collection/s products) or upward (e.g. bundles containing a product).   # noqa: E501
     """
 )
```

### Comparing `pds.api-client-1.2.0/src/pds/api_client/test/integration/test_bundles.py` & `pds.api-client-1.3.0/src/pds/api_client/test/integration/test_collections.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 import unittest
 from pds.api_client import Configuration
 from pds.api_client import ApiClient
-from pds.api_client.apis.paths.bundles_identifier_collections_all import BundlesIdentifierCollectionsAll
-from pds.api_client.apis.paths.classes_class_identifier_members import ClassesClassIdentifierMembers
+from pds.api_client.api.by_product_classes_api import ByProductClassesApi
+from pds.api_client.api.all_products_api import AllProductsApi
+from pds.api_client.models.pds4_products import Pds4Products
+
+
+class CollectionsApiTestCase(unittest.TestCase):
 
-class MyTestCase(unittest.TestCase):
     def setUp(self):
         # create an instance of the API class
         configuration = Configuration()
         configuration.host = 'http://localhost:8080'
         api_client = ApiClient(configuration)
-        self.bundlesCollections = ClassesClassIdentifierMembers(api_client)
+        self.product_by_class = ByProductClassesApi(api_client)
+        self.all_products = AllProductsApi(api_client)
 
-    def test_collections_of_a_bundle_default(self):
+    def test_all_collections(self):
 
-        results = self.bundlesCollections.get(
-            path_params={
-                'class': 'bundles',
-                'identifier': 'urn:nasa:pds:insight_rad::2.1'
-            },
-            query_params={'fields': ['ops:Data_File_Info.ops:file_ref']},
-            accept_content_types=('application/json',)
+        api_response = self.product_by_class.class_list(
+            'collections',
+            start=0,
+            limit=10
+        )
+
+        assert len(api_response.data) == 1
+        assert api_response.summary.hits == 1
+
+        assert all([hasattr(c, 'id') for c in api_response.data])
+
+        # select one collection with lidvid 'urn:nasa:pds:insight_rad:data_calibrated::7.0'
+        collection = [c for c in api_response.data if c.id == 'urn:nasa:pds:mars2020.spice:spice_kernels::3.0'][0]
+        assert hasattr(collection, 'type')
+        assert collection.type == 'Product_Collection'
+
+        assert hasattr(collection, 'title')
+        assert collection.title == "Mars 2020 Perseverance Rover Mission SPICE Kernel Collection"
+
+    def test_all_collections_one_property(self):
+        api_response = self.product_by_class.class_list(
+            'collections',
+            start=0,
+            limit=20,
+            fields=['ops:Label_File_Info.ops:file_ref']
+        )
+
+        assert hasattr(api_response, "data")
+
+        collections_expected_labels = iter([
+            "http://localhost:81/archive//custom-datasets/naif3/spice_kernels/collection_spice_kernels_v003.xml"
+        ])
+
+        for collection in api_response.data:
+            urls = collection.properties['ops:Label_File_Info.ops:file_ref']
+            assert next(collections_expected_labels) in urls[0]
+
+    def test_collection_by_lidvid_all(self):
+        collections = self.all_products.select_by_lidvid_all('urn:nasa:pds:mars2020.spice:spice_kernels')
+        assert hasattr(collections, 'data')
+        assert len(collections.data) > 0
+        assert hasattr(collections.data[0], 'id')
+        assert collections.data[0].id == 'urn:nasa:pds:mars2020.spice:spice_kernels::3.0'
+
+    @unittest.skip("Does not work with the latest version of the openapi generator")
+    def test_collection_by_lidvid_all_content_type(self):
+        collections: Pds4Products = self.product_identifier_all.get(
+            path_params={'identifier': 'urn:nasa:pds:insight_rad:data_derived::7.0'},
+            accept_content_types=('application/vnd.nasa.pds.pds4+json',)
         ).body
-        for collection in results.data:
-            urls = collection['properties']['ops:Data_File_Info.ops:file_ref']
-            for url in urls:
-                print(url)
-
-    def test_all_collections_of_a_bundle_as_deep_archive_does(self):
-
-        def get_collections(bundle_lidvid):
-            _apiquerylimit = 50
-            _propdataurl = "ops:Data_File_Info.ops:file_ref"
-            _propdatamd5 = "ops:Data_File_Info.ops:md5_checksum"
-            _proplabelurl = "ops:Label_File_Info.ops:file_ref"
-            _proplabelmd5 = "ops:Label_File_Info.ops:md5_checksum"
-            _fields = [_propdataurl, _propdatamd5, _proplabelurl, _proplabelmd5]
-
-            start = 0
-
-            found_something = True
-            while found_something:
-                page = self.bundlesCollections.get(
-                    path_params={
-                        'class': 'bundles',
-                        'identifier': bundle_lidvid
-                    },
-                    query_params={'start': start, 'limit':_apiquerylimit, 'fields': _fields},
-                    accept_content_types=('application/json',)
-                ).body
-
-                found_something = False
-                for c in page.data:
-                    found_something = True
-                    yield c
-                start += len(page.data)
-
-        n = 0
-        for collection in get_collections("urn:nasa:pds:insight_rad::2.1"):
-            print(collection['id'])
-            n += 1
-
-        assert n == 2  # 2 collections found in this bundle
-
+        assert 'data' in collections
+        assert len(collections.data) > 0
+        assert 'pds4' in collections['data'][0]
+        
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pds.api-client-1.2.0/test/test_paths/test_products_identifier_members_versions/test_get.py` & `pds.api-client-1.3.0/src/pds/api_client/demo/get_messenger_mdis_products.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,26 @@
-# coding: utf-8
+from __future__ import print_function
+from pds.api_client.rest import ApiException
+from pds.api_client import Configuration
+from pds.api_client import ApiClient
+from pds.api_client.api.product_references_api import ProductReferencesApi
+from pprint import pprint
+
+# create an instance of the API class
+configuration = Configuration()
+configuration.host = 'https://pds.nasa.gov/api/search/1'
+api_client = ApiClient(configuration)
+
+
+product_references = ProductReferencesApi(api_client)
+
+try:
+    # search product of collection urn:nasa:pds:messenger_mdis_2001
+    api_response = product_references.product_members(
+        'urn:nasa:pds:messenger_mdis_2001',
+        start=0,
+        limit=10
+    )
+    pprint(api_response['summary'])
 
-"""
-
-
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-from unittest.mock import patch
-
-import urllib3
-
-import pds.api_client
-from pds.api_client.paths.products_identifier_members_versions import get  # noqa: E501
-from pds.api_client import configuration, schemas, api_client
-
-from .. import ApiTestMixin
-
-
-class TestProductsIdentifierMembersVersions(ApiTestMixin, unittest.TestCase):
-    """
-    ProductsIdentifierMembersVersions unit test stubs
-        returns all of the members of the given lid/lidvid   # noqa: E501
-    """
-    _configuration = configuration.Configuration()
-
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    response_status = 200
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-if __name__ == '__main__':
-    unittest.main()
+except ApiException as e:
+    print("Exception when calling CollectionsApi->get_collection: %s\n" % e)
```

