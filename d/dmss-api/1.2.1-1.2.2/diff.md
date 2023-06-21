# Comparing `tmp/dmss-api-1.2.1.tar.gz` & `tmp/dmss-api-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmss-api-1.2.1.tar", last modified: Thu Mar 30 06:52:09 2023, max compression
+gzip compressed data, was "dmss-api-1.2.2.tar", last modified: Wed Jun 21 09:56:55 2023, max compression
```

## Comparing `dmss-api-1.2.1.tar` & `dmss-api-1.2.2.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.050015 dmss-api-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      374 2023-03-30 06:52:09.050015 dmss-api-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12534 2023-03-30 06:52:08.000000 dmss-api-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.030015 dmss-api-1.2.1/dmss_api/
--rw-r--r--   0 root         (0) root         (0)      675 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.038015 dmss-api-1.2.1/dmss_api/api/
--rw-r--r--   0 root         (0) root         (0)      218 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11182 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/access_control_api.py
--rw-r--r--   0 root         (0) root         (0)    10827 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/blob_api.py
--rw-r--r--   0 root         (0) root         (0)    10499 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/blueprint_api.py
--rw-r--r--   0 root         (0) root         (0)    14478 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/datasource_api.py
--rw-r--r--   0 root         (0) root         (0)   150401 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    41403 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/document_api.py
--rw-r--r--   0 root         (0) root         (0)    10544 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/entity_api.py
--rw-r--r--   0 root         (0) root         (0)    10306 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/export_api.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/health_check_api.py
--rw-r--r--   0 root         (0) root         (0)    10243 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/lookup_table_api.py
--rw-r--r--   0 root         (0) root         (0)    13697 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/personal_access_token_api.py
--rw-r--r--   0 root         (0) root         (0)    11622 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/reference_api.py
--rw-r--r--   0 root         (0) root         (0)     6429 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/search_api.py
--rw-r--r--   0 root         (0) root         (0)     5000 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api/whoami_api.py
--rw-r--r--   0 root         (0) root         (0)    36751 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.042015 dmss-api-1.2.1/dmss_api/apis/
--rw-r--r--   0 root         (0) root         (0)     1157 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17221 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5045 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.046015 dmss-api-1.2.1/dmss_api/model/
--rw-r--r--   0 root         (0) root         (0)      348 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11900 2023-03-30 06:52:07.000000 dmss-api-1.2.1/dmss_api/model/access_level.py
--rw-r--r--   0 root         (0) root         (0)    12074 2023-03-30 06:52:07.000000 dmss-api-1.2.1/dmss_api/model/acl.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-03-30 06:52:07.000000 dmss-api-1.2.1/dmss_api/model/data_source_information.py
--rw-r--r--   0 root         (0) root         (0)    11544 2023-03-30 06:52:07.000000 dmss-api-1.2.1/dmss_api/model/data_source_request.py
--rw-r--r--   0 root         (0) root         (0)    11219 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/entity.py
--rw-r--r--   0 root         (0) root         (0)    12703 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)    12292 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/get_blueprint_response.py
--rw-r--r--   0 root         (0) root         (0)    12227 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/lookup.py
--rw-r--r--   0 root         (0) root         (0)    12532 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/pat_data.py
--rw-r--r--   0 root         (0) root         (0)    14036 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/recipe.py
--rw-r--r--   0 root         (0) root         (0)    13139 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/recipe_attribute.py
--rw-r--r--   0 root         (0) root         (0)    11779 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/reference.py
--rw-r--r--   0 root         (0) root         (0)    13481 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/repository.py
--rw-r--r--   0 root         (0) root         (0)    12059 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/repository_type.py
--rw-r--r--   0 root         (0) root         (0)    12590 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/storage_attribute.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/storage_data_types.py
--rw-r--r--   0 root         (0) root         (0)    12532 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model/storage_recipe.py
--rw-r--r--   0 root         (0) root         (0)    80121 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.046015 dmss-api-1.2.1/dmss_api/models/
--rw-r--r--   0 root         (0) root         (0)     1284 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12643 2023-03-30 06:52:08.000000 dmss-api-1.2.1/dmss_api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.034015 dmss-api-1.2.1/dmss_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      374 2023-03-30 06:52:09.000000 dmss-api-1.2.1/dmss_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2230 2023-03-30 06:52:09.000000 dmss-api-1.2.1/dmss_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 06:52:09.000000 dmss-api-1.2.1/dmss_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-03-30 06:52:09.000000 dmss-api-1.2.1/dmss_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-30 06:52:09.000000 dmss-api-1.2.1/dmss_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-03-30 06:52:09.050015 dmss-api-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1011 2023-03-30 06:52:08.000000 dmss-api-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:52:09.050015 dmss-api-1.2.1/test/
--rw-r--r--   0 root         (0) root         (0)      799 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_access_control_api.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-03-30 06:52:07.000000 dmss-api-1.2.1/test/test_access_level.py
--rw-r--r--   0 root         (0) root         (0)      738 2023-03-30 06:52:07.000000 dmss-api-1.2.1/test/test_acl.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_blob_api.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_blueprint_api.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-03-30 06:52:07.000000 dmss-api-1.2.1/test/test_data_source_information.py
--rw-r--r--   0 root         (0) root         (0)      833 2023-03-30 06:52:07.000000 dmss-api-1.2.1/test/test_data_source_request.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_datasource_api.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_default_api.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_document_api.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_entity.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_entity_api.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_export_api.py
--rw-r--r--   0 root         (0) root         (0)      768 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_get_blueprint_response.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_health_check_api.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_lookup.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_lookup_table_api.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_pat_data.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_personal_access_token_api.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_recipe.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_recipe_attribute.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_reference.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_reference_api.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_repository.py
--rw-r--r--   0 root         (0) root         (0)      725 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_repository_type.py
--rw-r--r--   0 root         (0) root         (0)      642 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_search_api.py
--rw-r--r--   0 root         (0) root         (0)      739 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_storage_attribute.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_storage_data_types.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_storage_recipe.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-03-30 06:52:08.000000 dmss-api-1.2.1/test/test_whoami_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.866175 dmss-api-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-21 09:56:55.870175 dmss-api-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11760 2023-06-21 09:56:54.000000 dmss-api-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.842173 dmss-api-1.2.2/dmss_api/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.850174 dmss-api-1.2.2/dmss_api/api/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11182 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/access_control_api.py
+-rw-r--r--   0 root         (0) root         (0)     5345 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/attribute_api.py
+-rw-r--r--   0 root         (0) root         (0)    10827 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/blob_api.py
+-rw-r--r--   0 root         (0) root         (0)    10499 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/blueprint_api.py
+-rw-r--r--   0 root         (0) root         (0)    14478 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/datasource_api.py
+-rw-r--r--   0 root         (0) root         (0)   140550 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    27059 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/document_api.py
+-rw-r--r--   0 root         (0) root         (0)    10544 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/entity_api.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/export_api.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/health_check_api.py
+-rw-r--r--   0 root         (0) root         (0)    10424 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/lookup_table_api.py
+-rw-r--r--   0 root         (0) root         (0)    13697 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/personal_access_token_api.py
+-rw-r--r--   0 root         (0) root         (0)    11622 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/reference_api.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/search_api.py
+-rw-r--r--   0 root         (0) root         (0)     5000 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/whoami_api.py
+-rw-r--r--   0 root         (0) root         (0)    36751 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.850174 dmss-api-1.2.2/dmss_api/apis/
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17221 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.858174 dmss-api-1.2.2/dmss_api/model/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11900 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/access_level.py
+-rw-r--r--   0 root         (0) root         (0)    12074 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/acl.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/data_source_information.py
+-rw-r--r--   0 root         (0) root         (0)    11544 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/data_source_request.py
+-rw-r--r--   0 root         (0) root         (0)    11219 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/entity.py
+-rw-r--r--   0 root         (0) root         (0)    12703 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)    12292 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/get_blueprint_response.py
+-rw-r--r--   0 root         (0) root         (0)    12227 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/lookup.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/pat_data.py
+-rw-r--r--   0 root         (0) root         (0)    14036 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/recipe.py
+-rw-r--r--   0 root         (0) root         (0)    13139 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/recipe_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    11750 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/reference.py
+-rw-r--r--   0 root         (0) root         (0)    13481 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/repository.py
+-rw-r--r--   0 root         (0) root         (0)    12059 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/repository_type.py
+-rw-r--r--   0 root         (0) root         (0)    12590 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/storage_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/storage_data_types.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/storage_recipe.py
+-rw-r--r--   0 root         (0) root         (0)    80121 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.858174 dmss-api-1.2.2/dmss_api/models/
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12643 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.842173 dmss-api-1.2.2/dmss_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-21 09:56:55.870175 dmss-api-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-06-21 09:56:54.000000 dmss-api-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.866175 dmss-api-1.2.2/test/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_access_control_api.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_access_level.py
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_acl.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_attribute_api.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_blob_api.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_blueprint_api.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_data_source_information.py
+-rw-r--r--   0 root         (0) root         (0)      833 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_data_source_request.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_datasource_api.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_default_api.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_document_api.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_entity.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_entity_api.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_export_api.py
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_get_blueprint_response.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_health_check_api.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_lookup.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_lookup_table_api.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_pat_data.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_personal_access_token_api.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_recipe.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_recipe_attribute.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_reference.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_reference_api.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_repository.py
+-rw-r--r--   0 root         (0) root         (0)      725 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_repository_type.py
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_search_api.py
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_storage_attribute.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_storage_data_types.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_storage_recipe.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_whoami_api.py
```

### Comparing `dmss-api-1.2.1/README.md` & `dmss-api-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # dmss-api
 API for basic data modelling interaction
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 1.2.1
+- Package version: 1.2.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
@@ -95,64 +95,60 @@
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AccessControlApi* | [**get_acl**](docs/AccessControlApi.md#get_acl) | **GET** /api/acl/{data_source_id}/{document_id} | Get Acl
 *AccessControlApi* | [**set_acl**](docs/AccessControlApi.md#set_acl) | **PUT** /api/acl/{data_source_id}/{document_id} | Set Acl
+*AttributeApi* | [**attribute_get**](docs/AttributeApi.md#attribute_get) | **GET** /api/attribute/{reference} | Get Attribute
 *BlobApi* | [**blob_get_by_id**](docs/BlobApi.md#blob_get_by_id) | **GET** /api/blobs/{data_source_id}/{blob_id} | Get By Id
 *BlobApi* | [**blob_upload**](docs/BlobApi.md#blob_upload) | **PUT** /api/blobs/{data_source_id}/{blob_id} | Upload
 *BlueprintApi* | [**blueprint_get**](docs/BlueprintApi.md#blueprint_get) | **GET** /api/blueprint/{type_ref} | Get Blueprint
 *BlueprintApi* | [**blueprint_resolve**](docs/BlueprintApi.md#blueprint_resolve) | **GET** /api/resolve-path/{absolute_id} | Resolve Blueprint Id
 *DatasourceApi* | [**data_source_get**](docs/DatasourceApi.md#data_source_get) | **GET** /api/data-sources/{data_source_id} | Get
 *DatasourceApi* | [**data_source_get_all**](docs/DatasourceApi.md#data_source_get_all) | **GET** /api/data-sources | Get All
 *DatasourceApi* | [**data_source_save**](docs/DatasourceApi.md#data_source_save) | **POST** /api/data-sources/{data_source_id} | Save
+*DefaultApi* | [**attribute_get**](docs/DefaultApi.md#attribute_get) | **GET** /api/attribute/{reference} | Get Attribute
 *DefaultApi* | [**blob_get_by_id**](docs/DefaultApi.md#blob_get_by_id) | **GET** /api/blobs/{data_source_id}/{blob_id} | Get By Id
 *DefaultApi* | [**blob_upload**](docs/DefaultApi.md#blob_upload) | **PUT** /api/blobs/{data_source_id}/{blob_id} | Upload
 *DefaultApi* | [**blueprint_get**](docs/DefaultApi.md#blueprint_get) | **GET** /api/blueprint/{type_ref} | Get Blueprint
 *DefaultApi* | [**blueprint_resolve**](docs/DefaultApi.md#blueprint_resolve) | **GET** /api/resolve-path/{absolute_id} | Resolve Blueprint Id
 *DefaultApi* | [**create_lookup**](docs/DefaultApi.md#create_lookup) | **POST** /api/application/{application} | Create Lookup
 *DefaultApi* | [**data_source_get**](docs/DefaultApi.md#data_source_get) | **GET** /api/data-sources/{data_source_id} | Get
 *DefaultApi* | [**data_source_get_all**](docs/DefaultApi.md#data_source_get_all) | **GET** /api/data-sources | Get All
 *DefaultApi* | [**data_source_save**](docs/DefaultApi.md#data_source_save) | **POST** /api/data-sources/{data_source_id} | Save
-*DefaultApi* | [**document_add**](docs/DefaultApi.md#document_add) | **POST** /api/documents/{absolute_ref} | Add By Parent Id
-*DefaultApi* | [**document_add_simple**](docs/DefaultApi.md#document_add_simple) | **POST** /api/documents/{data_source_id}/add-raw | Add Raw
-*DefaultApi* | [**document_add_to_path**](docs/DefaultApi.md#document_add_to_path) | **POST** /api/documents-by-path/{path_reference} | Add To Path
-*DefaultApi* | [**document_get_by_id**](docs/DefaultApi.md#document_get_by_id) | **GET** /api/documents/{id_reference} | Get By Id
-*DefaultApi* | [**document_get_by_path**](docs/DefaultApi.md#document_get_by_path) | **GET** /api/documents-by-path/{absolute_path} | Get By Path
-*DefaultApi* | [**document_remove**](docs/DefaultApi.md#document_remove) | **DELETE** /api/documents/{id_reference} | Remove
-*DefaultApi* | [**document_remove_by_path**](docs/DefaultApi.md#document_remove_by_path) | **DELETE** /api/documents-by-path/{path_reference} | Remove By Path
+*DefaultApi* | [**document_add**](docs/DefaultApi.md#document_add) | **POST** /api/documents/{reference} | Add Document
+*DefaultApi* | [**document_add_simple**](docs/DefaultApi.md#document_add_simple) | **POST** /api/documents-add-raw/{data_source_id} | Add Raw
+*DefaultApi* | [**document_get**](docs/DefaultApi.md#document_get) | **GET** /api/documents/{reference} | Get
+*DefaultApi* | [**document_remove**](docs/DefaultApi.md#document_remove) | **DELETE** /api/documents/{reference} | Remove
 *DefaultApi* | [**document_update**](docs/DefaultApi.md#document_update) | **PUT** /api/documents/{id_reference} | Update
-*DefaultApi* | [**export**](docs/DefaultApi.md#export) | **GET** /api/export/{absolute_document_ref} | Export
-*DefaultApi* | [**export_meta**](docs/DefaultApi.md#export_meta) | **GET** /api/export/meta/{absolute_document_ref} | Export Meta
+*DefaultApi* | [**export**](docs/DefaultApi.md#export) | **GET** /api/export/{reference} | Export
+*DefaultApi* | [**export_meta**](docs/DefaultApi.md#export_meta) | **GET** /api/export/meta/{reference} | Export Meta
 *DefaultApi* | [**get_acl**](docs/DefaultApi.md#get_acl) | **GET** /api/acl/{data_source_id}/{document_id} | Get Acl
 *DefaultApi* | [**get_api_healthcheck_get**](docs/DefaultApi.md#get_api_healthcheck_get) | **GET** /api/healthcheck | Get
 *DefaultApi* | [**get_lookup**](docs/DefaultApi.md#get_lookup) | **GET** /api/application/{application} | Get Lookup
 *DefaultApi* | [**instantiate_entity**](docs/DefaultApi.md#instantiate_entity) | **POST** /api/entity | Instantiate
 *DefaultApi* | [**reference_delete**](docs/DefaultApi.md#reference_delete) | **DELETE** /api/reference/{data_source_id}/{document_dotted_id} | Delete Reference
 *DefaultApi* | [**reference_insert**](docs/DefaultApi.md#reference_insert) | **PUT** /api/reference/{data_source_id}/{document_dotted_id} | Insert Reference
 *DefaultApi* | [**search**](docs/DefaultApi.md#search) | **POST** /api/search | Search
 *DefaultApi* | [**set_acl**](docs/DefaultApi.md#set_acl) | **PUT** /api/acl/{data_source_id}/{document_id} | Set Acl
 *DefaultApi* | [**token_create**](docs/DefaultApi.md#token_create) | **POST** /api/token | New Personal Access Token
 *DefaultApi* | [**token_delete**](docs/DefaultApi.md#token_delete) | **DELETE** /api/token/{token_id} | Revoke Personal Access Token
 *DefaultApi* | [**token_list_all**](docs/DefaultApi.md#token_list_all) | **GET** /api/token | List All Pats
 *DefaultApi* | [**validate_entity**](docs/DefaultApi.md#validate_entity) | **POST** /api/entity/validate | Validate
 *DefaultApi* | [**whoami**](docs/DefaultApi.md#whoami) | **GET** /api/whoami | Get Information On Authenticated User
-*DocumentApi* | [**document_add**](docs/DocumentApi.md#document_add) | **POST** /api/documents/{absolute_ref} | Add By Parent Id
-*DocumentApi* | [**document_add_simple**](docs/DocumentApi.md#document_add_simple) | **POST** /api/documents/{data_source_id}/add-raw | Add Raw
-*DocumentApi* | [**document_add_to_path**](docs/DocumentApi.md#document_add_to_path) | **POST** /api/documents-by-path/{path_reference} | Add To Path
-*DocumentApi* | [**document_get_by_id**](docs/DocumentApi.md#document_get_by_id) | **GET** /api/documents/{id_reference} | Get By Id
-*DocumentApi* | [**document_get_by_path**](docs/DocumentApi.md#document_get_by_path) | **GET** /api/documents-by-path/{absolute_path} | Get By Path
-*DocumentApi* | [**document_remove**](docs/DocumentApi.md#document_remove) | **DELETE** /api/documents/{id_reference} | Remove
-*DocumentApi* | [**document_remove_by_path**](docs/DocumentApi.md#document_remove_by_path) | **DELETE** /api/documents-by-path/{path_reference} | Remove By Path
+*DocumentApi* | [**document_add**](docs/DocumentApi.md#document_add) | **POST** /api/documents/{reference} | Add Document
+*DocumentApi* | [**document_add_simple**](docs/DocumentApi.md#document_add_simple) | **POST** /api/documents-add-raw/{data_source_id} | Add Raw
+*DocumentApi* | [**document_get**](docs/DocumentApi.md#document_get) | **GET** /api/documents/{reference} | Get
+*DocumentApi* | [**document_remove**](docs/DocumentApi.md#document_remove) | **DELETE** /api/documents/{reference} | Remove
 *DocumentApi* | [**document_update**](docs/DocumentApi.md#document_update) | **PUT** /api/documents/{id_reference} | Update
 *EntityApi* | [**instantiate_entity**](docs/EntityApi.md#instantiate_entity) | **POST** /api/entity | Instantiate
 *EntityApi* | [**validate_entity**](docs/EntityApi.md#validate_entity) | **POST** /api/entity/validate | Validate
-*ExportApi* | [**export**](docs/ExportApi.md#export) | **GET** /api/export/{absolute_document_ref} | Export
-*ExportApi* | [**export_meta**](docs/ExportApi.md#export_meta) | **GET** /api/export/meta/{absolute_document_ref} | Export Meta
+*ExportApi* | [**export**](docs/ExportApi.md#export) | **GET** /api/export/{reference} | Export
+*ExportApi* | [**export_meta**](docs/ExportApi.md#export_meta) | **GET** /api/export/meta/{reference} | Export Meta
 *HealthCheckApi* | [**get_api_healthcheck_get**](docs/HealthCheckApi.md#get_api_healthcheck_get) | **GET** /api/healthcheck | Get
 *LookupTableApi* | [**create_lookup**](docs/LookupTableApi.md#create_lookup) | **POST** /api/application/{application} | Create Lookup
 *LookupTableApi* | [**get_lookup**](docs/LookupTableApi.md#get_lookup) | **GET** /api/application/{application} | Get Lookup
 *PersonalAccessTokenApi* | [**token_create**](docs/PersonalAccessTokenApi.md#token_create) | **POST** /api/token | New Personal Access Token
 *PersonalAccessTokenApi* | [**token_delete**](docs/PersonalAccessTokenApi.md#token_delete) | **DELETE** /api/token/{token_id} | Revoke Personal Access Token
 *PersonalAccessTokenApi* | [**token_list_all**](docs/PersonalAccessTokenApi.md#token_list_all) | **GET** /api/token | List All Pats
 *ReferenceApi* | [**reference_delete**](docs/ReferenceApi.md#reference_delete) | **DELETE** /api/reference/{data_source_id}/{document_dotted_id} | Delete Reference
```

### Comparing `dmss-api-1.2.1/dmss_api/__init__.py` & `dmss-api-1.2.2/dmss_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     API for basic data modelling interaction  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 # import ApiClient
 from dmss_api.api_client import ApiClient
 
 # import Configuration
 from dmss_api.configuration import Configuration
```

### Comparing `dmss-api-1.2.1/dmss_api/api/access_control_api.py` & `dmss-api-1.2.2/dmss_api/api/access_control_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/blob_api.py` & `dmss-api-1.2.2/dmss_api/api/blob_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/blueprint_api.py` & `dmss-api-1.2.2/dmss_api/api/blueprint_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/datasource_api.py` & `dmss-api-1.2.2/dmss_api/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/default_api.py` & `dmss-api-1.2.2/dmss_api/api/default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,135 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+        def __attribute_get(
+            self,
+            reference,
+            **kwargs
+        ):
+            """Get Attribute  # noqa: E501
+
+            Fetch the attribute from a reference.  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.attribute_get(reference, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                reference (str):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (int/float/tuple): timeout setting for this request. If
+                    one number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['reference'] = \
+                reference
+            return self.call_with_http_info(**kwargs)
+
+        self.attribute_get = _Endpoint(
+            settings={
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'auth': [
+                    'APIKeyHeader',
+                    'OAuth2AuthorizationCodeBearer'
+                ],
+                'endpoint_path': '/api/attribute/{reference}',
+                'operation_id': 'attribute_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'reference',
+                ],
+                'required': [
+                    'reference',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'reference':
+                        (str,),
+                },
+                'attribute_map': {
+                    'reference': 'reference',
+                },
+                'location_map': {
+                    'reference': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json',
+                    'text/plain'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client,
+            callable=__attribute_get
+        )
+
         def __blob_get_by_id(
             self,
             data_source_id,
             blob_id,
             **kwargs
         ):
             """Get By Id  # noqa: E501
@@ -579,24 +700,24 @@
             self,
             application,
             recipe_package,
             **kwargs
         ):
             """Create Lookup  # noqa: E501
 
-            Create a recipe lookup table from a package containing RecipeLinks. Associate it with an application. This can be used for setting Ui- and StorageRecipes for specific applications.  - **application**: name of application  # noqa: E501
+            Create a recipe lookup table from a package containing RecipeLinks. Associate it with an application. This can be used for setting Ui- and StorageRecipes for specific applications.  - **application**: name of application - **recipe_package**: List with one or more paths to package(s) that contain recipe links. (Example: 'system/SIMOS/recipe_links')  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.create_lookup(application, recipe_package, async_req=True)
             >>> result = thread.get()
 
             Args:
                 application (str):
-                recipe_package (str):
+                recipe_package ([str]):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -678,25 +799,26 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'application':
                         (str,),
                     'recipe_package':
-                        (str,),
+                        ([str],),
                 },
                 'attribute_map': {
                     'application': 'application',
                     'recipe_package': 'recipe_package',
                 },
                 'location_map': {
                     'application': 'path',
                     'recipe_package': 'query',
                 },
                 'collection_format_map': {
+                    'recipe_package': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
@@ -1066,33 +1188,34 @@
             },
             api_client=api_client,
             callable=__data_source_save
         )
 
         def __document_add(
             self,
-            absolute_ref,
-            body,
+            reference,
+            document,
             **kwargs
         ):
-            """Add By Parent Id  # noqa: E501
+            """Add Document  # noqa: E501
 
-            Add a new document to absolute ref (root of data source, or another document). If added to another document, a valid attribute type check is done. Select parent with format 'data_source/document_id.attribute.index.attribute'  # noqa: E501
+            Add a document to a package (or a data source) using a reference.  - **reference**:   - Reference to data source: PROTOCOL://DATA SOURCE   - Reference to package by id: PROTOCOL://DATA SOURCE/$ID   - Reference to package by path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE   The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_add(absolute_ref, body, async_req=True)
+            >>> thread = api.document_add(reference, document, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_ref (str):
-                body ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+                reference (str):
+                document (str):
 
             Keyword Args:
-                update_uncontained (bool): [optional] if omitted the server will use the default value of True
+                update_uncontained (bool): [optional] if omitted the server will use the default value of False
+                files ([file_type]): [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (int/float/tuple): timeout setting for this request. If
                     one number provided, it will be total request timeout. It can also
@@ -1129,81 +1252,88 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_ref'] = \
-                absolute_ref
-            kwargs['body'] = \
-                body
+            kwargs['reference'] = \
+                reference
+            kwargs['document'] = \
+                document
             return self.call_with_http_info(**kwargs)
 
         self.document_add = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{absolute_ref}',
+                'endpoint_path': '/api/documents/{reference}',
                 'operation_id': 'document_add',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_ref',
-                    'body',
+                    'reference',
+                    'document',
                     'update_uncontained',
+                    'files',
                 ],
                 'required': [
-                    'absolute_ref',
-                    'body',
+                    'reference',
+                    'document',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_ref':
+                    'reference':
+                        (str,),
+                    'document':
                         (str,),
-                    'body':
-                        ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                     'update_uncontained':
                         (bool,),
+                    'files':
+                        ([file_type],),
                 },
                 'attribute_map': {
-                    'absolute_ref': 'absolute_ref',
+                    'reference': 'reference',
+                    'document': 'document',
                     'update_uncontained': 'update_uncontained',
+                    'files': 'files',
                 },
                 'location_map': {
-                    'absolute_ref': 'path',
-                    'body': 'body',
+                    'reference': 'path',
+                    'document': 'form',
                     'update_uncontained': 'query',
+                    'files': 'form',
                 },
                 'collection_format_map': {
+                    'files': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [
-                    'application/json'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client,
             callable=__document_add
         )
 
         def __document_add_simple(
@@ -1279,15 +1409,15 @@
         self.document_add_simple = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{data_source_id}/add-raw',
+                'endpoint_path': '/api/documents-add-raw/{data_source_id}',
                 'operation_id': 'document_add_simple',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'data_source_id',
@@ -1334,179 +1464,34 @@
                     'application/json'
                 ]
             },
             api_client=api_client,
             callable=__document_add_simple
         )
 
-        def __document_add_to_path(
-            self,
-            path_reference,
-            document,
-            **kwargs
-        ):
-            """Add To Path  # noqa: E501
-
-            Same as 'add_to_parent', but reference parent by path instead of ID. Also supports files.  - **path_reference**: <data_source>/<path_to_entity>/<entity_name>.<attribute>  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_add_to_path(path_reference, document, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                path_reference (str):
-                document (str):
-
-            Keyword Args:
-                update_uncontained (bool): [optional] if omitted the server will use the default value of False
-                files ([file_type]): [optional]
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['path_reference'] = \
-                path_reference
-            kwargs['document'] = \
-                document
-            return self.call_with_http_info(**kwargs)
-
-        self.document_add_to_path = _Endpoint(
-            settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents-by-path/{path_reference}',
-                'operation_id': 'document_add_to_path',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'path_reference',
-                    'document',
-                    'update_uncontained',
-                    'files',
-                ],
-                'required': [
-                    'path_reference',
-                    'document',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'path_reference':
-                        (str,),
-                    'document':
-                        (str,),
-                    'update_uncontained':
-                        (bool,),
-                    'files':
-                        ([file_type],),
-                },
-                'attribute_map': {
-                    'path_reference': 'path_reference',
-                    'document': 'document',
-                    'update_uncontained': 'update_uncontained',
-                    'files': 'files',
-                },
-                'location_map': {
-                    'path_reference': 'path',
-                    'document': 'form',
-                    'update_uncontained': 'query',
-                    'files': 'form',
-                },
-                'collection_format_map': {
-                    'files': 'csv',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [
-                    'multipart/form-data'
-                ]
-            },
-            api_client=api_client,
-            callable=__document_add_to_path
-        )
-
-        def __document_get_by_id(
+        def __document_get(
             self,
-            id_reference,
+            reference,
             **kwargs
         ):
-            """Get By Id  # noqa: E501
+            """Get  # noqa: E501
 
-            Get document as JSON string.  - **id_reference**: <data_source>/<document_uuid> - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
+            Get document as JSON string.  - **reference**: A reference to a package or a data source   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)  The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_get_by_id(id_reference, async_req=True)
+            >>> thread = api.document_get(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                id_reference (str):
+                reference (str):
 
             Keyword Args:
-                depth (int): [optional] if omitted the server will use the default value of 999
+                depth (int): [optional] if omitted the server will use the default value of 0
+                resolve_links (bool): [optional] if omitted the server will use the default value of False
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (int/float/tuple): timeout setting for this request. If
                     one number provided, it will be total request timeout. It can also
@@ -1543,215 +1528,99 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
-        self.document_get_by_id = _Endpoint(
+        self.document_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{id_reference}',
-                'operation_id': 'document_get_by_id',
+                'endpoint_path': '/api/documents/{reference}',
+                'operation_id': 'document_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'reference',
                     'depth',
+                    'resolve_links',
                 ],
                 'required': [
-                    'id_reference',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'reference':
                         (str,),
                     'depth':
                         (int,),
+                    'resolve_links':
+                        (bool,),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'reference': 'reference',
                     'depth': 'depth',
+                    'resolve_links': 'resolve_links',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'reference': 'path',
                     'depth': 'query',
+                    'resolve_links': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__document_get_by_id
-        )
-
-        def __document_get_by_path(
-            self,
-            absolute_path,
-            **kwargs
-        ):
-            """Get By Path  # noqa: E501
-
-            Get a document by its absolute path.  - **absolute_path**: <protocol>://<data_source>/<path>.<attribute>  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_get_by_path(absolute_path, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                absolute_path (str):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_path'] = \
-                absolute_path
-            return self.call_with_http_info(**kwargs)
-
-        self.document_get_by_path = _Endpoint(
-            settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents-by-path/{absolute_path}',
-                'operation_id': 'document_get_by_path',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'absolute_path',
-                ],
-                'required': [
-                    'absolute_path',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'absolute_path':
-                        (str,),
-                },
-                'attribute_map': {
-                    'absolute_path': 'absolute_path',
-                },
-                'location_map': {
-                    'absolute_path': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client,
-            callable=__document_get_by_path
+            callable=__document_get
         )
 
         def __document_remove(
             self,
-            id_reference,
+            reference,
             **kwargs
         ):
             """Remove  # noqa: E501
 
-            Remove document - **id_reference**: <data_source>/<document_uuid>.<attribute_path>  Example: id_reference=SomeDataSource/3978d9ca-2d7a-4b47-8fed-57710f6cf50b.attributes.1 will remove the first element in the attribute list of a blueprint with the given id in data source 'SomeDataSource'.  # noqa: E501
+            Remove a document from DMSS.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_remove(id_reference, async_req=True)
+            >>> thread = api.document_remove(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                id_reference (str):
+                reference (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -1767,15 +1636,15 @@
                     Default is True.
                 _host_index (int/None): specifies the index of the server
                     that we want to use.
                     Default is read from the configuration.
                 async_req (bool): execute request asynchronously
 
             Returns:
-                str
+                bool, date, datetime, dict, float, int, list, str, none_type
                     If the method is called asynchronously, returns the request
                     thread.
             """
             kwargs['async_req'] = kwargs.get(
                 'async_req', False
             )
             kwargs['_return_http_data_only'] = kwargs.get(
@@ -1790,58 +1659,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
         self.document_remove = _Endpoint(
             settings={
-                'response_type': (str,),
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{id_reference}',
+                'endpoint_path': '/api/documents/{reference}',
                 'operation_id': 'document_remove',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'reference',
                 ],
                 'required': [
-                    'id_reference',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'reference':
                         (str,),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'reference': 'reference',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'reference': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -1849,135 +1718,14 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client,
             callable=__document_remove
         )
 
-        def __document_remove_by_path(
-            self,
-            path_reference,
-            **kwargs
-        ):
-            """Remove By Path  # noqa: E501
-
-            Remove a document from DMSS.  - **path_reference**: <data_source>/<path>.<attribute>  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_remove_by_path(path_reference, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                path_reference (str):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                bool, date, datetime, dict, float, int, list, str, none_type
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['path_reference'] = \
-                path_reference
-            return self.call_with_http_info(**kwargs)
-
-        self.document_remove_by_path = _Endpoint(
-            settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents-by-path/{path_reference}',
-                'operation_id': 'document_remove_by_path',
-                'http_method': 'DELETE',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'path_reference',
-                ],
-                'required': [
-                    'path_reference',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'path_reference':
-                        (str,),
-                },
-                'attribute_map': {
-                    'path_reference': 'path_reference',
-                },
-                'location_map': {
-                    'path_reference': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client,
-            callable=__document_remove_by_path
-        )
-
         def __document_update(
             self,
             id_reference,
             data,
             **kwargs
         ):
             """Update  # noqa: E501
@@ -2118,28 +1866,28 @@
             },
             api_client=api_client,
             callable=__document_update
         )
 
         def __export(
             self,
-            absolute_document_ref,
+            reference,
             **kwargs
         ):
             """Export  # noqa: E501
 
-            Download a zip-folder with one or more documents as json file(s).  - **absolute_document_ref**: <data_source>/<path>/<document_name>  # noqa: E501
+            Download a zip-folder with one or more documents as json file(s).  - **reference**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export(absolute_document_ref, async_req=True)
+            >>> thread = api.export(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_document_ref (str):
+                reference (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -2178,58 +1926,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_document_ref'] = \
-                absolute_document_ref
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
         self.export = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/{absolute_document_ref}',
+                'endpoint_path': '/api/export/{reference}',
                 'operation_id': 'export',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_document_ref',
+                    'reference',
                 ],
                 'required': [
-                    'absolute_document_ref',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_document_ref':
+                    'reference':
                         (str,),
                 },
                 'attribute_map': {
-                    'absolute_document_ref': 'absolute_document_ref',
+                    'reference': 'reference',
                 },
                 'location_map': {
-                    'absolute_document_ref': 'path',
+                    'reference': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/zip',
@@ -2240,28 +1988,28 @@
             },
             api_client=api_client,
             callable=__export
         )
 
         def __export_meta(
             self,
-            absolute_document_ref,
+            reference,
             **kwargs
         ):
             """Export Meta  # noqa: E501
 
-            Export only the metadata of an entity. An entities metadata is concatenated from the \"top down\". Inheriting parents meta, and overriding for any specified further down.  If no metadata is defined anywhere in the tree, an empty object is returned.  - **absolute_document_ref**: <data_source>/<path_to_entity>/<entity_name>  # noqa: E501
+            Export only the metadata of an entity. An entities metadata is concatenated from the \"top down\". Inheriting parents meta, and overriding for any specified further down.  If no metadata is defined anywhere in the tree, an empty object is returned.  - **reference**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export_meta(absolute_document_ref, async_req=True)
+            >>> thread = api.export_meta(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_document_ref (str):
+                reference (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -2300,58 +2048,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_document_ref'] = \
-                absolute_document_ref
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
         self.export_meta = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/meta/{absolute_document_ref}',
+                'endpoint_path': '/api/export/meta/{reference}',
                 'operation_id': 'export_meta',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_document_ref',
+                    'reference',
                 ],
                 'required': [
-                    'absolute_document_ref',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_document_ref':
+                    'reference':
                         (str,),
                 },
                 'attribute_map': {
-                    'absolute_document_ref': 'absolute_document_ref',
+                    'reference': 'reference',
                 },
                 'location_map': {
-                    'absolute_document_ref': 'path',
+                    'reference': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
```

### Comparing `dmss-api-1.2.1/dmss_api/api/document_api.py` & `dmss-api-1.2.2/dmss_api/api/document_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,33 +34,34 @@
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         def __document_add(
             self,
-            absolute_ref,
-            body,
+            reference,
+            document,
             **kwargs
         ):
-            """Add By Parent Id  # noqa: E501
+            """Add Document  # noqa: E501
 
-            Add a new document to absolute ref (root of data source, or another document). If added to another document, a valid attribute type check is done. Select parent with format 'data_source/document_id.attribute.index.attribute'  # noqa: E501
+            Add a document to a package (or a data source) using a reference.  - **reference**:   - Reference to data source: PROTOCOL://DATA SOURCE   - Reference to package by id: PROTOCOL://DATA SOURCE/$ID   - Reference to package by path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE   The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_add(absolute_ref, body, async_req=True)
+            >>> thread = api.document_add(reference, document, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_ref (str):
-                body ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+                reference (str):
+                document (str):
 
             Keyword Args:
-                update_uncontained (bool): [optional] if omitted the server will use the default value of True
+                update_uncontained (bool): [optional] if omitted the server will use the default value of False
+                files ([file_type]): [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (int/float/tuple): timeout setting for this request. If
                     one number provided, it will be total request timeout. It can also
@@ -97,81 +98,88 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_ref'] = \
-                absolute_ref
-            kwargs['body'] = \
-                body
+            kwargs['reference'] = \
+                reference
+            kwargs['document'] = \
+                document
             return self.call_with_http_info(**kwargs)
 
         self.document_add = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{absolute_ref}',
+                'endpoint_path': '/api/documents/{reference}',
                 'operation_id': 'document_add',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_ref',
-                    'body',
+                    'reference',
+                    'document',
                     'update_uncontained',
+                    'files',
                 ],
                 'required': [
-                    'absolute_ref',
-                    'body',
+                    'reference',
+                    'document',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_ref':
+                    'reference':
+                        (str,),
+                    'document':
                         (str,),
-                    'body':
-                        ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                     'update_uncontained':
                         (bool,),
+                    'files':
+                        ([file_type],),
                 },
                 'attribute_map': {
-                    'absolute_ref': 'absolute_ref',
+                    'reference': 'reference',
+                    'document': 'document',
                     'update_uncontained': 'update_uncontained',
+                    'files': 'files',
                 },
                 'location_map': {
-                    'absolute_ref': 'path',
-                    'body': 'body',
+                    'reference': 'path',
+                    'document': 'form',
                     'update_uncontained': 'query',
+                    'files': 'form',
                 },
                 'collection_format_map': {
+                    'files': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [
-                    'application/json'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client,
             callable=__document_add
         )
 
         def __document_add_simple(
@@ -247,15 +255,15 @@
         self.document_add_simple = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{data_source_id}/add-raw',
+                'endpoint_path': '/api/documents-add-raw/{data_source_id}',
                 'operation_id': 'document_add_simple',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'data_source_id',
@@ -302,36 +310,34 @@
                     'application/json'
                 ]
             },
             api_client=api_client,
             callable=__document_add_simple
         )
 
-        def __document_add_to_path(
+        def __document_get(
             self,
-            path_reference,
-            document,
+            reference,
             **kwargs
         ):
-            """Add To Path  # noqa: E501
+            """Get  # noqa: E501
 
-            Same as 'add_to_parent', but reference parent by path instead of ID. Also supports files.  - **path_reference**: <data_source>/<path_to_entity>/<entity_name>.<attribute>  # noqa: E501
+            Get document as JSON string.  - **reference**: A reference to a package or a data source   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)  The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_add_to_path(path_reference, document, async_req=True)
+            >>> thread = api.document_get(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                path_reference (str):
-                document (str):
+                reference (str):
 
             Keyword Args:
-                update_uncontained (bool): [optional] if omitted the server will use the default value of False
-                files ([file_type]): [optional]
+                depth (int): [optional] if omitted the server will use the default value of 0
+                resolve_links (bool): [optional] if omitted the server will use the default value of False
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (int/float/tuple): timeout setting for this request. If
                     one number provided, it will be total request timeout. It can also
@@ -368,358 +374,99 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['path_reference'] = \
-                path_reference
-            kwargs['document'] = \
-                document
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
-        self.document_add_to_path = _Endpoint(
+        self.document_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents-by-path/{path_reference}',
-                'operation_id': 'document_add_to_path',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'path_reference',
-                    'document',
-                    'update_uncontained',
-                    'files',
-                ],
-                'required': [
-                    'path_reference',
-                    'document',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'path_reference':
-                        (str,),
-                    'document':
-                        (str,),
-                    'update_uncontained':
-                        (bool,),
-                    'files':
-                        ([file_type],),
-                },
-                'attribute_map': {
-                    'path_reference': 'path_reference',
-                    'document': 'document',
-                    'update_uncontained': 'update_uncontained',
-                    'files': 'files',
-                },
-                'location_map': {
-                    'path_reference': 'path',
-                    'document': 'form',
-                    'update_uncontained': 'query',
-                    'files': 'form',
-                },
-                'collection_format_map': {
-                    'files': 'csv',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [
-                    'multipart/form-data'
-                ]
-            },
-            api_client=api_client,
-            callable=__document_add_to_path
-        )
-
-        def __document_get_by_id(
-            self,
-            id_reference,
-            **kwargs
-        ):
-            """Get By Id  # noqa: E501
-
-            Get document as JSON string.  - **id_reference**: <data_source>/<document_uuid> - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_get_by_id(id_reference, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                id_reference (str):
-
-            Keyword Args:
-                depth (int): [optional] if omitted the server will use the default value of 999
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
-            return self.call_with_http_info(**kwargs)
-
-        self.document_get_by_id = _Endpoint(
-            settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents/{id_reference}',
-                'operation_id': 'document_get_by_id',
+                'endpoint_path': '/api/documents/{reference}',
+                'operation_id': 'document_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'reference',
                     'depth',
+                    'resolve_links',
                 ],
                 'required': [
-                    'id_reference',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'reference':
                         (str,),
                     'depth':
                         (int,),
+                    'resolve_links':
+                        (bool,),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'reference': 'reference',
                     'depth': 'depth',
+                    'resolve_links': 'resolve_links',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'reference': 'path',
                     'depth': 'query',
+                    'resolve_links': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__document_get_by_id
-        )
-
-        def __document_get_by_path(
-            self,
-            absolute_path,
-            **kwargs
-        ):
-            """Get By Path  # noqa: E501
-
-            Get a document by its absolute path.  - **absolute_path**: <protocol>://<data_source>/<path>.<attribute>  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_get_by_path(absolute_path, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                absolute_path (str):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_path'] = \
-                absolute_path
-            return self.call_with_http_info(**kwargs)
-
-        self.document_get_by_path = _Endpoint(
-            settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents-by-path/{absolute_path}',
-                'operation_id': 'document_get_by_path',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'absolute_path',
-                ],
-                'required': [
-                    'absolute_path',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'absolute_path':
-                        (str,),
-                },
-                'attribute_map': {
-                    'absolute_path': 'absolute_path',
-                },
-                'location_map': {
-                    'absolute_path': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client,
-            callable=__document_get_by_path
+            callable=__document_get
         )
 
         def __document_remove(
             self,
-            id_reference,
+            reference,
             **kwargs
         ):
             """Remove  # noqa: E501
 
-            Remove document - **id_reference**: <data_source>/<document_uuid>.<attribute_path>  Example: id_reference=SomeDataSource/3978d9ca-2d7a-4b47-8fed-57710f6cf50b.attributes.1 will remove the first element in the attribute list of a blueprint with the given id in data source 'SomeDataSource'.  # noqa: E501
+            Remove a document from DMSS.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_remove(id_reference, async_req=True)
+            >>> thread = api.document_remove(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                id_reference (str):
+                reference (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -735,15 +482,15 @@
                     Default is True.
                 _host_index (int/None): specifies the index of the server
                     that we want to use.
                     Default is read from the configuration.
                 async_req (bool): execute request asynchronously
 
             Returns:
-                str
+                bool, date, datetime, dict, float, int, list, str, none_type
                     If the method is called asynchronously, returns the request
                     thread.
             """
             kwargs['async_req'] = kwargs.get(
                 'async_req', False
             )
             kwargs['_return_http_data_only'] = kwargs.get(
@@ -758,58 +505,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
         self.document_remove = _Endpoint(
             settings={
-                'response_type': (str,),
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{id_reference}',
+                'endpoint_path': '/api/documents/{reference}',
                 'operation_id': 'document_remove',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'reference',
                 ],
                 'required': [
-                    'id_reference',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'reference':
                         (str,),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'reference': 'reference',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'reference': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -817,135 +564,14 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client,
             callable=__document_remove
         )
 
-        def __document_remove_by_path(
-            self,
-            path_reference,
-            **kwargs
-        ):
-            """Remove By Path  # noqa: E501
-
-            Remove a document from DMSS.  - **path_reference**: <data_source>/<path>.<attribute>  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_remove_by_path(path_reference, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                path_reference (str):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                bool, date, datetime, dict, float, int, list, str, none_type
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['path_reference'] = \
-                path_reference
-            return self.call_with_http_info(**kwargs)
-
-        self.document_remove_by_path = _Endpoint(
-            settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents-by-path/{path_reference}',
-                'operation_id': 'document_remove_by_path',
-                'http_method': 'DELETE',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'path_reference',
-                ],
-                'required': [
-                    'path_reference',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'path_reference':
-                        (str,),
-                },
-                'attribute_map': {
-                    'path_reference': 'path_reference',
-                },
-                'location_map': {
-                    'path_reference': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client,
-            callable=__document_remove_by_path
-        )
-
         def __document_update(
             self,
             id_reference,
             data,
             **kwargs
         ):
             """Update  # noqa: E501
```

### Comparing `dmss-api-1.2.1/dmss_api/api/entity_api.py` & `dmss-api-1.2.2/dmss_api/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/export_api.py` & `dmss-api-1.2.2/dmss_api/api/lookup_table_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,44 +18,47 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from dmss_api.model.error_response import ErrorResponse
+from dmss_api.model.lookup import Lookup
 
 
-class ExportApi(object):
+class LookupTableApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-        def __export(
+        def __create_lookup(
             self,
-            absolute_document_ref,
+            application,
+            recipe_package,
             **kwargs
         ):
-            """Export  # noqa: E501
+            """Create Lookup  # noqa: E501
 
-            Download a zip-folder with one or more documents as json file(s).  - **absolute_document_ref**: <data_source>/<path>/<document_name>  # noqa: E501
+            Create a recipe lookup table from a package containing RecipeLinks. Associate it with an application. This can be used for setting Ui- and StorageRecipes for specific applications.  - **application**: name of application - **recipe_package**: List with one or more paths to package(s) that contain recipe links. (Example: 'system/SIMOS/recipe_links')  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export(absolute_document_ref, async_req=True)
+            >>> thread = api.create_lookup(application, recipe_package, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_document_ref (str):
+                application (str):
+                recipe_package ([str]):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -94,90 +97,98 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_document_ref'] = \
-                absolute_document_ref
+            kwargs['application'] = \
+                application
+            kwargs['recipe_package'] = \
+                recipe_package
             return self.call_with_http_info(**kwargs)
 
-        self.export = _Endpoint(
+        self.create_lookup = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/{absolute_document_ref}',
-                'operation_id': 'export',
-                'http_method': 'GET',
+                'endpoint_path': '/api/application/{application}',
+                'operation_id': 'create_lookup',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_document_ref',
+                    'application',
+                    'recipe_package',
                 ],
                 'required': [
-                    'absolute_document_ref',
+                    'application',
+                    'recipe_package',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_document_ref':
+                    'application':
                         (str,),
+                    'recipe_package':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'absolute_document_ref': 'absolute_document_ref',
+                    'application': 'application',
+                    'recipe_package': 'recipe_package',
                 },
                 'location_map': {
-                    'absolute_document_ref': 'path',
+                    'application': 'path',
+                    'recipe_package': 'query',
                 },
                 'collection_format_map': {
+                    'recipe_package': 'multi',
                 }
             },
             headers_map={
                 'accept': [
-                    'application/zip',
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__export
+            callable=__create_lookup
         )
 
-        def __export_meta(
+        def __get_lookup(
             self,
-            absolute_document_ref,
+            application,
             **kwargs
         ):
-            """Export Meta  # noqa: E501
+            """Get Lookup  # noqa: E501
 
-            Export only the metadata of an entity. An entities metadata is concatenated from the \"top down\". Inheriting parents meta, and overriding for any specified further down.  If no metadata is defined anywhere in the tree, an empty object is returned.  - **absolute_document_ref**: <data_source>/<path_to_entity>/<entity_name>  # noqa: E501
+            Fetch a single lookup table.  - **application**: name of application  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export_meta(absolute_document_ref, async_req=True)
+            >>> thread = api.get_lookup(application, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_document_ref (str):
+                application (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -193,15 +204,15 @@
                     Default is True.
                 _host_index (int/None): specifies the index of the server
                     that we want to use.
                     Default is read from the configuration.
                 async_req (bool): execute request asynchronously
 
             Returns:
-                bool, date, datetime, dict, float, int, list, str, none_type
+                Lookup
                     If the method is called asynchronously, returns the request
                     thread.
             """
             kwargs['async_req'] = kwargs.get(
                 'async_req', False
             )
             kwargs['_return_http_data_only'] = kwargs.get(
@@ -216,65 +227,65 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_document_ref'] = \
-                absolute_document_ref
+            kwargs['application'] = \
+                application
             return self.call_with_http_info(**kwargs)
 
-        self.export_meta = _Endpoint(
+        self.get_lookup = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (Lookup,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/meta/{absolute_document_ref}',
-                'operation_id': 'export_meta',
+                'endpoint_path': '/api/application/{application}',
+                'operation_id': 'get_lookup',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_document_ref',
+                    'application',
                 ],
                 'required': [
-                    'absolute_document_ref',
+                    'application',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_document_ref':
+                    'application':
                         (str,),
                 },
                 'attribute_map': {
-                    'absolute_document_ref': 'absolute_document_ref',
+                    'application': 'application',
                 },
                 'location_map': {
-                    'absolute_document_ref': 'path',
+                    'application': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__export_meta
+            callable=__get_lookup
         )
```

### Comparing `dmss-api-1.2.1/dmss_api/api/health_check_api.py` & `dmss-api-1.2.2/dmss_api/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/lookup_table_api.py` & `dmss-api-1.2.2/dmss_api/api/personal_access_token_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,49 +18,46 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from dmss_api.model.error_response import ErrorResponse
-from dmss_api.model.lookup import Lookup
+from dmss_api.model.pat_data import PATData
 
 
-class LookupTableApi(object):
+class PersonalAccessTokenApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-        def __create_lookup(
+        def __token_create(
             self,
-            application,
-            recipe_package,
             **kwargs
         ):
-            """Create Lookup  # noqa: E501
+            """New Personal Access Token  # noqa: E501
 
-            Create a recipe lookup table from a package containing RecipeLinks. Associate it with an application. This can be used for setting Ui- and StorageRecipes for specific applications.  - **application**: name of application  # noqa: E501
+            Create a personal access token (PAT).  - **scope**: WRITE, READ or NONE - **time_to_live**: Optional parameter to set time to life in seconds (default is 30 days)  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.create_lookup(application, recipe_package, async_req=True)
+            >>> thread = api.token_create(async_req=True)
             >>> result = thread.get()
 
-            Args:
-                application (str):
-                recipe_package (str):
 
             Keyword Args:
+                scope (dict): [optional]
+                time_to_live (int): [optional] if omitted the server will use the default value of 2592000
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (int/float/tuple): timeout setting for this request. If
                     one number provided, it will be total request timeout. It can also
@@ -74,15 +71,15 @@
                     Default is True.
                 _host_index (int/None): specifies the index of the server
                     that we want to use.
                     Default is read from the configuration.
                 async_req (bool): execute request asynchronously
 
             Returns:
-                None
+                str
                     If the method is called asynchronously, returns the request
                     thread.
             """
             kwargs['async_req'] = kwargs.get(
                 'async_req', False
             )
             kwargs['_return_http_data_only'] = kwargs.get(
@@ -97,97 +94,89 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['application'] = \
-                application
-            kwargs['recipe_package'] = \
-                recipe_package
             return self.call_with_http_info(**kwargs)
 
-        self.create_lookup = _Endpoint(
+        self.token_create = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (str,),
                 'auth': [
-                    'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/application/{application}',
-                'operation_id': 'create_lookup',
+                'endpoint_path': '/api/token',
+                'operation_id': 'token_create',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'application',
-                    'recipe_package',
-                ],
-                'required': [
-                    'application',
-                    'recipe_package',
+                    'scope',
+                    'time_to_live',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'application':
-                        (str,),
-                    'recipe_package':
-                        (str,),
+                    'scope':
+                        (dict,),
+                    'time_to_live':
+                        (int,),
                 },
                 'attribute_map': {
-                    'application': 'application',
-                    'recipe_package': 'recipe_package',
+                    'scope': 'scope',
+                    'time_to_live': 'time_to_live',
                 },
                 'location_map': {
-                    'application': 'path',
-                    'recipe_package': 'query',
+                    'scope': 'query',
+                    'time_to_live': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__create_lookup
+            callable=__token_create
         )
 
-        def __get_lookup(
+        def __token_delete(
             self,
-            application,
+            token_id,
             **kwargs
         ):
-            """Get Lookup  # noqa: E501
+            """Revoke Personal Access Token  # noqa: E501
 
-            Fetch a single lookup table.  - **application**: name of application  # noqa: E501
+            Delete a personal access token (PAT).  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.get_lookup(application, async_req=True)
+            >>> thread = api.token_delete(token_id, async_req=True)
             >>> result = thread.get()
 
             Args:
-                application (str):
+                token_id (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -203,15 +192,15 @@
                     Default is True.
                 _host_index (int/None): specifies the index of the server
                     that we want to use.
                     Default is read from the configuration.
                 async_req (bool): execute request asynchronously
 
             Returns:
-                Lookup
+                str
                     If the method is called asynchronously, returns the request
                     thread.
             """
             kwargs['async_req'] = kwargs.get(
                 'async_req', False
             )
             kwargs['_return_http_data_only'] = kwargs.get(
@@ -226,65 +215,172 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['application'] = \
-                application
+            kwargs['token_id'] = \
+                token_id
             return self.call_with_http_info(**kwargs)
 
-        self.get_lookup = _Endpoint(
+        self.token_delete = _Endpoint(
             settings={
-                'response_type': (Lookup,),
+                'response_type': (str,),
                 'auth': [
-                    'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/application/{application}',
-                'operation_id': 'get_lookup',
-                'http_method': 'GET',
+                'endpoint_path': '/api/token/{token_id}',
+                'operation_id': 'token_delete',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'application',
+                    'token_id',
                 ],
                 'required': [
-                    'application',
+                    'token_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'application':
+                    'token_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'application': 'application',
+                    'token_id': 'token_id',
+                },
+                'location_map': {
+                    'token_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json',
+                    'text/plain'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client,
+            callable=__token_delete
+        )
+
+        def __token_list_all(
+            self,
+            **kwargs
+        ):
+            """List All Pats  # noqa: E501
+
+            Get a list of all personal access tokens (PATs).  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.token_list_all(async_req=True)
+            >>> result = thread.get()
+
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (int/float/tuple): timeout setting for this request. If
+                    one number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                [PATData]
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            return self.call_with_http_info(**kwargs)
+
+        self.token_list_all = _Endpoint(
+            settings={
+                'response_type': ([PATData],),
+                'auth': [
+                    'OAuth2AuthorizationCodeBearer'
+                ],
+                'endpoint_path': '/api/token',
+                'operation_id': 'token_list_all',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
                 },
                 'location_map': {
-                    'application': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__get_lookup
+            callable=__token_list_all
         )
```

### Comparing `dmss-api-1.2.1/dmss_api/api/reference_api.py` & `dmss-api-1.2.2/dmss_api/api/reference_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/search_api.py` & `dmss-api-1.2.2/dmss_api/api/search_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api/whoami_api.py` & `dmss-api-1.2.2/dmss_api/api/whoami_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/api_client.py` & `dmss-api-1.2.2/dmss_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.2.1/python'
+        self.user_agent = 'OpenAPI-Generator/1.2.2/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `dmss-api-1.2.1/dmss_api/apis/__init__.py` & `dmss-api-1.2.2/dmss_api/apis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from dmss_api.api.access_control_api import AccessControlApi
+from dmss_api.api.attribute_api import AttributeApi
 from dmss_api.api.blob_api import BlobApi
 from dmss_api.api.blueprint_api import BlueprintApi
 from dmss_api.api.datasource_api import DatasourceApi
 from dmss_api.api.default_api import DefaultApi
 from dmss_api.api.document_api import DocumentApi
 from dmss_api.api.entity_api import EntityApi
 from dmss_api.api.export_api import ExportApi
```

### Comparing `dmss-api-1.2.1/dmss_api/configuration.py` & `dmss-api-1.2.2/dmss_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 1.2.1".\
+               "SDK Package Version: 1.2.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `dmss-api-1.2.1/dmss_api/exceptions.py` & `dmss-api-1.2.2/dmss_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/access_level.py` & `dmss-api-1.2.2/dmss_api/model/access_level.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/acl.py` & `dmss-api-1.2.2/dmss_api/model/acl.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/data_source_information.py` & `dmss-api-1.2.2/dmss_api/model/data_source_information.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/data_source_request.py` & `dmss-api-1.2.2/dmss_api/model/data_source_request.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/entity.py` & `dmss-api-1.2.2/dmss_api/model/entity.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/error_response.py` & `dmss-api-1.2.2/dmss_api/model/error_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/get_blueprint_response.py` & `dmss-api-1.2.2/dmss_api/model/get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/lookup.py` & `dmss-api-1.2.2/dmss_api/model/lookup.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/pat_data.py` & `dmss-api-1.2.2/dmss_api/model/pat_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pat_hash (str): [optional]  # noqa: E501
-            uuid (str): [optional] if omitted the server will use the default value of "626e6eae-525c-40ff-b9cf-7cb141717ed6"  # noqa: E501
+            uuid (str): [optional] if omitted the server will use the default value of "2a858b71-956f-4139-86a2-a7cf38d1b35b"  # noqa: E501
             roles ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -244,15 +244,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pat_hash (str): [optional]  # noqa: E501
-            uuid (str): [optional] if omitted the server will use the default value of "626e6eae-525c-40ff-b9cf-7cb141717ed6"  # noqa: E501
+            uuid (str): [optional] if omitted the server will use the default value of "2a858b71-956f-4139-86a2-a7cf38d1b35b"  # noqa: E501
             roles ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `dmss-api-1.2.1/dmss_api/model/recipe.py` & `dmss-api-1.2.2/dmss_api/model/recipe.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/recipe_attribute.py` & `dmss-api-1.2.2/dmss_api/model/recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/reference.py` & `dmss-api-1.2.2/dmss_api/model/storage_recipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from dmss_api.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from dmss_api.model.storage_attribute import StorageAttribute
+    globals()['StorageAttribute'] = StorageAttribute
 
-class Reference(ModelNormal):
+
+class StorageRecipe(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,81 +58,71 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 128,
-            'min_length': 1,
-            'regex': {
-                'pattern': r'^[A-Za-z0-9_-]*$',  # noqa: E501
-            },
-        },
-        ('type',): {
-            'max_length': 128,
-            'min_length': 3,
-            'regex': {
-                'pattern': r'^[A-Z:a-z0-9_\/-]*$',  # noqa: E501
-            },
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
+            'attributes': ({str: (StorageAttribute,)},),  # noqa: E501
+            'storage_affinity': (dict,),  # noqa: E501
+            'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': '_id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'storage_affinity': 'storageAffinity',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, type, *args, **kwargs):  # noqa: E501
-        """Reference - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """StorageRecipe - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
-            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,14 +147,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional] if omitted the server will use the default value of "dmss://system/SIMOS/StorageRecipe"  # noqa: E501
+            attributes ({str: (StorageAttribute,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            storage_affinity (dict): [optional]  # noqa: E501
+            description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,17 +178,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -203,21 +199,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, type, *args, **kwargs):  # noqa: E501
-        """Reference - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """StorageRecipe - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
-            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -242,14 +236,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional] if omitted the server will use the default value of "dmss://system/SIMOS/StorageRecipe"  # noqa: E501
+            attributes ({str: (StorageAttribute,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            storage_affinity (dict): [optional]  # noqa: E501
+            description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,17 +265,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `dmss-api-1.2.1/dmss_api/model/repository.py` & `dmss-api-1.2.2/dmss_api/model/repository.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/repository_type.py` & `dmss-api-1.2.2/dmss_api/model/repository_type.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/storage_attribute.py` & `dmss-api-1.2.2/dmss_api/model/storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/storage_data_types.py` & `dmss-api-1.2.2/dmss_api/model/storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/model/storage_recipe.py` & `dmss-api-1.2.2/dmss_api/model/reference.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from dmss_api.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from dmss_api.model.storage_attribute import StorageAttribute
-    globals()['StorageAttribute'] = StorageAttribute
 
-
-class StorageRecipe(ModelNormal):
+class Reference(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,71 +54,74 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('type',): {
+            'max_length': 128,
+            'min_length': 3,
+            'regex': {
+                'pattern': r'^[A-Z:a-z0-9_\/-]*$',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
+            'address': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'attributes': ({str: (StorageAttribute,)},),  # noqa: E501
-            'storage_affinity': (dict,),  # noqa: E501
-            'description': (str,),  # noqa: E501
+            'reference_type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
+        'address': 'address',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
-        'storage_affinity': 'storageAffinity',  # noqa: E501
-        'description': 'description',  # noqa: E501
+        'reference_type': 'referenceType',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """StorageRecipe - a model defined in OpenAPI
+    def _from_openapi_data(cls, address, type, reference_type, *args, **kwargs):  # noqa: E501
+        """Reference - a model defined in OpenAPI
 
         Args:
-            name (str):
+            address (str):
+            type (str):
+            reference_type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -147,18 +146,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional] if omitted the server will use the default value of "dmss://system/SIMOS/StorageRecipe"  # noqa: E501
-            attributes ({str: (StorageAttribute,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
-            storage_affinity (dict): [optional]  # noqa: E501
-            description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +173,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.address = address
+        self.type = type
+        self.reference_type = reference_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -199,19 +196,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """StorageRecipe - a model defined in OpenAPI
+    def __init__(self, address, type, reference_type, *args, **kwargs):  # noqa: E501
+        """Reference - a model defined in OpenAPI
 
         Args:
-            name (str):
+            address (str):
+            type (str):
+            reference_type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -236,18 +235,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional] if omitted the server will use the default value of "dmss://system/SIMOS/StorageRecipe"  # noqa: E501
-            attributes ({str: (StorageAttribute,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
-            storage_affinity (dict): [optional]  # noqa: E501
-            description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -265,15 +260,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.address = address
+        self.type = type
+        self.reference_type = reference_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `dmss-api-1.2.1/dmss_api/model_utils.py` & `dmss-api-1.2.2/dmss_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/models/__init__.py` & `dmss-api-1.2.2/dmss_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api/rest.py` & `dmss-api-1.2.2/dmss_api/rest.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/dmss_api.egg-info/SOURCES.txt` & `dmss-api-1.2.2/dmss_api.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 dmss_api.egg-info/PKG-INFO
 dmss_api.egg-info/SOURCES.txt
 dmss_api.egg-info/dependency_links.txt
 dmss_api.egg-info/requires.txt
 dmss_api.egg-info/top_level.txt
 dmss_api/api/__init__.py
 dmss_api/api/access_control_api.py
+dmss_api/api/attribute_api.py
 dmss_api/api/blob_api.py
 dmss_api/api/blueprint_api.py
 dmss_api/api/datasource_api.py
 dmss_api/api/default_api.py
 dmss_api/api/document_api.py
 dmss_api/api/entity_api.py
 dmss_api/api/export_api.py
@@ -46,14 +47,15 @@
 dmss_api/model/storage_attribute.py
 dmss_api/model/storage_data_types.py
 dmss_api/model/storage_recipe.py
 dmss_api/models/__init__.py
 test/test_access_control_api.py
 test/test_access_level.py
 test/test_acl.py
+test/test_attribute_api.py
 test/test_blob_api.py
 test/test_blueprint_api.py
 test/test_data_source_information.py
 test/test_data_source_request.py
 test/test_datasource_api.py
 test/test_default_api.py
 test/test_document_api.py
```

### Comparing `dmss-api-1.2.1/setup.py` & `dmss-api-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "dmss-api"
-VERSION = "1.2.1"
+VERSION = "1.2.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `dmss-api-1.2.1/test/test_access_control_api.py` & `dmss-api-1.2.2/test/test_access_control_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_access_level.py` & `dmss-api-1.2.2/test/test_access_level.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_acl.py` & `dmss-api-1.2.2/test/test_acl.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_blob_api.py` & `dmss-api-1.2.2/test/test_blob_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_blueprint_api.py` & `dmss-api-1.2.2/test/test_blueprint_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_data_source_information.py` & `dmss-api-1.2.2/test/test_data_source_information.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_data_source_request.py` & `dmss-api-1.2.2/test/test_data_source_request.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_datasource_api.py` & `dmss-api-1.2.2/test/test_datasource_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_default_api.py` & `dmss-api-1.2.2/test/test_default_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 
     def setUp(self):
         self.api = DefaultApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_attribute_get(self):
+        """Test case for attribute_get
+
+        Get Attribute  # noqa: E501
+        """
+        pass
+
     def test_blob_get_by_id(self):
         """Test case for blob_get_by_id
 
         Get By Id  # noqa: E501
         """
         pass
 
@@ -78,60 +85,39 @@
         Save  # noqa: E501
         """
         pass
 
     def test_document_add(self):
         """Test case for document_add
 
-        Add By Parent Id  # noqa: E501
+        Add Document  # noqa: E501
         """
         pass
 
     def test_document_add_simple(self):
         """Test case for document_add_simple
 
         Add Raw  # noqa: E501
         """
         pass
 
-    def test_document_add_to_path(self):
-        """Test case for document_add_to_path
-
-        Add To Path  # noqa: E501
-        """
-        pass
-
-    def test_document_get_by_id(self):
-        """Test case for document_get_by_id
-
-        Get By Id  # noqa: E501
-        """
-        pass
-
-    def test_document_get_by_path(self):
-        """Test case for document_get_by_path
+    def test_document_get(self):
+        """Test case for document_get
 
-        Get By Path  # noqa: E501
+        Get  # noqa: E501
         """
         pass
 
     def test_document_remove(self):
         """Test case for document_remove
 
         Remove  # noqa: E501
         """
         pass
 
-    def test_document_remove_by_path(self):
-        """Test case for document_remove_by_path
-
-        Remove By Path  # noqa: E501
-        """
-        pass
-
     def test_document_update(self):
         """Test case for document_update
 
         Update  # noqa: E501
         """
         pass
```

### Comparing `dmss-api-1.2.1/test/test_document_api.py` & `dmss-api-1.2.2/test/test_document_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,60 +22,39 @@
 
     def tearDown(self):
         pass
 
     def test_document_add(self):
         """Test case for document_add
 
-        Add By Parent Id  # noqa: E501
+        Add Document  # noqa: E501
         """
         pass
 
     def test_document_add_simple(self):
         """Test case for document_add_simple
 
         Add Raw  # noqa: E501
         """
         pass
 
-    def test_document_add_to_path(self):
-        """Test case for document_add_to_path
+    def test_document_get(self):
+        """Test case for document_get
 
-        Add To Path  # noqa: E501
-        """
-        pass
-
-    def test_document_get_by_id(self):
-        """Test case for document_get_by_id
-
-        Get By Id  # noqa: E501
-        """
-        pass
-
-    def test_document_get_by_path(self):
-        """Test case for document_get_by_path
-
-        Get By Path  # noqa: E501
+        Get  # noqa: E501
         """
         pass
 
     def test_document_remove(self):
         """Test case for document_remove
 
         Remove  # noqa: E501
         """
         pass
 
-    def test_document_remove_by_path(self):
-        """Test case for document_remove_by_path
-
-        Remove By Path  # noqa: E501
-        """
-        pass
-
     def test_document_update(self):
         """Test case for document_update
 
         Update  # noqa: E501
         """
         pass
```

### Comparing `dmss-api-1.2.1/test/test_entity.py` & `dmss-api-1.2.2/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_entity_api.py` & `dmss-api-1.2.2/test/test_entity_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_error_response.py` & `dmss-api-1.2.2/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_export_api.py` & `dmss-api-1.2.2/test/test_export_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_get_blueprint_response.py` & `dmss-api-1.2.2/test/test_get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_health_check_api.py` & `dmss-api-1.2.2/test/test_health_check_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_lookup.py` & `dmss-api-1.2.2/test/test_lookup.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_lookup_table_api.py` & `dmss-api-1.2.2/test/test_lookup_table_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_pat_data.py` & `dmss-api-1.2.2/test/test_pat_data.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_personal_access_token_api.py` & `dmss-api-1.2.2/test/test_personal_access_token_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_recipe.py` & `dmss-api-1.2.2/test/test_recipe.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_recipe_attribute.py` & `dmss-api-1.2.2/test/test_recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_reference.py` & `dmss-api-1.2.2/test/test_reference.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_reference_api.py` & `dmss-api-1.2.2/test/test_reference_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_repository.py` & `dmss-api-1.2.2/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_repository_type.py` & `dmss-api-1.2.2/test/test_repository_type.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_search_api.py` & `dmss-api-1.2.2/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_storage_attribute.py` & `dmss-api-1.2.2/test/test_storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_storage_data_types.py` & `dmss-api-1.2.2/test/test_storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_storage_recipe.py` & `dmss-api-1.2.2/test/test_storage_recipe.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.1/test/test_whoami_api.py` & `dmss-api-1.2.2/test/test_whoami_api.py`

 * *Files identical despite different names*

